root@192.168.239.147's password:
    ┌──────────────────────────────────────────────────────────────────────┐
    │                 • MobaXterm Personal Edition v23.1 •                 │
    │               (SSH client, X server and network tools)               │
    │                                                                      │
    │ ⮞ SSH session to root@192.168.239.147                                │
    │   • Direct SSH      :  ✓                                             │
    │   • SSH compression :  ✓                                             │
    │   • SSH-browser     :  ✓                                             │
    │   • X11-forwarding  :  ✗  (disabled or not supported by server)      │
    │                                                                      │
    │ ⮞ For more info, ctrl+click on help or visit our website.            │
    └──────────────────────────────────────────────────────────────────────┘

Last login: Fri Jul 14 22:38:23 2023

    [root@localhost ~]# hostname
    localhost.localdomain
    [root@localhost ~]# hostnamectl set-hostname iscsi_client
    [root@localhost ~]# hostname
    iscsi_client
    [root@localhost ~]# yum install -y iscsi-initiator-utils
    Loaded plugins: fastestmirror 
    Determining fastest mirrors
     * base: centos.mirror.net.in
     * extras: centos.mirror.net.in
     * updates: centos.mirror.net.in
    base                                                                              | 3.6 kB  00:00:00
    extras                                                                            | 2.9 kB  00:00:00
    updates                                                                           | 2.9 kB  00:00:00
    (1/4): base/7/x86_64/group_gz                                                     | 153 kB  00:00:00
    (2/4): extras/7/x86_64/primary_db                                                 | 250 kB  00:00:00
    (3/4): updates/7/x86_64/primary_db                                                |  22 MB  00:00:02
    (4/4): base/7/x86_64/primary_db                                                   | 6.1 MB  00:00:03
    Resolving Dependencies
    --> Running transaction check
    ---> Package iscsi-initiator-utils.x86_64 0:6.2.0.874-22.el7_9 will be installed
    --> Processing Dependency: iscsi-initiator-utils-iscsiuio >= 6.2.0.874-22.el7_9 for package: iscsi-initiator-utils-6.2.0.874-22.el7_9.x86_64
    --> Running transaction check
    ---> Package iscsi-initiator-utils-iscsiuio.x86_64 0:6.2.0.874-22.el7_9 will be installed
    --> Finished Dependency Resolution
    
    Dependencies Resolved
    
    =========================================================================================================
     Package                                Arch           Version                     Repository       Size
    =========================================================================================================
    Installing:
     iscsi-initiator-utils                  x86_64         6.2.0.874-22.el7_9          updates         423 k
    Installing for dependencies:
     iscsi-initiator-utils-iscsiuio         x86_64         6.2.0.874-22.el7_9          updates          94 k
    
    Transaction Summary
    =========================================================================================================
    Install  1 Package (+1 Dependent package)
    
    Total download size: 517 k
    Installed size: 2.5 M
    Downloading packages:
    warning: /var/cache/yum/x86_64/7/updates/packages/iscsi-initiator-utils-iscsiuio-6.2.0.874-22.el7_9.x86_64.rpm: Header V3 RSA/SHA256 Signature, key ID f4a80eb5: NOKEY
    Public key for iscsi-initiator-utils-iscsiuio-6.2.0.874-22.el7_9.x86_64.rpm is not installed
    (1/2): iscsi-initiator-utils-iscsiuio-6.2.0.874-22.el7_9.x86_64.rpm               |  94 kB  00:00:00
    (2/2): iscsi-initiator-utils-6.2.0.874-22.el7_9.x86_64.rpm                        | 423 kB  00:00:00
    ---------------------------------------------------------------------------------------------------------
    Total                                                                    2.8 MB/s | 517 kB  00:00:00
    Retrieving key from file:///etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7
    Importing GPG key 0xF4A80EB5:
     Userid     : "CentOS-7 Key (CentOS 7 Official Signing Key) <security@centos.org>"
     Fingerprint: 6341 ab27 53d7 8a78 a7c2 7bb1 24c6 a8a7 f4a8 0eb5
     Package    : centos-release-7-9.2009.0.el7.centos.x86_64 (@anaconda)
     From       : /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7
    Running transaction check
    Running transaction test
    Transaction test succeeded
    Running transaction
      Installing : iscsi-initiator-utils-iscsiuio-6.2.0.874-22.el7_9.x86_64                              1/2
      Installing : iscsi-initiator-utils-6.2.0.874-22.el7_9.x86_64                                       2/2
      Verifying  : iscsi-initiator-utils-6.2.0.874-22.el7_9.x86_64                                       1/2
      Verifying  : iscsi-initiator-utils-iscsiuio-6.2.0.874-22.el7_9.x86_64                              2/2
    
    Installed:
      iscsi-initiator-utils.x86_64 0:6.2.0.874-22.el7_9
    
    Dependency Installed:
      iscsi-initiator-utils-iscsiuio.x86_64 0:6.2.0.874-22.el7_9
    
    Complete!
    [root@localhost ~]# systemctl stop firewalld
    [root@localhost ~]# targetcli
    -bash: targetcli: command not found
    [root@localhost ~]# yum install -y targetcli
    Loaded plugins: fastestmirror
    Loading mirror speeds from cached hostfile
     * base: centos.mirror.net.in
     * extras: centos.mirror.net.in
     * updates: centos.mirror.net.in
    Resolving Dependencies
    --> Running transaction check
    ---> Package targetcli.noarch 0:2.1.53-1.el7_9 will be installed
    --> Processing Dependency: python-rtslib >= 2.1.fb41 for package: targetcli-2.1.53-1.el7_9.noarch
    --> Processing Dependency: python-ethtool for package: targetcli-2.1.53-1.el7_9.noarch
    --> Processing Dependency: python-configshell for package: targetcli-2.1.53-1.el7_9.noarch
    --> Running transaction check
    ---> Package python-configshell.noarch 1:1.1.26-1.el7 will be installed
    --> Processing Dependency: python-urwid for package: 1:python-configshell-1.1.26-1.el7.noarch
    --> Processing Dependency: python-six for package: 1:python-configshell-1.1.26-1.el7.noarch
    --> Processing Dependency: pyparsing for package: 1:python-configshell-1.1.26-1.el7.noarch
    ---> Package python-ethtool.x86_64 0:0.8-8.el7 will be installed
    --> Processing Dependency: libnl.so.1()(64bit) for package: python-ethtool-0.8-8.el7.x86_64
    ---> Package python-rtslib.noarch 0:2.1.74-1.el7_9 will be installed
    --> Processing Dependency: python-kmod for package: python-rtslib-2.1.74-1.el7_9.noarch
    --> Running transaction check
    ---> Package libnl.x86_64 0:1.1.4-3.el7 will be installed
    ---> Package pyparsing.noarch 0:1.5.6-9.el7 will be installed
    ---> Package python-kmod.x86_64 0:0.9-4.el7 will be installed
    ---> Package python-six.noarch 0:1.9.0-2.el7 will be installed
    ---> Package python-urwid.x86_64 0:1.1.1-3.el7 will be installed
    --> Finished Dependency Resolution
    
    Dependencies Resolved
    
    =========================================================================================================
     Package                        Arch               Version                     Repository           Size
    =========================================================================================================
    Installing:
     targetcli                      noarch             2.1.53-1.el7_9              updates              75 k
    Installing for dependencies:
     libnl                          x86_64             1.1.4-3.el7                 base                128 k
     pyparsing                      noarch             1.5.6-9.el7                 base                 94 k
     python-configshell             noarch             1:1.1.26-1.el7              base                 68 k
     python-ethtool                 x86_64             0.8-8.el7                   base                 34 k
     python-kmod                    x86_64             0.9-4.el7                   base                 57 k
     python-rtslib                  noarch             2.1.74-1.el7_9              updates             104 k
     python-six                     noarch             1.9.0-2.el7                 base                 29 k
     python-urwid                   x86_64             1.1.1-3.el7                 base                654 k
    
    Transaction Summary
    =========================================================================================================
    Install  1 Package (+8 Dependent packages)
    
    Total download size: 1.2 M
    Installed size: 5.2 M
    Downloading packages:
    (1/9): libnl-1.1.4-3.el7.x86_64.rpm                                               | 128 kB  00:00:00
    (2/9): pyparsing-1.5.6-9.el7.noarch.rpm                                           |  94 kB  00:00:00
    (3/9): python-ethtool-0.8-8.el7.x86_64.rpm                                        |  34 kB  00:00:00
    (4/9): python-configshell-1.1.26-1.el7.noarch.rpm                                 |  68 kB  00:00:00
    (5/9): python-kmod-0.9-4.el7.x86_64.rpm                                           |  57 kB  00:00:00
    (6/9): python-six-1.9.0-2.el7.noarch.rpm                                          |  29 kB  00:00:00
    (7/9): targetcli-2.1.53-1.el7_9.noarch.rpm                                        |  75 kB  00:00:00
    (8/9): python-rtslib-2.1.74-1.el7_9.noarch.rpm                                    | 104 kB  00:00:00
    (9/9): python-urwid-1.1.1-3.el7.x86_64.rpm                                        | 654 kB  00:00:00
    ---------------------------------------------------------------------------------------------------------
    Total                                                                    3.4 MB/s | 1.2 MB  00:00:00
    Running transaction check
    Running transaction test
    Transaction test succeeded
    Running transaction
      Installing : python-six-1.9.0-2.el7.noarch                                                         1/9
      Installing : pyparsing-1.5.6-9.el7.noarch                                                          2/9
      Installing : python-kmod-0.9-4.el7.x86_64                                                          3/9
      Installing : python-rtslib-2.1.74-1.el7_9.noarch                                                   4/9
      Installing : libnl-1.1.4-3.el7.x86_64                                                              5/9
      Installing : python-ethtool-0.8-8.el7.x86_64                                                       6/9
      Installing : python-urwid-1.1.1-3.el7.x86_64                                                       7/9
      Installing : 1:python-configshell-1.1.26-1.el7.noarch                                              8/9
      Installing : targetcli-2.1.53-1.el7_9.noarch                                                       9/9
      Verifying  : python-urwid-1.1.1-3.el7.x86_64                                                       1/9
      Verifying  : libnl-1.1.4-3.el7.x86_64                                                              2/9
      Verifying  : python-ethtool-0.8-8.el7.x86_64                                                       3/9
      Verifying  : python-rtslib-2.1.74-1.el7_9.noarch                                                   4/9
      Verifying  : targetcli-2.1.53-1.el7_9.noarch                                                       5/9
      Verifying  : python-kmod-0.9-4.el7.x86_64                                                          6/9
      Verifying  : python-six-1.9.0-2.el7.noarch                                                         7/9
      Verifying  : pyparsing-1.5.6-9.el7.noarch                                                          8/9
      Verifying  : 1:python-configshell-1.1.26-1.el7.noarch                                              9/9
    
    Installed:
      targetcli.noarch 0:2.1.53-1.el7_9
    
    Dependency Installed:
      libnl.x86_64 0:1.1.4-3.el7                           pyparsing.noarch 0:1.5.6-9.el7
      python-configshell.noarch 1:1.1.26-1.el7             python-ethtool.x86_64 0:0.8-8.el7
      python-kmod.x86_64 0:0.9-4.el7                       python-rtslib.noarch 0:2.1.74-1.el7_9
      python-six.noarch 0:1.9.0-2.el7                      python-urwid.x86_64 0:1.1.1-3.el7
    
    Complete!
    [root@localhost ~]# targetcli
    Warning: Could not load preferences file /root/.targetcli/prefs.bin.
    targetcli shell version 2.1.53
    Copyright 2011-2013 by Datera, Inc and others.
    For help on commands, type 'help'.
    
    /> cd backstores/block
    /backstores/block> cd iscsi
    No such path /backstores/block/iscsi
    /backstores/block> cd ..
    /backstores> ls
    o- backstores ..................................................................................... [...]
      o- block ......................................................................... [Storage Objects: 0]
      o- fileio ........................................................................ [Storage Objects: 0]
      o- pscsi ......................................................................... [Storage Objects: 0]
      o- ramdisk ....................................................................... [Storage Objects: 0]
    /backstores> cd ..
    /> cd iscsi
    /iscsi>
    /iscsi>
    [1]+  Stopped                 targetcli
    [root@localhost ~]# cat /etc/iscsi/initiatorname.iscsi
    InitiatorName=iqn.1994-05.com.redhat:b4d9b7267f7
    [root@localhost ~]# iscsi
    -bash: iscsi: command not found
    [root@localhost ~]# hostname
    iscsi_client
    [root@localhost ~]# yum install -y iscsi-initiator-utils
    Loaded plugins: fastestmirror
    Loading mirror speeds from cached hostfile
     * base: centos.mirror.net.in
     * extras: centos.mirror.net.in
     * updates: centos.mirror.net.in
    Package iscsi-initiator-utils-6.2.0.874-22.el7_9.x86_64 already installed and latest version
    Nothing to do
    [root@localhost ~]# cd /etc/iscsi/
    [root@localhost iscsi]# cat initiatorname.iscsi
    InitiatorName=iqn.1994-05.com.redhat:b4d9b7267f7
    [root@localhost iscsi]# systemctl restart iscsi
    [root@localhost iscsi]# iscsiadm -m -t st -p 192.168.239.146 --login
    Try `iscsiadm --help' for more information.
    [root@localhost iscsi]# yum install -y iscsi-initiator-utils
    Loaded plugins: fastestmirror
    Loading mirror speeds from cached hostfile
     * base: centos.mirror.net.in
     * extras: centos.mirror.net.in
     * updates: centos.mirror.net.in
    Package iscsi-initiator-utils-6.2.0.874-22.el7_9.x86_64 already installed and latest version
    Nothing to do
    [root@localhost iscsi]# cd
    [root@localhost ~]# iscsiadm -m -t st -p 192.168.239.146 --login
    Try `iscsiadm --help' for more information.
    [root@localhost ~]# iscsiadm -m session
    iscsiadm: No active sessions.
    [root@localhost ~]# lsblk
    NAME            MAJ:MIN RM  SIZE RO TYPE MOUNTPOINT
    sda               8:0    0   20G  0 disk
    ├─sda1            8:1    0    1G  0 part /boot
    └─sda2            8:2    0   19G  0 part
      ├─centos-root 253:0    0   17G  0 lvm  /
      └─centos-swap 253:1    0    2G  0 lvm  [SWAP]
    sr0              11:0    1  973M  0 rom
    [root@localhost ~]# systemctl start iscsi
    [root@localhost ~]# iscsiadm -m session
    iscsiadm: No active sessions.
    [root@localhost ~]# iscsiadm -m -t st -p 192.168.239.146 --login
    Try `iscsiadm --help' for more information.
    [root@localhost ~]# lsblk
    NAME            MAJ:MIN RM  SIZE RO TYPE MOUNTPOINT
    sda               8:0    0   20G  0 disk
    ├─sda1            8:1    0    1G  0 part /boot
    └─sda2            8:2    0   19G  0 part
      ├─centos-root 253:0    0   17G  0 lvm  /
      └─centos-swap 253:1    0    2G  0 lvm  [SWAP]
    sr0              11:0    1  973M  0 rom
    [root@localhost ~]# history
        1  hostname
        2  hostnamectl set-hostname iscsi_client
        3  hostname
        4  yum install -y iscsi-initiator-utils
        5  systemctl stop firewalld
        6  targetcli
        7  yum install -y targetcli
        8  targetcli
        9  cat /etc/iscsi/initiatorname.iscsi
       10  iscsi
       11  hostname
       12  yum install -y iscsi-initiator-utils
       13  cd /etc/iscsi/
       14  cat initiatorname.iscsi
       15  systemctl restart iscsi
       16  iscsiadm -m -t st -p 192.168.239.146 --login
       17  yum install -y iscsi-initiator-utils
       18  cd
       19  iscsiadm -m -t st -p 192.168.239.146 --login
       20  iscsiadm -m session
       21  lsblk
       22  systemctl start iscsi
       23  iscsiadm -m session
       24  iscsiadm -m -t st -p 192.168.239.146 --login
       25  lsblk
       26  history
    [root@localhost ~]# cd /etc/iscsi/
    [root@localhost iscsi]# cat initiatorname.iscsi
    InitiatorName=iqn.1994-05.com.redhat:b4d9b7267f7
    [root@localhost iscsi]# iscsiadm -m discovery -t st -p 192.168.239.146
    192.168.239.146:3260,1 iqn.2023-07.siddhu.cdac.sbm:disk1
    [root@localhost iscsi]# lsblk
    NAME            MAJ:MIN RM  SIZE RO TYPE MOUNTPOINT
    sda               8:0    0   20G  0 disk
    ├─sda1            8:1    0    1G  0 part /boot
    └─sda2            8:2    0   19G  0 part
      ├─centos-root 253:0    0   17G  0 lvm  /
      └─centos-swap 253:1    0    2G  0 lvm  [SWAP]
    sr0              11:0    1  973M  0 rom
    [root@localhost iscsi]# fdisk -l
    
    Disk /dev/sda: 21.5 GB, 21474836480 bytes, 41943040 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 512 bytes
    Disk label type: dos
    Disk identifier: 0x000cd7d9
    
       Device Boot      Start         End      Blocks   Id  System
    /dev/sda1   *        2048     2099199     1048576   83  Linux
    /dev/sda2         2099200    41943039    19921920   8e  Linux LVM
    
    Disk /dev/mapper/centos-root: 18.2 GB, 18249416704 bytes, 35643392 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 512 bytes
    
    
    Disk /dev/mapper/centos-swap: 2147 MB, 2147483648 bytes, 4194304 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 512 bytes
    
    [root@localhost iscsi]# lsblk
    NAME            MAJ:MIN RM  SIZE RO TYPE MOUNTPOINT
    sda               8:0    0   20G  0 disk
    ├─sda1            8:1    0    1G  0 part /boot
    └─sda2            8:2    0   19G  0 part
      ├─centos-root 253:0    0   17G  0 lvm  /
      └─centos-swap 253:1    0    2G  0 lvm  [SWAP]
    sr0              11:0    1  973M  0 rom
    [root@localhost iscsi]# iscsiadm -m discovery -t st -p 192.168.239.146 --login
    192.168.239.146:3260,1 iqn.2023-07.siddhu.cdac.sbm:disk1
    Logging in to [iface: default, target: iqn.2023-07.siddhu.cdac.sbm:disk1, portal: 192.168.239.146,3260] (multiple)
    Login to [iface: default, target: iqn.2023-07.siddhu.cdac.sbm:disk1, portal: 192.168.239.146,3260] successful.
    [root@localhost iscsi]# lsblk
    NAME            MAJ:MIN RM  SIZE RO TYPE MOUNTPOINT
    sda               8:0    0   20G  0 disk
    ├─sda1            8:1    0    1G  0 part /boot
    └─sda2            8:2    0   19G  0 part
      ├─centos-root 253:0    0   17G  0 lvm  /
      └─centos-swap 253:1    0    2G  0 lvm  [SWAP]
    sdb               8:16   0    1G  0 disk
    sr0              11:0    1  973M  0 rom
    [root@localhost iscsi]# fdisk -l
    
    Disk /dev/sda: 21.5 GB, 21474836480 bytes, 41943040 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 512 bytes
    Disk label type: dos
    Disk identifier: 0x000cd7d9
    
       Device Boot      Start         End      Blocks   Id  System
    /dev/sda1   *        2048     2099199     1048576   83  Linux
    /dev/sda2         2099200    41943039    19921920   8e  Linux LVM
    
    Disk /dev/mapper/centos-root: 18.2 GB, 18249416704 bytes, 35643392 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 512 bytes
    
    
    Disk /dev/mapper/centos-swap: 2147 MB, 2147483648 bytes, 4194304 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 512 bytes
    
    
    Disk /dev/sdb: 1073 MB, 1073741824 bytes, 2097152 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 4194304 bytes
    
    [root@localhost iscsi]# fdisk /dev/sd
    sda   sda1  sda2  sdb
    [root@localhost iscsi]# fdisk /dev/sd
    sda   sda1  sda2  sdb
    [root@localhost iscsi]# fdisk /dev/sdb
    Welcome to fdisk (util-linux 2.23.2).
    
    Changes will remain in memory only, until you decide to write them.
    Be careful before using the write command.
    
    Device does not contain a recognized partition table
    Building a new DOS disklabel with disk identifier 0xddedc6bf.
    
    Command (m for help): n
    Partition type:
       p   primary (0 primary, 0 extended, 4 free)
       e   extended
    Select (default p): p
    Partition number (1-4, default 1): 1
    First sector (8192-2097151, default 8192):
    Using default value 8192
    Last sector, +sectors or +size{K,M,G} (8192-2097151, default 2097151):
    Using default value 2097151
    Partition 1 of type Linux and of size 1020 MiB is set
    
    Command (m for help): w
    The partition table has been altered!
    
    Calling ioctl() to re-read partition table.
    Syncing disks.
    [root@localhost iscsi]# fdisk -l
    
    Disk /dev/sda: 21.5 GB, 21474836480 bytes, 41943040 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 512 bytes
    Disk label type: dos
    Disk identifier: 0x000cd7d9
    
       Device Boot      Start         End      Blocks   Id  System
    /dev/sda1   *        2048     2099199     1048576   83  Linux
    /dev/sda2         2099200    41943039    19921920   8e  Linux LVM
    
    Disk /dev/mapper/centos-root: 18.2 GB, 18249416704 bytes, 35643392 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 512 bytes
    
    
    Disk /dev/mapper/centos-swap: 2147 MB, 2147483648 bytes, 4194304 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 512 bytes
    
    
    Disk /dev/sdb: 1073 MB, 1073741824 bytes, 2097152 sectors
    Units = sectors of 1 * 512 = 512 bytes
    Sector size (logical/physical): 512 bytes / 512 bytes
    I/O size (minimum/optimal): 512 bytes / 4194304 bytes
    Disk label type: dos
    Disk identifier: 0xddedc6bf
    
       Device Boot      Start         End      Blocks   Id  System
    /dev/sdb1            8192     2097151     1044480   83  Linux
    [root@localhost iscsi]# mkdir /mnt/disk-1
    [root@localhost iscsi]# mkfs.ext4 /dev/sdb
    sdb   sdb1
    [root@localhost iscsi]# mkfs.ext4 /dev/sdb
    mke2fs 1.42.9 (28-Dec-2013)
    /dev/sdb is entire device, not just one partition!
    Proceed anyway? (y,n) y
    Filesystem label=
    OS type: Linux
    Block size=4096 (log=2)
    Fragment size=4096 (log=2)
    Stride=0 blocks, Stripe width=1024 blocks
    65536 inodes, 262144 blocks
    13107 blocks (5.00%) reserved for the super user
    First data block=0
    Maximum filesystem blocks=268435456
    8 block groups
    32768 blocks per group, 32768 fragments per group
    8192 inodes per group
    Superblock backups stored on blocks:
            32768, 98304, 163840, 229376
    
    Allocating group tables: done
    Writing inode tables: done
    Creating journal (8192 blocks): done
    Writing superblocks and filesystem accounting information: done
    
    [root@localhost iscsi]# mount /dev/sdb1 /mnt/disk-1/
    mount: special device /dev/sdb1 does not exist
    [root@localhost iscsi]# mount /dev/sdb /mnt/disk-1/
    [root@localhost iscsi]# lsblk
    NAME            MAJ:MIN RM  SIZE RO TYPE MOUNTPOINT
    sda               8:0    0   20G  0 disk
    ├─sda1            8:1    0    1G  0 part /boot
    └─sda2            8:2    0   19G  0 part
      ├─centos-root 253:0    0   17G  0 lvm  /
      └─centos-swap 253:1    0    2G  0 lvm  [SWAP]
    sdb               8:16   0    1G  0 disk /mnt/disk-1
    sr0              11:0    1  973M  0 rom
    [root@localhost iscsi]# mount /dev/sdh1 /mnt/disk-1/
    mount: special device /dev/sdh1 does not exist
    [root@localhost iscsi]# iscsiadm -m -t st -p 192.168.239.146 --login
    Try `iscsiadm --help' for more information.
    [root@localhost iscsi]# history
        1  hostname
        2  hostnamectl set-hostname iscsi_client
        3  hostname
        4  yum install -y iscsi-initiator-utils
        5  systemctl stop firewalld
        6  targetcli
        7  yum install -y targetcli
        8  targetcli
        9  cat /etc/iscsi/initiatorname.iscsi
       10  iscsi
       11  hostname
       12  yum install -y iscsi-initiator-utils
       13  cd /etc/iscsi/
       14  cat initiatorname.iscsi
       15  systemctl restart iscsi
       16  iscsiadm -m -t st -p 192.168.239.146 --login
       17  yum install -y iscsi-initiator-utils
       18  cd
       19  iscsiadm -m -t st -p 192.168.239.146 --login
       20  iscsiadm -m session
       21  lsblk
       22  systemctl start iscsi
       23  iscsiadm -m session
       24  iscsiadm -m -t st -p 192.168.239.146 --login
       25  lsblk
       26  history
       27  cd /etc/iscsi/
       28  cat initiatorname.iscsi
       29  iscsiadm -m discovery -t st -p 192.168.239.146
       30  lsblk
       31  fdisk -l
       32  lsblk
       33  iscsiadm -m discovery -t st -p 192.168.239.146 --login
       34  lsblk
       35  fdisk -l
       36  fdisk /dev/sdb
       37  fdisk -l
       38  mkdir /mnt/disk-1
       39  mkfs.ext4 /dev/sdb
       40  mount /dev/sdb1 /mnt/disk-1/
       41  mount /dev/sdb /mnt/disk-1/
       42  lsblk
       43  mount /dev/sdh1 /mnt/disk-1/
       44  iscsiadm -m -t st -p 192.168.239.146 --login
       45  history
    [root@localhost iscsi]#
