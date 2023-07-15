1. Add new hard disk drive (HDD): Physically connect the new hard disk drive to the servers. 

2. Create a directory for mounting the new drive:
   
        #mkdir /mnt/disk1
   
       This command will create a new directory where the new hard disk will be mounted. 

3. Format in XFS and create a filesystem on the new hard disk: To do this, you will have to partition the hard disk, format it with a file syste then mount it

       #mount /dev/sdb1 /mnt/disk1

4. Edit the /etc/hosts file: Open the hosts file with a text editor:
   
       #nano /etc/hosts
       
       Then, add the following lines to the file, which will map the IP addresses to the server names:
       txt
       192.168.xxx.xxx  server1.hpcsa.com server1
       192.168.xxx.xxx  server2.hpcsa.com server2
       192.168.xxx.xxx  server3.hpcsa.com server3
       192.168.xxx.xxx  client.hpcsa.com client
       
       Replace the "xxx" with the actual numbers of each server and client's IP address.

5. Stop the firewall service: Run the following command to stop the firewall service on each server:
   
       systemctl stop firewalld
       
   
6. Install the required packages: Install wget, centos-release-gluster, epel-release, and glusterfs-server packages:
   
       yum install wget centos-release-gluster epel-release glusterfs-server -y
   

7. Start and enable Gluster daemon: The following commands will start the gluster daemon and set it to start automatically at boot:
   
       systemctl start glusterd
       systemctl enable glusterd
       
   
8. Add peers: Add other servers as peers to the GlusterFS cluster from server 1:
   
       gluster peer probe server2.hpcsa.com
       gluster peer probe server3.hpcsa.com
       
   
9. Check the status of the GlusterFS cluster: The following commands will display the status of the peers and the list of servers in the pool:
   
       gluster peer status
       gluster pool list
       
   
10. Create a new directory for the Gluster volume on each server: 
   
           mkdir /mnt/disk1/diskvol
           
   
11. Create and start a Gluster volume: This command creates a Gluster volume named 'gdisk1' with a replication factor of 3. It then starts the volume:
   
         gluster volume create gdisk1 replica 3 
         
         server2.hpcsa.com:/mnt/disk1/diskvol/gdisk1  server2.hpcsa.com:/mnt/disk1/distvol/gdisk1  server3.hpcsa.com:/mnt/disk1/distvol/gdisk1
         
         gluster volume start gdisk1
         
   
12. Display information about the Gluster volume: This command displays information about the 'gdisk1' volume:
   
         gluster volume info gdisk1
         
   
13. On the client, install glusterfs-fuse package: This package allows GlusterFS volumes to be mounted via fuse:
   
         yum install glusterfs-fuse
   
   
14. Create a directory for mounting the Gluster volume:
   
         mkdir /mnt/gdrive
   
   
15. Mount the Gluster volume on the client: This command mounts the 'gdisk1' volume to the newly created directory:
   
         mount -t glusterfs server1:/gdisk1 /mnt/gdrive
         
         Now, the Gluster volume 'gdisk1' is available on the client at the '/mnt/gdrive' directory.
