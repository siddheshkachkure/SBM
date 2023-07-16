    root@192.168.239.158's password:
        ┌──────────────────────────────────────────────────────────────────────┐
        │                 • MobaXterm Personal Edition v23.1 •                 │
        │               (SSH client, X server and network tools)               │
        │                                                                      │
        │ ⮞ SSH session to root@192.168.239.158                                │
        │   • Direct SSH      :  ✓                                             │
        │   • SSH compression :  ✓                                             │
        │   • SSH-browser     :  ✓                                             │
        │   • X11-forwarding  :  ✗  (disabled or not supported by server)      │
        │                                                                      │
        │ ⮞ For more info, ctrl+click on help or visit our website.            │
        └──────────────────────────────────────────────────────────────────────┘
    
    Last login: Sun Jul 16 21:14:00 2023
    [root@ceph5 ~]# vim /etc/chrony.conf
    [root@ceph5 ~]# systemctl restart chronyd
    [root@ceph5 ~]# rbd create disk01 --size 4096
    [root@ceph5 ~]# rbd ls -l
    NAME    SIZE PARENT FMT PROT LOCK
    disk01 4 GiB          2
    [root@ceph5 ~]# modprobe rbd
    [root@ceph5 ~]# rbd feature disable disk01 exclusive-lock object-map fast-diff deep-flatten
    [root@ceph5 ~]# rbd map disk01
    /dev/rbd0
    [root@ceph5 ~]# rbd showmapped
    id pool image  snap device
    0  rbd  disk01 -    /dev/rbd0
    [root@ceph5 ~]# lsblk
    NAME            MAJ:MIN RM  SIZE RO TYPE MOUNTPOINT
    sda               8:0    0   20G  0 disk
    ├─sda1            8:1    0    1G  0 part /boot
    └─sda2            8:2    0   19G  0 part
      ├─centos-root 253:0    0   17G  0 lvm  /
      └─centos-swap 253:1    0    2G  0 lvm  [SWAP]
    sr0              11:0    1  973M  0 rom
    rbd0            252:0    0    4G  0 disk
    [root@ceph5 ~]# mkfs.xfs /dev/rbd0
    Discarding blocks...Done.
    meta-data=/dev/rbd0              isize=512    agcount=8, agsize=131072 blks
             =                       sectsz=512   attr=2, projid32bit=1
             =                       crc=1        finobt=0, sparse=0
    data     =                       bsize=4096   blocks=1048576, imaxpct=25
             =                       sunit=1024   swidth=1024 blks
    naming   =version 2              bsize=4096   ascii-ci=0 ftype=1
    log      =internal log           bsize=4096   blocks=2560, version=2
             =                       sectsz=512   sunit=8 blks, lazy-count=1
    realtime =none                   extsz=4096   blocks=0, rtextents=0
    [root@ceph5 ~]# mkdir -p /mnt/mydisk
    [root@ceph5 ~]# mount /dev/rbd0 /mnt/mydisk
    [root@ceph5 ~]# df -h
    Filesystem               Size  Used Avail Use% Mounted on
    devtmpfs                 475M     0  475M   0% /dev
    tmpfs                    487M     0  487M   0% /dev/shm
    tmpfs                    487M  7.7M  479M   2% /run
    tmpfs                    487M     0  487M   0% /sys/fs/cgroup
    /dev/mapper/centos-root   17G  1.8G   16G  11% /
    /dev/sda1               1014M  138M  877M  14% /boot
    tmpfs                     98M     0   98M   0% /run/user/0
    /dev/rbd0                4.0G   33M  4.0G   1% /mnt/mydisk
    [root@ceph5 ~]# vim /etc/hosts
    [root@ceph5 ~]# systemctl restart chronyd
    [root@ceph5 ~]# df -h
    Filesystem               Size  Used Avail Use% Mounted on
    devtmpfs                 475M     0  475M   0% /dev
    tmpfs                    487M     0  487M   0% /dev/shm
    tmpfs                    487M  7.7M  479M   2% /run
    tmpfs                    487M     0  487M   0% /sys/fs/cgroup
    /dev/mapper/centos-root   17G  1.8G   16G  11% /
    /dev/sda1               1014M  138M  877M  14% /boot
    tmpfs                     98M     0   98M   0% /run/user/0
    /dev/rbd0                4.0G   33M  4.0G   1% /mnt/mydisk
    [root@ceph5 ~]#
