root@192.168.239.146's password:
    ┌──────────────────────────────────────────────────────────────────────┐
    │                 • MobaXterm Personal Edition v23.1 •                 │
    │               (SSH client, X server and network tools)               │
    │                                                                      │
    │ ⮞ SSH session to root@192.168.239.146                                │
    │   • Direct SSH      :  ✓                                             │
    │   • SSH compression :  ✓                                             │
    │   • SSH-browser     :  ✓                                             │
    │   • X11-forwarding  :  ✗  (disabled or not supported by server)      │
    │                                                                      │
    │ ⮞ For more info, ctrl+click on help or visit our website.            │
    └──────────────────────────────────────────────────────────────────────┘

Last login: Fri Jul 14 22:38:16 2023

    [root@localhost ~]# lsblk
    NAME            MAJ:MIN RM  SIZE RO TYPE MOUNTPOINT
    sda               8:0    0   20G  0 disk
    ├─sda1            8:1    0    1G  0 part /boot
    └─sda2            8:2    0   19G  0 part
      ├─centos-root 253:0    0   17G  0 lvm  /
      └─centos-swap 253:1    0    2G  0 lvm  [SWAP]
    sdb               8:16   0   20G  0 disk
    sdc               8:32   0   20G  0 disk
    sdd               8:48   0   20G  0 disk
    sde               8:64   0   20G  0 disk
    sr0              11:0    1  973M  0 rom
    [root@localhost ~]# pvcreate
      No command with matching syntax recognised.  Run 'pvcreate --help' for more in                         formation.
      Correct command syntax is:
      pvcreate PV ...

    
    [root@localhost ~]# pvcreate /dev/sdb /dev/sdc /dev/sdd /dev/sde
      Physical volume "/dev/sdb" successfully created.
      Physical volume "/dev/sdc" successfully created.
      Physical volume "/dev/sdd" successfully created.
      Physical volume "/dev/sde" successfully created.
    [root@localhost ~]# vgcreate vg_iscsi /dev/sdb /dev/sdc /dev/sdd /dev/sde
      Volume group "vg_iscsi" successfully created
    [root@localhost ~]# lvcreate -n lv_iscsi-disk-01 -L 1G vg_iscsi
      Logical volume "lv_iscsi-disk-01" created.
    [root@localhost ~]# lvs
      LV               VG       Attr       LSize   Pool Origin Data%  Meta%  Move Lo                         g Cpy%Sync Convert
      root             centos   -wi-ao---- <17.00g                                                           
      swap             centos   -wi-ao----   2.00g                                                           
      lv_iscsi-disk-01 vg_iscsi -wi-a-----   1.00g                                                           
    [root@localhost ~]# lvcreate -n lv_iscsi-disk-02 -L 1G vg_iscsi
      Logical volume "lv_iscsi-disk-02" created.
    [root@localhost ~]# yum install -y targetcli
    Loaded plugins: fastestmirror
    Determining fastest mirrors
     * base: centos.mirror.net.in
     * extras: centos.mirror.net.in
     * updates: centos.mirror.net.in
    base                                                     | 3.6 kB     00:00
    extras                                                   | 2.9 kB     00:00
    updates                                                  | 2.9 kB     00:00
    (1/4): base/7/x86_64/group_gz                              | 153 kB   00:00
    (2/4): extras/7/x86_64/primary_db                          | 250 kB   00:00
    (3/4): updates/7/x86_64/primary_db                         |  22 MB   00:00
    (4/4): base/7/x86_64/primary_db                            | 6.1 MB   00:02
    Resolving Dependencies
    --> Running transaction check
    ---> Package targetcli.noarch 0:2.1.53-1.el7_9 will be installed
    --> Processing Dependency: python-rtslib >= 2.1.fb41 for package: targetcli-2.1.                         53-1.el7_9.noarch
    --> Processing Dependency: python-ethtool for package: targetcli-2.1.53-1.el7_9.                         noarch
    --> Processing Dependency: python-configshell for package: targetcli-2.1.53-1.el                         7_9.noarch
    --> Running transaction check
    ---> Package python-configshell.noarch 1:1.1.26-1.el7 will be installed
    --> Processing Dependency: python-urwid for package: 1:python-configshell-1.1.26                         -1.el7.noarch
    --> Processing Dependency: python-six for package: 1:python-configshell-1.1.26-1                         .el7.noarch
    --> Processing Dependency: pyparsing for package: 1:python-configshell-1.1.26-1.                         el7.noarch
    ---> Package python-ethtool.x86_64 0:0.8-8.el7 will be installed
    --> Processing Dependency: libnl.so.1()(64bit) for package: python-ethtool-0.8-8                         .el7.x86_64
    ---> Package python-rtslib.noarch 0:2.1.74-1.el7_9 will be installed
    --> Processing Dependency: python-kmod for package: python-rtslib-2.1.74-1.el7_9                         .noarch
    --> Running transaction check
    ---> Package libnl.x86_64 0:1.1.4-3.el7 will be installed
    ---> Package pyparsing.noarch 0:1.5.6-9.el7 will be installed
    ---> Package python-kmod.x86_64 0:0.9-4.el7 will be installed
    ---> Package python-six.noarch 0:1.9.0-2.el7 will be installed
    ---> Package python-urwid.x86_64 0:1.1.1-3.el7 will be installed
    --> Finished Dependency Resolution
    
    Dependencies Resolved
    
    ================================================================================
     Package                  Arch         Version              Repository     Size
    ================================================================================
    Installing:
     targetcli                noarch       2.1.53-1.el7_9       updates        75 k
    Installing for dependencies:
     libnl                    x86_64       1.1.4-3.el7          base          128 k
     pyparsing                noarch       1.5.6-9.el7          base           94 k
     python-configshell       noarch       1:1.1.26-1.el7       base           68 k
     python-ethtool           x86_64       0.8-8.el7            base           34 k
     python-kmod              x86_64       0.9-4.el7            base           57 k
     python-rtslib            noarch       2.1.74-1.el7_9       updates       104 k
     python-six               noarch       1.9.0-2.el7          base           29 k
     python-urwid             x86_64       1.1.1-3.el7          base          654 k
    
    Transaction Summary
    ================================================================================
    Install  1 Package (+8 Dependent packages)
    
    Total download size: 1.2 M
    Installed size: 5.2 M
    Downloading packages:
    warning: /var/cache/yum/x86_64/7/base/packages/pyparsing-1.5.6-9.el7.noarch.rpm:                          Header V3 RSA/SHA256 Signature, key ID f4a80eb5: NOKEY
    Public key for pyparsing-1.5.6-9.el7.noarch.rpm is not installed
    (1/9): pyparsing-1.5.6-9.el7.noarch.rpm                    |  94 kB   00:00
    (2/9): libnl-1.1.4-3.el7.x86_64.rpm                        | 128 kB   00:00
    (3/9): python-configshell-1.1.26-1.el7.noarch.rpm          |  68 kB   00:00
    (4/9): python-ethtool-0.8-8.el7.x86_64.rpm                 |  34 kB   00:00
    (5/9): python-kmod-0.9-4.el7.x86_64.rpm                    |  57 kB   00:00
    (6/9): python-six-1.9.0-2.el7.noarch.rpm                   |  29 kB   00:00
    Public key for targetcli-2.1.53-1.el7_9.noarch.rpm is not installed
    (7/9): targetcli-2.1.53-1.el7_9.noarch.rpm                 |  75 kB   00:00
    (8/9): python-rtslib-2.1.74-1.el7_9.noarch.rpm             | 104 kB   00:00
    (9/9): python-urwid-1.1.1-3.el7.x86_64.rpm                 | 654 kB   00:00
    --------------------------------------------------------------------------------
    Total                                              3.1 MB/s | 1.2 MB  00:00
    Retrieving key from file:///etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7
    Importing GPG key 0xF4A80EB5:
     Userid     : "CentOS-7 Key (CentOS 7 Official Signing Key) <security@centos.org                         >"
     Fingerprint: 6341 ab27 53d7 8a78 a7c2 7bb1 24c6 a8a7 f4a8 0eb5
     Package    : centos-release-7-9.2009.0.el7.centos.x86_64 (@anaconda)
     From       : /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7
    Running transaction check
    Running transaction test
    Transaction test succeeded
    Running transaction
      Installing : python-six-1.9.0-2.el7.noarch                                1/9
      Installing : pyparsing-1.5.6-9.el7.noarch                                 2/9
      Installing : python-kmod-0.9-4.el7.x86_64                                 3/9
      Installing : python-rtslib-2.1.74-1.el7_9.noarch                          4/9
      Installing : libnl-1.1.4-3.el7.x86_64                                     5/9
      Installing : python-ethtool-0.8-8.el7.x86_64                              6/9
      Installing : python-urwid-1.1.1-3.el7.x86_64                              7/9
      Installing : 1:python-configshell-1.1.26-1.el7.noarch                     8/9
      Installing : targetcli-2.1.53-1.el7_9.noarch                              9/9
      Verifying  : python-urwid-1.1.1-3.el7.x86_64                              1/9
      Verifying  : libnl-1.1.4-3.el7.x86_64                                     2/9
      Verifying  : python-ethtool-0.8-8.el7.x86_64                              3/9
      Verifying  : python-rtslib-2.1.74-1.el7_9.noarch                          4/9
      Verifying  : targetcli-2.1.53-1.el7_9.noarch                              5/9
      Verifying  : python-kmod-0.9-4.el7.x86_64                                 6/9
      Verifying  : python-six-1.9.0-2.el7.noarch                                7/9
      Verifying  : pyparsing-1.5.6-9.el7.noarch                                 8/9
      Verifying  : 1:python-configshell-1.1.26-1.el7.noarch                     9/9
    
    Installed:
      targetcli.noarch 0:2.1.53-1.el7_9
    
    Dependency Installed:
      libnl.x86_64 0:1.1.4-3.el7
      pyparsing.noarch 0:1.5.6-9.el7
      python-configshell.noarch 1:1.1.26-1.el7
      python-ethtool.x86_64 0:0.8-8.el7
      python-kmod.x86_64 0:0.9-4.el7
      python-rtslib.noarch 0:2.1.74-1.el7_9
      python-six.noarch 0:1.9.0-2.el7
      python-urwid.x86_64 0:1.1.1-3.el7
    
    Complete!
    [root@localhost ~]# systemctl stop firewalld
    [root@localhost ~]# targetcli
    Warning: Could not load preferences file /root/.targetcli/prefs.bin.
    targetcli shell version 2.1.53
    Copyright 2011-2013 by Datera, Inc and others.
    For help on commands, type 'help'.
    
    /> cd backstore/block
    No such path /backstore
    /> cd backstores/block
    /backstores/block> cd ..
    /backstores> ls
    o- backstores ............................................................ [...]
      o- block ................................................ [Storage Objects: 0]
      o- fileio ............................................... [Storage Objects: 0]
      o- pscsi ................................................ [Storage Objects: 0]
      o- ramdisk .............................................. [Storage Objects: 0]
    /backstores> cd iscsi
    No such path /backstores/iscsi
    /backstores> cd
    
    /iscsi> create ign.2023-07.siddhu.cdac.sbm:disk1
    WWN not valid as: iqn, naa, eui
    /iscsi> create iqn.2023-07.siddhu.cdac.sbm:disk1
    Created target iqn.2023-07.siddhu.cdac.sbm:disk1.
    Created TPG 1.
    Global pref auto_add_default_portal=true
    Created default portal listening on all IPs (0.0.0.0), port 3260.
    /iscsi> cd iqn.2023-07.siddhu.cdac.sbm:disk1/
    /iscsi/iqn.20...dac.sbm:disk1> cd
    
    /iscsi/iqn.20...dac.sbm:disk1> cd..
    /iscsi> cd ..
    /> ls
    o- / ..................................................................... [...]
      o- backstores .......................................................... [...]
      | o- block .............................................. [Storage Objects: 0]
      | o- fileio ............................................. [Storage Objects: 0]
      | o- pscsi .............................................. [Storage Objects: 0]
      | o- ramdisk ............................................ [Storage Objects: 0]
      o- iscsi ........................................................ [Targets: 1]
      | o- iqn.2023-07.siddhu.cdac.sbm:disk1 ............................. [TPGs: 1]
      |   o- tpg1 ........................................... [no-gen-acls, no-auth]
      |     o- acls ...................................................... [ACLs: 0]
      |     o- luns ...................................................... [LUNs: 0]
      |     o- portals ................................................ [Portals: 1]
      |       o- 0.0.0.0:3260 ................................................. [OK]
      o- loopback ..................................................... [Targets: 0]
    /> exit
    Global pref auto_save_on_exit=true
    Configuration saved to /etc/target/saveconfig.json
    [root@localhost ~]# systemctl restart targetcli
    Failed to restart targetcli.service: Unit not found.
    [root@localhost ~]# systemctl restart target
    [root@localhost ~]# systemctl status target
    ● target.service - Restore LIO kernel target configuration
       Loaded: loaded (/usr/lib/systemd/system/target.service; disabled; vendor pres                         et: disabled)
       Active: active (exited) since Fri 2023-07-14 23:08:30 IST; 9s ago
      Process: 1601 ExecStart=/usr/bin/targetctl restore (code=exited, status=0/SUCC                         ESS)
     Main PID: 1601 (code=exited, status=0/SUCCESS)
    
    Jul 14 23:08:30 localhost.localdomain systemd[1]: Starting Restore LIO kernel...
    Jul 14 23:08:30 localhost.localdomain systemd[1]: Started Restore LIO kernel ...
    Hint: Some lines were ellipsized, use -l to show in full.
    [root@localhost ~]# hostname
    localhost.localdomain
    [root@localhost ~]# hostnamectl set-hostname iscsi_server
    [root@localhost ~]# hostname
    iscsi_server
    [root@localhost ~]# targetcli
    targetcli shell version 2.1.53
    Copyright 2011-2013 by Datera, Inc and others.
    For help on commands, type 'help'.
    
    /> ls
    o- / .............................................................................................. [...]
      o- backstores ................................................................................... [...]
      | o- block ....................................................................... [Storage Objects: 0]
      | o- fileio ...................................................................... [Storage Objects: 0]
      | o- pscsi ....................................................................... [Storage Objects: 0]
      | o- ramdisk ..................................................................... [Storage Objects: 0]
      o- iscsi ................................................................................. [Targets: 1]
      | o- iqn.2023-07.siddhu.cdac.sbm:disk1 ...................................................... [TPGs: 1]
      |   o- tpg1 .................................................................... [no-gen-acls, no-auth]
      |     o- acls ............................................................................... [ACLs: 0]
      |     o- luns ............................................................................... [LUNs: 0]
      |     o- portals ......................................................................... [Portals: 1]
      |       o- 0.0.0.0:3260 .......................................................................... [OK]
      o- loopback .............................................................................. [Targets: 0]
    /> cd backstores/block
    /backstores/block> create block1 /dev/mapper/vg_iscsi-lv_iscsi--disk--0
    /dev/mapper/vg_iscsi-lv_iscsi--disk--01  /dev/mapper/vg_iscsi-lv_iscsi--disk--02
    /backstores/block> create block1 /dev/mapper/vg_iscsi-lv_iscsi--disk--01
    Created block storage object block1 using /dev/mapper/vg_iscsi-lv_iscsi--disk--01.
    /backstores/block> cd ..
    /backstores> cd ..
    /> cd iscsi
    /iscsi> ls
    o- iscsi ................................................................................... [Targets: 1]
      o- iqn.2023-07.siddhu.cdac.sbm:disk1 ........................................................ [TPGs: 1]
        o- tpg1 ...................................................................... [no-gen-acls, no-auth]
          o- acls ................................................................................. [ACLs: 0]
          o- luns ................................................................................. [LUNs: 0]
          o- portals ........................................................................... [Portals: 1]
            o- 0.0.0.0:3260 ............................................................................ [OK]
    /iscsi> cd iqn.2023-07.siddhu.cdac.sbm:disk1/tpg1/acls
    /iscsi/iqn.20...sk1/tpg1/acls> create
    Missing required parameter wwn
    /iscsi/iqn.20...sk1/tpg1/acls> create iqn.1994-05.com.redhat:b4d9b7267f7
    Created Node ACL for iqn.1994-05.com.redhat:b4d9b7267f7
    /iscsi/iqn.20...sk1/tpg1/acls> cd /iscsi/iqn.2023-07.siddhu.cdac.sbm:disk1/tpg1/luns
    /iscsi/iqn.20...sk1/tpg1/luns> create /backstores/block/block1
    Created LUN 0.
    Created LUN 0->0 mapping in node ACL iqn.1994-05.com.redhat:b4d9b7267f7
    /iscsi/iqn.20...sk1/tpg1/luns> exit
    Global pref auto_save_on_exit=true
    Last 10 configs saved in /etc/target/backup/.
    Configuration saved to /etc/target/saveconfig.json
    [root@localhost ~]# systemctl restart target
    [root@localhost ~]# systemctl status target
    ● target.service - Restore LIO kernel target configuration
       Loaded: loaded (/usr/lib/systemd/system/target.service; disabled; vendor preset: disabled)
       Active: active (exited) since Fri 2023-07-14 23:28:05 IST; 10s ago
      Process: 1702 ExecStop=/usr/bin/targetctl clear (code=exited, status=0/SUCCESS)
      Process: 1709 ExecStart=/usr/bin/targetctl restore (code=exited, status=0/SUCCESS)
     Main PID: 1709 (code=exited, status=0/SUCCESS)
    
    Jul 14 23:28:05 iscsi_server systemd[1]: Stopped Restore LIO kernel target configuration.
    Jul 14 23:28:05 iscsi_server systemd[1]: Starting Restore LIO kernel target configuration...
    Jul 14 23:28:05 iscsi_server systemd[1]: Started Restore LIO kernel target configuration.
    [root@localhost ~]# targetcli
    targetcli shell version 2.1.53
    Copyright 2011-2013 by Datera, Inc and others.
    For help on commands, type 'help'.
    
    /iscsi/iqn.20...sk1/tpg1/luns> cd ..
    /iscsi/iqn.20...bm:disk1/tpg1> cd..
    /iscsi/iqn.20...dac.sbm:disk1> cd
    
    /iscsi> cd ..
    /> ls
    o- / .............................................................................................. [...]
      o- backstores ................................................................................... [...]
      | o- block ....................................................................... [Storage Objects: 1]
      | | o- block1 ................. [/dev/mapper/vg_iscsi-lv_iscsi--disk--01 (1.0GiB) write-thru activated]
      | |   o- alua ........................................................................ [ALUA Groups: 1]
      | |     o- default_tg_pt_gp ............................................ [ALUA state: Active/optimized]
      | o- fileio ...................................................................... [Storage Objects: 0]
      | o- pscsi ....................................................................... [Storage Objects: 0]
      | o- ramdisk ..................................................................... [Storage Objects: 0]
      o- iscsi ................................................................................. [Targets: 1]
      | o- iqn.2023-07.siddhu.cdac.sbm:disk1 ...................................................... [TPGs: 1]
      |   o- tpg1 .................................................................... [no-gen-acls, no-auth]
      |     o- acls ............................................................................... [ACLs: 1]
      |     | o- iqn.1994-05.com.redhat:b4d9b7267f7 ........................................ [Mapped LUNs: 1]
      |     |   o- mapped_lun0 ..................................................... [lun0 block/block1 (rw)]
      |     o- luns ............................................................................... [LUNs: 1]
      |     | o- lun0 ........... [block/block1 (/dev/mapper/vg_iscsi-lv_iscsi--disk--01) (default_tg_pt_gp)]
      |     o- portals ......................................................................... [Portals: 1]
      |       o- 0.0.0.0:3260 .......................................................................... [OK]
      o- loopback .............................................................................. [Targets: 0]
    /> exit
    Global pref auto_save_on_exit=true
    Last 10 configs saved in /etc/target/backup/.
    Configuration saved to /etc/target/saveconfig.json
    [root@localhost ~]# history
        1  lsblk
        2  pvcreate
        3  pvcreate /dev/sdb /dev/sdc /dev/sdd /dev/sde
        4  vgcreate vg_iscsi /dev/sdb /dev/sdc /dev/sdd /dev/sde
        5  lvcreate -n lv_iscsi-disk-01 -L 1G vg_iscsi
        6  lvs
        7  lvcreate -n lv_iscsi-disk-02 -L 1G vg_iscsi
        8  yum install -y targetcli
        9  systemctl stop firewalld
       10  targetcli
       11  systemctl restart targetcli
       12  systemctl restart target
       13  systemctl status target
       14  hostname
       15  hostnamectl set-hostname iscsi_server
       16  hostname
       17  targetcli
       18  systemctl restart target
       19  systemctl status target
       20  targetcli
       21  history
    [root@localhost ~]#
