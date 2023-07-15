For Gluster-FS Cluster 
Make 4 Centos7 VMs hving minimal installation 

      VM  Name            Core  HardDrive  Extra-HD
      1   gfs1 (server1)    1      20        20
      2   gfs2 (server2)    1      20        20
      3   gfs3 (server3)    1      20        20
      4   gfs4 (server4)    1      20        --

* Step 1: Disable firewall, selinux on each vm

      systemctl stop firewalld
      systemctl disable firewalld
      yum install vim -y
      vim /etc/selinux/config
        SELINUX=disbaled
      setenforce 0
* Step 2: Set hostname for each VM

    * On server 1
  
           hostnamectl set-hostname gfs1.in
    * On sevrer 2
    
          hostnamectl set-hostname gfs2.in
    * On sevrer 3
    
          hostnamectl set-hostname gfs3.in
    * On Client
    
          hostnamectl set-hostname gfs4.in
* Step 3: Enter your IP & fqdn name in /etc/hosts in Each VM

      vim /etc/hosts
        <server1-IP> gfs1.in
        <server2-IP> gfs2.in
        <server3-IP> gfs3.in
        <client-IP> gfs4.in
* Step 4: Configure our extra added Hard-Disks in Each VM [here in the VM extra HD is --(sdb)--]
    * Run all these commands to configure 
  
            lsblk
            fdisk /dev/sdb
            mkfs.xfs /dev/sdb1 
            mkdir /mnt/disk1
            mount /dev/sdb1 /mnt/disk1/
            lsblk
* Step 5: Now install required packages Gluster-FS -> Run this Command twice for installing 

      yum install wget centos-release-gluster epel-release glusterfs-server -y
* Step 6: Start & Enable Gluster daemon

      systemctl start glusterd
      systemctl enable glusterd
* Step 7: Add peers - Add other servers as peers to the GLUSTER-FS Cluster from server 1:

      gluster peer probe gfs2.in
      gluster peer probe gfs3.in
* Step 8: Check the status of the GlusterFS cluster

      gluster peer status
      gluster pool list
* Step 9: Create a new directory for the CLuster colume on each server:

      mkdir /mnt/disk1/diskvol
* Step 10: Create, start and check info of a GLuster Volume for replication: 

      gluster volume create gdisk1 replica 3 gfs1.in:/mnt/disk1/diskvol/gdisk1  gfs2.in:/mnt/disk1/diskvol/gdisk1  gfs3.in:/mnt/disk1/diskvol/gdisk1
      gluster volume start gdisk1
      gluster volume info gdisk1
      df -h
      du -h
      ll -h
      cd /mnt/disk1/diskvol/
      du -sh gdisk1/
* Step 11: On the client, install glusterfs-fuse package: This package allows GlusterFS volumes to be mounted via fuse:

      yum install glusterfs-fuse
* Step 12: On the Client, Create a directory for mounting the Gluster volume:-> and mount gdisk1 /mnt/gdrive

      mkdir /mnt/gdrive1
      mount -t glusterfs node1.hpcsa.in:/gdisk2 /mnt/gdrive
      df -h 
      lsblk
* Step 13: On the Client, Run following Command to make blank file in specific drive
  * Here in this command bs-> bite size count-> how many mb or gb file you want.

            cd /mnt/gdrive
            dd if=/dev/zero of=file.data bs=1024 count=1000000
            df -h         
* Step 14: Now on Server Check the size of the respective replicated files such as for gdrive1

      cd /mnt/disk1/diskvol/
      df -h
You can also Create the same for Distributed & Dispersed(With Parity) as from Step 10: only replace 1st command with below cmds and name the disk as per your choice replacing gdisk1 with (----)

    gluster volume create gdisk2 gfs1.in:/mnt/disk1/diskvol/gdisk2  gfs2.in:/mnt/disk1/diskvol/gdisk2  gfs3.in:/mnt/disk1/diskvol/gdisk2

    gluster volume create gdisk3 desperse 3 redundancy 1 gfs1.in:/mnt/disk1/diskvol/gdisk3  gfs2.in:/mnt/disk1/diskvol/gdisk3  gfs3.in:/mnt/disk1/diskvol/gdisk3

Now Follow the same from Step 10.
