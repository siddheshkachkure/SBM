        ┌──────────────────────────────────────────────────────────────────────┐
        │                 • MobaXterm Personal Edition v23.1 •                 │
        │               (SSH client, X server and network tools)               │
        │                                                                      │
        │ ⮞ SSH session to root@192.168.239.155                                │
        │   • Direct SSH      :  ✓                                             │
        │   • SSH compression :  ✓                                             │
        │   • SSH-browser     :  ✓                                             │
        │   • X11-forwarding  :  ✗  (disabled or not supported by server)      │
        │                                                                      │
        │ ⮞ For more info, ctrl+click on help or visit our website.            │
        └──────────────────────────────────────────────────────────────────────┘
    
    Last login: Sun Jul 16 19:58:44 2023
    [root@ceph2 ~]# hostnamectl set-hostname ceph2.in
    [root@ceph2 ~]# su
    [root@ceph2 ~]# hostname
    ceph2.in
    [root@ceph2 ~]# yum install vim
    Loaded plugins: fastestmirror
    Determining fastest mirrors
     * base: centos.mirror.net.in
     * extras: centos.mirror.net.in
     * updates: centos.mirror.net.in
    base                                                                                           | 3.6 kB  00:00:00
    extras                                                                                         | 2.9 kB  00:00:00
    updates                                                                                        | 2.9 kB  00:00:00
    (1/4): base/7/x86_64/group_gz                                                                  | 153 kB  00:00:00
    (2/4): extras/7/x86_64/primary_db                                                              | 250 kB  00:00:00
    (3/4): updates/7/x86_64/primary_db                                                             |  22 MB  00:00:00
    (4/4): base/7/x86_64/primary_db                                                                | 6.1 MB  00:00:00
    Resolving Dependencies
    --> Running transaction check
    ---> Package vim-enhanced.x86_64 2:7.4.629-8.el7_9 will be installed
    --> Processing Dependency: vim-common = 2:7.4.629-8.el7_9 for package: 2:vim-enhanced-7.4.629-8.el7_9.x86_64
    --> Processing Dependency: perl(:MODULE_COMPAT_5.16.3) for package: 2:vim-enhanced-7.4.629-8.el7_9.x86_64
    --> Processing Dependency: libperl.so()(64bit) for package: 2:vim-enhanced-7.4.629-8.el7_9.x86_64
    --> Processing Dependency: libgpm.so.2()(64bit) for package: 2:vim-enhanced-7.4.629-8.el7_9.x86_64
    --> Running transaction check
    ---> Package gpm-libs.x86_64 0:1.20.7-6.el7 will be installed
    ---> Package perl.x86_64 4:5.16.3-299.el7_9 will be installed
    --> Processing Dependency: perl(Socket) >= 1.3 for package: 4:perl-5.16.3-299.el7_9.x86_64
    --> Processing Dependency: perl(Scalar::Util) >= 1.10 for package: 4:perl-5.16.3-299.el7_9.x86_64
    --> Processing Dependency: perl-macros for package: 4:perl-5.16.3-299.el7_9.x86_64
    --> Processing Dependency: perl(threads::shared) for package: 4:perl-5.16.3-299.el7_9.x86_64
    --> Processing Dependency: perl(threads) for package: 4:perl-5.16.3-299.el7_9.x86_64
    --> Processing Dependency: perl(constant) for package: 4:perl-5.16.3-299.el7_9.x86_64
    --> Processing Dependency: perl(Time::Local) for package: 4:perl-5.16.3-299.el7_9.x86_64
    --> Processing Dependency: perl(Time::HiRes) for package: 4:perl-5.16.3-299.el7_9.x86_64
    --> Processing Dependency: perl(Storable) for package: 4:perl-5.16.3-299.el7_9.x86_64
    --> Processing Dependency: perl(Socket) for package: 4:perl-5.16.3-299.el7_9.x86_64
    --> Processing Dependency: perl(Scalar::Util) for package: 4:perl-5.16.3-299.el7_9.x86_64
    --> Processing Dependency: perl(Pod::Simple::XHTML) for package: 4:perl-5.16.3-299.el7_9.x86_64
    --> Processing Dependency: perl(Pod::Simple::Search) for package: 4:perl-5.16.3-299.el7_9.x86_64
    --> Processing Dependency: perl(Getopt::Long) for package: 4:perl-5.16.3-299.el7_9.x86_64
    --> Processing Dependency: perl(Filter::Util::Call) for package: 4:perl-5.16.3-299.el7_9.x86_64
    --> Processing Dependency: perl(File::Temp) for package: 4:perl-5.16.3-299.el7_9.x86_64
    --> Processing Dependency: perl(File::Spec::Unix) for package: 4:perl-5.16.3-299.el7_9.x86_64
    --> Processing Dependency: perl(File::Spec::Functions) for package: 4:perl-5.16.3-299.el7_9.x86_64
    --> Processing Dependency: perl(File::Spec) for package: 4:perl-5.16.3-299.el7_9.x86_64
    --> Processing Dependency: perl(File::Path) for package: 4:perl-5.16.3-299.el7_9.x86_64
    --> Processing Dependency: perl(Exporter) for package: 4:perl-5.16.3-299.el7_9.x86_64
    --> Processing Dependency: perl(Cwd) for package: 4:perl-5.16.3-299.el7_9.x86_64
    --> Processing Dependency: perl(Carp) for package: 4:perl-5.16.3-299.el7_9.x86_64
    ---> Package perl-libs.x86_64 4:5.16.3-299.el7_9 will be installed
    ---> Package vim-common.x86_64 2:7.4.629-8.el7_9 will be installed
    --> Processing Dependency: vim-filesystem for package: 2:vim-common-7.4.629-8.el7_9.x86_64
    --> Running transaction check
    ---> Package perl-Carp.noarch 0:1.26-244.el7 will be installed
    ---> Package perl-Exporter.noarch 0:5.68-3.el7 will be installed
    ---> Package perl-File-Path.noarch 0:2.09-2.el7 will be installed
    ---> Package perl-File-Temp.noarch 0:0.23.01-3.el7 will be installed
    ---> Package perl-Filter.x86_64 0:1.49-3.el7 will be installed
    ---> Package perl-Getopt-Long.noarch 0:2.40-3.el7 will be installed
    --> Processing Dependency: perl(Pod::Usage) >= 1.14 for package: perl-Getopt-Long-2.40-3.el7.noarch
    --> Processing Dependency: perl(Text::ParseWords) for package: perl-Getopt-Long-2.40-3.el7.noarch
    ---> Package perl-PathTools.x86_64 0:3.40-5.el7 will be installed
    ---> Package perl-Pod-Simple.noarch 1:3.28-4.el7 will be installed
    --> Processing Dependency: perl(Pod::Escapes) >= 1.04 for package: 1:perl-Pod-Simple-3.28-4.el7.noarch
    --> Processing Dependency: perl(Encode) for package: 1:perl-Pod-Simple-3.28-4.el7.noarch
    ---> Package perl-Scalar-List-Utils.x86_64 0:1.27-248.el7 will be installed
    ---> Package perl-Socket.x86_64 0:2.010-5.el7 will be installed
    ---> Package perl-Storable.x86_64 0:2.45-3.el7 will be installed
    ---> Package perl-Time-HiRes.x86_64 4:1.9725-3.el7 will be installed
    ---> Package perl-Time-Local.noarch 0:1.2300-2.el7 will be installed
    ---> Package perl-constant.noarch 0:1.27-2.el7 will be installed
    ---> Package perl-macros.x86_64 4:5.16.3-299.el7_9 will be installed
    ---> Package perl-threads.x86_64 0:1.87-4.el7 will be installed
    ---> Package perl-threads-shared.x86_64 0:1.43-6.el7 will be installed
    ---> Package vim-filesystem.x86_64 2:7.4.629-8.el7_9 will be installed
    --> Running transaction check
    ---> Package perl-Encode.x86_64 0:2.51-7.el7 will be installed
    ---> Package perl-Pod-Escapes.noarch 1:1.04-299.el7_9 will be installed
    ---> Package perl-Pod-Usage.noarch 0:1.63-3.el7 will be installed
    --> Processing Dependency: perl(Pod::Text) >= 3.15 for package: perl-Pod-Usage-1.63-3.el7.noarch
    --> Processing Dependency: perl-Pod-Perldoc for package: perl-Pod-Usage-1.63-3.el7.noarch
    ---> Package perl-Text-ParseWords.noarch 0:3.29-4.el7 will be installed
    --> Running transaction check
    ---> Package perl-Pod-Perldoc.noarch 0:3.20-4.el7 will be installed
    --> Processing Dependency: perl(parent) for package: perl-Pod-Perldoc-3.20-4.el7.noarch
    --> Processing Dependency: perl(HTTP::Tiny) for package: perl-Pod-Perldoc-3.20-4.el7.noarch
    ---> Package perl-podlators.noarch 0:2.5.1-3.el7 will be installed
    --> Running transaction check
    ---> Package perl-HTTP-Tiny.noarch 0:0.033-3.el7 will be installed
    ---> Package perl-parent.noarch 1:0.225-244.el7 will be installed
    --> Finished Dependency Resolution
    
    Dependencies Resolved
    
    ======================================================================================================================
     Package                             Arch                Version                           Repository            Size
    ======================================================================================================================
    Installing:
     vim-enhanced                        x86_64              2:7.4.629-8.el7_9                 updates              1.1 M
    Installing for dependencies:
     gpm-libs                            x86_64              1.20.7-6.el7                      base                  32 k
     perl                                x86_64              4:5.16.3-299.el7_9                updates              8.0 M
     perl-Carp                           noarch              1.26-244.el7                      base                  19 k
     perl-Encode                         x86_64              2.51-7.el7                        base                 1.5 M
     perl-Exporter                       noarch              5.68-3.el7                        base                  28 k
     perl-File-Path                      noarch              2.09-2.el7                        base                  26 k
     perl-File-Temp                      noarch              0.23.01-3.el7                     base                  56 k
     perl-Filter                         x86_64              1.49-3.el7                        base                  76 k
     perl-Getopt-Long                    noarch              2.40-3.el7                        base                  56 k
     perl-HTTP-Tiny                      noarch              0.033-3.el7                       base                  38 k
     perl-PathTools                      x86_64              3.40-5.el7                        base                  82 k
     perl-Pod-Escapes                    noarch              1:1.04-299.el7_9                  updates               52 k
     perl-Pod-Perldoc                    noarch              3.20-4.el7                        base                  87 k
     perl-Pod-Simple                     noarch              1:3.28-4.el7                      base                 216 k
     perl-Pod-Usage                      noarch              1.63-3.el7                        base                  27 k
     perl-Scalar-List-Utils              x86_64              1.27-248.el7                      base                  36 k
     perl-Socket                         x86_64              2.010-5.el7                       base                  49 k
     perl-Storable                       x86_64              2.45-3.el7                        base                  77 k
     perl-Text-ParseWords                noarch              3.29-4.el7                        base                  14 k
     perl-Time-HiRes                     x86_64              4:1.9725-3.el7                    base                  45 k
     perl-Time-Local                     noarch              1.2300-2.el7                      base                  24 k
     perl-constant                       noarch              1.27-2.el7                        base                  19 k
     perl-libs                           x86_64              4:5.16.3-299.el7_9                updates              690 k
     perl-macros                         x86_64              4:5.16.3-299.el7_9                updates               44 k
     perl-parent                         noarch              1:0.225-244.el7                   base                  12 k
     perl-podlators                      noarch              2.5.1-3.el7                       base                 112 k
     perl-threads                        x86_64              1.87-4.el7                        base                  49 k
     perl-threads-shared                 x86_64              1.43-6.el7                        base                  39 k
     vim-common                          x86_64              2:7.4.629-8.el7_9                 updates              5.9 M
     vim-filesystem                      x86_64              2:7.4.629-8.el7_9                 updates               11 k
    
    Transaction Summary
    ======================================================================================================================
    Install  1 Package (+30 Dependent packages)
    
    Total download size: 18 M
    Installed size: 60 M
    Is this ok [y/d/N]: y
    Downloading packages:
    warning: /var/cache/yum/x86_64/7/base/packages/gpm-libs-1.20.7-6.el7.x86_64.rpm: Header V3 RSA/SHA256 Signature, key ID f4a80eb5: NOKEY
    Public key for gpm-libs-1.20.7-6.el7.x86_64.rpm is not installed
    (1/31): gpm-libs-1.20.7-6.el7.x86_64.rpm                                                       |  32 kB  00:00:01
    (2/31): perl-Carp-1.26-244.el7.noarch.rpm                                                      |  19 kB  00:00:01
    (3/31): perl-Exporter-5.68-3.el7.noarch.rpm                                                    |  28 kB  00:00:00
    (4/31): perl-File-Path-2.09-2.el7.noarch.rpm                                                   |  26 kB  00:00:00
    (5/31): perl-File-Temp-0.23.01-3.el7.noarch.rpm                                                |  56 kB  00:00:00
    (6/31): perl-Filter-1.49-3.el7.x86_64.rpm                                                      |  76 kB  00:00:00
    (7/31): perl-Getopt-Long-2.40-3.el7.noarch.rpm                                                 |  56 kB  00:00:00
    (8/31): perl-HTTP-Tiny-0.033-3.el7.noarch.rpm                                                  |  38 kB  00:00:00
    (9/31): perl-PathTools-3.40-5.el7.x86_64.rpm                                                   |  82 kB  00:00:00
    (10/31): perl-Pod-Perldoc-3.20-4.el7.noarch.rpm                                                |  87 kB  00:00:00
    Public key for perl-Pod-Escapes-1.04-299.el7_9.noarch.rpm is not installed
    (11/31): perl-Pod-Escapes-1.04-299.el7_9.noarch.rpm                                            |  52 kB  00:00:00
    (12/31): perl-Pod-Simple-3.28-4.el7.noarch.rpm                                                 | 216 kB  00:00:00
    (13/31): perl-Pod-Usage-1.63-3.el7.noarch.rpm                                                  |  27 kB  00:00:00
    (14/31): perl-Scalar-List-Utils-1.27-248.el7.x86_64.rpm                                        |  36 kB  00:00:00
    (15/31): perl-Socket-2.010-5.el7.x86_64.rpm                                                    |  49 kB  00:00:00
    (16/31): perl-Storable-2.45-3.el7.x86_64.rpm                                                   |  77 kB  00:00:00
    (17/31): perl-Text-ParseWords-3.29-4.el7.noarch.rpm                                            |  14 kB  00:00:00
    (18/31): perl-Time-HiRes-1.9725-3.el7.x86_64.rpm                                               |  45 kB  00:00:00
    (19/31): perl-Time-Local-1.2300-2.el7.noarch.rpm                                               |  24 kB  00:00:00
    (20/31): perl-constant-1.27-2.el7.noarch.rpm                                                   |  19 kB  00:00:00
    (21/31): perl-Encode-2.51-7.el7.x86_64.rpm                                                     | 1.5 MB  00:00:00
    (22/31): perl-libs-5.16.3-299.el7_9.x86_64.rpm                                                 | 690 kB  00:00:00
    (23/31): perl-macros-5.16.3-299.el7_9.x86_64.rpm                                               |  44 kB  00:00:00
    (24/31): perl-parent-0.225-244.el7.noarch.rpm                                                  |  12 kB  00:00:00
    (25/31): perl-podlators-2.5.1-3.el7.noarch.rpm                                                 | 112 kB  00:00:00
    (26/31): perl-threads-1.87-4.el7.x86_64.rpm                                                    |  49 kB  00:00:00
    (27/31): perl-threads-shared-1.43-6.el7.x86_64.rpm                                             |  39 kB  00:00:00
    (28/31): perl-5.16.3-299.el7_9.x86_64.rpm                                                      | 8.0 MB  00:00:02
    (29/31): vim-enhanced-7.4.629-8.el7_9.x86_64.rpm                                               | 1.1 MB  00:00:00
    (30/31): vim-filesystem-7.4.629-8.el7_9.x86_64.rpm                                             |  11 kB  00:00:00
    (31/31): vim-common-7.4.629-8.el7_9.x86_64.rpm                                                 | 5.9 MB  00:00:00
    ----------------------------------------------------------------------------------------------------------------------
    Total                                                                                 5.4 MB/s |  18 MB  00:00:03
    Retrieving key from file:///etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7
    Importing GPG key 0xF4A80EB5:
     Userid     : "CentOS-7 Key (CentOS 7 Official Signing Key) <security@centos.org>"
     Fingerprint: 6341 ab27 53d7 8a78 a7c2 7bb1 24c6 a8a7 f4a8 0eb5
     Package    : centos-release-7-9.2009.0.el7.centos.x86_64 (@anaconda)
     From       : /etc/pki/rpm-gpg/RPM-GPG-KEY-CentOS-7
    Is this ok [y/N]: y
    Running transaction check
    Running transaction test
    Transaction test succeeded
    Running transaction
      Installing : 1:perl-parent-0.225-244.el7.noarch                                                                1/31
      Installing : perl-HTTP-Tiny-0.033-3.el7.noarch                                                                 2/31
      Installing : perl-podlators-2.5.1-3.el7.noarch                                                                 3/31
      Installing : perl-Pod-Perldoc-3.20-4.el7.noarch                                                                4/31
      Installing : 1:perl-Pod-Escapes-1.04-299.el7_9.noarch                                                          5/31
      Installing : perl-Encode-2.51-7.el7.x86_64                                                                     6/31
      Installing : perl-Text-ParseWords-3.29-4.el7.noarch                                                            7/31
      Installing : perl-Pod-Usage-1.63-3.el7.noarch                                                                  8/31
      Installing : 4:perl-macros-5.16.3-299.el7_9.x86_64                                                             9/31
      Installing : perl-Storable-2.45-3.el7.x86_64                                                                  10/31
      Installing : perl-Exporter-5.68-3.el7.noarch                                                                  11/31
      Installing : perl-constant-1.27-2.el7.noarch                                                                  12/31
      Installing : perl-Socket-2.010-5.el7.x86_64                                                                   13/31
      Installing : perl-Time-Local-1.2300-2.el7.noarch                                                              14/31
      Installing : perl-Carp-1.26-244.el7.noarch                                                                    15/31
      Installing : perl-PathTools-3.40-5.el7.x86_64                                                                 16/31
      Installing : perl-Scalar-List-Utils-1.27-248.el7.x86_64                                                       17/31
      Installing : 1:perl-Pod-Simple-3.28-4.el7.noarch                                                              18/31
      Installing : perl-File-Temp-0.23.01-3.el7.noarch                                                              19/31
      Installing : perl-File-Path-2.09-2.el7.noarch                                                                 20/31
      Installing : perl-threads-shared-1.43-6.el7.x86_64                                                            21/31
      Installing : perl-threads-1.87-4.el7.x86_64                                                                   22/31
      Installing : 4:perl-Time-HiRes-1.9725-3.el7.x86_64                                                            23/31
      Installing : perl-Filter-1.49-3.el7.x86_64                                                                    24/31
      Installing : 4:perl-libs-5.16.3-299.el7_9.x86_64                                                              25/31
      Installing : perl-Getopt-Long-2.40-3.el7.noarch                                                               26/31
      Installing : 4:perl-5.16.3-299.el7_9.x86_64                                                                   27/31
      Installing : gpm-libs-1.20.7-6.el7.x86_64                                                                     28/31
      Installing : 2:vim-filesystem-7.4.629-8.el7_9.x86_64                                                          29/31
      Installing : 2:vim-common-7.4.629-8.el7_9.x86_64                                                              30/31
      Installing : 2:vim-enhanced-7.4.629-8.el7_9.x86_64                                                            31/31
      Verifying  : perl-HTTP-Tiny-0.033-3.el7.noarch                                                                 1/31
      Verifying  : perl-threads-shared-1.43-6.el7.x86_64                                                             2/31
      Verifying  : perl-Storable-2.45-3.el7.x86_64                                                                   3/31
      Verifying  : perl-Exporter-5.68-3.el7.noarch                                                                   4/31
      Verifying  : perl-constant-1.27-2.el7.noarch                                                                   5/31
      Verifying  : perl-PathTools-3.40-5.el7.x86_64                                                                  6/31
      Verifying  : 4:perl-macros-5.16.3-299.el7_9.x86_64                                                             7/31
      Verifying  : 2:vim-enhanced-7.4.629-8.el7_9.x86_64                                                             8/31
      Verifying  : 1:perl-parent-0.225-244.el7.noarch                                                                9/31
      Verifying  : perl-Socket-2.010-5.el7.x86_64                                                                   10/31
      Verifying  : 2:vim-filesystem-7.4.629-8.el7_9.x86_64                                                          11/31
      Verifying  : perl-File-Temp-0.23.01-3.el7.noarch                                                              12/31
      Verifying  : 1:perl-Pod-Simple-3.28-4.el7.noarch                                                              13/31
      Verifying  : perl-Time-Local-1.2300-2.el7.noarch                                                              14/31
      Verifying  : 1:perl-Pod-Escapes-1.04-299.el7_9.noarch                                                         15/31
      Verifying  : perl-Carp-1.26-244.el7.noarch                                                                    16/31
      Verifying  : 2:vim-common-7.4.629-8.el7_9.x86_64                                                              17/31
      Verifying  : perl-Scalar-List-Utils-1.27-248.el7.x86_64                                                       18/31
      Verifying  : perl-Pod-Usage-1.63-3.el7.noarch                                                                 19/31
      Verifying  : perl-Encode-2.51-7.el7.x86_64                                                                    20/31
      Verifying  : perl-Pod-Perldoc-3.20-4.el7.noarch                                                               21/31
      Verifying  : perl-podlators-2.5.1-3.el7.noarch                                                                22/31
      Verifying  : 4:perl-5.16.3-299.el7_9.x86_64                                                                   23/31
      Verifying  : perl-File-Path-2.09-2.el7.noarch                                                                 24/31
      Verifying  : perl-threads-1.87-4.el7.x86_64                                                                   25/31
      Verifying  : 4:perl-Time-HiRes-1.9725-3.el7.x86_64                                                            26/31
      Verifying  : gpm-libs-1.20.7-6.el7.x86_64                                                                     27/31
      Verifying  : perl-Filter-1.49-3.el7.x86_64                                                                    28/31
      Verifying  : perl-Getopt-Long-2.40-3.el7.noarch                                                               29/31
      Verifying  : perl-Text-ParseWords-3.29-4.el7.noarch                                                           30/31
      Verifying  : 4:perl-libs-5.16.3-299.el7_9.x86_64                                                              31/31
    
    Installed:
      vim-enhanced.x86_64 2:7.4.629-8.el7_9
    
    Dependency Installed:
      gpm-libs.x86_64 0:1.20.7-6.el7                          perl.x86_64 4:5.16.3-299.el7_9
      perl-Carp.noarch 0:1.26-244.el7                         perl-Encode.x86_64 0:2.51-7.el7
      perl-Exporter.noarch 0:5.68-3.el7                       perl-File-Path.noarch 0:2.09-2.el7
      perl-File-Temp.noarch 0:0.23.01-3.el7                   perl-Filter.x86_64 0:1.49-3.el7
      perl-Getopt-Long.noarch 0:2.40-3.el7                    perl-HTTP-Tiny.noarch 0:0.033-3.el7
      perl-PathTools.x86_64 0:3.40-5.el7                      perl-Pod-Escapes.noarch 1:1.04-299.el7_9
      perl-Pod-Perldoc.noarch 0:3.20-4.el7                    perl-Pod-Simple.noarch 1:3.28-4.el7
      perl-Pod-Usage.noarch 0:1.63-3.el7                      perl-Scalar-List-Utils.x86_64 0:1.27-248.el7
      perl-Socket.x86_64 0:2.010-5.el7                        perl-Storable.x86_64 0:2.45-3.el7
      perl-Text-ParseWords.noarch 0:3.29-4.el7                perl-Time-HiRes.x86_64 4:1.9725-3.el7
      perl-Time-Local.noarch 0:1.2300-2.el7                   perl-constant.noarch 0:1.27-2.el7
      perl-libs.x86_64 4:5.16.3-299.el7_9                     perl-macros.x86_64 4:5.16.3-299.el7_9
      perl-parent.noarch 1:0.225-244.el7                      perl-podlators.noarch 0:2.5.1-3.el7
      perl-threads.x86_64 0:1.87-4.el7                        perl-threads-shared.x86_64 0:1.43-6.el7
      vim-common.x86_64 2:7.4.629-8.el7_9                     vim-filesystem.x86_64 2:7.4.629-8.el7_9
    
    Complete!
    [root@ceph2 ~]# vim /etc/hosts
    [root@ceph2 ~]# cat /etc/hosts
    127.0.0.1   localhost localhost.localdomain localhost4 localhost4.localdomain4
    ::1         localhost localhost.localdomain localhost6 localhost6.localdomain6
    192.168.239.154 ceph1.in
    192.168.239.155 ceph2.in
    192.168.239.156 ceph3.in
    192.168.239.157 ceph4.in
    192.168.239.158 ceph5.in
    
    [root@ceph2 ~]# systemctl stop firewalld
    [root@ceph2 ~]# systemctl disable firewalld
    Removed symlink /etc/systemd/system/multi-user.target.wants/firewalld.service.
    Removed symlink /etc/systemd/system/dbus-org.fedoraproject.FirewallD1.service.
    [root@ceph2 ~]# vim /etc/selinux/config
    [root@ceph2 ~]# cat /etc/selinux/config
    
    # This file controls the state of SELinux on the system.
    # SELINUX= can take one of these three values:
    #     enforcing - SELinux security policy is enforced.
    #     permissive - SELinux prints warnings instead of enforcing.
    #     disabled - No SELinux policy is loaded.
    SELINUX=disbaled
    # SELINUXTYPE= can take one of three values:
    #     targeted - Targeted processes are protected,
    #     minimum - Modification of targeted policy. Only selected processes are protected.
    #     mls - Multi Level Security protection.
    SELINUXTYPE=targeted
    
    
    [root@ceph2 ~]# getenforce
    Enforcing
    [root@ceph2 ~]# setenfroce 0
    bash: setenfroce: command not found
    [root@ceph2 ~]# setenforce 0
    [root@ceph2 ~]# getenforce
    Permissive
    [root@ceph2 ~]# yum install chrony -y
    Loaded plugins: fastestmirror
    Loading mirror speeds from cached hostfile
     * base: centos.mirror.net.in
     * extras: centos.mirror.net.in
     * updates: centos.mirror.net.in
    Package chrony-3.4-1.el7.x86_64 already installed and latest version
    Nothing to do
    [root@ceph2 ~]# chronyc sourcestats
    210 Number of sources = 4
    Name/IP Address            NP  NR  Span  Frequency  Freq Skew  Offset  Std Dev
    ==============================================================================
    static.15.192.216.95.cli>   0   0     0     +0.000   2000.000     +0ns  4000ms
    139.59.15.185               0   0     0     +0.000   2000.000     +0ns  4000ms
    ntpd-rs.sidnlabs.nl         0   0     0     +0.000   2000.000     +0ns  4000ms
    ntp.nic.in                  0   0     0     +0.000   2000.000     +0ns  4000ms
    [root@ceph2 ~]# useradd cephadm && echo "siddhu" | passwd --stdin cephadm
    Changing password for user cephadm.
    passwd: all authentication tokens updated successfully.
    [root@ceph2 ~]# echo "cephadm ALL = (root) NOPASSWD:ALL" | sudo tee /etc/sudoers.d/cephadm
    cephadm ALL = (root) NOPASSWD:ALL
    [root@ceph2 ~]# chmod 0440 /etc/sudoers.d/cephadm
    [root@ceph2 ~]# sudo yum install -y https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm
    Loaded plugins: fastestmirror
    epel-release-latest-7.noarch.rpm                                                               |  15 kB  00:00:00
    Examining /var/tmp/yum-root-WnqvfK/epel-release-latest-7.noarch.rpm: epel-release-7-14.noarch
    Marking /var/tmp/yum-root-WnqvfK/epel-release-latest-7.noarch.rpm to be installed
    Resolving Dependencies
    --> Running transaction check
    ---> Package epel-release.noarch 0:7-14 will be installed
    --> Finished Dependency Resolution
    
    Dependencies Resolved
    
    ======================================================================================================================
     Package                    Arch                 Version            Repository                                   Size
    ======================================================================================================================
    Installing:
     epel-release               noarch               7-14               /epel-release-latest-7.noarch                25 k
    
    Transaction Summary
    ======================================================================================================================
    Install  1 Package
    
    Total size: 25 k
    Installed size: 25 k
    Downloading packages:
    Running transaction check
    Running transaction test
    Transaction test succeeded
    Running transaction
      Installing : epel-release-7-14.noarch                                                                           1/1
      Verifying  : epel-release-7-14.noarch                                                                           1/1
    
    Installed:
      epel-release.noarch 0:7-14
    
    Complete!
    [root@ceph2 ~]#
    Remote side unexpectedly closed network connection
    
    ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────
    
    Session stopped
        - Press <Return> to exit tab
        - Press R to restart session
        - Press S to save terminal output to file
    root@192.168.239.155's password:
        ┌──────────────────────────────────────────────────────────────────────┐
        │                 • MobaXterm Personal Edition v23.1 •                 │
        │               (SSH client, X server and network tools)               │
        │                                                                      │
        │ ⮞ SSH session to root@192.168.239.155                                │
        │   • Direct SSH      :  ✓                                             │
        │   • SSH compression :  ✓                                             │
        │   • SSH-browser     :  ✓                                             │
        │   • X11-forwarding  :  ✗  (disabled or not supported by server)      │
        │                                                                      │
        │ ⮞ For more info, ctrl+click on help or visit our website.            │
        └──────────────────────────────────────────────────────────────────────┘
    
    Last login: Sun Jul 16 21:12:53 2023
    [root@ceph2 ~]# vim /etc/chrony.conf
    [root@ceph2 ~]# vim /etc/chrony.conf
    [root@ceph2 ~]# systemctl restart chronyd
    [root@ceph2 ~]#     sudo rpm -Uvh https://download.ceph.com/rpm-mimic/el7/noarch/ceph-release-1-1.el7.noarch.rpm
    Retrieving https://download.ceph.com/rpm-mimic/el7/noarch/ceph-release-1-1.el7.noarch.rpm
    warning: /var/tmp/rpm-tmp.CP31Kp: Header V4 RSA/SHA256 Signature, key ID 460f3994: NOKEY
    Preparing...                          ################################# [100%]
    Updating / installing...
       1:ceph-release-1-1.el7             ################################# [100%]
    [root@ceph2 ~]#     yum update -y && sudo yum install ceph-deploy python2-pip  -y
    Loaded plugins: fastestmirror
    Loading mirror speeds from cached hostfile
    epel/x86_64/metalink                                                                           | 6.6 kB  00:00:00
     * base: centos.mirror.net.in
     * epel: repo.extreme-ix.org
     * extras: centos.mirror.net.in
     * updates: centos.mirror.net.in
    Ceph                                                                                           | 1.5 kB  00:00:00
    Ceph-noarch                                                                                    | 1.5 kB  00:00:00
    ceph-source                                                                                    | 1.5 kB  00:00:00
    epel                                                                                           | 4.7 kB  00:00:00
    (1/6): epel/x86_64/group_gz                                                                    |  99 kB  00:00:00
    (2/6): Ceph-noarch/primary                                                                     | 2.5 kB  00:00:00
    (3/6): ceph-source/primary                                                                     | 4.7 kB  00:00:00
    (4/6): Ceph/x86_64/primary                                                                     |  72 kB  00:00:00
    (5/6): epel/x86_64/updateinfo                                                                  | 1.0 MB  00:00:01
    (6/6): epel/x86_64/primary_db                                                                  | 7.0 MB  00:00:06
    Ceph                                                                                                          524/524
    Ceph-noarch                                                                                                     16/16
    ceph-source                                                                                                     30/30
    Resolving Dependencies
    --> Running transaction check
    ---> Package NetworkManager.x86_64 1:1.18.8-1.el7 will be updated
    ---> Package NetworkManager.x86_64 1:1.18.8-2.el7_9 will be an update
    ---> Package NetworkManager-libnm.x86_64 1:1.18.8-1.el7 will be updated
    ---> Package NetworkManager-libnm.x86_64 1:1.18.8-2.el7_9 will be an update
    ---> Package NetworkManager-team.x86_64 1:1.18.8-1.el7 will be updated
    ---> Package NetworkManager-team.x86_64 1:1.18.8-2.el7_9 will be an update
    ---> Package NetworkManager-tui.x86_64 1:1.18.8-1.el7 will be updated
    ---> Package NetworkManager-tui.x86_64 1:1.18.8-2.el7_9 will be an update
    ---> Package NetworkManager-wifi.x86_64 1:1.18.8-1.el7 will be updated
    ---> Package NetworkManager-wifi.x86_64 1:1.18.8-2.el7_9 will be an update
    ---> Package bash.x86_64 0:4.2.46-34.el7 will be updated
    ---> Package bash.x86_64 0:4.2.46-35.el7_9 will be an update
    ---> Package bind-export-libs.x86_64 32:9.11.4-26.P2.el7 will be updated
    ---> Package bind-export-libs.x86_64 32:9.11.4-26.P2.el7_9.13 will be an update
    ---> Package binutils.x86_64 0:2.27-44.base.el7 will be updated
    ---> Package binutils.x86_64 0:2.27-44.base.el7_9.1 will be an update
    ---> Package ca-certificates.noarch 0:2020.2.41-70.0.el7_8 will be updated
    ---> Package ca-certificates.noarch 0:2022.2.54-74.el7_9 will be an update
    ---> Package centos-release.x86_64 0:7-9.2009.0.el7.centos will be updated
    ---> Package centos-release.x86_64 0:7-9.2009.1.el7.centos will be an update
    ---> Package coreutils.x86_64 0:8.22-24.el7 will be updated
    ---> Package coreutils.x86_64 0:8.22-24.el7_9.2 will be an update
    ---> Package cronie.x86_64 0:1.4.11-23.el7 will be updated
    ---> Package cronie.x86_64 0:1.4.11-25.el7_9 will be an update
    ---> Package cronie-anacron.x86_64 0:1.4.11-23.el7 will be updated
    ---> Package cronie-anacron.x86_64 0:1.4.11-25.el7_9 will be an update
    ---> Package curl.x86_64 0:7.29.0-59.el7 will be updated
    ---> Package curl.x86_64 0:7.29.0-59.el7_9.1 will be an update
    ---> Package cyrus-sasl-lib.x86_64 0:2.1.26-23.el7 will be updated
    ---> Package cyrus-sasl-lib.x86_64 0:2.1.26-24.el7_9 will be an update
    ---> Package device-mapper.x86_64 7:1.02.170-6.el7 will be updated
    ---> Package device-mapper.x86_64 7:1.02.170-6.el7_9.5 will be an update
    ---> Package device-mapper-event.x86_64 7:1.02.170-6.el7 will be updated
    ---> Package device-mapper-event.x86_64 7:1.02.170-6.el7_9.5 will be an update
    ---> Package device-mapper-event-libs.x86_64 7:1.02.170-6.el7 will be updated
    ---> Package device-mapper-event-libs.x86_64 7:1.02.170-6.el7_9.5 will be an update
    ---> Package device-mapper-libs.x86_64 7:1.02.170-6.el7 will be updated
    ---> Package device-mapper-libs.x86_64 7:1.02.170-6.el7_9.5 will be an update
    ---> Package device-mapper-persistent-data.x86_64 0:0.8.5-3.el7 will be updated
    ---> Package device-mapper-persistent-data.x86_64 0:0.8.5-3.el7_9.2 will be an update
    ---> Package dhclient.x86_64 12:4.2.5-82.el7.centos will be updated
    ---> Package dhclient.x86_64 12:4.2.5-83.el7.centos.1 will be an update
    ---> Package dhcp-common.x86_64 12:4.2.5-82.el7.centos will be updated
    ---> Package dhcp-common.x86_64 12:4.2.5-83.el7.centos.1 will be an update
    ---> Package dhcp-libs.x86_64 12:4.2.5-82.el7.centos will be updated
    ---> Package dhcp-libs.x86_64 12:4.2.5-83.el7.centos.1 will be an update
    ---> Package diffutils.x86_64 0:3.3-5.el7 will be updated
    ---> Package diffutils.x86_64 0:3.3-6.el7_9 will be an update
    ---> Package dmidecode.x86_64 1:3.2-5.el7 will be updated
    ---> Package dmidecode.x86_64 1:3.2-5.el7_9.1 will be an update
    ---> Package expat.x86_64 0:2.1.0-12.el7 will be updated
    ---> Package expat.x86_64 0:2.1.0-15.el7_9 will be an update
    ---> Package firewalld.noarch 0:0.6.3-11.el7 will be updated
    ---> Package firewalld.noarch 0:0.6.3-13.el7_9 will be an update
    ---> Package firewalld-filesystem.noarch 0:0.6.3-11.el7 will be updated
    ---> Package firewalld-filesystem.noarch 0:0.6.3-13.el7_9 will be an update
    ---> Package freetype.x86_64 0:2.8-14.el7 will be updated
    ---> Package freetype.x86_64 0:2.8-14.el7_9.1 will be an update
    ---> Package glib2.x86_64 0:2.56.1-7.el7 will be updated
    ---> Package glib2.x86_64 0:2.56.1-9.el7_9 will be an update
    ---> Package glibc.x86_64 0:2.17-317.el7 will be updated
    ---> Package glibc.x86_64 0:2.17-326.el7_9 will be an update
    ---> Package glibc-common.x86_64 0:2.17-317.el7 will be updated
    ---> Package glibc-common.x86_64 0:2.17-326.el7_9 will be an update
    ---> Package grub2.x86_64 1:2.02-0.86.el7.centos will be updated
    ---> Package grub2.x86_64 1:2.02-0.87.0.2.el7.centos.11 will be an update
    ---> Package grub2-common.noarch 1:2.02-0.86.el7.centos will be updated
    ---> Package grub2-common.noarch 1:2.02-0.87.0.2.el7.centos.11 will be an update
    ---> Package grub2-pc.x86_64 1:2.02-0.86.el7.centos will be updated
    ---> Package grub2-pc.x86_64 1:2.02-0.87.0.2.el7.centos.11 will be an update
    ---> Package grub2-pc-modules.noarch 1:2.02-0.86.el7.centos will be updated
    ---> Package grub2-pc-modules.noarch 1:2.02-0.87.0.2.el7.centos.11 will be an update
    ---> Package grub2-tools.x86_64 1:2.02-0.86.el7.centos will be updated
    ---> Package grub2-tools.x86_64 1:2.02-0.87.0.2.el7.centos.11 will be an update
    ---> Package grub2-tools-extra.x86_64 1:2.02-0.86.el7.centos will be updated
    ---> Package grub2-tools-extra.x86_64 1:2.02-0.87.0.2.el7.centos.11 will be an update
    ---> Package grub2-tools-minimal.x86_64 1:2.02-0.86.el7.centos will be updated
    ---> Package grub2-tools-minimal.x86_64 1:2.02-0.87.0.2.el7.centos.11 will be an update
    ---> Package gzip.x86_64 0:1.5-10.el7 will be updated
    ---> Package gzip.x86_64 0:1.5-11.el7_9 will be an update
    ---> Package initscripts.x86_64 0:9.49.53-1.el7 will be updated
    ---> Package initscripts.x86_64 0:9.49.53-1.el7_9.1 will be an update
    ---> Package iprutils.x86_64 0:2.4.17.1-3.el7 will be updated
    ---> Package iprutils.x86_64 0:2.4.17.1-3.el7_7 will be an update
    ---> Package iwl100-firmware.noarch 0:39.31.5.1-79.el7 will be updated
    ---> Package iwl100-firmware.noarch 0:39.31.5.1-80.el7_9 will be an update
    ---> Package iwl1000-firmware.noarch 1:39.31.5.1-79.el7 will be updated
    ---> Package iwl1000-firmware.noarch 1:39.31.5.1-80.el7_9 will be an update
    ---> Package iwl105-firmware.noarch 0:18.168.6.1-79.el7 will be updated
    ---> Package iwl105-firmware.noarch 0:18.168.6.1-80.el7_9 will be an update
    ---> Package iwl135-firmware.noarch 0:18.168.6.1-79.el7 will be updated
    ---> Package iwl135-firmware.noarch 0:18.168.6.1-80.el7_9 will be an update
    ---> Package iwl2000-firmware.noarch 0:18.168.6.1-79.el7 will be updated
    ---> Package iwl2000-firmware.noarch 0:18.168.6.1-80.el7_9 will be an update
    ---> Package iwl2030-firmware.noarch 0:18.168.6.1-79.el7 will be updated
    ---> Package iwl2030-firmware.noarch 0:18.168.6.1-80.el7_9 will be an update
    ---> Package iwl3160-firmware.noarch 0:25.30.13.0-79.el7 will be updated
    ---> Package iwl3160-firmware.noarch 0:25.30.13.0-80.el7_9 will be an update
    ---> Package iwl3945-firmware.noarch 0:15.32.2.9-79.el7 will be updated
    ---> Package iwl3945-firmware.noarch 0:15.32.2.9-80.el7_9 will be an update
    ---> Package iwl4965-firmware.noarch 0:228.61.2.24-79.el7 will be updated
    ---> Package iwl4965-firmware.noarch 0:228.61.2.24-80.el7_9 will be an update
    ---> Package iwl5000-firmware.noarch 0:8.83.5.1_1-79.el7 will be updated
    ---> Package iwl5000-firmware.noarch 0:8.83.5.1_1-80.el7_9 will be an update
    ---> Package iwl5150-firmware.noarch 0:8.24.2.2-79.el7 will be updated
    ---> Package iwl5150-firmware.noarch 0:8.24.2.2-80.el7_9 will be an update
    ---> Package iwl6000-firmware.noarch 0:9.221.4.1-79.el7 will be updated
    ---> Package iwl6000-firmware.noarch 0:9.221.4.1-80.el7_9 will be an update
    ---> Package iwl6000g2a-firmware.noarch 0:18.168.6.1-79.el7 will be updated
    ---> Package iwl6000g2a-firmware.noarch 0:18.168.6.1-80.el7_9 will be an update
    ---> Package iwl6000g2b-firmware.noarch 0:18.168.6.1-79.el7 will be updated
    ---> Package iwl6000g2b-firmware.noarch 0:18.168.6.1-80.el7_9 will be an update
    ---> Package iwl6050-firmware.noarch 0:41.28.5.1-79.el7 will be updated
    ---> Package iwl6050-firmware.noarch 0:41.28.5.1-80.el7_9 will be an update
    ---> Package iwl7260-firmware.noarch 0:25.30.13.0-79.el7 will be updated
    ---> Package iwl7260-firmware.noarch 0:25.30.13.0-80.el7_9 will be an update
    ---> Package kbd.x86_64 0:1.15.5-15.el7 will be updated
    ---> Package kbd.x86_64 0:1.15.5-16.el7_9 will be an update
    ---> Package kbd-legacy.noarch 0:1.15.5-15.el7 will be updated
    ---> Package kbd-legacy.noarch 0:1.15.5-16.el7_9 will be an update
    ---> Package kbd-misc.noarch 0:1.15.5-15.el7 will be updated
    ---> Package kbd-misc.noarch 0:1.15.5-16.el7_9 will be an update
    ---> Package kernel.x86_64 0:3.10.0-1160.92.1.el7 will be installed
    ---> Package kernel-tools.x86_64 0:3.10.0-1160.el7 will be updated
    ---> Package kernel-tools.x86_64 0:3.10.0-1160.92.1.el7 will be an update
    ---> Package kernel-tools-libs.x86_64 0:3.10.0-1160.el7 will be updated
    ---> Package kernel-tools-libs.x86_64 0:3.10.0-1160.92.1.el7 will be an update
    ---> Package kexec-tools.x86_64 0:2.0.15-51.el7 will be updated
    ---> Package kexec-tools.x86_64 0:2.0.15-51.el7_9.3 will be an update
    ---> Package kpartx.x86_64 0:0.4.9-133.el7 will be updated
    ---> Package kpartx.x86_64 0:0.4.9-136.el7_9 will be an update
    ---> Package krb5-libs.x86_64 0:1.15.1-50.el7 will be updated
    ---> Package krb5-libs.x86_64 0:1.15.1-55.el7_9 will be an update
    ---> Package libblkid.x86_64 0:2.23.2-65.el7 will be updated
    ---> Package libblkid.x86_64 0:2.23.2-65.el7_9.1 will be an update
    ---> Package libcroco.x86_64 0:0.6.12-4.el7 will be updated
    ---> Package libcroco.x86_64 0:0.6.12-6.el7_9 will be an update
    ---> Package libcurl.x86_64 0:7.29.0-59.el7 will be updated
    ---> Package libcurl.x86_64 0:7.29.0-59.el7_9.1 will be an update
    ---> Package libmount.x86_64 0:2.23.2-65.el7 will be updated
    ---> Package libmount.x86_64 0:2.23.2-65.el7_9.1 will be an update
    ---> Package libsmartcols.x86_64 0:2.23.2-65.el7 will be updated
    ---> Package libsmartcols.x86_64 0:2.23.2-65.el7_9.1 will be an update
    ---> Package libuuid.x86_64 0:2.23.2-65.el7 will be updated
    ---> Package libuuid.x86_64 0:2.23.2-65.el7_9.1 will be an update
    ---> Package libxml2.x86_64 0:2.9.1-6.el7.5 will be updated
    ---> Package libxml2.x86_64 0:2.9.1-6.el7_9.6 will be an update
    ---> Package linux-firmware.noarch 0:20200421-79.git78c0348.el7 will be updated
    ---> Package linux-firmware.noarch 0:20200421-80.git78c0348.el7_9 will be an update
    ---> Package lvm2.x86_64 7:2.02.187-6.el7 will be updated
    ---> Package lvm2.x86_64 7:2.02.187-6.el7_9.5 will be an update
    ---> Package lvm2-libs.x86_64 7:2.02.187-6.el7 will be updated
    ---> Package lvm2-libs.x86_64 7:2.02.187-6.el7_9.5 will be an update
    ---> Package microcode_ctl.x86_64 2:2.1-73.el7 will be updated
    ---> Package microcode_ctl.x86_64 2:2.1-73.15.el7_9 will be an update
    ---> Package nspr.x86_64 0:4.21.0-1.el7 will be updated
    ---> Package nspr.x86_64 0:4.34.0-3.1.el7_9 will be an update
    ---> Package nss.x86_64 0:3.44.0-7.el7_7 will be updated
    ---> Package nss.x86_64 0:3.79.0-5.el7_9 will be an update
    ---> Package nss-pem.x86_64 0:1.0.3-7.el7 will be updated
    ---> Package nss-pem.x86_64 0:1.0.3-7.el7_9.1 will be an update
    ---> Package nss-softokn.x86_64 0:3.44.0-8.el7_7 will be updated
    ---> Package nss-softokn.x86_64 0:3.79.0-4.el7_9 will be an update
    ---> Package nss-softokn-freebl.x86_64 0:3.44.0-8.el7_7 will be updated
    ---> Package nss-softokn-freebl.x86_64 0:3.79.0-4.el7_9 will be an update
    ---> Package nss-sysinit.x86_64 0:3.44.0-7.el7_7 will be updated
    ---> Package nss-sysinit.x86_64 0:3.79.0-5.el7_9 will be an update
    ---> Package nss-tools.x86_64 0:3.44.0-7.el7_7 will be updated
    ---> Package nss-tools.x86_64 0:3.79.0-5.el7_9 will be an update
    ---> Package nss-util.x86_64 0:3.44.0-4.el7_7 will be updated
    ---> Package nss-util.x86_64 0:3.79.0-1.el7_9 will be an update
    ---> Package openldap.x86_64 0:2.4.44-22.el7 will be updated
    ---> Package openldap.x86_64 0:2.4.44-25.el7_9 will be an update
    ---> Package openssh.x86_64 0:7.4p1-21.el7 will be updated
    ---> Package openssh.x86_64 0:7.4p1-22.el7_9 will be an update
    ---> Package openssh-clients.x86_64 0:7.4p1-21.el7 will be updated
    ---> Package openssh-clients.x86_64 0:7.4p1-22.el7_9 will be an update
    ---> Package openssh-server.x86_64 0:7.4p1-21.el7 will be updated
    ---> Package openssh-server.x86_64 0:7.4p1-22.el7_9 will be an update
    ---> Package openssl.x86_64 1:1.0.2k-19.el7 will be updated
    ---> Package openssl.x86_64 1:1.0.2k-26.el7_9 will be an update
    ---> Package openssl-libs.x86_64 1:1.0.2k-19.el7 will be updated
    ---> Package openssl-libs.x86_64 1:1.0.2k-26.el7_9 will be an update
    ---> Package polkit.x86_64 0:0.112-26.el7 will be updated
    ---> Package polkit.x86_64 0:0.112-26.el7_9.1 will be an update
    ---> Package python.x86_64 0:2.7.5-89.el7 will be updated
    ---> Package python.x86_64 0:2.7.5-93.el7_9 will be an update
    ---> Package python-firewall.noarch 0:0.6.3-11.el7 will be updated
    ---> Package python-firewall.noarch 0:0.6.3-13.el7_9 will be an update
    ---> Package python-libs.x86_64 0:2.7.5-89.el7 will be updated
    ---> Package python-libs.x86_64 0:2.7.5-93.el7_9 will be an update
    ---> Package python-perf.x86_64 0:3.10.0-1160.el7 will be updated
    ---> Package python-perf.x86_64 0:3.10.0-1160.92.1.el7 will be an update
    ---> Package rpm.x86_64 0:4.11.3-45.el7 will be updated
    ---> Package rpm.x86_64 0:4.11.3-48.el7_9 will be an update
    ---> Package rpm-build-libs.x86_64 0:4.11.3-45.el7 will be updated
    ---> Package rpm-build-libs.x86_64 0:4.11.3-48.el7_9 will be an update
    ---> Package rpm-libs.x86_64 0:4.11.3-45.el7 will be updated
    ---> Package rpm-libs.x86_64 0:4.11.3-48.el7_9 will be an update
    ---> Package rpm-python.x86_64 0:4.11.3-45.el7 will be updated
    ---> Package rpm-python.x86_64 0:4.11.3-48.el7_9 will be an update
    ---> Package rsyslog.x86_64 0:8.24.0-55.el7 will be updated
    ---> Package rsyslog.x86_64 0:8.24.0-57.el7_9.3 will be an update
    ---> Package selinux-policy.noarch 0:3.13.1-268.el7 will be updated
    ---> Package selinux-policy.noarch 0:3.13.1-268.el7_9.2 will be an update
    ---> Package selinux-policy-targeted.noarch 0:3.13.1-268.el7 will be updated
    ---> Package selinux-policy-targeted.noarch 0:3.13.1-268.el7_9.2 will be an update
    ---> Package sudo.x86_64 0:1.8.23-10.el7 will be updated
    ---> Package sudo.x86_64 0:1.8.23-10.el7_9.3 will be an update
    ---> Package systemd.x86_64 0:219-78.el7 will be updated
    ---> Package systemd.x86_64 0:219-78.el7_9.7 will be an update
    ---> Package systemd-libs.x86_64 0:219-78.el7 will be updated
    ---> Package systemd-libs.x86_64 0:219-78.el7_9.7 will be an update
    ---> Package systemd-sysv.x86_64 0:219-78.el7 will be updated
    ---> Package systemd-sysv.x86_64 0:219-78.el7_9.7 will be an update
    ---> Package tuned.noarch 0:2.11.0-9.el7 will be updated
    ---> Package tuned.noarch 0:2.11.0-12.el7_9 will be an update
    ---> Package tzdata.noarch 0:2020a-1.el7 will be updated
    ---> Package tzdata.noarch 0:2023c-1.el7 will be an update
    ---> Package util-linux.x86_64 0:2.23.2-65.el7 will be updated
    ---> Package util-linux.x86_64 0:2.23.2-65.el7_9.1 will be an update
    ---> Package vim-minimal.x86_64 2:7.4.629-7.el7 will be updated
    ---> Package vim-minimal.x86_64 2:7.4.629-8.el7_9 will be an update
    ---> Package virt-what.x86_64 0:1.18-4.el7 will be updated
    ---> Package virt-what.x86_64 0:1.18-4.el7_9.1 will be an update
    ---> Package wpa_supplicant.x86_64 1:2.6-12.el7 will be updated
    ---> Package wpa_supplicant.x86_64 1:2.6-12.el7_9.2 will be an update
    ---> Package xz.x86_64 0:5.2.2-1.el7 will be updated
    ---> Package xz.x86_64 0:5.2.2-2.el7_9 will be an update
    ---> Package xz-libs.x86_64 0:5.2.2-1.el7 will be updated
    ---> Package xz-libs.x86_64 0:5.2.2-2.el7_9 will be an update
    ---> Package zlib.x86_64 0:1.2.7-18.el7 will be updated
    ---> Package zlib.x86_64 0:1.2.7-21.el7_9 will be an update
    --> Finished Dependency Resolution
    
    Dependencies Resolved
    
    ======================================================================================================================
     Package                                Arch            Version                                Repository        Size
    ======================================================================================================================
    Installing:
     kernel                                 x86_64          3.10.0-1160.92.1.el7                   updates           52 M
    Updating:
     NetworkManager                         x86_64          1:1.18.8-2.el7_9                       updates          1.9 M
     NetworkManager-libnm                   x86_64          1:1.18.8-2.el7_9                       updates          1.7 M
     NetworkManager-team                    x86_64          1:1.18.8-2.el7_9                       updates          165 k
     NetworkManager-tui                     x86_64          1:1.18.8-2.el7_9                       updates          329 k
     NetworkManager-wifi                    x86_64          1:1.18.8-2.el7_9                       updates          202 k
     bash                                   x86_64          4.2.46-35.el7_9                        updates          1.0 M
     bind-export-libs                       x86_64          32:9.11.4-26.P2.el7_9.13               updates          1.1 M
     binutils                               x86_64          2.27-44.base.el7_9.1                   updates          5.9 M
     ca-certificates                        noarch          2022.2.54-74.el7_9                     updates          911 k
     centos-release                         x86_64          7-9.2009.1.el7.centos                  updates           27 k
     coreutils                              x86_64          8.22-24.el7_9.2                        updates          3.3 M
     cronie                                 x86_64          1.4.11-25.el7_9                        updates           92 k
     cronie-anacron                         x86_64          1.4.11-25.el7_9                        updates           36 k
     curl                                   x86_64          7.29.0-59.el7_9.1                      updates          271 k
     cyrus-sasl-lib                         x86_64          2.1.26-24.el7_9                        updates          156 k
     device-mapper                          x86_64          7:1.02.170-6.el7_9.5                   updates          297 k
     device-mapper-event                    x86_64          7:1.02.170-6.el7_9.5                   updates          192 k
     device-mapper-event-libs               x86_64          7:1.02.170-6.el7_9.5                   updates          192 k
     device-mapper-libs                     x86_64          7:1.02.170-6.el7_9.5                   updates          325 k
     device-mapper-persistent-data          x86_64          0.8.5-3.el7_9.2                        updates          423 k
     dhclient                               x86_64          12:4.2.5-83.el7.centos.1               updates          286 k
     dhcp-common                            x86_64          12:4.2.5-83.el7.centos.1               updates          177 k
     dhcp-libs                              x86_64          12:4.2.5-83.el7.centos.1               updates          133 k
     diffutils                              x86_64          3.3-6.el7_9                            updates          322 k
     dmidecode                              x86_64          1:3.2-5.el7_9.1                        updates           82 k
     expat                                  x86_64          2.1.0-15.el7_9                         updates           83 k
     firewalld                              noarch          0.6.3-13.el7_9                         updates          449 k
     firewalld-filesystem                   noarch          0.6.3-13.el7_9                         updates           51 k
     freetype                               x86_64          2.8-14.el7_9.1                         updates          380 k
     glib2                                  x86_64          2.56.1-9.el7_9                         updates          2.5 M
     glibc                                  x86_64          2.17-326.el7_9                         updates          3.6 M
     glibc-common                           x86_64          2.17-326.el7_9                         updates           12 M
     grub2                                  x86_64          1:2.02-0.87.0.2.el7.centos.11          updates           34 k
     grub2-common                           noarch          1:2.02-0.87.0.2.el7.centos.11          updates          733 k
     grub2-pc                               x86_64          1:2.02-0.87.0.2.el7.centos.11          updates           34 k
     grub2-pc-modules                       noarch          1:2.02-0.87.0.2.el7.centos.11          updates          860 k
     grub2-tools                            x86_64          1:2.02-0.87.0.2.el7.centos.11          updates          1.8 M
     grub2-tools-extra                      x86_64          1:2.02-0.87.0.2.el7.centos.11          updates          1.0 M
     grub2-tools-minimal                    x86_64          1:2.02-0.87.0.2.el7.centos.11          updates          177 k
     gzip                                   x86_64          1.5-11.el7_9                           updates          130 k
     initscripts                            x86_64          9.49.53-1.el7_9.1                      updates          440 k
     iprutils                               x86_64          2.4.17.1-3.el7_7                       updates          243 k
     iwl100-firmware                        noarch          39.31.5.1-80.el7_9                     updates          155 k
     iwl1000-firmware                       noarch          1:39.31.5.1-80.el7_9                   updates          215 k
     iwl105-firmware                        noarch          18.168.6.1-80.el7_9                    updates          234 k
     iwl135-firmware                        noarch          18.168.6.1-80.el7_9                    updates          243 k
     iwl2000-firmware                       noarch          18.168.6.1-80.el7_9                    updates          237 k
     iwl2030-firmware                       noarch          18.168.6.1-80.el7_9                    updates          245 k
     iwl3160-firmware                       noarch          25.30.13.0-80.el7_9                    updates          1.5 M
     iwl3945-firmware                       noarch          15.32.2.9-80.el7_9                     updates           96 k
     iwl4965-firmware                       noarch          228.61.2.24-80.el7_9                   updates          109 k
     iwl5000-firmware                       noarch          8.83.5.1_1-80.el7_9                    updates          289 k
     iwl5150-firmware                       noarch          8.24.2.2-80.el7_9                      updates          152 k
     iwl6000-firmware                       noarch          9.221.4.1-80.el7_9                     updates          171 k
     iwl6000g2a-firmware                    noarch          18.168.6.1-80.el7_9                    updates          304 k
     iwl6000g2b-firmware                    noarch          18.168.6.1-80.el7_9                    updates          305 k
     iwl6050-firmware                       noarch          41.28.5.1-80.el7_9                     updates          241 k
     iwl7260-firmware                       noarch          25.30.13.0-80.el7_9                    updates          6.1 M
     kbd                                    x86_64          1.15.5-16.el7_9                        updates          347 k
     kbd-legacy                             noarch          1.15.5-16.el7_9                        updates          466 k
     kbd-misc                               noarch          1.15.5-16.el7_9                        updates          1.4 M
     kernel-tools                           x86_64          3.10.0-1160.92.1.el7                   updates          8.2 M
     kernel-tools-libs                      x86_64          3.10.0-1160.92.1.el7                   updates          8.1 M
     kexec-tools                            x86_64          2.0.15-51.el7_9.3                      updates          351 k
     kpartx                                 x86_64          0.4.9-136.el7_9                        updates           81 k
     krb5-libs                              x86_64          1.15.1-55.el7_9                        updates          810 k
     libblkid                               x86_64          2.23.2-65.el7_9.1                      updates          183 k
     libcroco                               x86_64          0.6.12-6.el7_9                         updates          105 k
     libcurl                                x86_64          7.29.0-59.el7_9.1                      updates          223 k
     libmount                               x86_64          2.23.2-65.el7_9.1                      updates          185 k
     libsmartcols                           x86_64          2.23.2-65.el7_9.1                      updates          143 k
     libuuid                                x86_64          2.23.2-65.el7_9.1                      updates           84 k
     libxml2                                x86_64          2.9.1-6.el7_9.6                        updates          668 k
     linux-firmware                         noarch          20200421-80.git78c0348.el7_9           updates           80 M
     lvm2                                   x86_64          7:2.02.187-6.el7_9.5                   updates          1.3 M
     lvm2-libs                              x86_64          7:2.02.187-6.el7_9.5                   updates          1.1 M
     microcode_ctl                          x86_64          2:2.1-73.15.el7_9                      updates          4.5 M
     nspr                                   x86_64          4.34.0-3.1.el7_9                       updates          128 k
     nss                                    x86_64          3.79.0-5.el7_9                         updates          895 k
     nss-pem                                x86_64          1.0.3-7.el7_9.1                        updates           75 k
     nss-softokn                            x86_64          3.79.0-4.el7_9                         updates          379 k
     nss-softokn-freebl                     x86_64          3.79.0-4.el7_9                         updates          337 k
     nss-sysinit                            x86_64          3.79.0-5.el7_9                         updates           66 k
     nss-tools                              x86_64          3.79.0-5.el7_9                         updates          555 k
     nss-util                               x86_64          3.79.0-1.el7_9                         updates           80 k
     openldap                               x86_64          2.4.44-25.el7_9                        updates          356 k
     openssh                                x86_64          7.4p1-22.el7_9                         updates          510 k
     openssh-clients                        x86_64          7.4p1-22.el7_9                         updates          655 k
     openssh-server                         x86_64          7.4p1-22.el7_9                         updates          459 k
     openssl                                x86_64          1:1.0.2k-26.el7_9                      updates          494 k
     openssl-libs                           x86_64          1:1.0.2k-26.el7_9                      updates          1.2 M
     polkit                                 x86_64          0.112-26.el7_9.1                       updates          170 k
     python                                 x86_64          2.7.5-93.el7_9                         updates           96 k
     python-firewall                        noarch          0.6.3-13.el7_9                         updates          355 k
     python-libs                            x86_64          2.7.5-93.el7_9                         updates          5.6 M
     python-perf                            x86_64          3.10.0-1160.92.1.el7                   updates          8.2 M
     rpm                                    x86_64          4.11.3-48.el7_9                        updates          1.2 M
     rpm-build-libs                         x86_64          4.11.3-48.el7_9                        updates          108 k
     rpm-libs                               x86_64          4.11.3-48.el7_9                        updates          279 k
     rpm-python                             x86_64          4.11.3-48.el7_9                        updates           84 k
     rsyslog                                x86_64          8.24.0-57.el7_9.3                      updates          622 k
     selinux-policy                         noarch          3.13.1-268.el7_9.2                     updates          498 k
     selinux-policy-targeted                noarch          3.13.1-268.el7_9.2                     updates          7.0 M
     sudo                                   x86_64          1.8.23-10.el7_9.3                      updates          844 k
     systemd                                x86_64          219-78.el7_9.7                         updates          5.1 M
     systemd-libs                           x86_64          219-78.el7_9.7                         updates          419 k
     systemd-sysv                           x86_64          219-78.el7_9.7                         updates           97 k
     tuned                                  noarch          2.11.0-12.el7_9                        updates          270 k
     tzdata                                 noarch          2023c-1.el7                            updates          497 k
     util-linux                             x86_64          2.23.2-65.el7_9.1                      updates          2.0 M
     vim-minimal                            x86_64          2:7.4.629-8.el7_9                      updates          443 k
     virt-what                              x86_64          1.18-4.el7_9.1                         updates           30 k
     wpa_supplicant                         x86_64          1:2.6-12.el7_9.2                       updates          1.2 M
     xz                                     x86_64          5.2.2-2.el7_9                          updates          229 k
     xz-libs                                x86_64          5.2.2-2.el7_9                          updates          103 k
     zlib                                   x86_64          1.2.7-21.el7_9                         updates           90 k
    
    Transaction Summary
    ======================================================================================================================
    Install    1 Package
    Upgrade  116 Packages
    
    Total download size: 255 M
    Downloading packages:
    Delta RPMs disabled because /usr/bin/applydeltarpm not installed.
    (1/117): NetworkManager-libnm-1.18.8-2.el7_9.x86_64.rpm                                        | 1.7 MB  00:00:00
    (2/117): NetworkManager-1.18.8-2.el7_9.x86_64.rpm                                              | 1.9 MB  00:00:00
    (3/117): NetworkManager-team-1.18.8-2.el7_9.x86_64.rpm                                         | 165 kB  00:00:00
    (4/117): NetworkManager-wifi-1.18.8-2.el7_9.x86_64.rpm                                         | 202 kB  00:00:00
    (5/117): bash-4.2.46-35.el7_9.x86_64.rpm                                                       | 1.0 MB  00:00:00
    (6/117): NetworkManager-tui-1.18.8-2.el7_9.x86_64.rpm                                          | 329 kB  00:00:00
    (7/117): bind-export-libs-9.11.4-26.P2.el7_9.13.x86_64.rpm                                     | 1.1 MB  00:00:00
    (8/117): centos-release-7-9.2009.1.el7.centos.x86_64.rpm                                       |  27 kB  00:00:00
    (9/117): ca-certificates-2022.2.54-74.el7_9.noarch.rpm                                         | 911 kB  00:00:00
    (10/117): binutils-2.27-44.base.el7_9.1.x86_64.rpm                                             | 5.9 MB  00:00:00
    (11/117): cronie-1.4.11-25.el7_9.x86_64.rpm                                                    |  92 kB  00:00:00
    (12/117): cronie-anacron-1.4.11-25.el7_9.x86_64.rpm                                            |  36 kB  00:00:00
    (13/117): curl-7.29.0-59.el7_9.1.x86_64.rpm                                                    | 271 kB  00:00:00
    (14/117): cyrus-sasl-lib-2.1.26-24.el7_9.x86_64.rpm                                            | 156 kB  00:00:00
    (15/117): device-mapper-1.02.170-6.el7_9.5.x86_64.rpm                                          | 297 kB  00:00:00
    (16/117): device-mapper-event-1.02.170-6.el7_9.5.x86_64.rpm                                    | 192 kB  00:00:00
    (17/117): device-mapper-event-libs-1.02.170-6.el7_9.5.x86_64.rpm                               | 192 kB  00:00:00
    (18/117): coreutils-8.22-24.el7_9.2.x86_64.rpm                                                 | 3.3 MB  00:00:00
    (19/117): device-mapper-libs-1.02.170-6.el7_9.5.x86_64.rpm                                     | 325 kB  00:00:00
    (20/117): dhclient-4.2.5-83.el7.centos.1.x86_64.rpm                                            | 286 kB  00:00:00
    (21/117): device-mapper-persistent-data-0.8.5-3.el7_9.2.x86_64.rpm                             | 423 kB  00:00:00
    (22/117): dhcp-common-4.2.5-83.el7.centos.1.x86_64.rpm                                         | 177 kB  00:00:00
    (23/117): dhcp-libs-4.2.5-83.el7.centos.1.x86_64.rpm                                           | 133 kB  00:00:00
    (24/117): dmidecode-3.2-5.el7_9.1.x86_64.rpm                                                   |  82 kB  00:00:00
    (25/117): expat-2.1.0-15.el7_9.x86_64.rpm                                                      |  83 kB  00:00:00
    (26/117): firewalld-filesystem-0.6.3-13.el7_9.noarch.rpm                                       |  51 kB  00:00:00
    (27/117): diffutils-3.3-6.el7_9.x86_64.rpm                                                     | 322 kB  00:00:00
    (28/117): freetype-2.8-14.el7_9.1.x86_64.rpm                                                   | 380 kB  00:00:00
    (29/117): glib2-2.56.1-9.el7_9.x86_64.rpm                                                      | 2.5 MB  00:00:00
    (30/117): firewalld-0.6.3-13.el7_9.noarch.rpm                                                  | 449 kB  00:00:00
    (31/117): glibc-2.17-326.el7_9.x86_64.rpm                                                      | 3.6 MB  00:00:00
    (32/117): grub2-2.02-0.87.0.2.el7.centos.11.x86_64.rpm                                         |  34 kB  00:00:00
    (33/117): grub2-pc-2.02-0.87.0.2.el7.centos.11.x86_64.rpm                                      |  34 kB  00:00:00
    (34/117): grub2-pc-modules-2.02-0.87.0.2.el7.centos.11.noarch.rpm                              | 860 kB  00:00:00
    (35/117): grub2-common-2.02-0.87.0.2.el7.centos.11.noarch.rpm                                  | 733 kB  00:00:00
    (36/117): glibc-common-2.17-326.el7_9.x86_64.rpm                                               |  12 MB  00:00:00
    (37/117): grub2-tools-minimal-2.02-0.87.0.2.el7.centos.11.x86_64.rpm                           | 177 kB  00:00:00
    (38/117): grub2-tools-extra-2.02-0.87.0.2.el7.centos.11.x86_64.rpm                             | 1.0 MB  00:00:00
    (39/117): gzip-1.5-11.el7_9.x86_64.rpm                                                         | 130 kB  00:00:00
    (40/117): grub2-tools-2.02-0.87.0.2.el7.centos.11.x86_64.rpm                                   | 1.8 MB  00:00:00
    (41/117): iprutils-2.4.17.1-3.el7_7.x86_64.rpm                                                 | 243 kB  00:00:00
    (42/117): iwl100-firmware-39.31.5.1-80.el7_9.noarch.rpm                                        | 155 kB  00:00:00
    (43/117): iwl1000-firmware-39.31.5.1-80.el7_9.noarch.rpm                                       | 215 kB  00:00:00
    (44/117): initscripts-9.49.53-1.el7_9.1.x86_64.rpm                                             | 440 kB  00:00:00
    (45/117): iwl105-firmware-18.168.6.1-80.el7_9.noarch.rpm                                       | 234 kB  00:00:00
    (46/117): iwl135-firmware-18.168.6.1-80.el7_9.noarch.rpm                                       | 243 kB  00:00:00
    (47/117): iwl2000-firmware-18.168.6.1-80.el7_9.noarch.rpm                                      | 237 kB  00:00:00
    (48/117): iwl2030-firmware-18.168.6.1-80.el7_9.noarch.rpm                                      | 245 kB  00:00:00
    (49/117): iwl3945-firmware-15.32.2.9-80.el7_9.noarch.rpm                                       |  96 kB  00:00:00
    (50/117): iwl4965-firmware-228.61.2.24-80.el7_9.noarch.rpm                                     | 109 kB  00:00:00
    (51/117): iwl5150-firmware-8.24.2.2-80.el7_9.noarch.rpm                                        | 152 kB  00:00:00
    (52/117): iwl5000-firmware-8.83.5.1_1-80.el7_9.noarch.rpm                                      | 289 kB  00:00:00
    (53/117): iwl6000-firmware-9.221.4.1-80.el7_9.noarch.rpm                                       | 171 kB  00:00:00
    (54/117): iwl6000g2a-firmware-18.168.6.1-80.el7_9.noarch.rpm                                   | 304 kB  00:00:00
    (55/117): iwl6000g2b-firmware-18.168.6.1-80.el7_9.noarch.rpm                                   | 305 kB  00:00:00
    (56/117): iwl6050-firmware-41.28.5.1-80.el7_9.noarch.rpm                                       | 241 kB  00:00:00
    (57/117): iwl3160-firmware-25.30.13.0-80.el7_9.noarch.rpm                                      | 1.5 MB  00:00:00
    (58/117): kbd-1.15.5-16.el7_9.x86_64.rpm                                                       | 347 kB  00:00:00
    (59/117): kbd-legacy-1.15.5-16.el7_9.noarch.rpm                                                | 466 kB  00:00:00
    (60/117): kbd-misc-1.15.5-16.el7_9.noarch.rpm                                                  | 1.4 MB  00:00:00
    (61/117): iwl7260-firmware-25.30.13.0-80.el7_9.noarch.rpm                                      | 6.1 MB  00:00:00
    (62/117): kernel-tools-libs-3.10.0-1160.92.1.el7.x86_64.rpm                                    | 8.1 MB  00:00:00
    (63/117): kernel-tools-3.10.0-1160.92.1.el7.x86_64.rpm                                         | 8.2 MB  00:00:00
    (64/117): kpartx-0.4.9-136.el7_9.x86_64.rpm                                                    |  81 kB  00:00:00
    (65/117): kexec-tools-2.0.15-51.el7_9.3.x86_64.rpm                                             | 351 kB  00:00:00
    (66/117): libblkid-2.23.2-65.el7_9.1.x86_64.rpm                                                | 183 kB  00:00:00
    (67/117): libcroco-0.6.12-6.el7_9.x86_64.rpm                                                   | 105 kB  00:00:00
    (68/117): krb5-libs-1.15.1-55.el7_9.x86_64.rpm                                                 | 810 kB  00:00:00
    (69/117): libcurl-7.29.0-59.el7_9.1.x86_64.rpm                                                 | 223 kB  00:00:00
    (70/117): libmount-2.23.2-65.el7_9.1.x86_64.rpm                                                | 185 kB  00:00:00
    (71/117): libuuid-2.23.2-65.el7_9.1.x86_64.rpm                                                 |  84 kB  00:00:00
    (72/117): libsmartcols-2.23.2-65.el7_9.1.x86_64.rpm                                            | 143 kB  00:00:00
    (73/117): libxml2-2.9.1-6.el7_9.6.x86_64.rpm                                                   | 668 kB  00:00:00
    (74/117): lvm2-2.02.187-6.el7_9.5.x86_64.rpm                                                   | 1.3 MB  00:00:00
    (75/117): lvm2-libs-2.02.187-6.el7_9.5.x86_64.rpm                                              | 1.1 MB  00:00:00
    (76/117): microcode_ctl-2.1-73.15.el7_9.x86_64.rpm                                             | 4.5 MB  00:00:00
    (77/117): nspr-4.34.0-3.1.el7_9.x86_64.rpm                                                     | 128 kB  00:00:00
    (78/117): nss-3.79.0-5.el7_9.x86_64.rpm                                                        | 895 kB  00:00:00
    (79/117): nss-pem-1.0.3-7.el7_9.1.x86_64.rpm                                                   |  75 kB  00:00:00
    (80/117): nss-softokn-3.79.0-4.el7_9.x86_64.rpm                                                | 379 kB  00:00:00
    (81/117): nss-softokn-freebl-3.79.0-4.el7_9.x86_64.rpm                                         | 337 kB  00:00:00
    (82/117): nss-sysinit-3.79.0-5.el7_9.x86_64.rpm                                                |  66 kB  00:00:00
    (83/117): nss-tools-3.79.0-5.el7_9.x86_64.rpm                                                  | 555 kB  00:00:00
    (84/117): nss-util-3.79.0-1.el7_9.x86_64.rpm                                                   |  80 kB  00:00:00
    (85/117): openldap-2.4.44-25.el7_9.x86_64.rpm                                                  | 356 kB  00:00:00
    (86/117): openssh-7.4p1-22.el7_9.x86_64.rpm                                                    | 510 kB  00:00:00
    (87/117): openssh-clients-7.4p1-22.el7_9.x86_64.rpm                                            | 655 kB  00:00:00
    (88/117): openssh-server-7.4p1-22.el7_9.x86_64.rpm                                             | 459 kB  00:00:00
    (89/117): openssl-1.0.2k-26.el7_9.x86_64.rpm                                                   | 494 kB  00:00:00
    (90/117): linux-firmware-20200421-80.git78c0348.el7_9.noarch.rpm                               |  80 MB  00:00:02
    (91/117): openssl-libs-1.0.2k-26.el7_9.x86_64.rpm                                              | 1.2 MB  00:00:00
    (92/117): python-2.7.5-93.el7_9.x86_64.rpm                                                     |  96 kB  00:00:00
    (93/117): polkit-0.112-26.el7_9.1.x86_64.rpm                                                   | 170 kB  00:00:00
    (94/117): python-firewall-0.6.3-13.el7_9.noarch.rpm                                            | 355 kB  00:00:00
    (95/117): python-perf-3.10.0-1160.92.1.el7.x86_64.rpm                                          | 8.2 MB  00:00:00
    (96/117): python-libs-2.7.5-93.el7_9.x86_64.rpm                                                | 5.6 MB  00:00:00
    (97/117): rpm-4.11.3-48.el7_9.x86_64.rpm                                                       | 1.2 MB  00:00:00
    (98/117): rpm-build-libs-4.11.3-48.el7_9.x86_64.rpm                                            | 108 kB  00:00:00
    (99/117): rpm-python-4.11.3-48.el7_9.x86_64.rpm                                                |  84 kB  00:00:00
    (100/117): rpm-libs-4.11.3-48.el7_9.x86_64.rpm                                                 | 279 kB  00:00:00
    (101/117): selinux-policy-3.13.1-268.el7_9.2.noarch.rpm                                        | 498 kB  00:00:00
    (102/117): rsyslog-8.24.0-57.el7_9.3.x86_64.rpm                                                | 622 kB  00:00:00
    (103/117): sudo-1.8.23-10.el7_9.3.x86_64.rpm                                                   | 844 kB  00:00:00
    (104/117): systemd-219-78.el7_9.7.x86_64.rpm                                                   | 5.1 MB  00:00:00
    (105/117): systemd-libs-219-78.el7_9.7.x86_64.rpm                                              | 419 kB  00:00:00
    (106/117): systemd-sysv-219-78.el7_9.7.x86_64.rpm                                              |  97 kB  00:00:00
    (107/117): tuned-2.11.0-12.el7_9.noarch.rpm                                                    | 270 kB  00:00:00
    (108/117): tzdata-2023c-1.el7.noarch.rpm                                                       | 497 kB  00:00:00
    (109/117): util-linux-2.23.2-65.el7_9.1.x86_64.rpm                                             | 2.0 MB  00:00:00
    (110/117): vim-minimal-7.4.629-8.el7_9.x86_64.rpm                                              | 443 kB  00:00:00
    (111/117): virt-what-1.18-4.el7_9.1.x86_64.rpm                                                 |  30 kB  00:00:00
    (112/117): wpa_supplicant-2.6-12.el7_9.2.x86_64.rpm                                            | 1.2 MB  00:00:00
    (113/117): xz-5.2.2-2.el7_9.x86_64.rpm                                                         | 229 kB  00:00:00
    (114/117): xz-libs-5.2.2-2.el7_9.x86_64.rpm                                                    | 103 kB  00:00:00
    (115/117): zlib-1.2.7-21.el7_9.x86_64.rpm                                                      |  90 kB  00:00:00
    (116/117): selinux-policy-targeted-3.13.1-268.el7_9.2.noarch.rpm                               | 7.0 MB  00:00:02
    (117/117): kernel-3.10.0-1160.92.1.el7.x86_64.rpm                                              |  52 MB  00:00:13
    ----------------------------------------------------------------------------------------------------------------------
    Total                                                                                  15 MB/s | 255 MB  00:00:16
    Running transaction check
    Running transaction test
    Transaction test succeeded
    Running transaction
    Warning: RPMDB altered outside of yum.
      Updating   : 1:grub2-common-2.02-0.87.0.2.el7.centos.11.noarch                                                1/233
      Updating   : centos-release-7-9.2009.1.el7.centos.x86_64                                                      2/233
      Updating   : 1:grub2-pc-modules-2.02-0.87.0.2.el7.centos.11.noarch                                            3/233
      Updating   : kbd-misc-1.15.5-16.el7_9.noarch                                                                  4/233
      Updating   : kbd-legacy-1.15.5-16.el7_9.noarch                                                                5/233
      Updating   : tzdata-2023c-1.el7.noarch                                                                        6/233
      Updating   : bash-4.2.46-35.el7_9.x86_64                                                                      7/233
      Updating   : glibc-common-2.17-326.el7_9.x86_64                                                               8/233
      Updating   : nss-softokn-freebl-3.79.0-4.el7_9.x86_64                                                         9/233
      Updating   : glibc-2.17-326.el7_9.x86_64                                                                     10/233
      Updating   : nspr-4.34.0-3.1.el7_9.x86_64                                                                    11/233
      Updating   : nss-util-3.79.0-1.el7_9.x86_64                                                                  12/233
      Updating   : zlib-1.2.7-21.el7_9.x86_64                                                                      13/233
      Updating   : xz-libs-5.2.2-2.el7_9.x86_64                                                                    14/233
      Updating   : systemd-libs-219-78.el7_9.7.x86_64                                                              15/233
      Updating   : libuuid-2.23.2-65.el7_9.1.x86_64                                                                16/233
      Updating   : expat-2.1.0-15.el7_9.x86_64                                                                     17/233
      Updating   : nss-softokn-3.79.0-4.el7_9.x86_64                                                               18/233
      Updating   : device-mapper-persistent-data-0.8.5-3.el7_9.2.x86_64                                            19/233
      Updating   : libxml2-2.9.1-6.el7_9.6.x86_64                                                                  20/233
      Updating   : freetype-2.8-14.el7_9.1.x86_64                                                                  21/233
      Updating   : 1:dmidecode-3.2-5.el7_9.1.x86_64                                                                22/233
      Updating   : 2:vim-minimal-7.4.629-8.el7_9.x86_64                                                            23/233
      Updating   : libsmartcols-2.23.2-65.el7_9.1.x86_64                                                           24/233
      Updating   : diffutils-3.3-6.el7_9.x86_64                                                                    25/233
      Updating   : kernel-tools-libs-3.10.0-1160.92.1.el7.x86_64                                                   26/233
      Updating   : linux-firmware-20200421-80.git78c0348.el7_9.noarch                                              27/233
      Updating   : ca-certificates-2022.2.54-74.el7_9.noarch                                                       28/233
      Updating   : 1:openssl-libs-1.0.2k-26.el7_9.x86_64                                                           29/233
      Updating   : coreutils-8.22-24.el7_9.2.x86_64                                                                30/233
      Updating   : krb5-libs-1.15.1-55.el7_9.x86_64                                                                31/233
      Updating   : libblkid-2.23.2-65.el7_9.1.x86_64                                                               32/233
      Updating   : libmount-2.23.2-65.el7_9.1.x86_64                                                               33/233
      Updating   : glib2-2.56.1-9.el7_9.x86_64                                                                     34/233
      Updating   : util-linux-2.23.2-65.el7_9.1.x86_64                                                             35/233
      Updating   : python-libs-2.7.5-93.el7_9.x86_64                                                               36/233
      Updating   : python-2.7.5-93.el7_9.x86_64                                                                    37/233
      Updating   : python-firewall-0.6.3-13.el7_9.noarch                                                           38/233
      Updating   : python-perf-3.10.0-1160.92.1.el7.x86_64                                                         39/233
      Updating   : virt-what-1.18-4.el7_9.1.x86_64                                                                 40/233
      Updating   : 32:bind-export-libs-9.11.4-26.P2.el7_9.13.x86_64                                                41/233
      Updating   : cyrus-sasl-lib-2.1.26-24.el7_9.x86_64                                                           42/233
      Updating   : selinux-policy-3.13.1-268.el7_9.2.noarch                                                        43/233
      Updating   : nss-pem-1.0.3-7.el7_9.1.x86_64                                                                  44/233
      Updating   : nss-sysinit-3.79.0-5.el7_9.x86_64                                                               45/233
      Updating   : nss-3.79.0-5.el7_9.x86_64                                                                       46/233
      Updating   : 1:NetworkManager-libnm-1.18.8-2.el7_9.x86_64                                                    47/233
      Updating   : nss-tools-3.79.0-5.el7_9.x86_64                                                                 48/233
      Updating   : libcurl-7.29.0-59.el7_9.1.x86_64                                                                49/233
      Updating   : curl-7.29.0-59.el7_9.1.x86_64                                                                   50/233
      Updating   : rpm-libs-4.11.3-48.el7_9.x86_64                                                                 51/233
      Updating   : rpm-4.11.3-48.el7_9.x86_64                                                                      52/233
      Updating   : openldap-2.4.44-25.el7_9.x86_64                                                                 53/233
      Updating   : systemd-219-78.el7_9.7.x86_64                                                                   54/233
      Updating   : initscripts-9.49.53-1.el7_9.1.x86_64                                                            55/233
      Updating   : 7:device-mapper-libs-1.02.170-6.el7_9.5.x86_64                                                  56/233
      Updating   : 7:device-mapper-1.02.170-6.el7_9.5.x86_64                                                       57/233
      Updating   : 1:grub2-tools-minimal-2.02-0.87.0.2.el7.centos.11.x86_64                                        58/233
      Updating   : 7:device-mapper-event-libs-1.02.170-6.el7_9.5.x86_64                                            59/233
      Updating   : 1:grub2-tools-2.02-0.87.0.2.el7.centos.11.x86_64                                                60/233
      Updating   : polkit-0.112-26.el7_9.1.x86_64                                                                  61/233
      Updating   : 12:dhcp-libs-4.2.5-83.el7.centos.1.x86_64                                                       62/233
      Updating   : openssh-7.4p1-22.el7_9.x86_64                                                                   63/233
      Updating   : 12:dhcp-common-4.2.5-83.el7.centos.1.x86_64                                                     64/233
      Updating   : 1:grub2-tools-extra-2.02-0.87.0.2.el7.centos.11.x86_64                                          65/233
      Updating   : 1:grub2-pc-2.02-0.87.0.2.el7.centos.11.x86_64                                                   66/233
      Updating   : 7:device-mapper-event-1.02.170-6.el7_9.5.x86_64                                                 67/233
      Updating   : 7:lvm2-libs-2.02.187-6.el7_9.5.x86_64                                                           68/233
      Updating   : cronie-anacron-1.4.11-25.el7_9.x86_64                                                           69/233
      Updating   : cronie-1.4.11-25.el7_9.x86_64                                                                   70/233
      Updating   : systemd-sysv-219-78.el7_9.7.x86_64                                                              71/233
      Updating   : 1:wpa_supplicant-2.6-12.el7_9.2.x86_64                                                          72/233
      Updating   : 1:NetworkManager-1.18.8-2.el7_9.x86_64                                                          73/233
      Updating   : rpm-build-libs-4.11.3-48.el7_9.x86_64                                                           74/233
      Updating   : firewalld-filesystem-0.6.3-13.el7_9.noarch                                                      75/233
      Updating   : firewalld-0.6.3-13.el7_9.noarch                                                                 76/233
      Updating   : rpm-python-4.11.3-48.el7_9.x86_64                                                               77/233
      Updating   : 1:NetworkManager-tui-1.18.8-2.el7_9.x86_64                                                      78/233
      Updating   : 1:NetworkManager-team-1.18.8-2.el7_9.x86_64                                                     79/233
      Updating   : 1:NetworkManager-wifi-1.18.8-2.el7_9.x86_64                                                     80/233
      Updating   : 7:lvm2-2.02.187-6.el7_9.5.x86_64                                                                81/233
      Updating   : 1:grub2-2.02-0.87.0.2.el7.centos.11.x86_64                                                      82/233
      Updating   : 12:dhclient-4.2.5-83.el7.centos.1.x86_64                                                        83/233
      Updating   : openssh-clients-7.4p1-22.el7_9.x86_64                                                           84/233
      Updating   : openssh-server-7.4p1-22.el7_9.x86_64                                                            85/233
      Updating   : tuned-2.11.0-12.el7_9.noarch                                                                    86/233
      Updating   : kpartx-0.4.9-136.el7_9.x86_64                                                                   87/233
      Installing : kernel-3.10.0-1160.92.1.el7.x86_64                                                              88/233
      Updating   : kbd-1.15.5-16.el7_9.x86_64                                                                      89/233
      Updating   : 2:microcode_ctl-2.1-73.15.el7_9.x86_64                                                          90/233
      Updating   : kexec-tools-2.0.15-51.el7_9.3.x86_64                                                            91/233
      Updating   : rsyslog-8.24.0-57.el7_9.3.x86_64                                                                92/233
      Updating   : sudo-1.8.23-10.el7_9.3.x86_64                                                                   93/233
      Updating   : selinux-policy-targeted-3.13.1-268.el7_9.2.noarch                                               94/233
      Updating   : libcroco-0.6.12-6.el7_9.x86_64                                                                  95/233
      Updating   : 1:openssl-1.0.2k-26.el7_9.x86_64                                                                96/233
      Updating   : binutils-2.27-44.base.el7_9.1.x86_64                                                            97/233
      Updating   : gzip-1.5-11.el7_9.x86_64                                                                        98/233
      Updating   : kernel-tools-3.10.0-1160.92.1.el7.x86_64                                                        99/233
      Updating   : xz-5.2.2-2.el7_9.x86_64                                                                        100/233
      Updating   : iprutils-2.4.17.1-3.el7_7.x86_64                                                               101/233
      Updating   : iwl2000-firmware-18.168.6.1-80.el7_9.noarch                                                    102/233
      Updating   : iwl2030-firmware-18.168.6.1-80.el7_9.noarch                                                    103/233
      Updating   : iwl135-firmware-18.168.6.1-80.el7_9.noarch                                                     104/233
      Updating   : iwl3945-firmware-15.32.2.9-80.el7_9.noarch                                                     105/233
      Updating   : iwl7260-firmware-25.30.13.0-80.el7_9.noarch                                                    106/233
      Updating   : iwl6000g2a-firmware-18.168.6.1-80.el7_9.noarch                                                 107/233
      Updating   : 1:iwl1000-firmware-39.31.5.1-80.el7_9.noarch                                                   108/233
      Updating   : iwl6000g2b-firmware-18.168.6.1-80.el7_9.noarch                                                 109/233
      Updating   : iwl5000-firmware-8.83.5.1_1-80.el7_9.noarch                                                    110/233
      Updating   : iwl105-firmware-18.168.6.1-80.el7_9.noarch                                                     111/233
      Updating   : iwl4965-firmware-228.61.2.24-80.el7_9.noarch                                                   112/233
      Updating   : iwl100-firmware-39.31.5.1-80.el7_9.noarch                                                      113/233
      Updating   : iwl6050-firmware-41.28.5.1-80.el7_9.noarch                                                     114/233
      Updating   : iwl3160-firmware-25.30.13.0-80.el7_9.noarch                                                    115/233
      Updating   : iwl6000-firmware-9.221.4.1-80.el7_9.noarch                                                     116/233
      Updating   : iwl5150-firmware-8.24.2.2-80.el7_9.noarch                                                      117/233
      Cleanup    : 12:dhclient-4.2.5-82.el7.centos.x86_64                                                         118/233
      Cleanup    : 2:microcode_ctl-2.1-73.el7.x86_64                                                              119/233
      Cleanup    : tuned-2.11.0-9.el7.noarch                                                                      120/233
      Cleanup    : firewalld-0.6.3-11.el7.noarch                                                                  121/233
      Cleanup    : selinux-policy-targeted-3.13.1-268.el7.noarch                                                  122/233
      Cleanup    : selinux-policy-3.13.1-268.el7.noarch                                                           123/233
      Cleanup    : 1:grub2-2.02-0.86.el7.centos.x86_64                                                            124/233
      Cleanup    : 1:grub2-pc-2.02-0.86.el7.centos.x86_64                                                         125/233
      Cleanup    : 1:grub2-pc-modules-2.02-0.86.el7.centos.noarch                                                 126/233
      Cleanup    : python-firewall-0.6.3-11.el7.noarch                                                            127/233
      Cleanup    : 12:dhcp-common-4.2.5-82.el7.centos.x86_64                                                      128/233
      Cleanup    : 12:dhcp-libs-4.2.5-82.el7.centos.x86_64                                                        129/233
      Cleanup    : linux-firmware-20200421-79.git78c0348.el7.noarch                                               130/233
      Cleanup    : firewalld-filesystem-0.6.3-11.el7.noarch                                                       131/233
      Cleanup    : iwl2000-firmware-18.168.6.1-79.el7.noarch                                                      132/233
      Cleanup    : iwl2030-firmware-18.168.6.1-79.el7.noarch                                                      133/233
      Cleanup    : iwl135-firmware-18.168.6.1-79.el7.noarch                                                       134/233
      Cleanup    : iwl3945-firmware-15.32.2.9-79.el7.noarch                                                       135/233
      Cleanup    : iwl7260-firmware-25.30.13.0-79.el7.noarch                                                      136/233
      Cleanup    : iwl6000g2a-firmware-18.168.6.1-79.el7.noarch                                                   137/233
      Cleanup    : 1:iwl1000-firmware-39.31.5.1-79.el7.noarch                                                     138/233
      Cleanup    : iwl6000g2b-firmware-18.168.6.1-79.el7.noarch                                                   139/233
      Cleanup    : iwl5000-firmware-8.83.5.1_1-79.el7.noarch                                                      140/233
      Cleanup    : iwl105-firmware-18.168.6.1-79.el7.noarch                                                       141/233
      Cleanup    : iwl4965-firmware-228.61.2.24-79.el7.noarch                                                     142/233
      Cleanup    : iwl100-firmware-39.31.5.1-79.el7.noarch                                                        143/233
      Cleanup    : iwl6050-firmware-41.28.5.1-79.el7.noarch                                                       144/233
      Cleanup    : iwl3160-firmware-25.30.13.0-79.el7.noarch                                                      145/233
      Cleanup    : iwl6000-firmware-9.221.4.1-79.el7.noarch                                                       146/233
      Cleanup    : iwl5150-firmware-8.24.2.2-79.el7.noarch                                                        147/233
      Cleanup    : rpm-python-4.11.3-45.el7.x86_64                                                                148/233
      Cleanup    : 1:NetworkManager-tui-1.18.8-1.el7.x86_64                                                       149/233
      Cleanup    : openssh-server-7.4p1-21.el7.x86_64                                                             150/233
      Cleanup    : 7:lvm2-2.02.187-6.el7.x86_64                                                                   151/233
      Cleanup    : 1:openssl-1.0.2k-19.el7.x86_64                                                                 152/233
      Cleanup    : openssh-clients-7.4p1-21.el7.x86_64                                                            153/233
      Cleanup    : openssh-7.4p1-21.el7.x86_64                                                                    154/233
      Cleanup    : 7:lvm2-libs-2.02.187-6.el7.x86_64                                                              155/233
      Cleanup    : rpm-build-libs-4.11.3-45.el7.x86_64                                                            156/233
      Cleanup    : 1:grub2-tools-extra-2.02-0.86.el7.centos.x86_64                                                157/233
      Cleanup    : kexec-tools-2.0.15-51.el7.x86_64                                                               158/233
      Cleanup    : 1:grub2-tools-2.02-0.86.el7.centos.x86_64                                                      159/233
      Cleanup    : 7:device-mapper-event-1.02.170-6.el7.x86_64                                                    160/233
      Cleanup    : rsyslog-8.24.0-55.el7.x86_64                                                                   161/233
      Cleanup    : sudo-1.8.23-10.el7.x86_64                                                                      162/233
      Cleanup    : 1:grub2-tools-minimal-2.02-0.86.el7.centos.x86_64                                              163/233
      Cleanup    : cronie-anacron-1.4.11-23.el7.x86_64                                                            164/233
      Cleanup    : cronie-1.4.11-23.el7.x86_64                                                                    165/233
      Cleanup    : xz-5.2.2-1.el7.x86_64                                                                          166/233
      Cleanup    : 1:NetworkManager-wifi-1.18.8-1.el7.x86_64                                                      167/233
      Cleanup    : kernel-tools-3.10.0-1160.el7.x86_64                                                            168/233
      Cleanup    : binutils-2.27-44.base.el7.x86_64                                                               169/233
      Cleanup    : kbd-1.15.5-15.el7.x86_64                                                                       170/233
      Cleanup    : initscripts-9.49.53-1.el7.x86_64                                                               171/233
      Cleanup    : freetype-2.8-14.el7.x86_64                                                                     172/233
      Cleanup    : device-mapper-persistent-data-0.8.5-3.el7.x86_64                                               173/233
      Cleanup    : python-perf-3.10.0-1160.el7.x86_64                                                             174/233
      Cleanup    : virt-what-1.18-4.el7.x86_64                                                                    175/233
      Cleanup    : 32:bind-export-libs-9.11.4-26.P2.el7.x86_64                                                    176/233
      Cleanup    : libcroco-0.6.12-4.el7.x86_64                                                                   177/233
      Cleanup    : libxml2-2.9.1-6.el7.5.x86_64                                                                   178/233
      Cleanup    : 1:NetworkManager-team-1.18.8-1.el7.x86_64                                                      179/233
      Cleanup    : 1:NetworkManager-1.18.8-1.el7.x86_64                                                           180/233
      Cleanup    : 1:NetworkManager-libnm-1.18.8-1.el7.x86_64                                                     181/233
      Cleanup    : polkit-0.112-26.el7.x86_64                                                                     182/233
      Cleanup    : 1:wpa_supplicant-2.6-12.el7.x86_64                                                             183/233
      Cleanup    : glib2-2.56.1-7.el7.x86_64                                                                      184/233
      Cleanup    : iprutils-2.4.17.1-3.el7.x86_64                                                                 185/233
      Cleanup    : 7:device-mapper-event-libs-1.02.170-6.el7.x86_64                                               186/233
      Cleanup    : gzip-1.5-10.el7.x86_64                                                                         187/233
      Cleanup    : kpartx-0.4.9-133.el7.x86_64                                                                    188/233
      Cleanup    : systemd-sysv-219-78.el7.x86_64                                                                 189/233
      Cleanup    : python-2.7.5-89.el7.x86_64                                                                     190/233
      Cleanup    : python-libs-2.7.5-89.el7.x86_64                                                                191/233
      Cleanup    : 7:device-mapper-1.02.170-6.el7.x86_64                                                          192/233
      Cleanup    : 7:device-mapper-libs-1.02.170-6.el7.x86_64                                                     193/233
      Cleanup    : systemd-219-78.el7.x86_64                                                                      194/233
      Cleanup    : util-linux-2.23.2-65.el7.x86_64                                                                195/233
      Cleanup    : curl-7.29.0-59.el7.x86_64                                                                      196/233
      Cleanup    : libcurl-7.29.0-59.el7.x86_64                                                                   197/233
      Cleanup    : openldap-2.4.44-22.el7.x86_64                                                                  198/233
      Cleanup    : rpm-libs-4.11.3-45.el7.x86_64                                                                  199/233
      Cleanup    : rpm-4.11.3-45.el7.x86_64                                                                       200/233
      Cleanup    : nss-tools-3.44.0-7.el7_7.x86_64                                                                201/233
      Cleanup    : nss-sysinit-3.44.0-7.el7_7.x86_64                                                              202/233
      Cleanup    : nss-3.44.0-7.el7_7.x86_64                                                                      203/233
      Cleanup    : nss-pem-1.0.3-7.el7.x86_64                                                                     204/233
      Cleanup    : nss-softokn-3.44.0-8.el7_7.x86_64                                                              205/233
      Cleanup    : libmount-2.23.2-65.el7.x86_64                                                                  206/233
      Cleanup    : libblkid-2.23.2-65.el7.x86_64                                                                  207/233
      Cleanup    : cyrus-sasl-lib-2.1.26-23.el7.x86_64                                                            208/233
      Cleanup    : krb5-libs-1.15.1-50.el7.x86_64                                                                 209/233
      Cleanup    : coreutils-8.22-24.el7.x86_64                                                                   210/233
      Cleanup    : 1:openssl-libs-1.0.2k-19.el7.x86_64                                                            211/233
      Cleanup    : systemd-libs-219-78.el7.x86_64                                                                 212/233
      Cleanup    : diffutils-3.3-5.el7.x86_64                                                                     213/233
      Cleanup    : ca-certificates-2020.2.41-70.0.el7_8.noarch                                                    214/233
      Cleanup    : xz-libs-5.2.2-1.el7.x86_64                                                                     215/233
      Cleanup    : zlib-1.2.7-18.el7.x86_64                                                                       216/233
      Cleanup    : libuuid-2.23.2-65.el7.x86_64                                                                   217/233
      Cleanup    : libsmartcols-2.23.2-65.el7.x86_64                                                              218/233
      Cleanup    : expat-2.1.0-12.el7.x86_64                                                                      219/233
      Cleanup    : 1:dmidecode-3.2-5.el7.x86_64                                                                   220/233
      Cleanup    : kernel-tools-libs-3.10.0-1160.el7.x86_64                                                       221/233
      Cleanup    : 2:vim-minimal-7.4.629-7.el7.x86_64                                                             222/233
      Cleanup    : centos-release-7-9.2009.0.el7.centos.x86_64                                                    223/233
      Cleanup    : kbd-legacy-1.15.5-15.el7.noarch                                                                224/233
      Cleanup    : kbd-misc-1.15.5-15.el7.noarch                                                                  225/233
      Cleanup    : 1:grub2-common-2.02-0.86.el7.centos.noarch                                                     226/233
      Cleanup    : glibc-common-2.17-317.el7.x86_64                                                               227/233
      Cleanup    : bash-4.2.46-34.el7.x86_64                                                                      228/233
      Cleanup    : nspr-4.21.0-1.el7.x86_64                                                                       229/233
      Cleanup    : nss-util-3.44.0-4.el7_7.x86_64                                                                 230/233
      Cleanup    : nss-softokn-freebl-3.44.0-8.el7_7.x86_64                                                       231/233
      Cleanup    : glibc-2.17-317.el7.x86_64                                                                      232/233
      Cleanup    : tzdata-2020a-1.el7.noarch                                                                      233/233
      Verifying  : 7:device-mapper-event-1.02.170-6.el7_9.5.x86_64                                                  1/233
      Verifying  : libblkid-2.23.2-65.el7_9.1.x86_64                                                                2/233
      Verifying  : linux-firmware-20200421-80.git78c0348.el7_9.noarch                                               3/233
      Verifying  : firewalld-filesystem-0.6.3-13.el7_9.noarch                                                       4/233
      Verifying  : selinux-policy-targeted-3.13.1-268.el7_9.2.noarch                                                5/233
      Verifying  : iwl5150-firmware-8.24.2.2-80.el7_9.noarch                                                        6/233
      Verifying  : python-libs-2.7.5-93.el7_9.x86_64                                                                7/233
      Verifying  : 1:NetworkManager-tui-1.18.8-2.el7_9.x86_64                                                       8/233
      Verifying  : centos-release-7-9.2009.1.el7.centos.x86_64                                                      9/233
      Verifying  : kernel-3.10.0-1160.92.1.el7.x86_64                                                              10/233
      Verifying  : 7:lvm2-2.02.187-6.el7_9.5.x86_64                                                                11/233
      Verifying  : 12:dhcp-common-4.2.5-83.el7.centos.1.x86_64                                                     12/233
      Verifying  : iwl6000-firmware-9.221.4.1-80.el7_9.noarch                                                      13/233
      Verifying  : sudo-1.8.23-10.el7_9.3.x86_64                                                                   14/233
      Verifying  : iwl3160-firmware-25.30.13.0-80.el7_9.noarch                                                     15/233
      Verifying  : libcurl-7.29.0-59.el7_9.1.x86_64                                                                16/233
      Verifying  : kbd-1.15.5-16.el7_9.x86_64                                                                      17/233
      Verifying  : selinux-policy-3.13.1-268.el7_9.2.noarch                                                        18/233
      Verifying  : openldap-2.4.44-25.el7_9.x86_64                                                                 19/233
      Verifying  : 1:grub2-tools-2.02-0.87.0.2.el7.centos.11.x86_64                                                20/233
      Verifying  : 1:grub2-2.02-0.87.0.2.el7.centos.11.x86_64                                                      21/233
      Verifying  : 7:device-mapper-1.02.170-6.el7_9.5.x86_64                                                       22/233
      Verifying  : freetype-2.8-14.el7_9.1.x86_64                                                                  23/233
      Verifying  : 2:microcode_ctl-2.1-73.15.el7_9.x86_64                                                          24/233
      Verifying  : 1:grub2-common-2.02-0.87.0.2.el7.centos.11.noarch                                               25/233
      Verifying  : nss-softokn-freebl-3.79.0-4.el7_9.x86_64                                                        26/233
      Verifying  : systemd-libs-219-78.el7_9.7.x86_64                                                              27/233
      Verifying  : cronie-1.4.11-25.el7_9.x86_64                                                                   28/233
      Verifying  : libxml2-2.9.1-6.el7_9.6.x86_64                                                                  29/233
      Verifying  : cronie-anacron-1.4.11-25.el7_9.x86_64                                                           30/233
      Verifying  : 1:dmidecode-3.2-5.el7_9.1.x86_64                                                                31/233
      Verifying  : systemd-219-78.el7_9.7.x86_64                                                                   32/233
      Verifying  : 1:grub2-tools-extra-2.02-0.87.0.2.el7.centos.11.x86_64                                          33/233
      Verifying  : expat-2.1.0-15.el7_9.x86_64                                                                     34/233
      Verifying  : binutils-2.27-44.base.el7_9.1.x86_64                                                            35/233
      Verifying  : libmount-2.23.2-65.el7_9.1.x86_64                                                               36/233
      Verifying  : zlib-1.2.7-21.el7_9.x86_64                                                                      37/233
      Verifying  : tzdata-2023c-1.el7.noarch                                                                       38/233
      Verifying  : 32:bind-export-libs-9.11.4-26.P2.el7_9.13.x86_64                                                39/233
      Verifying  : initscripts-9.49.53-1.el7_9.1.x86_64                                                            40/233
      Verifying  : device-mapper-persistent-data-0.8.5-3.el7_9.2.x86_64                                            41/233
      Verifying  : 1:openssl-libs-1.0.2k-26.el7_9.x86_64                                                           42/233
      Verifying  : iwl6050-firmware-41.28.5.1-80.el7_9.noarch                                                      43/233
      Verifying  : nss-pem-1.0.3-7.el7_9.1.x86_64                                                                  44/233
      Verifying  : kbd-legacy-1.15.5-16.el7_9.noarch                                                               45/233
      Verifying  : 12:dhcp-libs-4.2.5-83.el7.centos.1.x86_64                                                       46/233
      Verifying  : bash-4.2.46-35.el7_9.x86_64                                                                     47/233
      Verifying  : iprutils-2.4.17.1-3.el7_7.x86_64                                                                48/233
      Verifying  : curl-7.29.0-59.el7_9.1.x86_64                                                                   49/233
      Verifying  : iwl100-firmware-39.31.5.1-80.el7_9.noarch                                                       50/233
      Verifying  : iwl4965-firmware-228.61.2.24-80.el7_9.noarch                                                    51/233
      Verifying  : 2:vim-minimal-7.4.629-8.el7_9.x86_64                                                            52/233
      Verifying  : cyrus-sasl-lib-2.1.26-24.el7_9.x86_64                                                           53/233
      Verifying  : nss-tools-3.79.0-5.el7_9.x86_64                                                                 54/233
      Verifying  : openssh-clients-7.4p1-22.el7_9.x86_64                                                           55/233
      Verifying  : nspr-4.34.0-3.1.el7_9.x86_64                                                                    56/233
      Verifying  : nss-softokn-3.79.0-4.el7_9.x86_64                                                               57/233
      Verifying  : 1:NetworkManager-team-1.18.8-2.el7_9.x86_64                                                     58/233
      Verifying  : 7:device-mapper-libs-1.02.170-6.el7_9.5.x86_64                                                  59/233
      Verifying  : iwl105-firmware-18.168.6.1-80.el7_9.noarch                                                      60/233
      Verifying  : iwl5000-firmware-8.83.5.1_1-80.el7_9.noarch                                                     61/233
      Verifying  : glibc-2.17-326.el7_9.x86_64                                                                     62/233
      Verifying  : firewalld-0.6.3-13.el7_9.noarch                                                                 63/233
      Verifying  : krb5-libs-1.15.1-55.el7_9.x86_64                                                                64/233
      Verifying  : kexec-tools-2.0.15-51.el7_9.3.x86_64                                                            65/233
      Verifying  : iwl6000g2b-firmware-18.168.6.1-80.el7_9.noarch                                                  66/233
      Verifying  : libsmartcols-2.23.2-65.el7_9.1.x86_64                                                           67/233
      Verifying  : coreutils-8.22-24.el7_9.2.x86_64                                                                68/233
      Verifying  : rpm-libs-4.11.3-48.el7_9.x86_64                                                                 69/233
      Verifying  : 1:wpa_supplicant-2.6-12.el7_9.2.x86_64                                                          70/233
      Verifying  : 1:grub2-pc-2.02-0.87.0.2.el7.centos.11.x86_64                                                   71/233
      Verifying  : util-linux-2.23.2-65.el7_9.1.x86_64                                                             72/233
      Verifying  : rpm-python-4.11.3-48.el7_9.x86_64                                                               73/233
      Verifying  : libuuid-2.23.2-65.el7_9.1.x86_64                                                                74/233
      Verifying  : openssh-server-7.4p1-22.el7_9.x86_64                                                            75/233
      Verifying  : xz-libs-5.2.2-2.el7_9.x86_64                                                                    76/233
      Verifying  : 1:iwl1000-firmware-39.31.5.1-80.el7_9.noarch                                                    77/233
      Verifying  : 1:openssl-1.0.2k-26.el7_9.x86_64                                                                78/233
      Verifying  : tuned-2.11.0-12.el7_9.noarch                                                                    79/233
      Verifying  : iwl6000g2a-firmware-18.168.6.1-80.el7_9.noarch                                                  80/233
      Verifying  : diffutils-3.3-6.el7_9.x86_64                                                                    81/233
      Verifying  : kpartx-0.4.9-136.el7_9.x86_64                                                                   82/233
      Verifying  : virt-what-1.18-4.el7_9.1.x86_64                                                                 83/233
      Verifying  : nss-sysinit-3.79.0-5.el7_9.x86_64                                                               84/233
      Verifying  : 1:grub2-tools-minimal-2.02-0.87.0.2.el7.centos.11.x86_64                                        85/233
      Verifying  : iwl7260-firmware-25.30.13.0-80.el7_9.noarch                                                     86/233
      Verifying  : rpm-4.11.3-48.el7_9.x86_64                                                                      87/233
      Verifying  : 12:dhclient-4.2.5-83.el7.centos.1.x86_64                                                        88/233
      Verifying  : kernel-tools-3.10.0-1160.92.1.el7.x86_64                                                        89/233
      Verifying  : openssh-7.4p1-22.el7_9.x86_64                                                                   90/233
      Verifying  : python-2.7.5-93.el7_9.x86_64                                                                    91/233
      Verifying  : glib2-2.56.1-9.el7_9.x86_64                                                                     92/233
      Verifying  : kbd-misc-1.15.5-16.el7_9.noarch                                                                 93/233
      Verifying  : 1:NetworkManager-wifi-1.18.8-2.el7_9.x86_64                                                     94/233
      Verifying  : iwl3945-firmware-15.32.2.9-80.el7_9.noarch                                                      95/233
      Verifying  : 1:NetworkManager-1.18.8-2.el7_9.x86_64                                                          96/233
      Verifying  : nss-3.79.0-5.el7_9.x86_64                                                                       97/233
      Verifying  : iwl135-firmware-18.168.6.1-80.el7_9.noarch                                                      98/233
      Verifying  : rsyslog-8.24.0-57.el7_9.3.x86_64                                                                99/233
      Verifying  : 7:lvm2-libs-2.02.187-6.el7_9.5.x86_64                                                          100/233
      Verifying  : kernel-tools-libs-3.10.0-1160.92.1.el7.x86_64                                                  101/233
      Verifying  : 1:NetworkManager-libnm-1.18.8-2.el7_9.x86_64                                                   102/233
      Verifying  : systemd-sysv-219-78.el7_9.7.x86_64                                                             103/233
      Verifying  : python-firewall-0.6.3-13.el7_9.noarch                                                          104/233
      Verifying  : 1:grub2-pc-modules-2.02-0.87.0.2.el7.centos.11.noarch                                          105/233
      Verifying  : 7:device-mapper-event-libs-1.02.170-6.el7_9.5.x86_64                                           106/233
      Verifying  : nss-util-3.79.0-1.el7_9.x86_64                                                                 107/233
      Verifying  : gzip-1.5-11.el7_9.x86_64                                                                       108/233
      Verifying  : glibc-common-2.17-326.el7_9.x86_64                                                             109/233
      Verifying  : libcroco-0.6.12-6.el7_9.x86_64                                                                 110/233
      Verifying  : ca-certificates-2022.2.54-74.el7_9.noarch                                                      111/233
      Verifying  : iwl2030-firmware-18.168.6.1-80.el7_9.noarch                                                    112/233
      Verifying  : python-perf-3.10.0-1160.92.1.el7.x86_64                                                        113/233
      Verifying  : iwl2000-firmware-18.168.6.1-80.el7_9.noarch                                                    114/233
      Verifying  : xz-5.2.2-2.el7_9.x86_64                                                                        115/233
      Verifying  : polkit-0.112-26.el7_9.1.x86_64                                                                 116/233
      Verifying  : rpm-build-libs-4.11.3-48.el7_9.x86_64                                                          117/233
      Verifying  : rpm-4.11.3-45.el7.x86_64                                                                       118/233
      Verifying  : firewalld-filesystem-0.6.3-11.el7.noarch                                                       119/233
      Verifying  : glibc-common-2.17-317.el7.x86_64                                                               120/233
      Verifying  : selinux-policy-targeted-3.13.1-268.el7.noarch                                                  121/233
      Verifying  : ca-certificates-2020.2.41-70.0.el7_8.noarch                                                    122/233
      Verifying  : linux-firmware-20200421-79.git78c0348.el7.noarch                                               123/233
      Verifying  : 7:device-mapper-event-1.02.170-6.el7.x86_64                                                    124/233
      Verifying  : freetype-2.8-14.el7.x86_64                                                                     125/233
      Verifying  : iwl2000-firmware-18.168.6.1-79.el7.noarch                                                      126/233
      Verifying  : glib2-2.56.1-7.el7.x86_64                                                                      127/233
      Verifying  : python-2.7.5-89.el7.x86_64                                                                     128/233
      Verifying  : 1:iwl1000-firmware-39.31.5.1-79.el7.noarch                                                     129/233
      Verifying  : virt-what-1.18-4.el7.x86_64                                                                    130/233
      Verifying  : zlib-1.2.7-18.el7.x86_64                                                                       131/233
      Verifying  : iwl5150-firmware-8.24.2.2-79.el7.noarch                                                        132/233
      Verifying  : nss-pem-1.0.3-7.el7.x86_64                                                                     133/233
      Verifying  : systemd-219-78.el7.x86_64                                                                      134/233
      Verifying  : 7:device-mapper-1.02.170-6.el7.x86_64                                                          135/233
      Verifying  : iwl100-firmware-39.31.5.1-79.el7.noarch                                                        136/233
      Verifying  : openssh-server-7.4p1-21.el7.x86_64                                                             137/233
      Verifying  : libblkid-2.23.2-65.el7.x86_64                                                                  138/233
      Verifying  : 1:grub2-common-2.02-0.86.el7.centos.noarch                                                     139/233
      Verifying  : rpm-libs-4.11.3-45.el7.x86_64                                                                  140/233
      Verifying  : iwl6000g2b-firmware-18.168.6.1-79.el7.noarch                                                   141/233
      Verifying  : 12:dhcp-libs-4.2.5-82.el7.centos.x86_64                                                        142/233
      Verifying  : 1:grub2-tools-2.02-0.86.el7.centos.x86_64                                                      143/233
      Verifying  : 1:openssl-libs-1.0.2k-19.el7.x86_64                                                            144/233
      Verifying  : 1:NetworkManager-team-1.18.8-1.el7.x86_64                                                      145/233
      Verifying  : kernel-tools-libs-3.10.0-1160.el7.x86_64                                                       146/233
      Verifying  : iwl3160-firmware-25.30.13.0-79.el7.noarch                                                      147/233
      Verifying  : iwl6000-firmware-9.221.4.1-79.el7.noarch                                                       148/233
      Verifying  : sudo-1.8.23-10.el7.x86_64                                                                      149/233
      Verifying  : 7:lvm2-2.02.187-6.el7.x86_64                                                                   150/233
      Verifying  : nss-3.44.0-7.el7_7.x86_64                                                                      151/233
      Verifying  : iwl3945-firmware-15.32.2.9-79.el7.noarch                                                       152/233
      Verifying  : selinux-policy-3.13.1-268.el7.noarch                                                           153/233
      Verifying  : 1:NetworkManager-libnm-1.18.8-1.el7.x86_64                                                     154/233
      Verifying  : libuuid-2.23.2-65.el7.x86_64                                                                   155/233
      Verifying  : 2:vim-minimal-7.4.629-7.el7.x86_64                                                             156/233
      Verifying  : nss-tools-3.44.0-7.el7_7.x86_64                                                                157/233
      Verifying  : 12:dhclient-4.2.5-82.el7.centos.x86_64                                                         158/233
      Verifying  : 1:wpa_supplicant-2.6-12.el7.x86_64                                                             159/233
      Verifying  : 2:microcode_ctl-2.1-73.el7.x86_64                                                              160/233
      Verifying  : 1:grub2-2.02-0.86.el7.centos.x86_64                                                            161/233
      Verifying  : kbd-misc-1.15.5-15.el7.noarch                                                                  162/233
      Verifying  : 1:NetworkManager-1.18.8-1.el7.x86_64                                                           163/233
      Verifying  : initscripts-9.49.53-1.el7.x86_64                                                               164/233
      Verifying  : 32:bind-export-libs-9.11.4-26.P2.el7.x86_64                                                    165/233
      Verifying  : rsyslog-8.24.0-55.el7.x86_64                                                                   166/233
      Verifying  : nss-sysinit-3.44.0-7.el7_7.x86_64                                                              167/233
      Verifying  : iwl6050-firmware-41.28.5.1-79.el7.noarch                                                       168/233
      Verifying  : iwl135-firmware-18.168.6.1-79.el7.noarch                                                       169/233
      Verifying  : openssh-clients-7.4p1-21.el7.x86_64                                                            170/233
      Verifying  : 1:openssl-1.0.2k-19.el7.x86_64                                                                 171/233
      Verifying  : 7:device-mapper-event-libs-1.02.170-6.el7.x86_64                                               172/233
      Verifying  : rpm-python-4.11.3-45.el7.x86_64                                                                173/233
      Verifying  : coreutils-8.22-24.el7.x86_64                                                                   174/233
      Verifying  : tzdata-2020a-1.el7.noarch                                                                      175/233
      Verifying  : libcurl-7.29.0-59.el7.x86_64                                                                   176/233
      Verifying  : 7:lvm2-libs-2.02.187-6.el7.x86_64                                                              177/233
      Verifying  : 1:grub2-pc-2.02-0.86.el7.centos.x86_64                                                         178/233
      Verifying  : krb5-libs-1.15.1-50.el7.x86_64                                                                 179/233
      Verifying  : cronie-anacron-1.4.11-23.el7.x86_64                                                            180/233
      Verifying  : gzip-1.5-10.el7.x86_64                                                                         181/233
      Verifying  : nspr-4.21.0-1.el7.x86_64                                                                       182/233
      Verifying  : nss-softokn-freebl-3.44.0-8.el7_7.x86_64                                                       183/233
      Verifying  : iwl5000-firmware-8.83.5.1_1-79.el7.noarch                                                      184/233
      Verifying  : python-firewall-0.6.3-11.el7.noarch                                                            185/233
      Verifying  : rpm-build-libs-4.11.3-45.el7.x86_64                                                            186/233
      Verifying  : iwl4965-firmware-228.61.2.24-79.el7.noarch                                                     187/233
      Verifying  : binutils-2.27-44.base.el7.x86_64                                                               188/233
      Verifying  : libxml2-2.9.1-6.el7.5.x86_64                                                                   189/233
      Verifying  : libcroco-0.6.12-4.el7.x86_64                                                                   190/233
      Verifying  : centos-release-7-9.2009.0.el7.centos.x86_64                                                    191/233
      Verifying  : systemd-libs-219-78.el7.x86_64                                                                 192/233
      Verifying  : 1:dmidecode-3.2-5.el7.x86_64                                                                   193/233
      Verifying  : iwl7260-firmware-25.30.13.0-79.el7.noarch                                                      194/233
      Verifying  : cronie-1.4.11-23.el7.x86_64                                                                    195/233
      Verifying  : openldap-2.4.44-22.el7.x86_64                                                                  196/233
      Verifying  : iwl6000g2a-firmware-18.168.6.1-79.el7.noarch                                                   197/233
      Verifying  : kbd-legacy-1.15.5-15.el7.noarch                                                                198/233
      Verifying  : tuned-2.11.0-9.el7.noarch                                                                      199/233
      Verifying  : iwl2030-firmware-18.168.6.1-79.el7.noarch                                                      200/233
      Verifying  : 7:device-mapper-libs-1.02.170-6.el7.x86_64                                                     201/233
      Verifying  : kbd-1.15.5-15.el7.x86_64                                                                       202/233
      Verifying  : python-perf-3.10.0-1160.el7.x86_64                                                             203/233
      Verifying  : 1:NetworkManager-tui-1.18.8-1.el7.x86_64                                                       204/233
      Verifying  : diffutils-3.3-5.el7.x86_64                                                                     205/233
      Verifying  : xz-libs-5.2.2-1.el7.x86_64                                                                     206/233
      Verifying  : polkit-0.112-26.el7.x86_64                                                                     207/233
      Verifying  : curl-7.29.0-59.el7.x86_64                                                                      208/233
      Verifying  : iprutils-2.4.17.1-3.el7.x86_64                                                                 209/233
      Verifying  : 1:NetworkManager-wifi-1.18.8-1.el7.x86_64                                                      210/233
      Verifying  : 1:grub2-pc-modules-2.02-0.86.el7.centos.noarch                                                 211/233
      Verifying  : expat-2.1.0-12.el7.x86_64                                                                      212/233
      Verifying  : glibc-2.17-317.el7.x86_64                                                                      213/233
      Verifying  : bash-4.2.46-34.el7.x86_64                                                                      214/233
      Verifying  : openssh-7.4p1-21.el7.x86_64                                                                    215/233
      Verifying  : kpartx-0.4.9-133.el7.x86_64                                                                    216/233
      Verifying  : nss-util-3.44.0-4.el7_7.x86_64                                                                 217/233
      Verifying  : python-libs-2.7.5-89.el7.x86_64                                                                218/233
      Verifying  : iwl105-firmware-18.168.6.1-79.el7.noarch                                                       219/233
      Verifying  : kernel-tools-3.10.0-1160.el7.x86_64                                                            220/233
      Verifying  : xz-5.2.2-1.el7.x86_64                                                                          221/233
      Verifying  : 12:dhcp-common-4.2.5-82.el7.centos.x86_64                                                      222/233
      Verifying  : firewalld-0.6.3-11.el7.noarch                                                                  223/233
      Verifying  : kexec-tools-2.0.15-51.el7.x86_64                                                               224/233
      Verifying  : 1:grub2-tools-minimal-2.02-0.86.el7.centos.x86_64                                              225/233
      Verifying  : nss-softokn-3.44.0-8.el7_7.x86_64                                                              226/233
      Verifying  : systemd-sysv-219-78.el7.x86_64                                                                 227/233
      Verifying  : 1:grub2-tools-extra-2.02-0.86.el7.centos.x86_64                                                228/233
      Verifying  : device-mapper-persistent-data-0.8.5-3.el7.x86_64                                               229/233
      Verifying  : libsmartcols-2.23.2-65.el7.x86_64                                                              230/233
      Verifying  : cyrus-sasl-lib-2.1.26-23.el7.x86_64                                                            231/233
      Verifying  : util-linux-2.23.2-65.el7.x86_64                                                                232/233
      Verifying  : libmount-2.23.2-65.el7.x86_64                                                                  233/233
    
    Installed:
      kernel.x86_64 0:3.10.0-1160.92.1.el7
    
    Updated:
      NetworkManager.x86_64 1:1.18.8-2.el7_9                     NetworkManager-libnm.x86_64 1:1.18.8-2.el7_9
      NetworkManager-team.x86_64 1:1.18.8-2.el7_9                NetworkManager-tui.x86_64 1:1.18.8-2.el7_9
      NetworkManager-wifi.x86_64 1:1.18.8-2.el7_9                bash.x86_64 0:4.2.46-35.el7_9
      bind-export-libs.x86_64 32:9.11.4-26.P2.el7_9.13           binutils.x86_64 0:2.27-44.base.el7_9.1
      ca-certificates.noarch 0:2022.2.54-74.el7_9                centos-release.x86_64 0:7-9.2009.1.el7.centos
      coreutils.x86_64 0:8.22-24.el7_9.2                         cronie.x86_64 0:1.4.11-25.el7_9
      cronie-anacron.x86_64 0:1.4.11-25.el7_9                    curl.x86_64 0:7.29.0-59.el7_9.1
      cyrus-sasl-lib.x86_64 0:2.1.26-24.el7_9                    device-mapper.x86_64 7:1.02.170-6.el7_9.5
      device-mapper-event.x86_64 7:1.02.170-6.el7_9.5            device-mapper-event-libs.x86_64 7:1.02.170-6.el7_9.5
      device-mapper-libs.x86_64 7:1.02.170-6.el7_9.5             device-mapper-persistent-data.x86_64 0:0.8.5-3.el7_9.2
      dhclient.x86_64 12:4.2.5-83.el7.centos.1                   dhcp-common.x86_64 12:4.2.5-83.el7.centos.1
      dhcp-libs.x86_64 12:4.2.5-83.el7.centos.1                  diffutils.x86_64 0:3.3-6.el7_9
      dmidecode.x86_64 1:3.2-5.el7_9.1                           expat.x86_64 0:2.1.0-15.el7_9
      firewalld.noarch 0:0.6.3-13.el7_9                          firewalld-filesystem.noarch 0:0.6.3-13.el7_9
      freetype.x86_64 0:2.8-14.el7_9.1                           glib2.x86_64 0:2.56.1-9.el7_9
      glibc.x86_64 0:2.17-326.el7_9                              glibc-common.x86_64 0:2.17-326.el7_9
      grub2.x86_64 1:2.02-0.87.0.2.el7.centos.11                 grub2-common.noarch 1:2.02-0.87.0.2.el7.centos.11
      grub2-pc.x86_64 1:2.02-0.87.0.2.el7.centos.11              grub2-pc-modules.noarch 1:2.02-0.87.0.2.el7.centos.11
      grub2-tools.x86_64 1:2.02-0.87.0.2.el7.centos.11           grub2-tools-extra.x86_64 1:2.02-0.87.0.2.el7.centos.11
      grub2-tools-minimal.x86_64 1:2.02-0.87.0.2.el7.centos.11   gzip.x86_64 0:1.5-11.el7_9
      initscripts.x86_64 0:9.49.53-1.el7_9.1                     iprutils.x86_64 0:2.4.17.1-3.el7_7
      iwl100-firmware.noarch 0:39.31.5.1-80.el7_9                iwl1000-firmware.noarch 1:39.31.5.1-80.el7_9
      iwl105-firmware.noarch 0:18.168.6.1-80.el7_9               iwl135-firmware.noarch 0:18.168.6.1-80.el7_9
      iwl2000-firmware.noarch 0:18.168.6.1-80.el7_9              iwl2030-firmware.noarch 0:18.168.6.1-80.el7_9
      iwl3160-firmware.noarch 0:25.30.13.0-80.el7_9              iwl3945-firmware.noarch 0:15.32.2.9-80.el7_9
      iwl4965-firmware.noarch 0:228.61.2.24-80.el7_9             iwl5000-firmware.noarch 0:8.83.5.1_1-80.el7_9
      iwl5150-firmware.noarch 0:8.24.2.2-80.el7_9                iwl6000-firmware.noarch 0:9.221.4.1-80.el7_9
      iwl6000g2a-firmware.noarch 0:18.168.6.1-80.el7_9           iwl6000g2b-firmware.noarch 0:18.168.6.1-80.el7_9
      iwl6050-firmware.noarch 0:41.28.5.1-80.el7_9               iwl7260-firmware.noarch 0:25.30.13.0-80.el7_9
      kbd.x86_64 0:1.15.5-16.el7_9                               kbd-legacy.noarch 0:1.15.5-16.el7_9
      kbd-misc.noarch 0:1.15.5-16.el7_9                          kernel-tools.x86_64 0:3.10.0-1160.92.1.el7
      kernel-tools-libs.x86_64 0:3.10.0-1160.92.1.el7            kexec-tools.x86_64 0:2.0.15-51.el7_9.3
      kpartx.x86_64 0:0.4.9-136.el7_9                            krb5-libs.x86_64 0:1.15.1-55.el7_9
      libblkid.x86_64 0:2.23.2-65.el7_9.1                        libcroco.x86_64 0:0.6.12-6.el7_9
      libcurl.x86_64 0:7.29.0-59.el7_9.1                         libmount.x86_64 0:2.23.2-65.el7_9.1
      libsmartcols.x86_64 0:2.23.2-65.el7_9.1                    libuuid.x86_64 0:2.23.2-65.el7_9.1
      libxml2.x86_64 0:2.9.1-6.el7_9.6                           linux-firmware.noarch 0:20200421-80.git78c0348.el7_9
      lvm2.x86_64 7:2.02.187-6.el7_9.5                           lvm2-libs.x86_64 7:2.02.187-6.el7_9.5
      microcode_ctl.x86_64 2:2.1-73.15.el7_9                     nspr.x86_64 0:4.34.0-3.1.el7_9
      nss.x86_64 0:3.79.0-5.el7_9                                nss-pem.x86_64 0:1.0.3-7.el7_9.1
      nss-softokn.x86_64 0:3.79.0-4.el7_9                        nss-softokn-freebl.x86_64 0:3.79.0-4.el7_9
      nss-sysinit.x86_64 0:3.79.0-5.el7_9                        nss-tools.x86_64 0:3.79.0-5.el7_9
      nss-util.x86_64 0:3.79.0-1.el7_9                           openldap.x86_64 0:2.4.44-25.el7_9
      openssh.x86_64 0:7.4p1-22.el7_9                            openssh-clients.x86_64 0:7.4p1-22.el7_9
      openssh-server.x86_64 0:7.4p1-22.el7_9                     openssl.x86_64 1:1.0.2k-26.el7_9
      openssl-libs.x86_64 1:1.0.2k-26.el7_9                      polkit.x86_64 0:0.112-26.el7_9.1
      python.x86_64 0:2.7.5-93.el7_9                             python-firewall.noarch 0:0.6.3-13.el7_9
      python-libs.x86_64 0:2.7.5-93.el7_9                        python-perf.x86_64 0:3.10.0-1160.92.1.el7
      rpm.x86_64 0:4.11.3-48.el7_9                               rpm-build-libs.x86_64 0:4.11.3-48.el7_9
      rpm-libs.x86_64 0:4.11.3-48.el7_9                          rpm-python.x86_64 0:4.11.3-48.el7_9
      rsyslog.x86_64 0:8.24.0-57.el7_9.3                         selinux-policy.noarch 0:3.13.1-268.el7_9.2
      selinux-policy-targeted.noarch 0:3.13.1-268.el7_9.2        sudo.x86_64 0:1.8.23-10.el7_9.3
      systemd.x86_64 0:219-78.el7_9.7                            systemd-libs.x86_64 0:219-78.el7_9.7
      systemd-sysv.x86_64 0:219-78.el7_9.7                       tuned.noarch 0:2.11.0-12.el7_9
      tzdata.noarch 0:2023c-1.el7                                util-linux.x86_64 0:2.23.2-65.el7_9.1
      vim-minimal.x86_64 2:7.4.629-8.el7_9                       virt-what.x86_64 0:1.18-4.el7_9.1
      wpa_supplicant.x86_64 1:2.6-12.el7_9.2                     xz.x86_64 0:5.2.2-2.el7_9
      xz-libs.x86_64 0:5.2.2-2.el7_9                             zlib.x86_64 0:1.2.7-21.el7_9
    
    Complete!
    Loaded plugins: fastestmirror
    Loading mirror speeds from cached hostfile
     * base: centos.mirror.net.in
     * epel: epel.excellmedia.net
     * extras: centos.mirror.net.in
     * updates: centos.mirror.net.in
    Resolving Dependencies
    --> Running transaction check
    ---> Package ceph-deploy.noarch 0:2.0.1-0 will be installed
    ---> Package python2-pip.noarch 0:8.1.2-14.el7 will be installed
    --> Processing Dependency: python-setuptools for package: python2-pip-8.1.2-14.el7.noarch
    --> Running transaction check
    ---> Package python-setuptools.noarch 0:0.9.8-7.el7 will be installed
    --> Processing Dependency: python-backports-ssl_match_hostname for package: python-setuptools-0.9.8-7.el7.noarch
    --> Running transaction check
    ---> Package python-backports-ssl_match_hostname.noarch 0:3.5.0.1-1.el7 will be installed
    --> Processing Dependency: python-ipaddress for package: python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch
    --> Processing Dependency: python-backports for package: python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch
    --> Running transaction check
    ---> Package python-backports.x86_64 0:1.0-8.el7 will be installed
    ---> Package python-ipaddress.noarch 0:1.0.16-2.el7 will be installed
    --> Finished Dependency Resolution
    
    Dependencies Resolved
    
    ======================================================================================================================
     Package                                       Arch             Version                   Repository             Size
    ======================================================================================================================
    Installing:
     ceph-deploy                                   noarch           2.0.1-0                   Ceph-noarch           286 k
     python2-pip                                   noarch           8.1.2-14.el7              epel                  1.7 M
    Installing for dependencies:
     python-backports                              x86_64           1.0-8.el7                 base                  5.8 k
     python-backports-ssl_match_hostname           noarch           3.5.0.1-1.el7             base                   13 k
     python-ipaddress                              noarch           1.0.16-2.el7              base                   34 k
     python-setuptools                             noarch           0.9.8-7.el7               base                  397 k
    
    Transaction Summary
    ======================================================================================================================
    Install  2 Packages (+4 Dependent packages)
    
    Total download size: 2.4 M
    Installed size: 11 M
    Downloading packages:
    (1/6): python-backports-1.0-8.el7.x86_64.rpm                                                   | 5.8 kB  00:00:00
    (2/6): python-ipaddress-1.0.16-2.el7.noarch.rpm                                                |  34 kB  00:00:00
    (3/6): python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch.rpm                            |  13 kB  00:00:00
    (4/6): python-setuptools-0.9.8-7.el7.noarch.rpm                                                | 397 kB  00:00:00
    warning: /var/cache/yum/x86_64/7/epel/packages/python2-pip-8.1.2-14.el7.noarch.rpm: Header V4 RSA/SHA256 Signature, key ID 352c64e5: NOKEY
    Public key for python2-pip-8.1.2-14.el7.noarch.rpm is not installed
    (5/6): python2-pip-8.1.2-14.el7.noarch.rpm                                                     | 1.7 MB  00:00:00
    warning: /var/cache/yum/x86_64/7/Ceph-noarch/packages/ceph-deploy-2.0.1-0.noarch.rpm: Header V4 RSA/SHA256 Signature, key ID 460f3994: NOKEY
    Public key for ceph-deploy-2.0.1-0.noarch.rpm is not installed
    (6/6): ceph-deploy-2.0.1-0.noarch.rpm                                                          | 286 kB  00:00:01
    ----------------------------------------------------------------------------------------------------------------------
    Total                                                                                 1.7 MB/s | 2.4 MB  00:00:01
    Retrieving key from file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
    Importing GPG key 0x352C64E5:
     Userid     : "Fedora EPEL (7) <epel@fedoraproject.org>"
     Fingerprint: 91e9 7d7c 4a5e 96f1 7f3e 888f 6a2f aea2 352c 64e5
     Package    : epel-release-7-14.noarch (@/epel-release-latest-7.noarch)
     From       : /etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
    Retrieving key from https://download.ceph.com/keys/release.asc
    Importing GPG key 0x460F3994:
     Userid     : "Ceph.com (release key) <security@ceph.com>"
     Fingerprint: 08b7 3419 ac32 b4e9 66c1 a330 e84a c2c0 460f 3994
     From       : https://download.ceph.com/keys/release.asc
    Running transaction check
    Running transaction test
    Transaction test succeeded
    Running transaction
      Installing : python-ipaddress-1.0.16-2.el7.noarch                                                               1/6
      Installing : python-backports-1.0-8.el7.x86_64                                                                  2/6
      Installing : python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch                                           3/6
      Installing : python-setuptools-0.9.8-7.el7.noarch                                                               4/6
      Installing : python2-pip-8.1.2-14.el7.noarch                                                                    5/6
      Installing : ceph-deploy-2.0.1-0.noarch                                                                         6/6
      Verifying  : python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch                                           1/6
      Verifying  : python2-pip-8.1.2-14.el7.noarch                                                                    2/6
      Verifying  : python-backports-1.0-8.el7.x86_64                                                                  3/6
      Verifying  : python-ipaddress-1.0.16-2.el7.noarch                                                               4/6
      Verifying  : ceph-deploy-2.0.1-0.noarch                                                                         5/6
      Verifying  : python-setuptools-0.9.8-7.el7.noarch                                                               6/6
    
    Installed:
      ceph-deploy.noarch 0:2.0.1-0                            python2-pip.noarch 0:8.1.2-14.el7
    
    Dependency Installed:
      python-backports.x86_64 0:1.0-8.el7             python-backports-ssl_match_hostname.noarch 0:3.5.0.1-1.el7
      python-ipaddress.noarch 0:1.0.16-2.el7          python-setuptools.noarch 0:0.9.8-7.el7
    
    Complete!
    [root@ceph2 ~]# su - sephadm
    su: user sephadm does not exist
    [root@ceph2 ~]# su - cephadm
    [cephadm@ceph2 ~]$ ssh-keygen
    Generating public/private rsa key pair.
    Enter file in which to save the key (/home/cephadm/.ssh/id_rsa):
    Created directory '/home/cephadm/.ssh'.
    Enter passphrase (empty for no passphrase):
    Enter same passphrase again:
    Your identification has been saved in /home/cephadm/.ssh/id_rsa.
    Your public key has been saved in /home/cephadm/.ssh/id_rsa.pub.
    The key fingerprint is:
    SHA256:ohnhbnzUvMDSLWe90kLCWOCiPuxJx31e2XCkZxB9rPQ cephadm@ceph2.in
    The key's randomart image is:
    +---[RSA 2048]----+
    |    .    .. .    |
    |   . .    .o o   |
    |  . o .  ...+    |
    | . o B + .+. E   |
    |.   = X So.+     |
    |o .o.* O oB.     |
    | = o*...+oo.     |
    |o +. .o .o       |
    | o     .         |
    +----[SHA256]-----+
    [cephadm@ceph2 ~]$ ssh-copy-id cephadm@ceph1.in
    /bin/ssh-copy-id: INFO: Source of key(s) to be installed: "/home/cephadm/.ssh/id_rsa.pub"
    The authenticity of host 'ceph1.in (192.168.239.154)' can't be established.
    ECDSA key fingerprint is SHA256:JbQFp/4SaYFpszIjBlpttyXEMGiNiL5rz5A+HcTkXQo.
    ECDSA key fingerprint is MD5:9c:7c:9f:fd:38:b0:70:5c:20:ab:69:3b:07:05:3f:1c.
    Are you sure you want to continue connecting (yes/no)? yes
    /bin/ssh-copy-id: INFO: attempting to log in with the new key(s), to filter out any that are already installed
    /bin/ssh-copy-id: INFO: 1 key(s) remain to be installed -- if you are prompted now it is to install the new keys
    cephadm@ceph1.in's password:
    Permission denied, please try again.
    cephadm@ceph1.in's password:
    
    Number of key(s) added: 1
    
    Now try logging into the machine, with:   "ssh 'cephadm@ceph1.in'"
    and check to make sure that only the key(s) you wanted were added.
    
    [cephadm@ceph2 ~]$ ssh cephadm@ceph1.in
    Last failed login: Sun Jul 16 21:29:52 IST 2023 from ceph2.in on ssh:notty
    There was 1 failed login attempt since the last successful login.
    [cephadm@ceph1 ~]$ exit
    logout
    Connection to ceph1.in closed.
    [cephadm@ceph2 ~]$ ssh-copy-id cephadm@ceph2.in
    /bin/ssh-copy-id: INFO: Source of key(s) to be installed: "/home/cephadm/.ssh/id_rsa.pub"
    The authenticity of host 'ceph2.in (192.168.239.155)' can't be established.
    ECDSA key fingerprint is SHA256:JbQFp/4SaYFpszIjBlpttyXEMGiNiL5rz5A+HcTkXQo.
    ECDSA key fingerprint is MD5:9c:7c:9f:fd:38:b0:70:5c:20:ab:69:3b:07:05:3f:1c.
    Are you sure you want to continue connecting (yes/no)? yes
    /bin/ssh-copy-id: INFO: attempting to log in with the new key(s), to filter out any that are already installed
    /bin/ssh-copy-id: INFO: 1 key(s) remain to be installed -- if you are prompted now it is to install the new keys
    cephadm@ceph2.in's password:
    
    Number of key(s) added: 1
    
    Now try logging into the machine, with:   "ssh 'cephadm@ceph2.in'"
    and check to make sure that only the key(s) you wanted were added.
    
    [cephadm@ceph2 ~]$ ssh-copy-id cephadm@ceph3.in
    /bin/ssh-copy-id: INFO: Source of key(s) to be installed: "/home/cephadm/.ssh/id_rsa.pub"
    The authenticity of host 'ceph3.in (192.168.239.156)' can't be established.
    ECDSA key fingerprint is SHA256:JbQFp/4SaYFpszIjBlpttyXEMGiNiL5rz5A+HcTkXQo.
    ECDSA key fingerprint is MD5:9c:7c:9f:fd:38:b0:70:5c:20:ab:69:3b:07:05:3f:1c.
    Are you sure you want to continue connecting (yes/no)? yes
    /bin/ssh-copy-id: INFO: attempting to log in with the new key(s), to filter out any that are already installed
    /bin/ssh-copy-id: INFO: 1 key(s) remain to be installed -- if you are prompted now it is to install the new keys
    cephadm@ceph3.in's password:
    
    Number of key(s) added: 1
    
    Now try logging into the machine, with:   "ssh 'cephadm@ceph3.in'"
    and check to make sure that only the key(s) you wanted were added.
    
    [cephadm@ceph2 ~]$ ssh-copy-id cephadm@ceph4.in
    /bin/ssh-copy-id: INFO: Source of key(s) to be installed: "/home/cephadm/.ssh/id_rsa.pub"
    The authenticity of host 'ceph4.in (192.168.239.157)' can't be established.
    ECDSA key fingerprint is SHA256:JbQFp/4SaYFpszIjBlpttyXEMGiNiL5rz5A+HcTkXQo.
    ECDSA key fingerprint is MD5:9c:7c:9f:fd:38:b0:70:5c:20:ab:69:3b:07:05:3f:1c.
    Are you sure you want to continue connecting (yes/no)? yes
    /bin/ssh-copy-id: INFO: attempting to log in with the new key(s), to filter out any that are already installed
    /bin/ssh-copy-id: INFO: 1 key(s) remain to be installed -- if you are prompted now it is to install the new keys
    cephadm@ceph4.in's password:
    
    Number of key(s) added: 1
    
    Now try logging into the machine, with:   "ssh 'cephadm@ceph4.in'"
    and check to make sure that only the key(s) you wanted were added.
    
    [cephadm@ceph2 ~]$ ssh-copy-id cephadm@ceph5.in
    /bin/ssh-copy-id: INFO: Source of key(s) to be installed: "/home/cephadm/.ssh/id_rsa.pub"
    The authenticity of host 'ceph5.in (192.168.239.158)' can't be established.
    ECDSA key fingerprint is SHA256:JbQFp/4SaYFpszIjBlpttyXEMGiNiL5rz5A+HcTkXQo.
    ECDSA key fingerprint is MD5:9c:7c:9f:fd:38:b0:70:5c:20:ab:69:3b:07:05:3f:1c.
    Are you sure you want to continue connecting (yes/no)? yes
    /bin/ssh-copy-id: INFO: attempting to log in with the new key(s), to filter out any that are already installed
    /bin/ssh-copy-id: INFO: 1 key(s) remain to be installed -- if you are prompted now it is to install the new keys
    cephadm@ceph5.in's password:
    
    Number of key(s) added: 1
    
    Now try logging into the machine, with:   "ssh 'cephadm@ceph5.in'"
    and check to make sure that only the key(s) you wanted were added.
    
    [cephadm@ceph2 ~]$ vim ~/.ssh/config
    [cephadm@ceph2 ~]$ chmod 644 ~/.ssh/config
    [cephadm@ceph2 ~]$ ssh cephadm@ceph1.in
    ssh: Could not resolve hostname ceph1: Name or service not known
    [cephadm@ceph2 ~]$ ssh cephadm@ceph1.in
    ssh: Could not resolve hostname ceph1: Name or service not known
    [cephadm@ceph2 ~]$ vim ~/.ssh/config
    [cephadm@ceph2 ~]$ ssh cephadm@ceph1.in
    Last login: Sun Jul 16 21:30:20 2023 from ceph2.in
    [cephadm@ceph1 ~]$ exit
    logout
    Connection to ceph1.in closed.
    [cephadm@ceph2 ~]$ ssh cephadm@ceph3.in
    [cephadm@ceph3 ~]$ exit
    logout
    Connection to ceph3.in closed.
    [cephadm@ceph2 ~]$ ssh cephadm@ceph4.in
    [cephadm@ceph4 ~]$ exit
    logout
    Connection to ceph4.in closed.
    [cephadm@ceph2 ~]$ mkdir ceph_cluster
    [cephadm@ceph2 ~]$ cd ceph_cluster/
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy new ceph-monitor
    usage: ceph-deploy new [-h] [--no-ssh-copykey] [--fsid FSID]
                           [--cluster-network CLUSTER_NETWORK]
                           [--public-network PUBLIC_NETWORK]
                           MON [MON ...]
    ceph-deploy new: error: hostname: ceph-monitor is not resolvable
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy new ceph1.in
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy new ceph1.in
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  func                          : <function new at 0x7f83cfb2ded8>
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f83cf2a4b48>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  ssh_copykey                   : True
    [ceph_deploy.cli][INFO  ]  mon                           : ['ceph1.in']
    [ceph_deploy.cli][INFO  ]  public_network                : None
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  cluster_network               : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  fsid                          : None
    [ceph_deploy.new][DEBUG ] Creating new cluster named ceph
    [ceph_deploy.new][INFO  ] making sure passwordless SSH succeeds
    [ceph1.in][DEBUG ] connected to host: ceph2.in
    [ceph1.in][INFO  ] Running command: ssh -CT -o BatchMode=yes ceph1.in
    [ceph1.in][DEBUG ] connection detected need for sudo
    [ceph1.in][DEBUG ] connected to host: ceph1.in
    [ceph1.in][DEBUG ] detect platform information from remote host
    [ceph1.in][DEBUG ] detect machine type
    [ceph1.in][DEBUG ] find the location of an executable
    [ceph1.in][INFO  ] Running command: sudo /usr/sbin/ip link show
    [ceph1.in][INFO  ] Running command: sudo /usr/sbin/ip addr show
    [ceph1.in][DEBUG ] IP addresses found: [u'192.168.239.154']
    [ceph_deploy.new][DEBUG ] Resolving host ceph1.in
    [ceph_deploy.new][DEBUG ] Monitor ceph1 at 192.168.239.154
    [ceph_deploy.new][DEBUG ] Monitor initial members are ['ceph1']
    [ceph_deploy.new][DEBUG ] Monitor addrs are ['192.168.239.154']
    [ceph_deploy.new][DEBUG ] Creating a random mon key...
    [ceph_deploy.new][DEBUG ] Writing monitor keyring to ceph.mon.keyring...
    [ceph_deploy.new][DEBUG ] Writing initial config to ceph.conf...
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy new ceph1.in
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy new ceph1.in
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  func                          : <function new at 0x7f538e27ced8>
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f538d9f3b48>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  ssh_copykey                   : True
    [ceph_deploy.cli][INFO  ]  mon                           : ['ceph1.in']
    [ceph_deploy.cli][INFO  ]  public_network                : None
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  cluster_network               : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  fsid                          : None
    [ceph_deploy.new][DEBUG ] Creating new cluster named ceph
    [ceph_deploy.new][INFO  ] making sure passwordless SSH succeeds
    [ceph1.in][DEBUG ] connected to host: ceph2.in
    [ceph1.in][INFO  ] Running command: ssh -CT -o BatchMode=yes ceph1.in
    [ceph1.in][DEBUG ] connection detected need for sudo
    [ceph1.in][DEBUG ] connected to host: ceph1.in
    [ceph1.in][DEBUG ] detect platform information from remote host
    [ceph1.in][DEBUG ] detect machine type
    [ceph1.in][DEBUG ] find the location of an executable
    [ceph1.in][INFO  ] Running command: sudo /usr/sbin/ip link show
    [ceph1.in][INFO  ] Running command: sudo /usr/sbin/ip addr show
    [ceph1.in][DEBUG ] IP addresses found: [u'192.168.239.154']
    [ceph_deploy.new][DEBUG ] Resolving host ceph1.in
    [ceph_deploy.new][DEBUG ] Monitor ceph1 at 192.168.239.154
    [ceph_deploy.new][DEBUG ] Monitor initial members are ['ceph1']
    [ceph_deploy.new][DEBUG ] Monitor addrs are ['192.168.239.154']
    [ceph_deploy.new][DEBUG ] Creating a random mon key...
    [ceph_deploy.new][DEBUG ] Writing monitor keyring to ceph.mon.keyring...
    [ceph_deploy.new][DEBUG ] Writing initial config to ceph.conf...
    [cephadm@ceph2 ceph_cluster]$ vim ceph
    ceph.conf             ceph-deploy-ceph.log  ceph.mon.keyring
    [cephadm@ceph2 ceph_cluster]$ vim ceph
    ceph.conf             ceph-deploy-ceph.log  ceph.mon.keyring
    [cephadm@ceph2 ceph_cluster]$ vim ceph
    ceph.conf             ceph-deploy-ceph.log  ceph.mon.keyring
    [cephadm@ceph2 ceph_cluster]$ vim ceph
    ceph.conf             ceph-deploy-ceph.log  ceph.mon.keyring
    [cephadm@ceph2 ceph_cluster]$ vim ceph.conf
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy install ceph2.in ceph3.in ceph4.in ceph1.in
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy install ceph2.in ceph3.in ceph4.in ceph1.in
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  testing                       : None
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f22b9613290>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  dev_commit                    : None
    [ceph_deploy.cli][INFO  ]  install_mds                   : False
    [ceph_deploy.cli][INFO  ]  stable                        : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  adjust_repos                  : True
    [ceph_deploy.cli][INFO  ]  func                          : <function install at 0x7f22ba0e06e0>
    [ceph_deploy.cli][INFO  ]  install_mgr                   : False
    [ceph_deploy.cli][INFO  ]  install_all                   : False
    [ceph_deploy.cli][INFO  ]  repo                          : False
    [ceph_deploy.cli][INFO  ]  host                          : ['ceph2.in', 'ceph3.in', 'ceph4.in', 'ceph1.in']
    [ceph_deploy.cli][INFO  ]  install_rgw                   : False
    [ceph_deploy.cli][INFO  ]  install_tests                 : False
    [ceph_deploy.cli][INFO  ]  repo_url                      : None
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  install_osd                   : False
    [ceph_deploy.cli][INFO  ]  version_kind                  : stable
    [ceph_deploy.cli][INFO  ]  install_common                : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  dev                           : master
    [ceph_deploy.cli][INFO  ]  nogpgcheck                    : False
    [ceph_deploy.cli][INFO  ]  local_mirror                  : None
    [ceph_deploy.cli][INFO  ]  release                       : None
    [ceph_deploy.cli][INFO  ]  install_mon                   : False
    [ceph_deploy.cli][INFO  ]  gpg_url                       : None
    [ceph_deploy.install][DEBUG ] Installing stable version mimic on cluster ceph hosts ceph2.in ceph3.in ceph4.in ceph1.in
    [ceph_deploy.install][DEBUG ] Detecting platform for host ceph2.in ...
    [ceph2.in][DEBUG ] connection detected need for sudo
    [ceph2.in][DEBUG ] connected to host: ceph2.in
    [ceph2.in][DEBUG ] detect platform information from remote host
    [ceph2.in][DEBUG ] detect machine type
    [ceph_deploy.install][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph2.in][INFO  ] installing Ceph on ceph2.in
    [ceph2.in][INFO  ] Running command: sudo yum clean all
    [ceph2.in][DEBUG ] Loaded plugins: fastestmirror
    [ceph2.in][DEBUG ] Cleaning repos: Ceph Ceph-noarch base ceph-source epel extras updates
    [ceph2.in][DEBUG ] Cleaning up list of fastest mirrors
    [ceph2.in][INFO  ] Running command: sudo yum -y install epel-release
    [ceph2.in][DEBUG ] Loaded plugins: fastestmirror
    [ceph2.in][DEBUG ] Determining fastest mirrors
    [ceph2.in][DEBUG ]  * base: centos.mirror.net.in
    [ceph2.in][DEBUG ]  * epel: epel.excellmedia.net
    [ceph2.in][DEBUG ]  * extras: centos.mirror.net.in
    [ceph2.in][DEBUG ]  * updates: centos.mirror.net.in
    [ceph2.in][DEBUG ] Package epel-release-7-14.noarch already installed and latest version
    [ceph2.in][DEBUG ] Nothing to do
    [ceph2.in][INFO  ] Running command: sudo yum -y install yum-plugin-priorities
    [ceph2.in][DEBUG ] Loaded plugins: fastestmirror
    [ceph2.in][DEBUG ] Loading mirror speeds from cached hostfile
    [ceph2.in][DEBUG ]  * base: centos.mirror.net.in
    [ceph2.in][DEBUG ]  * epel: epel.excellmedia.net
    [ceph2.in][DEBUG ]  * extras: centos.mirror.net.in
    [ceph2.in][DEBUG ]  * updates: centos.mirror.net.in
    [ceph2.in][DEBUG ] Resolving Dependencies
    [ceph2.in][DEBUG ] --> Running transaction check
    [ceph2.in][DEBUG ] ---> Package yum-plugin-priorities.noarch 0:1.1.31-54.el7_8 will be installed
    [ceph2.in][DEBUG ] --> Finished Dependency Resolution
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] Dependencies Resolved
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] ================================================================================
    [ceph2.in][DEBUG ]  Package                    Arch        Version                 Repository
    [ceph2.in][DEBUG ]                                                                            Size
    [ceph2.in][DEBUG ] ================================================================================
    [ceph2.in][DEBUG ] Installing:
    [ceph2.in][DEBUG ]  yum-plugin-priorities      noarch      1.1.31-54.el7_8         base       29 k
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] Transaction Summary
    [ceph2.in][DEBUG ] ================================================================================
    [ceph2.in][DEBUG ] Install  1 Package
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] Total download size: 29 k
    [ceph2.in][DEBUG ] Installed size: 28 k
    [ceph2.in][DEBUG ] Downloading packages:
    [ceph2.in][DEBUG ] Running transaction check
    [ceph2.in][DEBUG ] Running transaction test
    [ceph2.in][DEBUG ] Transaction test succeeded
    [ceph2.in][DEBUG ] Running transaction
    [ceph2.in][DEBUG ]   Installing : yum-plugin-priorities-1.1.31-54.el7_8.noarch                 1/1
    [ceph2.in][DEBUG ]   Verifying  : yum-plugin-priorities-1.1.31-54.el7_8.noarch                 1/1
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] Installed:
    [ceph2.in][DEBUG ]   yum-plugin-priorities.noarch 0:1.1.31-54.el7_8
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] Complete!
    [ceph2.in][DEBUG ] Configure Yum priorities to include obsoletes
    [ceph2.in][WARNIN] check_obsoletes has been enabled for Yum priorities plugin
    [ceph2.in][INFO  ] Running command: sudo rpm --import https://download.ceph.com/keys/release.asc
    [ceph2.in][INFO  ] Running command: sudo yum remove -y ceph-release
    [ceph2.in][DEBUG ] Loaded plugins: fastestmirror, priorities
    [ceph2.in][DEBUG ] Resolving Dependencies
    [ceph2.in][DEBUG ] --> Running transaction check
    [ceph2.in][DEBUG ] ---> Package ceph-release.noarch 0:1-1.el7 will be erased
    [ceph2.in][DEBUG ] --> Finished Dependency Resolution
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] Dependencies Resolved
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] ================================================================================
    [ceph2.in][DEBUG ]  Package              Arch           Version            Repository         Size
    [ceph2.in][DEBUG ] ================================================================================
    [ceph2.in][DEBUG ] Removing:
    [ceph2.in][DEBUG ]  ceph-release         noarch         1-1.el7            installed         535
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] Transaction Summary
    [ceph2.in][DEBUG ] ================================================================================
    [ceph2.in][DEBUG ] Remove  1 Package
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] Installed size: 535
    [ceph2.in][DEBUG ] Downloading packages:
    [ceph2.in][DEBUG ] Running transaction check
    [ceph2.in][DEBUG ] Running transaction test
    [ceph2.in][DEBUG ] Transaction test succeeded
    [ceph2.in][DEBUG ] Running transaction
    [ceph2.in][DEBUG ]   Erasing    : ceph-release-1-1.el7.noarch                                  1/1
    [ceph2.in][DEBUG ]   Verifying  : ceph-release-1-1.el7.noarch                                  1/1
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] Removed:
    [ceph2.in][DEBUG ]   ceph-release.noarch 0:1-1.el7
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] Complete!
    [ceph2.in][INFO  ] Running command: sudo yum install -y https://download.ceph.com/rpm-mimic/el7/noarch/ceph-release-1-0.el7.noarch.rpm
    [ceph2.in][DEBUG ] Loaded plugins: fastestmirror, priorities
    [ceph2.in][DEBUG ] Examining /var/tmp/yum-root-WnqvfK/ceph-release-1-0.el7.noarch.rpm: ceph-release-1-1.el7.noarch
    [ceph2.in][DEBUG ] Marking /var/tmp/yum-root-WnqvfK/ceph-release-1-0.el7.noarch.rpm to be installed
    [ceph2.in][DEBUG ] Resolving Dependencies
    [ceph2.in][DEBUG ] --> Running transaction check
    [ceph2.in][DEBUG ] ---> Package ceph-release.noarch 0:1-1.el7 will be installed
    [ceph2.in][DEBUG ] --> Finished Dependency Resolution
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] Dependencies Resolved
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] ================================================================================
    [ceph2.in][DEBUG ]  Package          Arch       Version     Repository                        Size
    [ceph2.in][DEBUG ] ================================================================================
    [ceph2.in][DEBUG ] Installing:
    [ceph2.in][DEBUG ]  ceph-release     noarch     1-1.el7     /ceph-release-1-0.el7.noarch     535
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] Transaction Summary
    [ceph2.in][DEBUG ] ================================================================================
    [ceph2.in][DEBUG ] Install  1 Package
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] Total size: 535
    [ceph2.in][DEBUG ] Installed size: 535
    [ceph2.in][DEBUG ] Downloading packages:
    [ceph2.in][DEBUG ] Running transaction check
    [ceph2.in][DEBUG ] Running transaction test
    [ceph2.in][DEBUG ] Transaction test succeeded
    [ceph2.in][DEBUG ] Running transaction
    [ceph2.in][DEBUG ]   Installing : ceph-release-1-1.el7.noarch                                  1/1
    [ceph2.in][DEBUG ]   Verifying  : ceph-release-1-1.el7.noarch                                  1/1
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] Installed:
    [ceph2.in][DEBUG ]   ceph-release.noarch 0:1-1.el7
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] Complete!
    [ceph2.in][WARNIN] ensuring that /etc/yum.repos.d/ceph.repo contains a high priority
    [ceph2.in][WARNIN] altered ceph.repo priorities to contain: priority=1
    [ceph2.in][INFO  ] Running command: sudo yum -y install ceph ceph-radosgw
    [ceph2.in][DEBUG ] Loaded plugins: fastestmirror, priorities
    [ceph2.in][DEBUG ] Loading mirror speeds from cached hostfile
    [ceph2.in][DEBUG ]  * base: centos.mirror.net.in
    [ceph2.in][DEBUG ]  * epel: epel.excellmedia.net
    [ceph2.in][DEBUG ]  * extras: centos.mirror.net.in
    [ceph2.in][DEBUG ]  * updates: centos.mirror.net.in
    [ceph2.in][DEBUG ] 8 packages excluded due to repository priority protections
    [ceph2.in][DEBUG ] Resolving Dependencies
    [ceph2.in][DEBUG ] --> Running transaction check
    [ceph2.in][DEBUG ] ---> Package ceph.x86_64 2:13.2.10-0.el7 will be installed
    [ceph2.in][DEBUG ] --> Processing Dependency: ceph-mds = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: ceph-osd = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: ceph-mon = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: ceph-mgr = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] ---> Package ceph-radosgw.x86_64 2:13.2.10-0.el7 will be installed
    [ceph2.in][DEBUG ] --> Processing Dependency: ceph-base = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: ceph-selinux = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: librgw2 = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: librados2 = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: mailcap for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: librados.so.2()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: libtcmalloc.so.4()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: libibverbs.so.1()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: liboath.so.0()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: libceph-common.so.0()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Running transaction check
    [ceph2.in][DEBUG ] ---> Package ceph-base.x86_64 2:13.2.10-0.el7 will be installed
    [ceph2.in][DEBUG ] --> Processing Dependency: libcephfs2 = 2:13.2.10-0.el7 for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: librbd1 = 2:13.2.10-0.el7 for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: ceph-common = 2:13.2.10-0.el7 for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: gdisk for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: psmisc for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: cryptsetup for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: python-requests for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: libleveldb.so.1()(64bit) for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: libfuse.so.2()(64bit) for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: liblttng-ust.so.0()(64bit) for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] ---> Package ceph-mds.x86_64 2:13.2.10-0.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package ceph-mgr.x86_64 2:13.2.10-0.el7 will be installed
    [ceph2.in][DEBUG ] --> Processing Dependency: python-cherrypy for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: python-werkzeug for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: python-six for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: python-routes for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: python-bcrypt for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: python-pecan for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: pyOpenSSL for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: python-jinja2 for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] ---> Package ceph-mon.x86_64 2:13.2.10-0.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package ceph-osd.x86_64 2:13.2.10-0.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package ceph-selinux.x86_64 2:13.2.10-0.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package gperftools-libs.x86_64 0:2.6.1-1.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package libibverbs.x86_64 0:22.4-6.el7_9 will be installed
    [ceph2.in][DEBUG ] --> Processing Dependency: rdma-core(x86-64) = 22.4-6.el7_9 for package: libibverbs-22.4-6.el7_9.x86_64
    [ceph2.in][DEBUG ] ---> Package liboath.x86_64 0:2.6.2-1.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package librados2.x86_64 2:13.2.10-0.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package librgw2.x86_64 2:13.2.10-0.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package mailcap.noarch 0:2.1.41-2.el7 will be installed
    [ceph2.in][DEBUG ] --> Running transaction check
    [ceph2.in][DEBUG ] ---> Package ceph-common.x86_64 2:13.2.10-0.el7 will be installed
    [ceph2.in][DEBUG ] --> Processing Dependency: python-cephfs = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: libradosstriper1 = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: python-rgw = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: python-rbd = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: python-rados = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: python-ceph-argparse = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: python-prettytable for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: libbabeltrace-ctf.so.1()(64bit) for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: libbabeltrace.so.1()(64bit) for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: libradosstriper.so.1()(64bit) for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph2.in][DEBUG ] ---> Package cryptsetup.x86_64 0:2.0.3-6.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package fuse-libs.x86_64 0:2.9.2-11.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package gdisk.x86_64 0:0.8.10-3.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package leveldb.x86_64 0:1.12.0-11.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package libcephfs2.x86_64 2:13.2.10-0.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package librbd1.x86_64 2:13.2.10-0.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package lttng-ust.x86_64 0:2.4.1-4.el7 will be installed
    [ceph2.in][DEBUG ] --> Processing Dependency: liburcu-bp.so.1()(64bit) for package: lttng-ust-2.4.1-4.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: liburcu-cds.so.1()(64bit) for package: lttng-ust-2.4.1-4.el7.x86_64
    [ceph2.in][DEBUG ] ---> Package psmisc.x86_64 0:22.20-17.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package pyOpenSSL.x86_64 0:0.13.1-4.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package python-cherrypy.noarch 0:3.2.2-4.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package python-jinja2.noarch 0:2.7.2-4.el7 will be installed
    [ceph2.in][DEBUG ] --> Processing Dependency: python-babel >= 0.8 for package: python-jinja2-2.7.2-4.el7.noarch
    [ceph2.in][DEBUG ] --> Processing Dependency: python-markupsafe for package: python-jinja2-2.7.2-4.el7.noarch
    [ceph2.in][DEBUG ] ---> Package python-pecan.noarch 0:0.4.5-2.el7 will be installed
    [ceph2.in][DEBUG ] --> Processing Dependency: python-mako >= 0.4.0 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph2.in][DEBUG ] --> Processing Dependency: python-simplegeneric >= 0.8 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph2.in][DEBUG ] --> Processing Dependency: python-webob >= 1.2 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph2.in][DEBUG ] --> Processing Dependency: python-webtest >= 1.3.1 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph2.in][DEBUG ] --> Processing Dependency: python-singledispatch for package: python-pecan-0.4.5-2.el7.noarch
    [ceph2.in][DEBUG ] ---> Package python-requests.noarch 0:2.6.0-10.el7 will be installed
    [ceph2.in][DEBUG ] --> Processing Dependency: python-urllib3 >= 1.10.2-1 for package: python-requests-2.6.0-10.el7.noarch
    [ceph2.in][DEBUG ] --> Processing Dependency: python-chardet >= 2.2.1-1 for package: python-requests-2.6.0-10.el7.noarch
    [ceph2.in][DEBUG ] ---> Package python-routes.noarch 0:1.13-2.el7 will be installed
    [ceph2.in][DEBUG ] --> Processing Dependency: python-repoze-lru for package: python-routes-1.13-2.el7.noarch
    [ceph2.in][DEBUG ] ---> Package python-six.noarch 0:1.9.0-2.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package python-werkzeug.noarch 0:0.9.1-2.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package python2-bcrypt.x86_64 0:3.1.6-2.el7 will be installed
    [ceph2.in][DEBUG ] --> Processing Dependency: python-cffi for package: python2-bcrypt-3.1.6-2.el7.x86_64
    [ceph2.in][DEBUG ] --> Processing Dependency: python2-six for package: python2-bcrypt-3.1.6-2.el7.x86_64
    [ceph2.in][DEBUG ] ---> Package rdma-core.x86_64 0:22.4-6.el7_9 will be installed
    [ceph2.in][DEBUG ] --> Processing Dependency: pciutils for package: rdma-core-22.4-6.el7_9.x86_64
    [ceph2.in][DEBUG ] --> Running transaction check
    [ceph2.in][DEBUG ] ---> Package libbabeltrace.x86_64 0:1.2.4-3.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package libradosstriper1.x86_64 2:13.2.10-0.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package pciutils.x86_64 0:3.5.1-3.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package python-babel.noarch 0:0.9.6-8.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package python-ceph-argparse.x86_64 2:13.2.10-0.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package python-cephfs.x86_64 2:13.2.10-0.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package python-cffi.x86_64 0:1.6.0-5.el7 will be installed
    [ceph2.in][DEBUG ] --> Processing Dependency: python-pycparser for package: python-cffi-1.6.0-5.el7.x86_64
    [ceph2.in][DEBUG ] ---> Package python-chardet.noarch 0:2.2.1-3.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package python-mako.noarch 0:0.8.1-2.el7 will be installed
    [ceph2.in][DEBUG ] --> Processing Dependency: python-beaker for package: python-mako-0.8.1-2.el7.noarch
    [ceph2.in][DEBUG ] ---> Package python-markupsafe.x86_64 0:0.11-10.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package python-prettytable.noarch 0:0.7.2-3.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package python-rados.x86_64 2:13.2.10-0.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package python-rbd.x86_64 2:13.2.10-0.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package python-repoze-lru.noarch 0:0.4-3.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package python-rgw.x86_64 2:13.2.10-0.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package python-simplegeneric.noarch 0:0.8-7.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package python-singledispatch.noarch 0:3.4.0.2-2.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package python-urllib3.noarch 0:1.10.2-7.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package python-webob.noarch 0:1.2.3-7.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package python-webtest.noarch 0:1.3.4-6.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package python2-six.noarch 0:1.9.0-0.el7 will be installed
    [ceph2.in][DEBUG ] ---> Package userspace-rcu.x86_64 0:0.7.16-1.el7 will be installed
    [ceph2.in][DEBUG ] --> Running transaction check
    [ceph2.in][DEBUG ] ---> Package python-beaker.noarch 0:1.5.4-10.el7 will be installed
    [ceph2.in][DEBUG ] --> Processing Dependency: python-paste for package: python-beaker-1.5.4-10.el7.noarch
    [ceph2.in][DEBUG ] ---> Package python-pycparser.noarch 0:2.14-1.el7 will be installed
    [ceph2.in][DEBUG ] --> Processing Dependency: python-ply for package: python-pycparser-2.14-1.el7.noarch
    [ceph2.in][DEBUG ] --> Running transaction check
    [ceph2.in][DEBUG ] ---> Package python-paste.noarch 0:1.7.5.1-9.20111221hg1498.el7 will be installed
    [ceph2.in][DEBUG ] --> Processing Dependency: python-tempita for package: python-paste-1.7.5.1-9.20111221hg1498.el7.noarch
    [ceph2.in][DEBUG ] ---> Package python-ply.noarch 0:3.4-11.el7 will be installed
    [ceph2.in][DEBUG ] --> Running transaction check
    [ceph2.in][DEBUG ] ---> Package python-tempita.noarch 0:0.5.1-6.el7 will be installed
    [ceph2.in][DEBUG ] --> Finished Dependency Resolution
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] Dependencies Resolved
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] ================================================================================
    [ceph2.in][DEBUG ]  Package                Arch    Version                          Repository
    [ceph2.in][DEBUG ]                                                                            Size
    [ceph2.in][DEBUG ] ================================================================================
    [ceph2.in][DEBUG ] Installing:
    [ceph2.in][DEBUG ]  ceph                   x86_64  2:13.2.10-0.el7                  Ceph     3.0 k
    [ceph2.in][DEBUG ]  ceph-radosgw           x86_64  2:13.2.10-0.el7                  Ceph     4.5 M
    [ceph2.in][DEBUG ] Installing for dependencies:
    [ceph2.in][DEBUG ]  ceph-base              x86_64  2:13.2.10-0.el7                  Ceph     4.8 M
    [ceph2.in][DEBUG ]  ceph-common            x86_64  2:13.2.10-0.el7                  Ceph      14 M
    [ceph2.in][DEBUG ]  ceph-mds               x86_64  2:13.2.10-0.el7                  Ceph     1.7 M
    [ceph2.in][DEBUG ]  ceph-mgr               x86_64  2:13.2.10-0.el7                  Ceph     3.5 M
    [ceph2.in][DEBUG ]  ceph-mon               x86_64  2:13.2.10-0.el7                  Ceph     3.9 M
    [ceph2.in][DEBUG ]  ceph-osd               x86_64  2:13.2.10-0.el7                  Ceph      13 M
    [ceph2.in][DEBUG ]  ceph-selinux           x86_64  2:13.2.10-0.el7                  Ceph      21 k
    [ceph2.in][DEBUG ]  cryptsetup             x86_64  2.0.3-6.el7                      base     154 k
    [ceph2.in][DEBUG ]  fuse-libs              x86_64  2.9.2-11.el7                     base      93 k
    [ceph2.in][DEBUG ]  gdisk                  x86_64  0.8.10-3.el7                     base     190 k
    [ceph2.in][DEBUG ]  gperftools-libs        x86_64  2.6.1-1.el7                      base     272 k
    [ceph2.in][DEBUG ]  leveldb                x86_64  1.12.0-11.el7                    epel     161 k
    [ceph2.in][DEBUG ]  libbabeltrace          x86_64  1.2.4-3.el7                      epel     147 k
    [ceph2.in][DEBUG ]  libcephfs2             x86_64  2:13.2.10-0.el7                  Ceph     434 k
    [ceph2.in][DEBUG ]  libibverbs             x86_64  22.4-6.el7_9                     updates  269 k
    [ceph2.in][DEBUG ]  liboath                x86_64  2.6.2-1.el7                      epel      51 k
    [ceph2.in][DEBUG ]  librados2              x86_64  2:13.2.10-0.el7                  Ceph     2.9 M
    [ceph2.in][DEBUG ]  libradosstriper1       x86_64  2:13.2.10-0.el7                  Ceph     329 k
    [ceph2.in][DEBUG ]  librbd1                x86_64  2:13.2.10-0.el7                  Ceph     1.2 M
    [ceph2.in][DEBUG ]  librgw2                x86_64  2:13.2.10-0.el7                  Ceph     2.0 M
    [ceph2.in][DEBUG ]  lttng-ust              x86_64  2.4.1-4.el7                      epel     176 k
    [ceph2.in][DEBUG ]  mailcap                noarch  2.1.41-2.el7                     base      31 k
    [ceph2.in][DEBUG ]  pciutils               x86_64  3.5.1-3.el7                      base      93 k
    [ceph2.in][DEBUG ]  psmisc                 x86_64  22.20-17.el7                     base     141 k
    [ceph2.in][DEBUG ]  pyOpenSSL              x86_64  0.13.1-4.el7                     base     135 k
    [ceph2.in][DEBUG ]  python-babel           noarch  0.9.6-8.el7                      base     1.4 M
    [ceph2.in][DEBUG ]  python-beaker          noarch  1.5.4-10.el7                     base      80 k
    [ceph2.in][DEBUG ]  python-ceph-argparse   x86_64  2:13.2.10-0.el7                  Ceph      34 k
    [ceph2.in][DEBUG ]  python-cephfs          x86_64  2:13.2.10-0.el7                  Ceph      87 k
    [ceph2.in][DEBUG ]  python-cffi            x86_64  1.6.0-5.el7                      base     218 k
    [ceph2.in][DEBUG ]  python-chardet         noarch  2.2.1-3.el7                      base     227 k
    [ceph2.in][DEBUG ]  python-cherrypy        noarch  3.2.2-4.el7                      base     422 k
    [ceph2.in][DEBUG ]  python-jinja2          noarch  2.7.2-4.el7                      base     519 k
    [ceph2.in][DEBUG ]  python-mako            noarch  0.8.1-2.el7                      base     307 k
    [ceph2.in][DEBUG ]  python-markupsafe      x86_64  0.11-10.el7                      base      25 k
    [ceph2.in][DEBUG ]  python-paste           noarch  1.7.5.1-9.20111221hg1498.el7     base     866 k
    [ceph2.in][DEBUG ]  python-pecan           noarch  0.4.5-2.el7                      epel     255 k
    [ceph2.in][DEBUG ]  python-ply             noarch  3.4-11.el7                       base     123 k
    [ceph2.in][DEBUG ]  python-prettytable     noarch  0.7.2-3.el7                      base      37 k
    [ceph2.in][DEBUG ]  python-pycparser       noarch  2.14-1.el7                       base     104 k
    [ceph2.in][DEBUG ]  python-rados           x86_64  2:13.2.10-0.el7                  Ceph     189 k
    [ceph2.in][DEBUG ]  python-rbd             x86_64  2:13.2.10-0.el7                  Ceph     132 k
    [ceph2.in][DEBUG ]  python-repoze-lru      noarch  0.4-3.el7                        epel      13 k
    [ceph2.in][DEBUG ]  python-requests        noarch  2.6.0-10.el7                     base      95 k
    [ceph2.in][DEBUG ]  python-rgw             x86_64  2:13.2.10-0.el7                  Ceph      76 k
    [ceph2.in][DEBUG ]  python-routes          noarch  1.13-2.el7                       epel     640 k
    [ceph2.in][DEBUG ]  python-simplegeneric   noarch  0.8-7.el7                        epel      12 k
    [ceph2.in][DEBUG ]  python-singledispatch  noarch  3.4.0.2-2.el7                    epel      18 k
    [ceph2.in][DEBUG ]  python-six             noarch  1.9.0-2.el7                      base      29 k
    [ceph2.in][DEBUG ]  python-tempita         noarch  0.5.1-6.el7                      base      33 k
    [ceph2.in][DEBUG ]  python-urllib3         noarch  1.10.2-7.el7                     base     103 k
    [ceph2.in][DEBUG ]  python-webob           noarch  1.2.3-7.el7                      base     202 k
    [ceph2.in][DEBUG ]  python-webtest         noarch  1.3.4-6.el7                      base     102 k
    [ceph2.in][DEBUG ]  python-werkzeug        noarch  0.9.1-2.el7                      extras   562 k
    [ceph2.in][DEBUG ]  python2-bcrypt         x86_64  3.1.6-2.el7                      epel      39 k
    [ceph2.in][DEBUG ]  python2-six            noarch  1.9.0-0.el7                      epel     2.9 k
    [ceph2.in][DEBUG ]  rdma-core              x86_64  22.4-6.el7_9                     updates   51 k
    [ceph2.in][DEBUG ]  userspace-rcu          x86_64  0.7.16-1.el7                     epel      73 k
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] Transaction Summary
    [ceph2.in][DEBUG ] ================================================================================
    [ceph2.in][DEBUG ] Install  2 Packages (+58 Dependent packages)
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] Total download size: 61 M
    [ceph2.in][DEBUG ] Installed size: 207 M
    [ceph2.in][DEBUG ] Downloading packages:
    [ceph2.in][WARNIN] http://ftp.iij.ad.jp/pub/linux/Fedora/epel/7/x86_64/Packages/p/python2-six-1.9.0-0.el7.noarch.rpm: [Errno 12] Timeout on http://ftp.iij.ad.jp/pub/linux/Fedora/epel/7/x86_64/Packages/p/python2-six-1.9.0-0.el7.noarch.rpm: (28, 'Operation too slow. Less than 1000 bytes/sec transferred the last 30 seconds')
    [ceph2.in][WARNIN] Trying other mirror.
    [ceph2.in][DEBUG ] --------------------------------------------------------------------------------
    [ceph2.in][DEBUG ] Total                                              1.5 MB/s |  61 MB  00:40
    [ceph2.in][DEBUG ] Running transaction check
    [ceph2.in][DEBUG ] Running transaction test
    [ceph2.in][DEBUG ] Transaction test succeeded
    [ceph2.in][DEBUG ] Running transaction
    [ceph2.in][DEBUG ]   Installing : gperftools-libs-2.6.1-1.el7.x86_64                          1/60
    [ceph2.in][DEBUG ]   Installing : python-six-1.9.0-2.el7.noarch                               2/60
    [ceph2.in][DEBUG ]   Installing : fuse-libs-2.9.2-11.el7.x86_64                               3/60
    [ceph2.in][DEBUG ]   Installing : leveldb-1.12.0-11.el7.x86_64                                4/60
    [ceph2.in][DEBUG ]   Installing : liboath-2.6.2-1.el7.x86_64                                  5/60
    [ceph2.in][DEBUG ]   Installing : python-webob-1.2.3-7.el7.noarch                             6/60
    [ceph2.in][DEBUG ]   Installing : python-markupsafe-0.11-10.el7.x86_64                        7/60
    [ceph2.in][DEBUG ]   Installing : pyOpenSSL-0.13.1-4.el7.x86_64                               8/60
    [ceph2.in][DEBUG ]   Installing : 2:python-ceph-argparse-13.2.10-0.el7.x86_64                 9/60
    [ceph2.in][DEBUG ]   Installing : python-webtest-1.3.4-6.el7.noarch                          10/60
    [ceph2.in][DEBUG ]   Installing : python-urllib3-1.10.2-7.el7.noarch                         11/60
    [ceph2.in][DEBUG ]   Installing : python2-six-1.9.0-0.el7.noarch                             12/60
    [ceph2.in][DEBUG ]   Installing : python-singledispatch-3.4.0.2-2.el7.noarch                 13/60
    [ceph2.in][DEBUG ]   Installing : psmisc-22.20-17.el7.x86_64                                 14/60
    [ceph2.in][DEBUG ]   Installing : pciutils-3.5.1-3.el7.x86_64                                15/60
    [ceph2.in][DEBUG ]   Installing : rdma-core-22.4-6.el7_9.x86_64                              16/60
    [ceph2.in][DEBUG ]   Installing : libibverbs-22.4-6.el7_9.x86_64                             17/60
    [ceph2.in][DEBUG ]   Installing : gdisk-0.8.10-3.el7.x86_64                                  18/60
    [ceph2.in][DEBUG ]   Installing : python-simplegeneric-0.8-7.el7.noarch                      19/60
    [ceph2.in][DEBUG ]   Installing : python-tempita-0.5.1-6.el7.noarch                          20/60
    [ceph2.in][DEBUG ]   Installing : python-paste-1.7.5.1-9.20111221hg1498.el7.noarch           21/60
    [ceph2.in][DEBUG ]   Installing : python-beaker-1.5.4-10.el7.noarch                          22/60
    [ceph2.in][DEBUG ]   Installing : python-mako-0.8.1-2.el7.noarch                             23/60
    [ceph2.in][DEBUG ]   Installing : python-pecan-0.4.5-2.el7.noarch                            24/60
    [ceph2.in][DEBUG ]   Installing : python-cherrypy-3.2.2-4.el7.noarch                         25/60
    [ceph2.in][DEBUG ]   Installing : python-prettytable-0.7.2-3.el7.noarch                      26/60
    [ceph2.in][DEBUG ]   Installing : python-werkzeug-0.9.1-2.el7.noarch                         27/60
    [ceph2.in][DEBUG ]   Installing : python-repoze-lru-0.4-3.el7.noarch                         28/60
    [ceph2.in][DEBUG ]   Installing : python-routes-1.13-2.el7.noarch                            29/60
    [ceph2.in][DEBUG ]   Installing : python-babel-0.9.6-8.el7.noarch                            30/60
    [ceph2.in][DEBUG ]   Installing : python-jinja2-2.7.2-4.el7.noarch                           31/60
    [ceph2.in][DEBUG ]   Installing : python-chardet-2.2.1-3.el7.noarch                          32/60
    [ceph2.in][DEBUG ]   Installing : python-requests-2.6.0-10.el7.noarch                        33/60
    [ceph2.in][DEBUG ]   Installing : mailcap-2.1.41-2.el7.noarch                                34/60
    [ceph2.in][DEBUG ]   Installing : cryptsetup-2.0.3-6.el7.x86_64                              35/60
    [ceph2.in][DEBUG ]   Installing : libbabeltrace-1.2.4-3.el7.x86_64                           36/60
    [ceph2.in][DEBUG ]   Installing : userspace-rcu-0.7.16-1.el7.x86_64                          37/60
    [ceph2.in][DEBUG ]   Installing : lttng-ust-2.4.1-4.el7.x86_64                               38/60
    [ceph2.in][DEBUG ]   Installing : 2:librados2-13.2.10-0.el7.x86_64                           39/60
    [ceph2.in][DEBUG ]   Installing : 2:python-rados-13.2.10-0.el7.x86_64                        40/60
    [ceph2.in][DEBUG ]   Installing : 2:librbd1-13.2.10-0.el7.x86_64                             41/60
    [ceph2.in][DEBUG ]   Installing : 2:libcephfs2-13.2.10-0.el7.x86_64                          42/60
    [ceph2.in][DEBUG ]   Installing : 2:librgw2-13.2.10-0.el7.x86_64                             43/60
    [ceph2.in][DEBUG ]   Installing : 2:python-rgw-13.2.10-0.el7.x86_64                          44/60
    [ceph2.in][DEBUG ]   Installing : 2:python-cephfs-13.2.10-0.el7.x86_64                       45/60
    [ceph2.in][DEBUG ]   Installing : 2:python-rbd-13.2.10-0.el7.x86_64                          46/60
    [ceph2.in][DEBUG ]   Installing : 2:libradosstriper1-13.2.10-0.el7.x86_64                    47/60
    [ceph2.in][DEBUG ]   Installing : 2:ceph-common-13.2.10-0.el7.x86_64                         48/60
    [ceph2.in][DEBUG ]   Installing : 2:ceph-base-13.2.10-0.el7.x86_64                           49/60
    [ceph2.in][DEBUG ]   Installing : 2:ceph-selinux-13.2.10-0.el7.x86_64                        50/60
    [ceph2.in][DEBUG ] /usr/lib/python2.7/site-packages/ceph_disk/main.py:5689: UserWarning:
    [ceph2.in][DEBUG ] *******************************************************************************
    [ceph2.in][DEBUG ] This tool is now deprecated in favor of ceph-volume.
    [ceph2.in][DEBUG ] It is recommended to use ceph-volume for OSD deployments. For details see:
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ]     http://docs.ceph.com/docs/master/ceph-volume/#migrating
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] *******************************************************************************
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ]   warnings.warn(DEPRECATION_WARNING)
    [ceph2.in][DEBUG ] /usr/lib/python2.7/site-packages/ceph_disk/main.py:5721: UserWarning:
    [ceph2.in][DEBUG ] *******************************************************************************
    [ceph2.in][DEBUG ] This tool is now deprecated in favor of ceph-volume.
    [ceph2.in][DEBUG ] It is recommended to use ceph-volume for OSD deployments. For details see:
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ]     http://docs.ceph.com/docs/master/ceph-volume/#migrating
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] *******************************************************************************
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ]   warnings.warn(DEPRECATION_WARNING)
    [ceph2.in][DEBUG ]   Installing : 2:ceph-osd-13.2.10-0.el7.x86_64                            51/60
    [ceph2.in][DEBUG ]   Installing : 2:ceph-mds-13.2.10-0.el7.x86_64                            52/60
    [ceph2.in][DEBUG ]   Installing : 2:ceph-mon-13.2.10-0.el7.x86_64                            53/60
    [ceph2.in][DEBUG ]   Installing : python-ply-3.4-11.el7.noarch                               54/60
    [ceph2.in][DEBUG ]   Installing : python-pycparser-2.14-1.el7.noarch                         55/60
    [ceph2.in][DEBUG ]   Installing : python-cffi-1.6.0-5.el7.x86_64                             56/60
    [ceph2.in][DEBUG ]   Installing : python2-bcrypt-3.1.6-2.el7.x86_64                          57/60
    [ceph2.in][DEBUG ]   Installing : 2:ceph-mgr-13.2.10-0.el7.x86_64                            58/60
    [ceph2.in][DEBUG ]   Installing : 2:ceph-13.2.10-0.el7.x86_64                                59/60
    [ceph2.in][DEBUG ]   Installing : 2:ceph-radosgw-13.2.10-0.el7.x86_64                        60/60
    [ceph2.in][DEBUG ]   Verifying  : liboath-2.6.2-1.el7.x86_64                                  1/60
    [ceph2.in][DEBUG ]   Verifying  : 2:librbd1-13.2.10-0.el7.x86_64                              2/60
    [ceph2.in][DEBUG ]   Verifying  : 2:python-ceph-argparse-13.2.10-0.el7.x86_64                 3/60
    [ceph2.in][DEBUG ]   Verifying  : leveldb-1.12.0-11.el7.x86_64                                4/60
    [ceph2.in][DEBUG ]   Verifying  : pyOpenSSL-0.13.1-4.el7.x86_64                               5/60
    [ceph2.in][DEBUG ]   Verifying  : python2-bcrypt-3.1.6-2.el7.x86_64                           6/60
    [ceph2.in][DEBUG ]   Verifying  : python-ply-3.4-11.el7.noarch                                7/60
    [ceph2.in][DEBUG ]   Verifying  : userspace-rcu-0.7.16-1.el7.x86_64                           8/60
    [ceph2.in][DEBUG ]   Verifying  : libibverbs-22.4-6.el7_9.x86_64                              9/60
    [ceph2.in][DEBUG ]   Verifying  : rdma-core-22.4-6.el7_9.x86_64                              10/60
    [ceph2.in][DEBUG ]   Verifying  : fuse-libs-2.9.2-11.el7.x86_64                              11/60
    [ceph2.in][DEBUG ]   Verifying  : python-routes-1.13-2.el7.noarch                            12/60
    [ceph2.in][DEBUG ]   Verifying  : 2:libcephfs2-13.2.10-0.el7.x86_64                          13/60
    [ceph2.in][DEBUG ]   Verifying  : python-urllib3-1.10.2-7.el7.noarch                         14/60
    [ceph2.in][DEBUG ]   Verifying  : libbabeltrace-1.2.4-3.el7.x86_64                           15/60
    [ceph2.in][DEBUG ]   Verifying  : python-mako-0.8.1-2.el7.noarch                             16/60
    [ceph2.in][DEBUG ]   Verifying  : python2-six-1.9.0-0.el7.noarch                             17/60
    [ceph2.in][DEBUG ]   Verifying  : 2:ceph-mgr-13.2.10-0.el7.x86_64                            18/60
    [ceph2.in][DEBUG ]   Verifying  : 2:ceph-base-13.2.10-0.el7.x86_64                           19/60
    [ceph2.in][DEBUG ]   Verifying  : python-jinja2-2.7.2-4.el7.noarch                           20/60
    [ceph2.in][DEBUG ]   Verifying  : python-pecan-0.4.5-2.el7.noarch                            21/60
    [ceph2.in][DEBUG ]   Verifying  : python-six-1.9.0-2.el7.noarch                              22/60
    [ceph2.in][DEBUG ]   Verifying  : cryptsetup-2.0.3-6.el7.x86_64                              23/60
    [ceph2.in][DEBUG ]   Verifying  : mailcap-2.1.41-2.el7.noarch                                24/60
    [ceph2.in][DEBUG ]   Verifying  : python-singledispatch-3.4.0.2-2.el7.noarch                 25/60
    [ceph2.in][DEBUG ]   Verifying  : python-markupsafe-0.11-10.el7.x86_64                       26/60
    [ceph2.in][DEBUG ]   Verifying  : 2:python-rados-13.2.10-0.el7.x86_64                        27/60
    [ceph2.in][DEBUG ]   Verifying  : 2:python-rgw-13.2.10-0.el7.x86_64                          28/60
    [ceph2.in][DEBUG ]   Verifying  : 2:ceph-radosgw-13.2.10-0.el7.x86_64                        29/60
    [ceph2.in][DEBUG ]   Verifying  : python-chardet-2.2.1-3.el7.noarch                          30/60
    [ceph2.in][DEBUG ]   Verifying  : python-babel-0.9.6-8.el7.noarch                            31/60
    [ceph2.in][DEBUG ]   Verifying  : 2:librados2-13.2.10-0.el7.x86_64                           32/60
    [ceph2.in][DEBUG ]   Verifying  : python-paste-1.7.5.1-9.20111221hg1498.el7.noarch           33/60
    [ceph2.in][DEBUG ]   Verifying  : 2:ceph-osd-13.2.10-0.el7.x86_64                            34/60
    [ceph2.in][DEBUG ]   Verifying  : lttng-ust-2.4.1-4.el7.x86_64                               35/60
    [ceph2.in][DEBUG ]   Verifying  : python-webob-1.2.3-7.el7.noarch                            36/60
    [ceph2.in][DEBUG ]   Verifying  : 2:ceph-common-13.2.10-0.el7.x86_64                         37/60
    [ceph2.in][DEBUG ]   Verifying  : python-repoze-lru-0.4-3.el7.noarch                         38/60
    [ceph2.in][DEBUG ]   Verifying  : python-werkzeug-0.9.1-2.el7.noarch                         39/60
    [ceph2.in][DEBUG ]   Verifying  : python-beaker-1.5.4-10.el7.noarch                          40/60
    [ceph2.in][DEBUG ]   Verifying  : python-cffi-1.6.0-5.el7.x86_64                             41/60
    [ceph2.in][DEBUG ]   Verifying  : 2:ceph-selinux-13.2.10-0.el7.x86_64                        42/60
    [ceph2.in][DEBUG ]   Verifying  : python-requests-2.6.0-10.el7.noarch                        43/60
    [ceph2.in][DEBUG ]   Verifying  : python-pycparser-2.14-1.el7.noarch                         44/60
    [ceph2.in][DEBUG ]   Verifying  : python-prettytable-0.7.2-3.el7.noarch                      45/60
    [ceph2.in][DEBUG ]   Verifying  : 2:librgw2-13.2.10-0.el7.x86_64                             46/60
    [ceph2.in][DEBUG ]   Verifying  : 2:ceph-mds-13.2.10-0.el7.x86_64                            47/60
    [ceph2.in][DEBUG ]   Verifying  : python-cherrypy-3.2.2-4.el7.noarch                         48/60
    [ceph2.in][DEBUG ]   Verifying  : 2:python-cephfs-13.2.10-0.el7.x86_64                       49/60
    [ceph2.in][DEBUG ]   Verifying  : python-tempita-0.5.1-6.el7.noarch                          50/60
    [ceph2.in][DEBUG ]   Verifying  : 2:python-rbd-13.2.10-0.el7.x86_64                          51/60
    [ceph2.in][DEBUG ]   Verifying  : 2:ceph-mon-13.2.10-0.el7.x86_64                            52/60
    [ceph2.in][DEBUG ]   Verifying  : gperftools-libs-2.6.1-1.el7.x86_64                         53/60
    [ceph2.in][DEBUG ]   Verifying  : python-webtest-1.3.4-6.el7.noarch                          54/60
    [ceph2.in][DEBUG ]   Verifying  : 2:ceph-13.2.10-0.el7.x86_64                                55/60
    [ceph2.in][DEBUG ]   Verifying  : python-simplegeneric-0.8-7.el7.noarch                      56/60
    [ceph2.in][DEBUG ]   Verifying  : gdisk-0.8.10-3.el7.x86_64                                  57/60
    [ceph2.in][DEBUG ]   Verifying  : 2:libradosstriper1-13.2.10-0.el7.x86_64                    58/60
    [ceph2.in][DEBUG ]   Verifying  : pciutils-3.5.1-3.el7.x86_64                                59/60
    [ceph2.in][DEBUG ]   Verifying  : psmisc-22.20-17.el7.x86_64                                 60/60
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] Installed:
    [ceph2.in][DEBUG ]   ceph.x86_64 2:13.2.10-0.el7        ceph-radosgw.x86_64 2:13.2.10-0.el7
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] Dependency Installed:
    [ceph2.in][DEBUG ]   ceph-base.x86_64 2:13.2.10-0.el7
    [ceph2.in][DEBUG ]   ceph-common.x86_64 2:13.2.10-0.el7
    [ceph2.in][DEBUG ]   ceph-mds.x86_64 2:13.2.10-0.el7
    [ceph2.in][DEBUG ]   ceph-mgr.x86_64 2:13.2.10-0.el7
    [ceph2.in][DEBUG ]   ceph-mon.x86_64 2:13.2.10-0.el7
    [ceph2.in][DEBUG ]   ceph-osd.x86_64 2:13.2.10-0.el7
    [ceph2.in][DEBUG ]   ceph-selinux.x86_64 2:13.2.10-0.el7
    [ceph2.in][DEBUG ]   cryptsetup.x86_64 0:2.0.3-6.el7
    [ceph2.in][DEBUG ]   fuse-libs.x86_64 0:2.9.2-11.el7
    [ceph2.in][DEBUG ]   gdisk.x86_64 0:0.8.10-3.el7
    [ceph2.in][DEBUG ]   gperftools-libs.x86_64 0:2.6.1-1.el7
    [ceph2.in][DEBUG ]   leveldb.x86_64 0:1.12.0-11.el7
    [ceph2.in][DEBUG ]   libbabeltrace.x86_64 0:1.2.4-3.el7
    [ceph2.in][DEBUG ]   libcephfs2.x86_64 2:13.2.10-0.el7
    [ceph2.in][DEBUG ]   libibverbs.x86_64 0:22.4-6.el7_9
    [ceph2.in][DEBUG ]   liboath.x86_64 0:2.6.2-1.el7
    [ceph2.in][DEBUG ]   librados2.x86_64 2:13.2.10-0.el7
    [ceph2.in][DEBUG ]   libradosstriper1.x86_64 2:13.2.10-0.el7
    [ceph2.in][DEBUG ]   librbd1.x86_64 2:13.2.10-0.el7
    [ceph2.in][DEBUG ]   librgw2.x86_64 2:13.2.10-0.el7
    [ceph2.in][DEBUG ]   lttng-ust.x86_64 0:2.4.1-4.el7
    [ceph2.in][DEBUG ]   mailcap.noarch 0:2.1.41-2.el7
    [ceph2.in][DEBUG ]   pciutils.x86_64 0:3.5.1-3.el7
    [ceph2.in][DEBUG ]   psmisc.x86_64 0:22.20-17.el7
    [ceph2.in][DEBUG ]   pyOpenSSL.x86_64 0:0.13.1-4.el7
    [ceph2.in][DEBUG ]   python-babel.noarch 0:0.9.6-8.el7
    [ceph2.in][DEBUG ]   python-beaker.noarch 0:1.5.4-10.el7
    [ceph2.in][DEBUG ]   python-ceph-argparse.x86_64 2:13.2.10-0.el7
    [ceph2.in][DEBUG ]   python-cephfs.x86_64 2:13.2.10-0.el7
    [ceph2.in][DEBUG ]   python-cffi.x86_64 0:1.6.0-5.el7
    [ceph2.in][DEBUG ]   python-chardet.noarch 0:2.2.1-3.el7
    [ceph2.in][DEBUG ]   python-cherrypy.noarch 0:3.2.2-4.el7
    [ceph2.in][DEBUG ]   python-jinja2.noarch 0:2.7.2-4.el7
    [ceph2.in][DEBUG ]   python-mako.noarch 0:0.8.1-2.el7
    [ceph2.in][DEBUG ]   python-markupsafe.x86_64 0:0.11-10.el7
    [ceph2.in][DEBUG ]   python-paste.noarch 0:1.7.5.1-9.20111221hg1498.el7
    [ceph2.in][DEBUG ]   python-pecan.noarch 0:0.4.5-2.el7
    [ceph2.in][DEBUG ]   python-ply.noarch 0:3.4-11.el7
    [ceph2.in][DEBUG ]   python-prettytable.noarch 0:0.7.2-3.el7
    [ceph2.in][DEBUG ]   python-pycparser.noarch 0:2.14-1.el7
    [ceph2.in][DEBUG ]   python-rados.x86_64 2:13.2.10-0.el7
    [ceph2.in][DEBUG ]   python-rbd.x86_64 2:13.2.10-0.el7
    [ceph2.in][DEBUG ]   python-repoze-lru.noarch 0:0.4-3.el7
    [ceph2.in][DEBUG ]   python-requests.noarch 0:2.6.0-10.el7
    [ceph2.in][DEBUG ]   python-rgw.x86_64 2:13.2.10-0.el7
    [ceph2.in][DEBUG ]   python-routes.noarch 0:1.13-2.el7
    [ceph2.in][DEBUG ]   python-simplegeneric.noarch 0:0.8-7.el7
    [ceph2.in][DEBUG ]   python-singledispatch.noarch 0:3.4.0.2-2.el7
    [ceph2.in][DEBUG ]   python-six.noarch 0:1.9.0-2.el7
    [ceph2.in][DEBUG ]   python-tempita.noarch 0:0.5.1-6.el7
    [ceph2.in][DEBUG ]   python-urllib3.noarch 0:1.10.2-7.el7
    [ceph2.in][DEBUG ]   python-webob.noarch 0:1.2.3-7.el7
    [ceph2.in][DEBUG ]   python-webtest.noarch 0:1.3.4-6.el7
    [ceph2.in][DEBUG ]   python-werkzeug.noarch 0:0.9.1-2.el7
    [ceph2.in][DEBUG ]   python2-bcrypt.x86_64 0:3.1.6-2.el7
    [ceph2.in][DEBUG ]   python2-six.noarch 0:1.9.0-0.el7
    [ceph2.in][DEBUG ]   rdma-core.x86_64 0:22.4-6.el7_9
    [ceph2.in][DEBUG ]   userspace-rcu.x86_64 0:0.7.16-1.el7
    [ceph2.in][DEBUG ]
    [ceph2.in][DEBUG ] Complete!
    [ceph2.in][INFO  ] Running command: sudo ceph --version
    [ceph2.in][DEBUG ] ceph version 13.2.10 (564bdc4ae87418a232fc901524470e1a0f76d641) mimic (stable)
    [ceph_deploy.install][DEBUG ] Detecting platform for host ceph3.in ...
    [ceph3.in][DEBUG ] connection detected need for sudo
    [ceph3.in][DEBUG ] connected to host: ceph3.in
    [ceph3.in][DEBUG ] detect platform information from remote host
    [ceph3.in][DEBUG ] detect machine type
    [ceph_deploy.install][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph3.in][INFO  ] installing Ceph on ceph3.in
    [ceph3.in][INFO  ] Running command: sudo yum clean all
    [ceph3.in][DEBUG ] Loaded plugins: fastestmirror
    [ceph3.in][DEBUG ] Cleaning repos: base epel extras updates
    [ceph3.in][DEBUG ] Cleaning up list of fastest mirrors
    [ceph3.in][INFO  ] Running command: sudo yum -y install epel-release
    [ceph3.in][DEBUG ] Loaded plugins: fastestmirror
    [ceph3.in][DEBUG ] Determining fastest mirrors
    [ceph3.in][DEBUG ]  * base: centos.mirror.net.in
    [ceph3.in][DEBUG ]  * epel: epel.excellmedia.net
    [ceph3.in][DEBUG ]  * extras: centos.mirror.net.in
    [ceph3.in][DEBUG ]  * updates: centos.mirror.net.in
    [ceph3.in][DEBUG ] Package epel-release-7-14.noarch already installed and latest version
    [ceph3.in][DEBUG ] Nothing to do
    [ceph3.in][INFO  ] Running command: sudo yum -y install yum-plugin-priorities
    [ceph3.in][DEBUG ] Loaded plugins: fastestmirror
    [ceph3.in][DEBUG ] Loading mirror speeds from cached hostfile
    [ceph3.in][DEBUG ]  * base: centos.mirror.net.in
    [ceph3.in][DEBUG ]  * epel: epel.excellmedia.net
    [ceph3.in][DEBUG ]  * extras: centos.mirror.net.in
    [ceph3.in][DEBUG ]  * updates: centos.mirror.net.in
    [ceph3.in][DEBUG ] Resolving Dependencies
    [ceph3.in][DEBUG ] --> Running transaction check
    [ceph3.in][DEBUG ] ---> Package yum-plugin-priorities.noarch 0:1.1.31-54.el7_8 will be installed
    [ceph3.in][DEBUG ] --> Finished Dependency Resolution
    [ceph3.in][DEBUG ]
    [ceph3.in][DEBUG ] Dependencies Resolved
    [ceph3.in][DEBUG ]
    [ceph3.in][DEBUG ] ================================================================================
    [ceph3.in][DEBUG ]  Package                    Arch        Version                 Repository
    [ceph3.in][DEBUG ]                                                                            Size
    [ceph3.in][DEBUG ] ================================================================================
    [ceph3.in][DEBUG ] Installing:
    [ceph3.in][DEBUG ]  yum-plugin-priorities      noarch      1.1.31-54.el7_8         base       29 k
    [ceph3.in][DEBUG ]
    [ceph3.in][DEBUG ] Transaction Summary
    [ceph3.in][DEBUG ] ================================================================================
    [ceph3.in][DEBUG ] Install  1 Package
    [ceph3.in][DEBUG ]
    [ceph3.in][DEBUG ] Total download size: 29 k
    [ceph3.in][DEBUG ] Installed size: 28 k
    [ceph3.in][DEBUG ] Downloading packages:
    [ceph3.in][DEBUG ] Running transaction check
    [ceph3.in][DEBUG ] Running transaction test
    [ceph3.in][DEBUG ] Transaction test succeeded
    [ceph3.in][DEBUG ] Running transaction
    [ceph3.in][DEBUG ]   Installing : yum-plugin-priorities-1.1.31-54.el7_8.noarch                 1/1
    [ceph3.in][DEBUG ]   Verifying  : yum-plugin-priorities-1.1.31-54.el7_8.noarch                 1/1
    [ceph3.in][DEBUG ]
    [ceph3.in][DEBUG ] Installed:
    [ceph3.in][DEBUG ]   yum-plugin-priorities.noarch 0:1.1.31-54.el7_8
    [ceph3.in][DEBUG ]
    [ceph3.in][DEBUG ] Complete!
    [ceph3.in][DEBUG ] Configure Yum priorities to include obsoletes
    [ceph3.in][WARNIN] check_obsoletes has been enabled for Yum priorities plugin
    [ceph3.in][INFO  ] Running command: sudo rpm --import https://download.ceph.com/keys/release.asc
    [ceph3.in][INFO  ] Running command: sudo yum remove -y ceph-release
    [ceph3.in][DEBUG ] Loaded plugins: fastestmirror, priorities
    [ceph3.in][WARNIN] No Match for argument: ceph-release
    [ceph3.in][DEBUG ] No Packages marked for removal
    [ceph3.in][INFO  ] Running command: sudo yum install -y https://download.ceph.com/rpm-mimic/el7/noarch/ceph-release-1-0.el7.noarch.rpm
    [ceph3.in][DEBUG ] Loaded plugins: fastestmirror, priorities
    [ceph3.in][DEBUG ] Examining /var/tmp/yum-root-LlH6hj/ceph-release-1-0.el7.noarch.rpm: ceph-release-1-1.el7.noarch
    [ceph3.in][DEBUG ] Marking /var/tmp/yum-root-LlH6hj/ceph-release-1-0.el7.noarch.rpm to be installed
    [ceph3.in][DEBUG ] Resolving Dependencies
    [ceph3.in][DEBUG ] --> Running transaction check
    [ceph3.in][DEBUG ] ---> Package ceph-release.noarch 0:1-1.el7 will be installed
    [ceph3.in][DEBUG ] --> Finished Dependency Resolution
    [ceph3.in][DEBUG ]
    [ceph3.in][DEBUG ] Dependencies Resolved
    [ceph3.in][DEBUG ]
    [ceph3.in][DEBUG ] ================================================================================
    [ceph3.in][DEBUG ]  Package          Arch       Version     Repository                        Size
    [ceph3.in][DEBUG ] ================================================================================
    [ceph3.in][DEBUG ] Installing:
    [ceph3.in][DEBUG ]  ceph-release     noarch     1-1.el7     /ceph-release-1-0.el7.noarch     535
    [ceph3.in][DEBUG ]
    [ceph3.in][DEBUG ] Transaction Summary
    [ceph3.in][DEBUG ] ================================================================================
    [ceph3.in][DEBUG ] Install  1 Package
    [ceph3.in][DEBUG ]
    [ceph3.in][DEBUG ] Total size: 535
    [ceph3.in][DEBUG ] Installed size: 535
    [ceph3.in][DEBUG ] Downloading packages:
    [ceph3.in][DEBUG ] Running transaction check
    [ceph3.in][DEBUG ] Running transaction test
    [ceph3.in][DEBUG ] Transaction test succeeded
    [ceph3.in][DEBUG ] Running transaction
    [ceph3.in][DEBUG ]   Installing : ceph-release-1-1.el7.noarch                                  1/1
    [ceph3.in][DEBUG ]   Verifying  : ceph-release-1-1.el7.noarch                                  1/1
    [ceph3.in][DEBUG ]
    [ceph3.in][DEBUG ] Installed:
    [ceph3.in][DEBUG ]   ceph-release.noarch 0:1-1.el7
    [ceph3.in][DEBUG ]
    [ceph3.in][DEBUG ] Complete!
    [ceph3.in][WARNIN] ensuring that /etc/yum.repos.d/ceph.repo contains a high priority
    [ceph3.in][WARNIN] altered ceph.repo priorities to contain: priority=1
    [ceph3.in][INFO  ] Running command: sudo yum -y install ceph ceph-radosgw
    [ceph3.in][DEBUG ] Loaded plugins: fastestmirror, priorities
    [ceph3.in][DEBUG ] Loading mirror speeds from cached hostfile
    [ceph3.in][DEBUG ]  * base: centos.mirror.net.in
    [ceph3.in][DEBUG ]  * epel: epel.excellmedia.net
    [ceph3.in][DEBUG ]  * extras: centos.mirror.net.in
    [ceph3.in][DEBUG ]  * updates: centos.mirror.net.in
    [ceph3.in][DEBUG ] 8 packages excluded due to repository priority protections
    [ceph3.in][DEBUG ] Resolving Dependencies
    [ceph3.in][DEBUG ] --> Running transaction check
    [ceph3.in][DEBUG ] ---> Package ceph.x86_64 2:13.2.10-0.el7 will be installed
    [ceph3.in][DEBUG ] --> Processing Dependency: ceph-mds = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: ceph-osd = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: ceph-mon = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: ceph-mgr = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] ---> Package ceph-radosgw.x86_64 2:13.2.10-0.el7 will be installed
    [ceph3.in][DEBUG ] --> Processing Dependency: ceph-base = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: ceph-selinux = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: librgw2 = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: librados2 = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: mailcap for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: librados.so.2()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: libtcmalloc.so.4()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: libibverbs.so.1()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: liboath.so.0()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: libceph-common.so.0()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Running transaction check
    [ceph3.in][DEBUG ] ---> Package ceph-base.x86_64 2:13.2.10-0.el7 will be installed
    [ceph3.in][DEBUG ] --> Processing Dependency: libcephfs2 = 2:13.2.10-0.el7 for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: librbd1 = 2:13.2.10-0.el7 for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: ceph-common = 2:13.2.10-0.el7 for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: gdisk for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: python-setuptools for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: psmisc for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: cryptsetup for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: python-requests for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: libleveldb.so.1()(64bit) for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: libfuse.so.2()(64bit) for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: liblttng-ust.so.0()(64bit) for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] ---> Package ceph-mds.x86_64 2:13.2.10-0.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package ceph-mgr.x86_64 2:13.2.10-0.el7 will be installed
    [ceph3.in][DEBUG ] --> Processing Dependency: python-cherrypy for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: python-werkzeug for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: python-six for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: python-routes for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: python-bcrypt for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: python-pecan for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: pyOpenSSL for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: python-jinja2 for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] ---> Package ceph-mon.x86_64 2:13.2.10-0.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package ceph-osd.x86_64 2:13.2.10-0.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package ceph-selinux.x86_64 2:13.2.10-0.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package gperftools-libs.x86_64 0:2.6.1-1.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package libibverbs.x86_64 0:22.4-6.el7_9 will be installed
    [ceph3.in][DEBUG ] --> Processing Dependency: rdma-core(x86-64) = 22.4-6.el7_9 for package: libibverbs-22.4-6.el7_9.x86_64
    [ceph3.in][DEBUG ] ---> Package liboath.x86_64 0:2.6.2-1.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package librados2.x86_64 2:13.2.10-0.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package librgw2.x86_64 2:13.2.10-0.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package mailcap.noarch 0:2.1.41-2.el7 will be installed
    [ceph3.in][DEBUG ] --> Running transaction check
    [ceph3.in][DEBUG ] ---> Package ceph-common.x86_64 2:13.2.10-0.el7 will be installed
    [ceph3.in][DEBUG ] --> Processing Dependency: python-cephfs = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: libradosstriper1 = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: python-rgw = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: python-rbd = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: python-rados = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: python-ceph-argparse = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: python-prettytable for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: libbabeltrace-ctf.so.1()(64bit) for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: libbabeltrace.so.1()(64bit) for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: libradosstriper.so.1()(64bit) for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph3.in][DEBUG ] ---> Package cryptsetup.x86_64 0:2.0.3-6.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package fuse-libs.x86_64 0:2.9.2-11.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package gdisk.x86_64 0:0.8.10-3.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package leveldb.x86_64 0:1.12.0-11.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package libcephfs2.x86_64 2:13.2.10-0.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package librbd1.x86_64 2:13.2.10-0.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package lttng-ust.x86_64 0:2.4.1-4.el7 will be installed
    [ceph3.in][DEBUG ] --> Processing Dependency: liburcu-bp.so.1()(64bit) for package: lttng-ust-2.4.1-4.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: liburcu-cds.so.1()(64bit) for package: lttng-ust-2.4.1-4.el7.x86_64
    [ceph3.in][DEBUG ] ---> Package psmisc.x86_64 0:22.20-17.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package pyOpenSSL.x86_64 0:0.13.1-4.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package python-cherrypy.noarch 0:3.2.2-4.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package python-jinja2.noarch 0:2.7.2-4.el7 will be installed
    [ceph3.in][DEBUG ] --> Processing Dependency: python-babel >= 0.8 for package: python-jinja2-2.7.2-4.el7.noarch
    [ceph3.in][DEBUG ] --> Processing Dependency: python-markupsafe for package: python-jinja2-2.7.2-4.el7.noarch
    [ceph3.in][DEBUG ] ---> Package python-pecan.noarch 0:0.4.5-2.el7 will be installed
    [ceph3.in][DEBUG ] --> Processing Dependency: python-mako >= 0.4.0 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph3.in][DEBUG ] --> Processing Dependency: python-simplegeneric >= 0.8 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph3.in][DEBUG ] --> Processing Dependency: python-webob >= 1.2 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph3.in][DEBUG ] --> Processing Dependency: python-webtest >= 1.3.1 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph3.in][DEBUG ] --> Processing Dependency: python-singledispatch for package: python-pecan-0.4.5-2.el7.noarch
    [ceph3.in][DEBUG ] ---> Package python-requests.noarch 0:2.6.0-10.el7 will be installed
    [ceph3.in][DEBUG ] --> Processing Dependency: python-urllib3 >= 1.10.2-1 for package: python-requests-2.6.0-10.el7.noarch
    [ceph3.in][DEBUG ] --> Processing Dependency: python-chardet >= 2.2.1-1 for package: python-requests-2.6.0-10.el7.noarch
    [ceph3.in][DEBUG ] ---> Package python-routes.noarch 0:1.13-2.el7 will be installed
    [ceph3.in][DEBUG ] --> Processing Dependency: python-repoze-lru for package: python-routes-1.13-2.el7.noarch
    [ceph3.in][DEBUG ] ---> Package python-setuptools.noarch 0:0.9.8-7.el7 will be installed
    [ceph3.in][DEBUG ] --> Processing Dependency: python-backports-ssl_match_hostname for package: python-setuptools-0.9.8-7.el7.noarch
    [ceph3.in][DEBUG ] ---> Package python-six.noarch 0:1.9.0-2.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package python-werkzeug.noarch 0:0.9.1-2.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package python2-bcrypt.x86_64 0:3.1.6-2.el7 will be installed
    [ceph3.in][DEBUG ] --> Processing Dependency: python-cffi for package: python2-bcrypt-3.1.6-2.el7.x86_64
    [ceph3.in][DEBUG ] --> Processing Dependency: python2-six for package: python2-bcrypt-3.1.6-2.el7.x86_64
    [ceph3.in][DEBUG ] ---> Package rdma-core.x86_64 0:22.4-6.el7_9 will be installed
    [ceph3.in][DEBUG ] --> Processing Dependency: pciutils for package: rdma-core-22.4-6.el7_9.x86_64
    [ceph3.in][DEBUG ] --> Running transaction check
    [ceph3.in][DEBUG ] ---> Package libbabeltrace.x86_64 0:1.2.4-3.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package libradosstriper1.x86_64 2:13.2.10-0.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package pciutils.x86_64 0:3.5.1-3.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package python-babel.noarch 0:0.9.6-8.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package python-backports-ssl_match_hostname.noarch 0:3.5.0.1-1.el7 will be installed
    [ceph3.in][DEBUG ] --> Processing Dependency: python-ipaddress for package: python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch
    [ceph3.in][DEBUG ] --> Processing Dependency: python-backports for package: python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch
    [ceph3.in][DEBUG ] ---> Package python-ceph-argparse.x86_64 2:13.2.10-0.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package python-cephfs.x86_64 2:13.2.10-0.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package python-cffi.x86_64 0:1.6.0-5.el7 will be installed
    [ceph3.in][DEBUG ] --> Processing Dependency: python-pycparser for package: python-cffi-1.6.0-5.el7.x86_64
    [ceph3.in][DEBUG ] ---> Package python-chardet.noarch 0:2.2.1-3.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package python-mako.noarch 0:0.8.1-2.el7 will be installed
    [ceph3.in][DEBUG ] --> Processing Dependency: python-beaker for package: python-mako-0.8.1-2.el7.noarch
    [ceph3.in][DEBUG ] ---> Package python-markupsafe.x86_64 0:0.11-10.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package python-prettytable.noarch 0:0.7.2-3.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package python-rados.x86_64 2:13.2.10-0.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package python-rbd.x86_64 2:13.2.10-0.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package python-repoze-lru.noarch 0:0.4-3.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package python-rgw.x86_64 2:13.2.10-0.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package python-simplegeneric.noarch 0:0.8-7.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package python-singledispatch.noarch 0:3.4.0.2-2.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package python-urllib3.noarch 0:1.10.2-7.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package python-webob.noarch 0:1.2.3-7.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package python-webtest.noarch 0:1.3.4-6.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package python2-six.noarch 0:1.9.0-0.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package userspace-rcu.x86_64 0:0.7.16-1.el7 will be installed
    [ceph3.in][DEBUG ] --> Running transaction check
    [ceph3.in][DEBUG ] ---> Package python-backports.x86_64 0:1.0-8.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package python-beaker.noarch 0:1.5.4-10.el7 will be installed
    [ceph3.in][DEBUG ] --> Processing Dependency: python-paste for package: python-beaker-1.5.4-10.el7.noarch
    [ceph3.in][DEBUG ] ---> Package python-ipaddress.noarch 0:1.0.16-2.el7 will be installed
    [ceph3.in][DEBUG ] ---> Package python-pycparser.noarch 0:2.14-1.el7 will be installed
    [ceph3.in][DEBUG ] --> Processing Dependency: python-ply for package: python-pycparser-2.14-1.el7.noarch
    [ceph3.in][DEBUG ] --> Running transaction check
    [ceph3.in][DEBUG ] ---> Package python-paste.noarch 0:1.7.5.1-9.20111221hg1498.el7 will be installed
    [ceph3.in][DEBUG ] --> Processing Dependency: python-tempita for package: python-paste-1.7.5.1-9.20111221hg1498.el7.noarch
    [ceph3.in][DEBUG ] ---> Package python-ply.noarch 0:3.4-11.el7 will be installed
    [ceph3.in][DEBUG ] --> Running transaction check
    [ceph3.in][DEBUG ] ---> Package python-tempita.noarch 0:0.5.1-6.el7 will be installed
    [ceph3.in][DEBUG ] --> Finished Dependency Resolution
    [ceph3.in][DEBUG ]
    [ceph3.in][DEBUG ] Dependencies Resolved
    [ceph3.in][DEBUG ]
    [ceph3.in][DEBUG ] ================================================================================
    [ceph3.in][DEBUG ]  Package                      Arch   Version                      Repository
    [ceph3.in][DEBUG ]                                                                            Size
    [ceph3.in][DEBUG ] ================================================================================
    [ceph3.in][DEBUG ] Installing:
    [ceph3.in][DEBUG ]  ceph                         x86_64 2:13.2.10-0.el7              Ceph    3.0 k
    [ceph3.in][DEBUG ]  ceph-radosgw                 x86_64 2:13.2.10-0.el7              Ceph    4.5 M
    [ceph3.in][DEBUG ] Installing for dependencies:
    [ceph3.in][DEBUG ]  ceph-base                    x86_64 2:13.2.10-0.el7              Ceph    4.8 M
    [ceph3.in][DEBUG ]  ceph-common                  x86_64 2:13.2.10-0.el7              Ceph     14 M
    [ceph3.in][DEBUG ]  ceph-mds                     x86_64 2:13.2.10-0.el7              Ceph    1.7 M
    [ceph3.in][DEBUG ]  ceph-mgr                     x86_64 2:13.2.10-0.el7              Ceph    3.5 M
    [ceph3.in][DEBUG ]  ceph-mon                     x86_64 2:13.2.10-0.el7              Ceph    3.9 M
    [ceph3.in][DEBUG ]  ceph-osd                     x86_64 2:13.2.10-0.el7              Ceph     13 M
    [ceph3.in][DEBUG ]  ceph-selinux                 x86_64 2:13.2.10-0.el7              Ceph     21 k
    [ceph3.in][DEBUG ]  cryptsetup                   x86_64 2.0.3-6.el7                  base    154 k
    [ceph3.in][DEBUG ]  fuse-libs                    x86_64 2.9.2-11.el7                 base     93 k
    [ceph3.in][DEBUG ]  gdisk                        x86_64 0.8.10-3.el7                 base    190 k
    [ceph3.in][DEBUG ]  gperftools-libs              x86_64 2.6.1-1.el7                  base    272 k
    [ceph3.in][DEBUG ]  leveldb                      x86_64 1.12.0-11.el7                epel    161 k
    [ceph3.in][DEBUG ]  libbabeltrace                x86_64 1.2.4-3.el7                  epel    147 k
    [ceph3.in][DEBUG ]  libcephfs2                   x86_64 2:13.2.10-0.el7              Ceph    434 k
    [ceph3.in][DEBUG ]  libibverbs                   x86_64 22.4-6.el7_9                 updates 269 k
    [ceph3.in][DEBUG ]  liboath                      x86_64 2.6.2-1.el7                  epel     51 k
    [ceph3.in][DEBUG ]  librados2                    x86_64 2:13.2.10-0.el7              Ceph    2.9 M
    [ceph3.in][DEBUG ]  libradosstriper1             x86_64 2:13.2.10-0.el7              Ceph    329 k
    [ceph3.in][DEBUG ]  librbd1                      x86_64 2:13.2.10-0.el7              Ceph    1.2 M
    [ceph3.in][DEBUG ]  librgw2                      x86_64 2:13.2.10-0.el7              Ceph    2.0 M
    [ceph3.in][DEBUG ]  lttng-ust                    x86_64 2.4.1-4.el7                  epel    176 k
    [ceph3.in][DEBUG ]  mailcap                      noarch 2.1.41-2.el7                 base     31 k
    [ceph3.in][DEBUG ]  pciutils                     x86_64 3.5.1-3.el7                  base     93 k
    [ceph3.in][DEBUG ]  psmisc                       x86_64 22.20-17.el7                 base    141 k
    [ceph3.in][DEBUG ]  pyOpenSSL                    x86_64 0.13.1-4.el7                 base    135 k
    [ceph3.in][DEBUG ]  python-babel                 noarch 0.9.6-8.el7                  base    1.4 M
    [ceph3.in][DEBUG ]  python-backports             x86_64 1.0-8.el7                    base    5.8 k
    [ceph3.in][DEBUG ]  python-backports-ssl_match_hostname
    [ceph3.in][DEBUG ]                               noarch 3.5.0.1-1.el7                base     13 k
    [ceph3.in][DEBUG ]  python-beaker                noarch 1.5.4-10.el7                 base     80 k
    [ceph3.in][DEBUG ]  python-ceph-argparse         x86_64 2:13.2.10-0.el7              Ceph     34 k
    [ceph3.in][DEBUG ]  python-cephfs                x86_64 2:13.2.10-0.el7              Ceph     87 k
    [ceph3.in][DEBUG ]  python-cffi                  x86_64 1.6.0-5.el7                  base    218 k
    [ceph3.in][DEBUG ]  python-chardet               noarch 2.2.1-3.el7                  base    227 k
    [ceph3.in][DEBUG ]  python-cherrypy              noarch 3.2.2-4.el7                  base    422 k
    [ceph3.in][DEBUG ]  python-ipaddress             noarch 1.0.16-2.el7                 base     34 k
    [ceph3.in][DEBUG ]  python-jinja2                noarch 2.7.2-4.el7                  base    519 k
    [ceph3.in][DEBUG ]  python-mako                  noarch 0.8.1-2.el7                  base    307 k
    [ceph3.in][DEBUG ]  python-markupsafe            x86_64 0.11-10.el7                  base     25 k
    [ceph3.in][DEBUG ]  python-paste                 noarch 1.7.5.1-9.20111221hg1498.el7 base    866 k
    [ceph3.in][DEBUG ]  python-pecan                 noarch 0.4.5-2.el7                  epel    255 k
    [ceph3.in][DEBUG ]  python-ply                   noarch 3.4-11.el7                   base    123 k
    [ceph3.in][DEBUG ]  python-prettytable           noarch 0.7.2-3.el7                  base     37 k
    [ceph3.in][DEBUG ]  python-pycparser             noarch 2.14-1.el7                   base    104 k
    [ceph3.in][DEBUG ]  python-rados                 x86_64 2:13.2.10-0.el7              Ceph    189 k
    [ceph3.in][DEBUG ]  python-rbd                   x86_64 2:13.2.10-0.el7              Ceph    132 k
    [ceph3.in][DEBUG ]  python-repoze-lru            noarch 0.4-3.el7                    epel     13 k
    [ceph3.in][DEBUG ]  python-requests              noarch 2.6.0-10.el7                 base     95 k
    [ceph3.in][DEBUG ]  python-rgw                   x86_64 2:13.2.10-0.el7              Ceph     76 k
    [ceph3.in][DEBUG ]  python-routes                noarch 1.13-2.el7                   epel    640 k
    [ceph3.in][DEBUG ]  python-setuptools            noarch 0.9.8-7.el7                  base    397 k
    [ceph3.in][DEBUG ]  python-simplegeneric         noarch 0.8-7.el7                    epel     12 k
    [ceph3.in][DEBUG ]  python-singledispatch        noarch 3.4.0.2-2.el7                epel     18 k
    [ceph3.in][DEBUG ]  python-six                   noarch 1.9.0-2.el7                  base     29 k
    [ceph3.in][DEBUG ]  python-tempita               noarch 0.5.1-6.el7                  base     33 k
    [ceph3.in][DEBUG ]  python-urllib3               noarch 1.10.2-7.el7                 base    103 k
    [ceph3.in][DEBUG ]  python-webob                 noarch 1.2.3-7.el7                  base    202 k
    [ceph3.in][DEBUG ]  python-webtest               noarch 1.3.4-6.el7                  base    102 k
    [ceph3.in][DEBUG ]  python-werkzeug              noarch 0.9.1-2.el7                  extras  562 k
    [ceph3.in][DEBUG ]  python2-bcrypt               x86_64 3.1.6-2.el7                  epel     39 k
    [ceph3.in][DEBUG ]  python2-six                  noarch 1.9.0-0.el7                  epel    2.9 k
    [ceph3.in][DEBUG ]  rdma-core                    x86_64 22.4-6.el7_9                 updates  51 k
    [ceph3.in][DEBUG ]  userspace-rcu                x86_64 0.7.16-1.el7                 epel     73 k
    [ceph3.in][DEBUG ]
    [ceph3.in][DEBUG ] Transaction Summary
    [ceph3.in][DEBUG ] ================================================================================
    [ceph3.in][DEBUG ] Install  2 Packages (+62 Dependent packages)
    [ceph3.in][DEBUG ]
    [ceph3.in][DEBUG ] Total download size: 61 M
    [ceph3.in][DEBUG ] Installed size: 210 M
    [ceph3.in][DEBUG ] Downloading packages:
    [ceph3.in][DEBUG ] Public key for leveldb-1.12.0-11.el7.x86_64.rpm is not installed
    [ceph3.in][WARNIN] warning: /var/cache/yum/x86_64/7/epel/packages/leveldb-1.12.0-11.el7.x86_64.rpm: Header V3 RSA/SHA256 Signature, key ID 352c64e5: NOKEY
    [ceph3.in][DEBUG ] --------------------------------------------------------------------------------
    [ceph3.in][DEBUG ] Total                                              5.9 MB/s |  61 MB  00:10
    [ceph3.in][DEBUG ] Retrieving key from file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
    [ceph3.in][WARNIN] Importing GPG key 0x352C64E5:
    [ceph3.in][WARNIN]  Userid     : "Fedora EPEL (7) <epel@fedoraproject.org>"
    [ceph3.in][WARNIN]  Fingerprint: 91e9 7d7c 4a5e 96f1 7f3e 888f 6a2f aea2 352c 64e5
    [ceph3.in][WARNIN]  Package    : epel-release-7-14.noarch (@/epel-release-latest-7.noarch)
    [ceph3.in][WARNIN]  From       : /etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
    [ceph3.in][DEBUG ] Running transaction check
    [ceph3.in][DEBUG ] Running transaction test
    [ceph3.in][DEBUG ] Transaction test succeeded
    [ceph3.in][DEBUG ] Running transaction
    [ceph3.in][DEBUG ]   Installing : gperftools-libs-2.6.1-1.el7.x86_64                          1/64
    [ceph3.in][DEBUG ]   Installing : leveldb-1.12.0-11.el7.x86_64                                2/64
    [ceph3.in][DEBUG ]   Installing : python-six-1.9.0-2.el7.noarch                               3/64
    [ceph3.in][DEBUG ]   Installing : fuse-libs-2.9.2-11.el7.x86_64                               4/64
    [ceph3.in][DEBUG ]   Installing : liboath-2.6.2-1.el7.x86_64                                  5/64
    [ceph3.in][DEBUG ]   Installing : python-ipaddress-1.0.16-2.el7.noarch                        6/64
    [ceph3.in][DEBUG ]   Installing : python-webob-1.2.3-7.el7.noarch                             7/64
    [ceph3.in][DEBUG ]   Installing : python-markupsafe-0.11-10.el7.x86_64                        8/64
    [ceph3.in][DEBUG ]   Installing : pyOpenSSL-0.13.1-4.el7.x86_64                               9/64
    [ceph3.in][DEBUG ]   Installing : 2:python-ceph-argparse-13.2.10-0.el7.x86_64                10/64
    [ceph3.in][DEBUG ]   Installing : python-webtest-1.3.4-6.el7.noarch                          11/64
    [ceph3.in][DEBUG ]   Installing : python2-six-1.9.0-0.el7.noarch                             12/64
    [ceph3.in][DEBUG ]   Installing : python-singledispatch-3.4.0.2-2.el7.noarch                 13/64
    [ceph3.in][DEBUG ]   Installing : psmisc-22.20-17.el7.x86_64                                 14/64
    [ceph3.in][DEBUG ]   Installing : pciutils-3.5.1-3.el7.x86_64                                15/64
    [ceph3.in][DEBUG ]   Installing : rdma-core-22.4-6.el7_9.x86_64                              16/64
    [ceph3.in][DEBUG ]   Installing : libibverbs-22.4-6.el7_9.x86_64                             17/64
    [ceph3.in][DEBUG ]   Installing : gdisk-0.8.10-3.el7.x86_64                                  18/64
    [ceph3.in][DEBUG ]   Installing : python-simplegeneric-0.8-7.el7.noarch                      19/64
    [ceph3.in][DEBUG ]   Installing : python-tempita-0.5.1-6.el7.noarch                          20/64
    [ceph3.in][DEBUG ]   Installing : python-cherrypy-3.2.2-4.el7.noarch                         21/64
    [ceph3.in][DEBUG ]   Installing : python-prettytable-0.7.2-3.el7.noarch                      22/64
    [ceph3.in][DEBUG ]   Installing : python-werkzeug-0.9.1-2.el7.noarch                         23/64
    [ceph3.in][DEBUG ]   Installing : python-repoze-lru-0.4-3.el7.noarch                         24/64
    [ceph3.in][DEBUG ]   Installing : python-routes-1.13-2.el7.noarch                            25/64
    [ceph3.in][DEBUG ]   Installing : python-backports-1.0-8.el7.x86_64                          26/64
    [ceph3.in][DEBUG ]   Installing : python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch   27/64
    [ceph3.in][DEBUG ]   Installing : python-setuptools-0.9.8-7.el7.noarch                       28/64
    [ceph3.in][DEBUG ]   Installing : python-paste-1.7.5.1-9.20111221hg1498.el7.noarch           29/64
    [ceph3.in][DEBUG ]   Installing : python-beaker-1.5.4-10.el7.noarch                          30/64
    [ceph3.in][DEBUG ]   Installing : python-mako-0.8.1-2.el7.noarch                             31/64
    [ceph3.in][DEBUG ]   Installing : python-pecan-0.4.5-2.el7.noarch                            32/64
    [ceph3.in][DEBUG ]   Installing : python-urllib3-1.10.2-7.el7.noarch                         33/64
    [ceph3.in][DEBUG ]   Installing : python-babel-0.9.6-8.el7.noarch                            34/64
    [ceph3.in][DEBUG ]   Installing : python-jinja2-2.7.2-4.el7.noarch                           35/64
    [ceph3.in][DEBUG ]   Installing : python-chardet-2.2.1-3.el7.noarch                          36/64
    [ceph3.in][DEBUG ]   Installing : python-requests-2.6.0-10.el7.noarch                        37/64
    [ceph3.in][DEBUG ]   Installing : cryptsetup-2.0.3-6.el7.x86_64                              38/64
    [ceph3.in][DEBUG ]   Installing : libbabeltrace-1.2.4-3.el7.x86_64                           39/64
    [ceph3.in][DEBUG ]   Installing : userspace-rcu-0.7.16-1.el7.x86_64                          40/64
    [ceph3.in][DEBUG ]   Installing : lttng-ust-2.4.1-4.el7.x86_64                               41/64
    [ceph3.in][DEBUG ]   Installing : 2:librados2-13.2.10-0.el7.x86_64                           42/64
    [ceph3.in][DEBUG ]   Installing : 2:python-rados-13.2.10-0.el7.x86_64                        43/64
    [ceph3.in][DEBUG ]   Installing : 2:librbd1-13.2.10-0.el7.x86_64                             44/64
    [ceph3.in][DEBUG ]   Installing : 2:libcephfs2-13.2.10-0.el7.x86_64                          45/64
    [ceph3.in][DEBUG ]   Installing : 2:librgw2-13.2.10-0.el7.x86_64                             46/64
    [ceph3.in][DEBUG ]   Installing : 2:python-rgw-13.2.10-0.el7.x86_64                          47/64
    [ceph3.in][DEBUG ]   Installing : 2:python-cephfs-13.2.10-0.el7.x86_64                       48/64
    [ceph3.in][DEBUG ]   Installing : 2:python-rbd-13.2.10-0.el7.x86_64                          49/64
    [ceph3.in][DEBUG ]   Installing : 2:libradosstriper1-13.2.10-0.el7.x86_64                    50/64
    [ceph3.in][DEBUG ]   Installing : 2:ceph-common-13.2.10-0.el7.x86_64                         51/64
    [ceph3.in][DEBUG ]   Installing : 2:ceph-base-13.2.10-0.el7.x86_64                           52/64
    [ceph3.in][DEBUG ]   Installing : 2:ceph-selinux-13.2.10-0.el7.x86_64                        53/64
    [ceph3.in][DEBUG ]   Installing : 2:ceph-osd-13.2.10-0.el7.x86_64                            54/64
    [ceph3.in][DEBUG ]   Installing : 2:ceph-mds-13.2.10-0.el7.x86_64                            55/64
    [ceph3.in][DEBUG ]   Installing : 2:ceph-mon-13.2.10-0.el7.x86_64                            56/64
    [ceph3.in][DEBUG ]   Installing : python-ply-3.4-11.el7.noarch                               57/64
    [ceph3.in][DEBUG ]   Installing : python-pycparser-2.14-1.el7.noarch                         58/64
    [ceph3.in][DEBUG ]   Installing : python-cffi-1.6.0-5.el7.x86_64                             59/64
    [ceph3.in][DEBUG ]   Installing : python2-bcrypt-3.1.6-2.el7.x86_64                          60/64
    [ceph3.in][DEBUG ]   Installing : 2:ceph-mgr-13.2.10-0.el7.x86_64                            61/64
    [ceph3.in][DEBUG ]   Installing : mailcap-2.1.41-2.el7.noarch                                62/64
    [ceph3.in][DEBUG ]   Installing : 2:ceph-radosgw-13.2.10-0.el7.x86_64                        63/64
    [ceph3.in][DEBUG ]   Installing : 2:ceph-13.2.10-0.el7.x86_64                                64/64
    [ceph3.in][DEBUG ]   Verifying  : liboath-2.6.2-1.el7.x86_64                                  1/64
    [ceph3.in][DEBUG ]   Verifying  : python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch    2/64
    [ceph3.in][DEBUG ]   Verifying  : 2:librbd1-13.2.10-0.el7.x86_64                              3/64
    [ceph3.in][DEBUG ]   Verifying  : 2:python-ceph-argparse-13.2.10-0.el7.x86_64                 4/64
    [ceph3.in][DEBUG ]   Verifying  : mailcap-2.1.41-2.el7.noarch                                 5/64
    [ceph3.in][DEBUG ]   Verifying  : pyOpenSSL-0.13.1-4.el7.x86_64                               6/64
    [ceph3.in][DEBUG ]   Verifying  : python2-bcrypt-3.1.6-2.el7.x86_64                           7/64
    [ceph3.in][DEBUG ]   Verifying  : python-ply-3.4-11.el7.noarch                                8/64
    [ceph3.in][DEBUG ]   Verifying  : userspace-rcu-0.7.16-1.el7.x86_64                           9/64
    [ceph3.in][DEBUG ]   Verifying  : libibverbs-22.4-6.el7_9.x86_64                             10/64
    [ceph3.in][DEBUG ]   Verifying  : rdma-core-22.4-6.el7_9.x86_64                              11/64
    [ceph3.in][DEBUG ]   Verifying  : fuse-libs-2.9.2-11.el7.x86_64                              12/64
    [ceph3.in][DEBUG ]   Verifying  : python-setuptools-0.9.8-7.el7.noarch                       13/64
    [ceph3.in][DEBUG ]   Verifying  : python-routes-1.13-2.el7.noarch                            14/64
    [ceph3.in][DEBUG ]   Verifying  : 2:libcephfs2-13.2.10-0.el7.x86_64                          15/64
    [ceph3.in][DEBUG ]   Verifying  : python-urllib3-1.10.2-7.el7.noarch                         16/64
    [ceph3.in][DEBUG ]   Verifying  : libbabeltrace-1.2.4-3.el7.x86_64                           17/64
    [ceph3.in][DEBUG ]   Verifying  : python-mako-0.8.1-2.el7.noarch                             18/64
    [ceph3.in][DEBUG ]   Verifying  : python2-six-1.9.0-0.el7.noarch                             19/64
    [ceph3.in][DEBUG ]   Verifying  : 2:ceph-mgr-13.2.10-0.el7.x86_64                            20/64
    [ceph3.in][DEBUG ]   Verifying  : 2:ceph-base-13.2.10-0.el7.x86_64                           21/64
    [ceph3.in][DEBUG ]   Verifying  : python-jinja2-2.7.2-4.el7.noarch                           22/64
    [ceph3.in][DEBUG ]   Verifying  : python-pecan-0.4.5-2.el7.noarch                            23/64
    [ceph3.in][DEBUG ]   Verifying  : python-six-1.9.0-2.el7.noarch                              24/64
    [ceph3.in][DEBUG ]   Verifying  : cryptsetup-2.0.3-6.el7.x86_64                              25/64
    [ceph3.in][DEBUG ]   Verifying  : leveldb-1.12.0-11.el7.x86_64                               26/64
    [ceph3.in][DEBUG ]   Verifying  : python-singledispatch-3.4.0.2-2.el7.noarch                 27/64
    [ceph3.in][DEBUG ]   Verifying  : python-markupsafe-0.11-10.el7.x86_64                       28/64
    [ceph3.in][DEBUG ]   Verifying  : 2:python-rados-13.2.10-0.el7.x86_64                        29/64
    [ceph3.in][DEBUG ]   Verifying  : 2:python-rgw-13.2.10-0.el7.x86_64                          30/64
    [ceph3.in][DEBUG ]   Verifying  : 2:ceph-radosgw-13.2.10-0.el7.x86_64                        31/64
    [ceph3.in][DEBUG ]   Verifying  : python-chardet-2.2.1-3.el7.noarch                          32/64
    [ceph3.in][DEBUG ]   Verifying  : python-babel-0.9.6-8.el7.noarch                            33/64
    [ceph3.in][DEBUG ]   Verifying  : 2:librados2-13.2.10-0.el7.x86_64                           34/64
    [ceph3.in][DEBUG ]   Verifying  : python-paste-1.7.5.1-9.20111221hg1498.el7.noarch           35/64
    [ceph3.in][DEBUG ]   Verifying  : 2:ceph-osd-13.2.10-0.el7.x86_64                            36/64
    [ceph3.in][DEBUG ]   Verifying  : python-backports-1.0-8.el7.x86_64                          37/64
    [ceph3.in][DEBUG ]   Verifying  : lttng-ust-2.4.1-4.el7.x86_64                               38/64
    [ceph3.in][DEBUG ]   Verifying  : python-webob-1.2.3-7.el7.noarch                            39/64
    [ceph3.in][DEBUG ]   Verifying  : 2:ceph-common-13.2.10-0.el7.x86_64                         40/64
    [ceph3.in][DEBUG ]   Verifying  : python-repoze-lru-0.4-3.el7.noarch                         41/64
    [ceph3.in][DEBUG ]   Verifying  : python-werkzeug-0.9.1-2.el7.noarch                         42/64
    [ceph3.in][DEBUG ]   Verifying  : python-beaker-1.5.4-10.el7.noarch                          43/64
    [ceph3.in][DEBUG ]   Verifying  : python-cffi-1.6.0-5.el7.x86_64                             44/64
    [ceph3.in][DEBUG ]   Verifying  : 2:ceph-selinux-13.2.10-0.el7.x86_64                        45/64
    [ceph3.in][DEBUG ]   Verifying  : python-requests-2.6.0-10.el7.noarch                        46/64
    [ceph3.in][DEBUG ]   Verifying  : python-pycparser-2.14-1.el7.noarch                         47/64
    [ceph3.in][DEBUG ]   Verifying  : python-prettytable-0.7.2-3.el7.noarch                      48/64
    [ceph3.in][DEBUG ]   Verifying  : 2:librgw2-13.2.10-0.el7.x86_64                             49/64
    [ceph3.in][DEBUG ]   Verifying  : 2:ceph-mds-13.2.10-0.el7.x86_64                            50/64
    [ceph3.in][DEBUG ]   Verifying  : python-cherrypy-3.2.2-4.el7.noarch                         51/64
    [ceph3.in][DEBUG ]   Verifying  : 2:python-cephfs-13.2.10-0.el7.x86_64                       52/64
    [ceph3.in][DEBUG ]   Verifying  : python-tempita-0.5.1-6.el7.noarch                          53/64
    [ceph3.in][DEBUG ]   Verifying  : 2:python-rbd-13.2.10-0.el7.x86_64                          54/64
    [ceph3.in][DEBUG ]   Verifying  : 2:ceph-mon-13.2.10-0.el7.x86_64                            55/64
    [ceph3.in][DEBUG ]   Verifying  : gperftools-libs-2.6.1-1.el7.x86_64                         56/64
    [ceph3.in][DEBUG ]   Verifying  : python-ipaddress-1.0.16-2.el7.noarch                       57/64
    [ceph3.in][DEBUG ]   Verifying  : python-webtest-1.3.4-6.el7.noarch                          58/64
    [ceph3.in][DEBUG ]   Verifying  : 2:ceph-13.2.10-0.el7.x86_64                                59/64
    [ceph3.in][DEBUG ]   Verifying  : python-simplegeneric-0.8-7.el7.noarch                      60/64
    [ceph3.in][DEBUG ]   Verifying  : gdisk-0.8.10-3.el7.x86_64                                  61/64
    [ceph3.in][DEBUG ]   Verifying  : 2:libradosstriper1-13.2.10-0.el7.x86_64                    62/64
    [ceph3.in][DEBUG ]   Verifying  : pciutils-3.5.1-3.el7.x86_64                                63/64
    [ceph3.in][DEBUG ]   Verifying  : psmisc-22.20-17.el7.x86_64                                 64/64
    [ceph3.in][DEBUG ]
    [ceph3.in][DEBUG ] Installed:
    [ceph3.in][DEBUG ]   ceph.x86_64 2:13.2.10-0.el7        ceph-radosgw.x86_64 2:13.2.10-0.el7
    [ceph3.in][DEBUG ]
    [ceph3.in][DEBUG ] Dependency Installed:
    [ceph3.in][DEBUG ]   ceph-base.x86_64 2:13.2.10-0.el7
    [ceph3.in][DEBUG ]   ceph-common.x86_64 2:13.2.10-0.el7
    [ceph3.in][DEBUG ]   ceph-mds.x86_64 2:13.2.10-0.el7
    [ceph3.in][DEBUG ]   ceph-mgr.x86_64 2:13.2.10-0.el7
    [ceph3.in][DEBUG ]   ceph-mon.x86_64 2:13.2.10-0.el7
    [ceph3.in][DEBUG ]   ceph-osd.x86_64 2:13.2.10-0.el7
    [ceph3.in][DEBUG ]   ceph-selinux.x86_64 2:13.2.10-0.el7
    [ceph3.in][DEBUG ]   cryptsetup.x86_64 0:2.0.3-6.el7
    [ceph3.in][DEBUG ]   fuse-libs.x86_64 0:2.9.2-11.el7
    [ceph3.in][DEBUG ]   gdisk.x86_64 0:0.8.10-3.el7
    [ceph3.in][DEBUG ]   gperftools-libs.x86_64 0:2.6.1-1.el7
    [ceph3.in][DEBUG ]   leveldb.x86_64 0:1.12.0-11.el7
    [ceph3.in][DEBUG ]   libbabeltrace.x86_64 0:1.2.4-3.el7
    [ceph3.in][DEBUG ]   libcephfs2.x86_64 2:13.2.10-0.el7
    [ceph3.in][DEBUG ]   libibverbs.x86_64 0:22.4-6.el7_9
    [ceph3.in][DEBUG ]   liboath.x86_64 0:2.6.2-1.el7
    [ceph3.in][DEBUG ]   librados2.x86_64 2:13.2.10-0.el7
    [ceph3.in][DEBUG ]   libradosstriper1.x86_64 2:13.2.10-0.el7
    [ceph3.in][DEBUG ]   librbd1.x86_64 2:13.2.10-0.el7
    [ceph3.in][DEBUG ]   librgw2.x86_64 2:13.2.10-0.el7
    [ceph3.in][DEBUG ]   lttng-ust.x86_64 0:2.4.1-4.el7
    [ceph3.in][DEBUG ]   mailcap.noarch 0:2.1.41-2.el7
    [ceph3.in][DEBUG ]   pciutils.x86_64 0:3.5.1-3.el7
    [ceph3.in][DEBUG ]   psmisc.x86_64 0:22.20-17.el7
    [ceph3.in][DEBUG ]   pyOpenSSL.x86_64 0:0.13.1-4.el7
    [ceph3.in][DEBUG ]   python-babel.noarch 0:0.9.6-8.el7
    [ceph3.in][DEBUG ]   python-backports.x86_64 0:1.0-8.el7
    [ceph3.in][DEBUG ]   python-backports-ssl_match_hostname.noarch 0:3.5.0.1-1.el7
    [ceph3.in][DEBUG ]   python-beaker.noarch 0:1.5.4-10.el7
    [ceph3.in][DEBUG ]   python-ceph-argparse.x86_64 2:13.2.10-0.el7
    [ceph3.in][DEBUG ]   python-cephfs.x86_64 2:13.2.10-0.el7
    [ceph3.in][DEBUG ]   python-cffi.x86_64 0:1.6.0-5.el7
    [ceph3.in][DEBUG ]   python-chardet.noarch 0:2.2.1-3.el7
    [ceph3.in][DEBUG ]   python-cherrypy.noarch 0:3.2.2-4.el7
    [ceph3.in][DEBUG ]   python-ipaddress.noarch 0:1.0.16-2.el7
    [ceph3.in][DEBUG ]   python-jinja2.noarch 0:2.7.2-4.el7
    [ceph3.in][DEBUG ]   python-mako.noarch 0:0.8.1-2.el7
    [ceph3.in][DEBUG ]   python-markupsafe.x86_64 0:0.11-10.el7
    [ceph3.in][DEBUG ]   python-paste.noarch 0:1.7.5.1-9.20111221hg1498.el7
    [ceph3.in][DEBUG ]   python-pecan.noarch 0:0.4.5-2.el7
    [ceph3.in][DEBUG ]   python-ply.noarch 0:3.4-11.el7
    [ceph3.in][DEBUG ]   python-prettytable.noarch 0:0.7.2-3.el7
    [ceph3.in][DEBUG ]   python-pycparser.noarch 0:2.14-1.el7
    [ceph3.in][DEBUG ]   python-rados.x86_64 2:13.2.10-0.el7
    [ceph3.in][DEBUG ]   python-rbd.x86_64 2:13.2.10-0.el7
    [ceph3.in][DEBUG ]   python-repoze-lru.noarch 0:0.4-3.el7
    [ceph3.in][DEBUG ]   python-requests.noarch 0:2.6.0-10.el7
    [ceph3.in][DEBUG ]   python-rgw.x86_64 2:13.2.10-0.el7
    [ceph3.in][DEBUG ]   python-routes.noarch 0:1.13-2.el7
    [ceph3.in][DEBUG ]   python-setuptools.noarch 0:0.9.8-7.el7
    [ceph3.in][DEBUG ]   python-simplegeneric.noarch 0:0.8-7.el7
    [ceph3.in][DEBUG ]   python-singledispatch.noarch 0:3.4.0.2-2.el7
    [ceph3.in][DEBUG ]   python-six.noarch 0:1.9.0-2.el7
    [ceph3.in][DEBUG ]   python-tempita.noarch 0:0.5.1-6.el7
    [ceph3.in][DEBUG ]   python-urllib3.noarch 0:1.10.2-7.el7
    [ceph3.in][DEBUG ]   python-webob.noarch 0:1.2.3-7.el7
    [ceph3.in][DEBUG ]   python-webtest.noarch 0:1.3.4-6.el7
    [ceph3.in][DEBUG ]   python-werkzeug.noarch 0:0.9.1-2.el7
    [ceph3.in][DEBUG ]   python2-bcrypt.x86_64 0:3.1.6-2.el7
    [ceph3.in][DEBUG ]   python2-six.noarch 0:1.9.0-0.el7
    [ceph3.in][DEBUG ]   rdma-core.x86_64 0:22.4-6.el7_9
    [ceph3.in][DEBUG ]   userspace-rcu.x86_64 0:0.7.16-1.el7
    [ceph3.in][DEBUG ]
    [ceph3.in][DEBUG ] Complete!
    [ceph3.in][INFO  ] Running command: sudo ceph --version
    [ceph3.in][DEBUG ] ceph version 13.2.10 (564bdc4ae87418a232fc901524470e1a0f76d641) mimic (stable)
    [ceph_deploy.install][DEBUG ] Detecting platform for host ceph4.in ...
    [ceph4.in][DEBUG ] connection detected need for sudo
    [ceph4.in][DEBUG ] connected to host: ceph4.in
    [ceph4.in][DEBUG ] detect platform information from remote host
    [ceph4.in][DEBUG ] detect machine type
    [ceph_deploy.install][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph4.in][INFO  ] installing Ceph on ceph4.in
    [ceph4.in][INFO  ] Running command: sudo yum clean all
    [ceph4.in][DEBUG ] Loaded plugins: fastestmirror
    [ceph4.in][DEBUG ] Cleaning repos: base epel extras updates
    [ceph4.in][DEBUG ] Cleaning up list of fastest mirrors
    [ceph4.in][INFO  ] Running command: sudo yum -y install epel-release
    [ceph4.in][DEBUG ] Loaded plugins: fastestmirror
    [ceph4.in][DEBUG ] Determining fastest mirrors
    [ceph4.in][DEBUG ]  * base: centos.mirror.net.in
    [ceph4.in][DEBUG ]  * epel: repo.extreme-ix.org
    [ceph4.in][DEBUG ]  * extras: centos.mirror.net.in
    [ceph4.in][DEBUG ]  * updates: centos.mirror.net.in
    [ceph4.in][DEBUG ] Package epel-release-7-14.noarch already installed and latest version
    [ceph4.in][DEBUG ] Nothing to do
    [ceph4.in][INFO  ] Running command: sudo yum -y install yum-plugin-priorities
    [ceph4.in][DEBUG ] Loaded plugins: fastestmirror
    [ceph4.in][DEBUG ] Loading mirror speeds from cached hostfile
    [ceph4.in][DEBUG ]  * base: centos.mirror.net.in
    [ceph4.in][DEBUG ]  * epel: repo.extreme-ix.org
    [ceph4.in][DEBUG ]  * extras: centos.mirror.net.in
    [ceph4.in][DEBUG ]  * updates: centos.mirror.net.in
    [ceph4.in][DEBUG ] Resolving Dependencies
    [ceph4.in][DEBUG ] --> Running transaction check
    [ceph4.in][DEBUG ] ---> Package yum-plugin-priorities.noarch 0:1.1.31-54.el7_8 will be installed
    [ceph4.in][DEBUG ] --> Finished Dependency Resolution
    [ceph4.in][DEBUG ]
    [ceph4.in][DEBUG ] Dependencies Resolved
    [ceph4.in][DEBUG ]
    [ceph4.in][DEBUG ] ================================================================================
    [ceph4.in][DEBUG ]  Package                    Arch        Version                 Repository
    [ceph4.in][DEBUG ]                                                                            Size
    [ceph4.in][DEBUG ] ================================================================================
    [ceph4.in][DEBUG ] Installing:
    [ceph4.in][DEBUG ]  yum-plugin-priorities      noarch      1.1.31-54.el7_8         base       29 k
    [ceph4.in][DEBUG ]
    [ceph4.in][DEBUG ] Transaction Summary
    [ceph4.in][DEBUG ] ================================================================================
    [ceph4.in][DEBUG ] Install  1 Package
    [ceph4.in][DEBUG ]
    [ceph4.in][DEBUG ] Total download size: 29 k
    [ceph4.in][DEBUG ] Installed size: 28 k
    [ceph4.in][DEBUG ] Downloading packages:
    [ceph4.in][DEBUG ] Running transaction check
    [ceph4.in][DEBUG ] Running transaction test
    [ceph4.in][DEBUG ] Transaction test succeeded
    [ceph4.in][DEBUG ] Running transaction
    [ceph4.in][DEBUG ]   Installing : yum-plugin-priorities-1.1.31-54.el7_8.noarch                 1/1
    [ceph4.in][DEBUG ]   Verifying  : yum-plugin-priorities-1.1.31-54.el7_8.noarch                 1/1
    [ceph4.in][DEBUG ]
    [ceph4.in][DEBUG ] Installed:
    [ceph4.in][DEBUG ]   yum-plugin-priorities.noarch 0:1.1.31-54.el7_8
    [ceph4.in][DEBUG ]
    [ceph4.in][DEBUG ] Complete!
    [ceph4.in][DEBUG ] Configure Yum priorities to include obsoletes
    [ceph4.in][WARNIN] check_obsoletes has been enabled for Yum priorities plugin
    [ceph4.in][INFO  ] Running command: sudo rpm --import https://download.ceph.com/keys/release.asc
    [ceph4.in][INFO  ] Running command: sudo yum remove -y ceph-release
    [ceph4.in][DEBUG ] Loaded plugins: fastestmirror, priorities
    [ceph4.in][WARNIN] No Match for argument: ceph-release
    [ceph4.in][DEBUG ] No Packages marked for removal
    [ceph4.in][INFO  ] Running command: sudo yum install -y https://download.ceph.com/rpm-mimic/el7/noarch/ceph-release-1-0.el7.noarch.rpm
    [ceph4.in][DEBUG ] Loaded plugins: fastestmirror, priorities
    [ceph4.in][DEBUG ] Examining /var/tmp/yum-root-McVLyf/ceph-release-1-0.el7.noarch.rpm: ceph-release-1-1.el7.noarch
    [ceph4.in][DEBUG ] Marking /var/tmp/yum-root-McVLyf/ceph-release-1-0.el7.noarch.rpm to be installed
    [ceph4.in][DEBUG ] Resolving Dependencies
    [ceph4.in][DEBUG ] --> Running transaction check
    [ceph4.in][DEBUG ] ---> Package ceph-release.noarch 0:1-1.el7 will be installed
    [ceph4.in][DEBUG ] --> Finished Dependency Resolution
    [ceph4.in][DEBUG ]
    [ceph4.in][DEBUG ] Dependencies Resolved
    [ceph4.in][DEBUG ]
    [ceph4.in][DEBUG ] ================================================================================
    [ceph4.in][DEBUG ]  Package          Arch       Version     Repository                        Size
    [ceph4.in][DEBUG ] ================================================================================
    [ceph4.in][DEBUG ] Installing:
    [ceph4.in][DEBUG ]  ceph-release     noarch     1-1.el7     /ceph-release-1-0.el7.noarch     535
    [ceph4.in][DEBUG ]
    [ceph4.in][DEBUG ] Transaction Summary
    [ceph4.in][DEBUG ] ================================================================================
    [ceph4.in][DEBUG ] Install  1 Package
    [ceph4.in][DEBUG ]
    [ceph4.in][DEBUG ] Total size: 535
    [ceph4.in][DEBUG ] Installed size: 535
    [ceph4.in][DEBUG ] Downloading packages:
    [ceph4.in][DEBUG ] Running transaction check
    [ceph4.in][DEBUG ] Running transaction test
    [ceph4.in][DEBUG ] Transaction test succeeded
    [ceph4.in][DEBUG ] Running transaction
    [ceph4.in][DEBUG ]   Installing : ceph-release-1-1.el7.noarch                                  1/1
    [ceph4.in][DEBUG ]   Verifying  : ceph-release-1-1.el7.noarch                                  1/1
    [ceph4.in][DEBUG ]
    [ceph4.in][DEBUG ] Installed:
    [ceph4.in][DEBUG ]   ceph-release.noarch 0:1-1.el7
    [ceph4.in][DEBUG ]
    [ceph4.in][DEBUG ] Complete!
    [ceph4.in][WARNIN] ensuring that /etc/yum.repos.d/ceph.repo contains a high priority
    [ceph4.in][WARNIN] altered ceph.repo priorities to contain: priority=1
    [ceph4.in][INFO  ] Running command: sudo yum -y install ceph ceph-radosgw
    [ceph4.in][DEBUG ] Loaded plugins: fastestmirror, priorities
    [ceph4.in][DEBUG ] Loading mirror speeds from cached hostfile
    [ceph4.in][DEBUG ]  * base: centos.mirror.net.in
    [ceph4.in][DEBUG ]  * epel: repo.extreme-ix.org
    [ceph4.in][DEBUG ]  * extras: centos.mirror.net.in
    [ceph4.in][DEBUG ]  * updates: centos.mirror.net.in
    [ceph4.in][DEBUG ] 8 packages excluded due to repository priority protections
    [ceph4.in][DEBUG ] Resolving Dependencies
    [ceph4.in][DEBUG ] --> Running transaction check
    [ceph4.in][DEBUG ] ---> Package ceph.x86_64 2:13.2.10-0.el7 will be installed
    [ceph4.in][DEBUG ] --> Processing Dependency: ceph-mds = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: ceph-osd = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: ceph-mon = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: ceph-mgr = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] ---> Package ceph-radosgw.x86_64 2:13.2.10-0.el7 will be installed
    [ceph4.in][DEBUG ] --> Processing Dependency: ceph-base = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: ceph-selinux = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: librgw2 = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: librados2 = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: mailcap for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: librados.so.2()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: libtcmalloc.so.4()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: libibverbs.so.1()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: liboath.so.0()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: libceph-common.so.0()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Running transaction check
    [ceph4.in][DEBUG ] ---> Package ceph-base.x86_64 2:13.2.10-0.el7 will be installed
    [ceph4.in][DEBUG ] --> Processing Dependency: libcephfs2 = 2:13.2.10-0.el7 for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: librbd1 = 2:13.2.10-0.el7 for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: ceph-common = 2:13.2.10-0.el7 for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: gdisk for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: python-setuptools for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: psmisc for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: cryptsetup for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: python-requests for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: libleveldb.so.1()(64bit) for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: libfuse.so.2()(64bit) for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: liblttng-ust.so.0()(64bit) for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] ---> Package ceph-mds.x86_64 2:13.2.10-0.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package ceph-mgr.x86_64 2:13.2.10-0.el7 will be installed
    [ceph4.in][DEBUG ] --> Processing Dependency: python-cherrypy for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: python-werkzeug for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: python-six for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: python-routes for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: python-bcrypt for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: python-pecan for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: pyOpenSSL for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: python-jinja2 for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] ---> Package ceph-mon.x86_64 2:13.2.10-0.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package ceph-osd.x86_64 2:13.2.10-0.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package ceph-selinux.x86_64 2:13.2.10-0.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package gperftools-libs.x86_64 0:2.6.1-1.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package libibverbs.x86_64 0:22.4-6.el7_9 will be installed
    [ceph4.in][DEBUG ] --> Processing Dependency: rdma-core(x86-64) = 22.4-6.el7_9 for package: libibverbs-22.4-6.el7_9.x86_64
    [ceph4.in][DEBUG ] ---> Package liboath.x86_64 0:2.6.2-1.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package librados2.x86_64 2:13.2.10-0.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package librgw2.x86_64 2:13.2.10-0.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package mailcap.noarch 0:2.1.41-2.el7 will be installed
    [ceph4.in][DEBUG ] --> Running transaction check
    [ceph4.in][DEBUG ] ---> Package ceph-common.x86_64 2:13.2.10-0.el7 will be installed
    [ceph4.in][DEBUG ] --> Processing Dependency: python-cephfs = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: libradosstriper1 = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: python-rgw = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: python-rbd = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: python-rados = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: python-ceph-argparse = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: python-prettytable for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: libbabeltrace-ctf.so.1()(64bit) for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: libbabeltrace.so.1()(64bit) for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: libradosstriper.so.1()(64bit) for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph4.in][DEBUG ] ---> Package cryptsetup.x86_64 0:2.0.3-6.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package fuse-libs.x86_64 0:2.9.2-11.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package gdisk.x86_64 0:0.8.10-3.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package leveldb.x86_64 0:1.12.0-11.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package libcephfs2.x86_64 2:13.2.10-0.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package librbd1.x86_64 2:13.2.10-0.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package lttng-ust.x86_64 0:2.4.1-4.el7 will be installed
    [ceph4.in][DEBUG ] --> Processing Dependency: liburcu-bp.so.1()(64bit) for package: lttng-ust-2.4.1-4.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: liburcu-cds.so.1()(64bit) for package: lttng-ust-2.4.1-4.el7.x86_64
    [ceph4.in][DEBUG ] ---> Package psmisc.x86_64 0:22.20-17.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package pyOpenSSL.x86_64 0:0.13.1-4.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package python-cherrypy.noarch 0:3.2.2-4.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package python-jinja2.noarch 0:2.7.2-4.el7 will be installed
    [ceph4.in][DEBUG ] --> Processing Dependency: python-babel >= 0.8 for package: python-jinja2-2.7.2-4.el7.noarch
    [ceph4.in][DEBUG ] --> Processing Dependency: python-markupsafe for package: python-jinja2-2.7.2-4.el7.noarch
    [ceph4.in][DEBUG ] ---> Package python-pecan.noarch 0:0.4.5-2.el7 will be installed
    [ceph4.in][DEBUG ] --> Processing Dependency: python-mako >= 0.4.0 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph4.in][DEBUG ] --> Processing Dependency: python-simplegeneric >= 0.8 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph4.in][DEBUG ] --> Processing Dependency: python-webob >= 1.2 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph4.in][DEBUG ] --> Processing Dependency: python-webtest >= 1.3.1 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph4.in][DEBUG ] --> Processing Dependency: python-singledispatch for package: python-pecan-0.4.5-2.el7.noarch
    [ceph4.in][DEBUG ] ---> Package python-requests.noarch 0:2.6.0-10.el7 will be installed
    [ceph4.in][DEBUG ] --> Processing Dependency: python-urllib3 >= 1.10.2-1 for package: python-requests-2.6.0-10.el7.noarch
    [ceph4.in][DEBUG ] --> Processing Dependency: python-chardet >= 2.2.1-1 for package: python-requests-2.6.0-10.el7.noarch
    [ceph4.in][DEBUG ] ---> Package python-routes.noarch 0:1.13-2.el7 will be installed
    [ceph4.in][DEBUG ] --> Processing Dependency: python-repoze-lru for package: python-routes-1.13-2.el7.noarch
    [ceph4.in][DEBUG ] ---> Package python-setuptools.noarch 0:0.9.8-7.el7 will be installed
    [ceph4.in][DEBUG ] --> Processing Dependency: python-backports-ssl_match_hostname for package: python-setuptools-0.9.8-7.el7.noarch
    [ceph4.in][DEBUG ] ---> Package python-six.noarch 0:1.9.0-2.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package python-werkzeug.noarch 0:0.9.1-2.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package python2-bcrypt.x86_64 0:3.1.6-2.el7 will be installed
    [ceph4.in][DEBUG ] --> Processing Dependency: python-cffi for package: python2-bcrypt-3.1.6-2.el7.x86_64
    [ceph4.in][DEBUG ] --> Processing Dependency: python2-six for package: python2-bcrypt-3.1.6-2.el7.x86_64
    [ceph4.in][DEBUG ] ---> Package rdma-core.x86_64 0:22.4-6.el7_9 will be installed
    [ceph4.in][DEBUG ] --> Processing Dependency: pciutils for package: rdma-core-22.4-6.el7_9.x86_64
    [ceph4.in][DEBUG ] --> Running transaction check
    [ceph4.in][DEBUG ] ---> Package libbabeltrace.x86_64 0:1.2.4-3.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package libradosstriper1.x86_64 2:13.2.10-0.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package pciutils.x86_64 0:3.5.1-3.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package python-babel.noarch 0:0.9.6-8.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package python-backports-ssl_match_hostname.noarch 0:3.5.0.1-1.el7 will be installed
    [ceph4.in][DEBUG ] --> Processing Dependency: python-ipaddress for package: python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch
    [ceph4.in][DEBUG ] --> Processing Dependency: python-backports for package: python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch
    [ceph4.in][DEBUG ] ---> Package python-ceph-argparse.x86_64 2:13.2.10-0.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package python-cephfs.x86_64 2:13.2.10-0.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package python-cffi.x86_64 0:1.6.0-5.el7 will be installed
    [ceph4.in][DEBUG ] --> Processing Dependency: python-pycparser for package: python-cffi-1.6.0-5.el7.x86_64
    [ceph4.in][DEBUG ] ---> Package python-chardet.noarch 0:2.2.1-3.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package python-mako.noarch 0:0.8.1-2.el7 will be installed
    [ceph4.in][DEBUG ] --> Processing Dependency: python-beaker for package: python-mako-0.8.1-2.el7.noarch
    [ceph4.in][DEBUG ] ---> Package python-markupsafe.x86_64 0:0.11-10.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package python-prettytable.noarch 0:0.7.2-3.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package python-rados.x86_64 2:13.2.10-0.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package python-rbd.x86_64 2:13.2.10-0.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package python-repoze-lru.noarch 0:0.4-3.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package python-rgw.x86_64 2:13.2.10-0.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package python-simplegeneric.noarch 0:0.8-7.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package python-singledispatch.noarch 0:3.4.0.2-2.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package python-urllib3.noarch 0:1.10.2-7.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package python-webob.noarch 0:1.2.3-7.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package python-webtest.noarch 0:1.3.4-6.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package python2-six.noarch 0:1.9.0-0.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package userspace-rcu.x86_64 0:0.7.16-1.el7 will be installed
    [ceph4.in][DEBUG ] --> Running transaction check
    [ceph4.in][DEBUG ] ---> Package python-backports.x86_64 0:1.0-8.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package python-beaker.noarch 0:1.5.4-10.el7 will be installed
    [ceph4.in][DEBUG ] --> Processing Dependency: python-paste for package: python-beaker-1.5.4-10.el7.noarch
    [ceph4.in][DEBUG ] ---> Package python-ipaddress.noarch 0:1.0.16-2.el7 will be installed
    [ceph4.in][DEBUG ] ---> Package python-pycparser.noarch 0:2.14-1.el7 will be installed
    [ceph4.in][DEBUG ] --> Processing Dependency: python-ply for package: python-pycparser-2.14-1.el7.noarch
    [ceph4.in][DEBUG ] --> Running transaction check
    [ceph4.in][DEBUG ] ---> Package python-paste.noarch 0:1.7.5.1-9.20111221hg1498.el7 will be installed
    [ceph4.in][DEBUG ] --> Processing Dependency: python-tempita for package: python-paste-1.7.5.1-9.20111221hg1498.el7.noarch
    [ceph4.in][DEBUG ] ---> Package python-ply.noarch 0:3.4-11.el7 will be installed
    [ceph4.in][DEBUG ] --> Running transaction check
    [ceph4.in][DEBUG ] ---> Package python-tempita.noarch 0:0.5.1-6.el7 will be installed
    [ceph4.in][DEBUG ] --> Finished Dependency Resolution
    [ceph4.in][DEBUG ]
    [ceph4.in][DEBUG ] Dependencies Resolved
    [ceph4.in][DEBUG ]
    [ceph4.in][DEBUG ] ================================================================================
    [ceph4.in][DEBUG ]  Package                      Arch   Version                      Repository
    [ceph4.in][DEBUG ]                                                                            Size
    [ceph4.in][DEBUG ] ================================================================================
    [ceph4.in][DEBUG ] Installing:
    [ceph4.in][DEBUG ]  ceph                         x86_64 2:13.2.10-0.el7              Ceph    3.0 k
    [ceph4.in][DEBUG ]  ceph-radosgw                 x86_64 2:13.2.10-0.el7              Ceph    4.5 M
    [ceph4.in][DEBUG ] Installing for dependencies:
    [ceph4.in][DEBUG ]  ceph-base                    x86_64 2:13.2.10-0.el7              Ceph    4.8 M
    [ceph4.in][DEBUG ]  ceph-common                  x86_64 2:13.2.10-0.el7              Ceph     14 M
    [ceph4.in][DEBUG ]  ceph-mds                     x86_64 2:13.2.10-0.el7              Ceph    1.7 M
    [ceph4.in][DEBUG ]  ceph-mgr                     x86_64 2:13.2.10-0.el7              Ceph    3.5 M
    [ceph4.in][DEBUG ]  ceph-mon                     x86_64 2:13.2.10-0.el7              Ceph    3.9 M
    [ceph4.in][DEBUG ]  ceph-osd                     x86_64 2:13.2.10-0.el7              Ceph     13 M
    [ceph4.in][DEBUG ]  ceph-selinux                 x86_64 2:13.2.10-0.el7              Ceph     21 k
    [ceph4.in][DEBUG ]  cryptsetup                   x86_64 2.0.3-6.el7                  base    154 k
    [ceph4.in][DEBUG ]  fuse-libs                    x86_64 2.9.2-11.el7                 base     93 k
    [ceph4.in][DEBUG ]  gdisk                        x86_64 0.8.10-3.el7                 base    190 k
    [ceph4.in][DEBUG ]  gperftools-libs              x86_64 2.6.1-1.el7                  base    272 k
    [ceph4.in][DEBUG ]  leveldb                      x86_64 1.12.0-11.el7                epel    161 k
    [ceph4.in][DEBUG ]  libbabeltrace                x86_64 1.2.4-3.el7                  epel    147 k
    [ceph4.in][DEBUG ]  libcephfs2                   x86_64 2:13.2.10-0.el7              Ceph    434 k
    [ceph4.in][DEBUG ]  libibverbs                   x86_64 22.4-6.el7_9                 updates 269 k
    [ceph4.in][DEBUG ]  liboath                      x86_64 2.6.2-1.el7                  epel     51 k
    [ceph4.in][DEBUG ]  librados2                    x86_64 2:13.2.10-0.el7              Ceph    2.9 M
    [ceph4.in][DEBUG ]  libradosstriper1             x86_64 2:13.2.10-0.el7              Ceph    329 k
    [ceph4.in][DEBUG ]  librbd1                      x86_64 2:13.2.10-0.el7              Ceph    1.2 M
    [ceph4.in][DEBUG ]  librgw2                      x86_64 2:13.2.10-0.el7              Ceph    2.0 M
    [ceph4.in][DEBUG ]  lttng-ust                    x86_64 2.4.1-4.el7                  epel    176 k
    [ceph4.in][DEBUG ]  mailcap                      noarch 2.1.41-2.el7                 base     31 k
    [ceph4.in][DEBUG ]  pciutils                     x86_64 3.5.1-3.el7                  base     93 k
    [ceph4.in][DEBUG ]  psmisc                       x86_64 22.20-17.el7                 base    141 k
    [ceph4.in][DEBUG ]  pyOpenSSL                    x86_64 0.13.1-4.el7                 base    135 k
    [ceph4.in][DEBUG ]  python-babel                 noarch 0.9.6-8.el7                  base    1.4 M
    [ceph4.in][DEBUG ]  python-backports             x86_64 1.0-8.el7                    base    5.8 k
    [ceph4.in][DEBUG ]  python-backports-ssl_match_hostname
    [ceph4.in][DEBUG ]                               noarch 3.5.0.1-1.el7                base     13 k
    [ceph4.in][DEBUG ]  python-beaker                noarch 1.5.4-10.el7                 base     80 k
    [ceph4.in][DEBUG ]  python-ceph-argparse         x86_64 2:13.2.10-0.el7              Ceph     34 k
    [ceph4.in][DEBUG ]  python-cephfs                x86_64 2:13.2.10-0.el7              Ceph     87 k
    [ceph4.in][DEBUG ]  python-cffi                  x86_64 1.6.0-5.el7                  base    218 k
    [ceph4.in][DEBUG ]  python-chardet               noarch 2.2.1-3.el7                  base    227 k
    [ceph4.in][DEBUG ]  python-cherrypy              noarch 3.2.2-4.el7                  base    422 k
    [ceph4.in][DEBUG ]  python-ipaddress             noarch 1.0.16-2.el7                 base     34 k
    [ceph4.in][DEBUG ]  python-jinja2                noarch 2.7.2-4.el7                  base    519 k
    [ceph4.in][DEBUG ]  python-mako                  noarch 0.8.1-2.el7                  base    307 k
    [ceph4.in][DEBUG ]  python-markupsafe            x86_64 0.11-10.el7                  base     25 k
    [ceph4.in][DEBUG ]  python-paste                 noarch 1.7.5.1-9.20111221hg1498.el7 base    866 k
    [ceph4.in][DEBUG ]  python-pecan                 noarch 0.4.5-2.el7                  epel    255 k
    [ceph4.in][DEBUG ]  python-ply                   noarch 3.4-11.el7                   base    123 k
    [ceph4.in][DEBUG ]  python-prettytable           noarch 0.7.2-3.el7                  base     37 k
    [ceph4.in][DEBUG ]  python-pycparser             noarch 2.14-1.el7                   base    104 k
    [ceph4.in][DEBUG ]  python-rados                 x86_64 2:13.2.10-0.el7              Ceph    189 k
    [ceph4.in][DEBUG ]  python-rbd                   x86_64 2:13.2.10-0.el7              Ceph    132 k
    [ceph4.in][DEBUG ]  python-repoze-lru            noarch 0.4-3.el7                    epel     13 k
    [ceph4.in][DEBUG ]  python-requests              noarch 2.6.0-10.el7                 base     95 k
    [ceph4.in][DEBUG ]  python-rgw                   x86_64 2:13.2.10-0.el7              Ceph     76 k
    [ceph4.in][DEBUG ]  python-routes                noarch 1.13-2.el7                   epel    640 k
    [ceph4.in][DEBUG ]  python-setuptools            noarch 0.9.8-7.el7                  base    397 k
    [ceph4.in][DEBUG ]  python-simplegeneric         noarch 0.8-7.el7                    epel     12 k
    [ceph4.in][DEBUG ]  python-singledispatch        noarch 3.4.0.2-2.el7                epel     18 k
    [ceph4.in][DEBUG ]  python-six                   noarch 1.9.0-2.el7                  base     29 k
    [ceph4.in][DEBUG ]  python-tempita               noarch 0.5.1-6.el7                  base     33 k
    [ceph4.in][DEBUG ]  python-urllib3               noarch 1.10.2-7.el7                 base    103 k
    [ceph4.in][DEBUG ]  python-webob                 noarch 1.2.3-7.el7                  base    202 k
    [ceph4.in][DEBUG ]  python-webtest               noarch 1.3.4-6.el7                  base    102 k
    [ceph4.in][DEBUG ]  python-werkzeug              noarch 0.9.1-2.el7                  extras  562 k
    [ceph4.in][DEBUG ]  python2-bcrypt               x86_64 3.1.6-2.el7                  epel     39 k
    [ceph4.in][DEBUG ]  python2-six                  noarch 1.9.0-0.el7                  epel    2.9 k
    [ceph4.in][DEBUG ]  rdma-core                    x86_64 22.4-6.el7_9                 updates  51 k
    [ceph4.in][DEBUG ]  userspace-rcu                x86_64 0.7.16-1.el7                 epel     73 k
    [ceph4.in][DEBUG ]
    [ceph4.in][DEBUG ] Transaction Summary
    [ceph4.in][DEBUG ] ================================================================================
    [ceph4.in][DEBUG ] Install  2 Packages (+62 Dependent packages)
    [ceph4.in][DEBUG ]
    [ceph4.in][DEBUG ] Total download size: 61 M
    [ceph4.in][DEBUG ] Installed size: 210 M
    [ceph4.in][DEBUG ] Downloading packages:
    [ceph4.in][DEBUG ] Public key for leveldb-1.12.0-11.el7.x86_64.rpm is not installed
    [ceph4.in][WARNIN] warning: /var/cache/yum/x86_64/7/epel/packages/leveldb-1.12.0-11.el7.x86_64.rpm: Header V3 RSA/SHA256 Signature, key ID 352c64e5: NOKEY
    [ceph4.in][DEBUG ] --------------------------------------------------------------------------------
    [ceph4.in][DEBUG ] Total                                              5.4 MB/s |  61 MB  00:11
    [ceph4.in][DEBUG ] Retrieving key from file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
    [ceph4.in][WARNIN] Importing GPG key 0x352C64E5:
    [ceph4.in][WARNIN]  Userid     : "Fedora EPEL (7) <epel@fedoraproject.org>"
    [ceph4.in][WARNIN]  Fingerprint: 91e9 7d7c 4a5e 96f1 7f3e 888f 6a2f aea2 352c 64e5
    [ceph4.in][WARNIN]  Package    : epel-release-7-14.noarch (@/epel-release-latest-7.noarch)
    [ceph4.in][WARNIN]  From       : /etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
    [ceph4.in][DEBUG ] Running transaction check
    [ceph4.in][DEBUG ] Running transaction test
    [ceph4.in][DEBUG ] Transaction test succeeded
    [ceph4.in][DEBUG ] Running transaction
    [ceph4.in][DEBUG ]   Installing : gperftools-libs-2.6.1-1.el7.x86_64                          1/64
    [ceph4.in][DEBUG ]   Installing : leveldb-1.12.0-11.el7.x86_64                                2/64
    [ceph4.in][DEBUG ]   Installing : python-six-1.9.0-2.el7.noarch                               3/64
    [ceph4.in][DEBUG ]   Installing : fuse-libs-2.9.2-11.el7.x86_64                               4/64
    [ceph4.in][DEBUG ]   Installing : liboath-2.6.2-1.el7.x86_64                                  5/64
    [ceph4.in][DEBUG ]   Installing : python-ipaddress-1.0.16-2.el7.noarch                        6/64
    [ceph4.in][DEBUG ]   Installing : python-webob-1.2.3-7.el7.noarch                             7/64
    [ceph4.in][DEBUG ]   Installing : python-markupsafe-0.11-10.el7.x86_64                        8/64
    [ceph4.in][DEBUG ]   Installing : pyOpenSSL-0.13.1-4.el7.x86_64                               9/64
    [ceph4.in][DEBUG ]   Installing : 2:python-ceph-argparse-13.2.10-0.el7.x86_64                10/64
    [ceph4.in][DEBUG ]   Installing : python-webtest-1.3.4-6.el7.noarch                          11/64
    [ceph4.in][DEBUG ]   Installing : python2-six-1.9.0-0.el7.noarch                             12/64
    [ceph4.in][DEBUG ]   Installing : python-singledispatch-3.4.0.2-2.el7.noarch                 13/64
    [ceph4.in][DEBUG ]   Installing : psmisc-22.20-17.el7.x86_64                                 14/64
    [ceph4.in][DEBUG ]   Installing : pciutils-3.5.1-3.el7.x86_64                                15/64
    [ceph4.in][DEBUG ]   Installing : rdma-core-22.4-6.el7_9.x86_64                              16/64
    [ceph4.in][DEBUG ]   Installing : libibverbs-22.4-6.el7_9.x86_64                             17/64
    [ceph4.in][DEBUG ]   Installing : gdisk-0.8.10-3.el7.x86_64                                  18/64
    [ceph4.in][DEBUG ]   Installing : python-simplegeneric-0.8-7.el7.noarch                      19/64
    [ceph4.in][DEBUG ]   Installing : python-tempita-0.5.1-6.el7.noarch                          20/64
    [ceph4.in][DEBUG ]   Installing : python-cherrypy-3.2.2-4.el7.noarch                         21/64
    [ceph4.in][DEBUG ]   Installing : python-prettytable-0.7.2-3.el7.noarch                      22/64
    [ceph4.in][DEBUG ]   Installing : python-werkzeug-0.9.1-2.el7.noarch                         23/64
    [ceph4.in][DEBUG ]   Installing : python-repoze-lru-0.4-3.el7.noarch                         24/64
    [ceph4.in][DEBUG ]   Installing : python-routes-1.13-2.el7.noarch                            25/64
    [ceph4.in][DEBUG ]   Installing : python-backports-1.0-8.el7.x86_64                          26/64
    [ceph4.in][DEBUG ]   Installing : python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch   27/64
    [ceph4.in][DEBUG ]   Installing : python-setuptools-0.9.8-7.el7.noarch                       28/64
    [ceph4.in][DEBUG ]   Installing : python-paste-1.7.5.1-9.20111221hg1498.el7.noarch           29/64
    [ceph4.in][DEBUG ]   Installing : python-beaker-1.5.4-10.el7.noarch                          30/64
    [ceph4.in][DEBUG ]   Installing : python-mako-0.8.1-2.el7.noarch                             31/64
    [ceph4.in][DEBUG ]   Installing : python-pecan-0.4.5-2.el7.noarch                            32/64
    [ceph4.in][DEBUG ]   Installing : python-urllib3-1.10.2-7.el7.noarch                         33/64
    [ceph4.in][DEBUG ]   Installing : python-babel-0.9.6-8.el7.noarch                            34/64
    [ceph4.in][DEBUG ]   Installing : python-jinja2-2.7.2-4.el7.noarch                           35/64
    [ceph4.in][DEBUG ]   Installing : python-chardet-2.2.1-3.el7.noarch                          36/64
    [ceph4.in][DEBUG ]   Installing : python-requests-2.6.0-10.el7.noarch                        37/64
    [ceph4.in][DEBUG ]   Installing : cryptsetup-2.0.3-6.el7.x86_64                              38/64
    [ceph4.in][DEBUG ]   Installing : libbabeltrace-1.2.4-3.el7.x86_64                           39/64
    [ceph4.in][DEBUG ]   Installing : userspace-rcu-0.7.16-1.el7.x86_64                          40/64
    [ceph4.in][DEBUG ]   Installing : lttng-ust-2.4.1-4.el7.x86_64                               41/64
    [ceph4.in][DEBUG ]   Installing : 2:librados2-13.2.10-0.el7.x86_64                           42/64
    [ceph4.in][DEBUG ]   Installing : 2:python-rados-13.2.10-0.el7.x86_64                        43/64
    [ceph4.in][DEBUG ]   Installing : 2:librbd1-13.2.10-0.el7.x86_64                             44/64
    [ceph4.in][DEBUG ]   Installing : 2:libcephfs2-13.2.10-0.el7.x86_64                          45/64
    [ceph4.in][DEBUG ]   Installing : 2:librgw2-13.2.10-0.el7.x86_64                             46/64
    [ceph4.in][DEBUG ]   Installing : 2:python-rgw-13.2.10-0.el7.x86_64                          47/64
    [ceph4.in][DEBUG ]   Installing : 2:python-cephfs-13.2.10-0.el7.x86_64                       48/64
    [ceph4.in][DEBUG ]   Installing : 2:python-rbd-13.2.10-0.el7.x86_64                          49/64
    [ceph4.in][DEBUG ]   Installing : 2:libradosstriper1-13.2.10-0.el7.x86_64                    50/64
    [ceph4.in][DEBUG ]   Installing : 2:ceph-common-13.2.10-0.el7.x86_64                         51/64
    [ceph4.in][DEBUG ]   Installing : 2:ceph-base-13.2.10-0.el7.x86_64                           52/64
    [ceph4.in][DEBUG ]   Installing : 2:ceph-selinux-13.2.10-0.el7.x86_64                        53/64
    [ceph4.in][DEBUG ]   Installing : 2:ceph-osd-13.2.10-0.el7.x86_64                            54/64
    [ceph4.in][DEBUG ]   Installing : 2:ceph-mds-13.2.10-0.el7.x86_64                            55/64
    [ceph4.in][DEBUG ]   Installing : 2:ceph-mon-13.2.10-0.el7.x86_64                            56/64
    [ceph4.in][DEBUG ]   Installing : python-ply-3.4-11.el7.noarch                               57/64
    [ceph4.in][DEBUG ]   Installing : python-pycparser-2.14-1.el7.noarch                         58/64
    [ceph4.in][DEBUG ]   Installing : python-cffi-1.6.0-5.el7.x86_64                             59/64
    [ceph4.in][DEBUG ]   Installing : python2-bcrypt-3.1.6-2.el7.x86_64                          60/64
    [ceph4.in][DEBUG ]   Installing : 2:ceph-mgr-13.2.10-0.el7.x86_64                            61/64
    [ceph4.in][DEBUG ]   Installing : mailcap-2.1.41-2.el7.noarch                                62/64
    [ceph4.in][DEBUG ]   Installing : 2:ceph-radosgw-13.2.10-0.el7.x86_64                        63/64
    [ceph4.in][DEBUG ]   Installing : 2:ceph-13.2.10-0.el7.x86_64                                64/64
    [ceph4.in][DEBUG ]   Verifying  : liboath-2.6.2-1.el7.x86_64                                  1/64
    [ceph4.in][DEBUG ]   Verifying  : python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch    2/64
    [ceph4.in][DEBUG ]   Verifying  : 2:librbd1-13.2.10-0.el7.x86_64                              3/64
    [ceph4.in][DEBUG ]   Verifying  : 2:python-ceph-argparse-13.2.10-0.el7.x86_64                 4/64
    [ceph4.in][DEBUG ]   Verifying  : mailcap-2.1.41-2.el7.noarch                                 5/64
    [ceph4.in][DEBUG ]   Verifying  : pyOpenSSL-0.13.1-4.el7.x86_64                               6/64
    [ceph4.in][DEBUG ]   Verifying  : python2-bcrypt-3.1.6-2.el7.x86_64                           7/64
    [ceph4.in][DEBUG ]   Verifying  : python-ply-3.4-11.el7.noarch                                8/64
    [ceph4.in][DEBUG ]   Verifying  : userspace-rcu-0.7.16-1.el7.x86_64                           9/64
    [ceph4.in][DEBUG ]   Verifying  : libibverbs-22.4-6.el7_9.x86_64                             10/64
    [ceph4.in][DEBUG ]   Verifying  : rdma-core-22.4-6.el7_9.x86_64                              11/64
    [ceph4.in][DEBUG ]   Verifying  : fuse-libs-2.9.2-11.el7.x86_64                              12/64
    [ceph4.in][DEBUG ]   Verifying  : python-setuptools-0.9.8-7.el7.noarch                       13/64
    [ceph4.in][DEBUG ]   Verifying  : python-routes-1.13-2.el7.noarch                            14/64
    [ceph4.in][DEBUG ]   Verifying  : 2:libcephfs2-13.2.10-0.el7.x86_64                          15/64
    [ceph4.in][DEBUG ]   Verifying  : python-urllib3-1.10.2-7.el7.noarch                         16/64
    [ceph4.in][DEBUG ]   Verifying  : libbabeltrace-1.2.4-3.el7.x86_64                           17/64
    [ceph4.in][DEBUG ]   Verifying  : python-mako-0.8.1-2.el7.noarch                             18/64
    [ceph4.in][DEBUG ]   Verifying  : python2-six-1.9.0-0.el7.noarch                             19/64
    [ceph4.in][DEBUG ]   Verifying  : 2:ceph-mgr-13.2.10-0.el7.x86_64                            20/64
    [ceph4.in][DEBUG ]   Verifying  : 2:ceph-base-13.2.10-0.el7.x86_64                           21/64
    [ceph4.in][DEBUG ]   Verifying  : python-jinja2-2.7.2-4.el7.noarch                           22/64
    [ceph4.in][DEBUG ]   Verifying  : python-pecan-0.4.5-2.el7.noarch                            23/64
    [ceph4.in][DEBUG ]   Verifying  : python-six-1.9.0-2.el7.noarch                              24/64
    [ceph4.in][DEBUG ]   Verifying  : cryptsetup-2.0.3-6.el7.x86_64                              25/64
    [ceph4.in][DEBUG ]   Verifying  : leveldb-1.12.0-11.el7.x86_64                               26/64
    [ceph4.in][DEBUG ]   Verifying  : python-singledispatch-3.4.0.2-2.el7.noarch                 27/64
    [ceph4.in][DEBUG ]   Verifying  : python-markupsafe-0.11-10.el7.x86_64                       28/64
    [ceph4.in][DEBUG ]   Verifying  : 2:python-rados-13.2.10-0.el7.x86_64                        29/64
    [ceph4.in][DEBUG ]   Verifying  : 2:python-rgw-13.2.10-0.el7.x86_64                          30/64
    [ceph4.in][DEBUG ]   Verifying  : 2:ceph-radosgw-13.2.10-0.el7.x86_64                        31/64
    [ceph4.in][DEBUG ]   Verifying  : python-chardet-2.2.1-3.el7.noarch                          32/64
    [ceph4.in][DEBUG ]   Verifying  : python-babel-0.9.6-8.el7.noarch                            33/64
    [ceph4.in][DEBUG ]   Verifying  : 2:librados2-13.2.10-0.el7.x86_64                           34/64
    [ceph4.in][DEBUG ]   Verifying  : python-paste-1.7.5.1-9.20111221hg1498.el7.noarch           35/64
    [ceph4.in][DEBUG ]   Verifying  : 2:ceph-osd-13.2.10-0.el7.x86_64                            36/64
    [ceph4.in][DEBUG ]   Verifying  : python-backports-1.0-8.el7.x86_64                          37/64
    [ceph4.in][DEBUG ]   Verifying  : lttng-ust-2.4.1-4.el7.x86_64                               38/64
    [ceph4.in][DEBUG ]   Verifying  : python-webob-1.2.3-7.el7.noarch                            39/64
    [ceph4.in][DEBUG ]   Verifying  : 2:ceph-common-13.2.10-0.el7.x86_64                         40/64
    [ceph4.in][DEBUG ]   Verifying  : python-repoze-lru-0.4-3.el7.noarch                         41/64
    [ceph4.in][DEBUG ]   Verifying  : python-werkzeug-0.9.1-2.el7.noarch                         42/64
    [ceph4.in][DEBUG ]   Verifying  : python-beaker-1.5.4-10.el7.noarch                          43/64
    [ceph4.in][DEBUG ]   Verifying  : python-cffi-1.6.0-5.el7.x86_64                             44/64
    [ceph4.in][DEBUG ]   Verifying  : 2:ceph-selinux-13.2.10-0.el7.x86_64                        45/64
    [ceph4.in][DEBUG ]   Verifying  : python-requests-2.6.0-10.el7.noarch                        46/64
    [ceph4.in][DEBUG ]   Verifying  : python-pycparser-2.14-1.el7.noarch                         47/64
    [ceph4.in][DEBUG ]   Verifying  : python-prettytable-0.7.2-3.el7.noarch                      48/64
    [ceph4.in][DEBUG ]   Verifying  : 2:librgw2-13.2.10-0.el7.x86_64                             49/64
    [ceph4.in][DEBUG ]   Verifying  : 2:ceph-mds-13.2.10-0.el7.x86_64                            50/64
    [ceph4.in][DEBUG ]   Verifying  : python-cherrypy-3.2.2-4.el7.noarch                         51/64
    [ceph4.in][DEBUG ]   Verifying  : 2:python-cephfs-13.2.10-0.el7.x86_64                       52/64
    [ceph4.in][DEBUG ]   Verifying  : python-tempita-0.5.1-6.el7.noarch                          53/64
    [ceph4.in][DEBUG ]   Verifying  : 2:python-rbd-13.2.10-0.el7.x86_64                          54/64
    [ceph4.in][DEBUG ]   Verifying  : 2:ceph-mon-13.2.10-0.el7.x86_64                            55/64
    [ceph4.in][DEBUG ]   Verifying  : gperftools-libs-2.6.1-1.el7.x86_64                         56/64
    [ceph4.in][DEBUG ]   Verifying  : python-ipaddress-1.0.16-2.el7.noarch                       57/64
    [ceph4.in][DEBUG ]   Verifying  : python-webtest-1.3.4-6.el7.noarch                          58/64
    [ceph4.in][DEBUG ]   Verifying  : 2:ceph-13.2.10-0.el7.x86_64                                59/64
    [ceph4.in][DEBUG ]   Verifying  : python-simplegeneric-0.8-7.el7.noarch                      60/64
    [ceph4.in][DEBUG ]   Verifying  : gdisk-0.8.10-3.el7.x86_64                                  61/64
    [ceph4.in][DEBUG ]   Verifying  : 2:libradosstriper1-13.2.10-0.el7.x86_64                    62/64
    [ceph4.in][DEBUG ]   Verifying  : pciutils-3.5.1-3.el7.x86_64                                63/64
    [ceph4.in][DEBUG ]   Verifying  : psmisc-22.20-17.el7.x86_64                                 64/64
    [ceph4.in][DEBUG ]
    [ceph4.in][DEBUG ] Installed:
    [ceph4.in][DEBUG ]   ceph.x86_64 2:13.2.10-0.el7        ceph-radosgw.x86_64 2:13.2.10-0.el7
    [ceph4.in][DEBUG ]
    [ceph4.in][DEBUG ] Dependency Installed:
    [ceph4.in][DEBUG ]   ceph-base.x86_64 2:13.2.10-0.el7
    [ceph4.in][DEBUG ]   ceph-common.x86_64 2:13.2.10-0.el7
    [ceph4.in][DEBUG ]   ceph-mds.x86_64 2:13.2.10-0.el7
    [ceph4.in][DEBUG ]   ceph-mgr.x86_64 2:13.2.10-0.el7
    [ceph4.in][DEBUG ]   ceph-mon.x86_64 2:13.2.10-0.el7
    [ceph4.in][DEBUG ]   ceph-osd.x86_64 2:13.2.10-0.el7
    [ceph4.in][DEBUG ]   ceph-selinux.x86_64 2:13.2.10-0.el7
    [ceph4.in][DEBUG ]   cryptsetup.x86_64 0:2.0.3-6.el7
    [ceph4.in][DEBUG ]   fuse-libs.x86_64 0:2.9.2-11.el7
    [ceph4.in][DEBUG ]   gdisk.x86_64 0:0.8.10-3.el7
    [ceph4.in][DEBUG ]   gperftools-libs.x86_64 0:2.6.1-1.el7
    [ceph4.in][DEBUG ]   leveldb.x86_64 0:1.12.0-11.el7
    [ceph4.in][DEBUG ]   libbabeltrace.x86_64 0:1.2.4-3.el7
    [ceph4.in][DEBUG ]   libcephfs2.x86_64 2:13.2.10-0.el7
    [ceph4.in][DEBUG ]   libibverbs.x86_64 0:22.4-6.el7_9
    [ceph4.in][DEBUG ]   liboath.x86_64 0:2.6.2-1.el7
    [ceph4.in][DEBUG ]   librados2.x86_64 2:13.2.10-0.el7
    [ceph4.in][DEBUG ]   libradosstriper1.x86_64 2:13.2.10-0.el7
    [ceph4.in][DEBUG ]   librbd1.x86_64 2:13.2.10-0.el7
    [ceph4.in][DEBUG ]   librgw2.x86_64 2:13.2.10-0.el7
    [ceph4.in][DEBUG ]   lttng-ust.x86_64 0:2.4.1-4.el7
    [ceph4.in][DEBUG ]   mailcap.noarch 0:2.1.41-2.el7
    [ceph4.in][DEBUG ]   pciutils.x86_64 0:3.5.1-3.el7
    [ceph4.in][DEBUG ]   psmisc.x86_64 0:22.20-17.el7
    [ceph4.in][DEBUG ]   pyOpenSSL.x86_64 0:0.13.1-4.el7
    [ceph4.in][DEBUG ]   python-babel.noarch 0:0.9.6-8.el7
    [ceph4.in][DEBUG ]   python-backports.x86_64 0:1.0-8.el7
    [ceph4.in][DEBUG ]   python-backports-ssl_match_hostname.noarch 0:3.5.0.1-1.el7
    [ceph4.in][DEBUG ]   python-beaker.noarch 0:1.5.4-10.el7
    [ceph4.in][DEBUG ]   python-ceph-argparse.x86_64 2:13.2.10-0.el7
    [ceph4.in][DEBUG ]   python-cephfs.x86_64 2:13.2.10-0.el7
    [ceph4.in][DEBUG ]   python-cffi.x86_64 0:1.6.0-5.el7
    [ceph4.in][DEBUG ]   python-chardet.noarch 0:2.2.1-3.el7
    [ceph4.in][DEBUG ]   python-cherrypy.noarch 0:3.2.2-4.el7
    [ceph4.in][DEBUG ]   python-ipaddress.noarch 0:1.0.16-2.el7
    [ceph4.in][DEBUG ]   python-jinja2.noarch 0:2.7.2-4.el7
    [ceph4.in][DEBUG ]   python-mako.noarch 0:0.8.1-2.el7
    [ceph4.in][DEBUG ]   python-markupsafe.x86_64 0:0.11-10.el7
    [ceph4.in][DEBUG ]   python-paste.noarch 0:1.7.5.1-9.20111221hg1498.el7
    [ceph4.in][DEBUG ]   python-pecan.noarch 0:0.4.5-2.el7
    [ceph4.in][DEBUG ]   python-ply.noarch 0:3.4-11.el7
    [ceph4.in][DEBUG ]   python-prettytable.noarch 0:0.7.2-3.el7
    [ceph4.in][DEBUG ]   python-pycparser.noarch 0:2.14-1.el7
    [ceph4.in][DEBUG ]   python-rados.x86_64 2:13.2.10-0.el7
    [ceph4.in][DEBUG ]   python-rbd.x86_64 2:13.2.10-0.el7
    [ceph4.in][DEBUG ]   python-repoze-lru.noarch 0:0.4-3.el7
    [ceph4.in][DEBUG ]   python-requests.noarch 0:2.6.0-10.el7
    [ceph4.in][DEBUG ]   python-rgw.x86_64 2:13.2.10-0.el7
    [ceph4.in][DEBUG ]   python-routes.noarch 0:1.13-2.el7
    [ceph4.in][DEBUG ]   python-setuptools.noarch 0:0.9.8-7.el7
    [ceph4.in][DEBUG ]   python-simplegeneric.noarch 0:0.8-7.el7
    [ceph4.in][DEBUG ]   python-singledispatch.noarch 0:3.4.0.2-2.el7
    [ceph4.in][DEBUG ]   python-six.noarch 0:1.9.0-2.el7
    [ceph4.in][DEBUG ]   python-tempita.noarch 0:0.5.1-6.el7
    [ceph4.in][DEBUG ]   python-urllib3.noarch 0:1.10.2-7.el7
    [ceph4.in][DEBUG ]   python-webob.noarch 0:1.2.3-7.el7
    [ceph4.in][DEBUG ]   python-webtest.noarch 0:1.3.4-6.el7
    [ceph4.in][DEBUG ]   python-werkzeug.noarch 0:0.9.1-2.el7
    [ceph4.in][DEBUG ]   python2-bcrypt.x86_64 0:3.1.6-2.el7
    [ceph4.in][DEBUG ]   python2-six.noarch 0:1.9.0-0.el7
    [ceph4.in][DEBUG ]   rdma-core.x86_64 0:22.4-6.el7_9
    [ceph4.in][DEBUG ]   userspace-rcu.x86_64 0:0.7.16-1.el7
    [ceph4.in][DEBUG ]
    [ceph4.in][DEBUG ] Complete!
    [ceph4.in][INFO  ] Running command: sudo ceph --version
    [ceph4.in][DEBUG ] ceph version 13.2.10 (564bdc4ae87418a232fc901524470e1a0f76d641) mimic (stable)
    [ceph_deploy.install][DEBUG ] Detecting platform for host ceph1.in ...
    [ceph1.in][DEBUG ] connection detected need for sudo
    [ceph1.in][DEBUG ] connected to host: ceph1.in
    [ceph1.in][DEBUG ] detect platform information from remote host
    [ceph1.in][DEBUG ] detect machine type
    [ceph_deploy.install][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph1.in][INFO  ] installing Ceph on ceph1.in
    [ceph1.in][INFO  ] Running command: sudo yum clean all
    [ceph1.in][DEBUG ] Loaded plugins: fastestmirror
    [ceph1.in][DEBUG ] Cleaning repos: base epel extras updates
    [ceph1.in][DEBUG ] Cleaning up list of fastest mirrors
    [ceph1.in][INFO  ] Running command: sudo yum -y install epel-release
    [ceph1.in][DEBUG ] Loaded plugins: fastestmirror
    [ceph1.in][DEBUG ] Determining fastest mirrors
    [ceph1.in][DEBUG ]  * base: centos.mirror.net.in
    [ceph1.in][DEBUG ]  * epel: repo.extreme-ix.org
    [ceph1.in][DEBUG ]  * extras: centos.mirror.net.in
    [ceph1.in][DEBUG ]  * updates: centos.mirror.net.in
    [ceph1.in][DEBUG ] Package epel-release-7-14.noarch already installed and latest version
    [ceph1.in][DEBUG ] Nothing to do
    [ceph1.in][INFO  ] Running command: sudo yum -y install yum-plugin-priorities
    [ceph1.in][DEBUG ] Loaded plugins: fastestmirror
    [ceph1.in][DEBUG ] Loading mirror speeds from cached hostfile
    [ceph1.in][DEBUG ]  * base: centos.mirror.net.in
    [ceph1.in][DEBUG ]  * epel: repo.extreme-ix.org
    [ceph1.in][DEBUG ]  * extras: centos.mirror.net.in
    [ceph1.in][DEBUG ]  * updates: centos.mirror.net.in
    [ceph1.in][DEBUG ] Resolving Dependencies
    [ceph1.in][DEBUG ] --> Running transaction check
    [ceph1.in][DEBUG ] ---> Package yum-plugin-priorities.noarch 0:1.1.31-54.el7_8 will be installed
    [ceph1.in][DEBUG ] --> Finished Dependency Resolution
    [ceph1.in][DEBUG ]
    [ceph1.in][DEBUG ] Dependencies Resolved
    [ceph1.in][DEBUG ]
    [ceph1.in][DEBUG ] ================================================================================
    [ceph1.in][DEBUG ]  Package                    Arch        Version                 Repository
    [ceph1.in][DEBUG ]                                                                            Size
    [ceph1.in][DEBUG ] ================================================================================
    [ceph1.in][DEBUG ] Installing:
    [ceph1.in][DEBUG ]  yum-plugin-priorities      noarch      1.1.31-54.el7_8         base       29 k
    [ceph1.in][DEBUG ]
    [ceph1.in][DEBUG ] Transaction Summary
    [ceph1.in][DEBUG ] ================================================================================
    [ceph1.in][DEBUG ] Install  1 Package
    [ceph1.in][DEBUG ]
    [ceph1.in][DEBUG ] Total download size: 29 k
    [ceph1.in][DEBUG ] Installed size: 28 k
    [ceph1.in][DEBUG ] Downloading packages:
    [ceph1.in][DEBUG ] Running transaction check
    [ceph1.in][DEBUG ] Running transaction test
    [ceph1.in][DEBUG ] Transaction test succeeded
    [ceph1.in][DEBUG ] Running transaction
    [ceph1.in][DEBUG ]   Installing : yum-plugin-priorities-1.1.31-54.el7_8.noarch                 1/1
    [ceph1.in][DEBUG ]   Verifying  : yum-plugin-priorities-1.1.31-54.el7_8.noarch                 1/1
    [ceph1.in][DEBUG ]
    [ceph1.in][DEBUG ] Installed:
    [ceph1.in][DEBUG ]   yum-plugin-priorities.noarch 0:1.1.31-54.el7_8
    [ceph1.in][DEBUG ]
    [ceph1.in][DEBUG ] Complete!
    [ceph1.in][DEBUG ] Configure Yum priorities to include obsoletes
    [ceph1.in][WARNIN] check_obsoletes has been enabled for Yum priorities plugin
    [ceph1.in][INFO  ] Running command: sudo rpm --import https://download.ceph.com/keys/release.asc
    [ceph1.in][INFO  ] Running command: sudo yum remove -y ceph-release
    [ceph1.in][DEBUG ] Loaded plugins: fastestmirror, priorities
    [ceph1.in][WARNIN] No Match for argument: ceph-release
    [ceph1.in][DEBUG ] No Packages marked for removal
    [ceph1.in][INFO  ] Running command: sudo yum install -y https://download.ceph.com/rpm-mimic/el7/noarch/ceph-release-1-0.el7.noarch.rpm
    [ceph1.in][DEBUG ] Loaded plugins: fastestmirror, priorities
    [ceph1.in][DEBUG ] Examining /var/tmp/yum-root-OXmyaC/ceph-release-1-0.el7.noarch.rpm: ceph-release-1-1.el7.noarch
    [ceph1.in][DEBUG ] Marking /var/tmp/yum-root-OXmyaC/ceph-release-1-0.el7.noarch.rpm to be installed
    [ceph1.in][DEBUG ] Resolving Dependencies
    [ceph1.in][DEBUG ] --> Running transaction check
    [ceph1.in][DEBUG ] ---> Package ceph-release.noarch 0:1-1.el7 will be installed
    [ceph1.in][DEBUG ] --> Finished Dependency Resolution
    [ceph1.in][DEBUG ]
    [ceph1.in][DEBUG ] Dependencies Resolved
    [ceph1.in][DEBUG ]
    [ceph1.in][DEBUG ] ================================================================================
    [ceph1.in][DEBUG ]  Package          Arch       Version     Repository                        Size
    [ceph1.in][DEBUG ] ================================================================================
    [ceph1.in][DEBUG ] Installing:
    [ceph1.in][DEBUG ]  ceph-release     noarch     1-1.el7     /ceph-release-1-0.el7.noarch     535
    [ceph1.in][DEBUG ]
    [ceph1.in][DEBUG ] Transaction Summary
    [ceph1.in][DEBUG ] ================================================================================
    [ceph1.in][DEBUG ] Install  1 Package
    [ceph1.in][DEBUG ]
    [ceph1.in][DEBUG ] Total size: 535
    [ceph1.in][DEBUG ] Installed size: 535
    [ceph1.in][DEBUG ] Downloading packages:
    [ceph1.in][DEBUG ] Running transaction check
    [ceph1.in][DEBUG ] Running transaction test
    [ceph1.in][DEBUG ] Transaction test succeeded
    [ceph1.in][DEBUG ] Running transaction
    [ceph1.in][DEBUG ]   Installing : ceph-release-1-1.el7.noarch                                  1/1
    [ceph1.in][DEBUG ]   Verifying  : ceph-release-1-1.el7.noarch                                  1/1
    [ceph1.in][DEBUG ]
    [ceph1.in][DEBUG ] Installed:
    [ceph1.in][DEBUG ]   ceph-release.noarch 0:1-1.el7
    [ceph1.in][DEBUG ]
    [ceph1.in][DEBUG ] Complete!
    [ceph1.in][WARNIN] ensuring that /etc/yum.repos.d/ceph.repo contains a high priority
    [ceph1.in][WARNIN] altered ceph.repo priorities to contain: priority=1
    [ceph1.in][INFO  ] Running command: sudo yum -y install ceph ceph-radosgw
    [ceph1.in][DEBUG ] Loaded plugins: fastestmirror, priorities
    [ceph1.in][DEBUG ] Loading mirror speeds from cached hostfile
    [ceph1.in][DEBUG ]  * base: centos.mirror.net.in
    [ceph1.in][DEBUG ]  * epel: repo.extreme-ix.org
    [ceph1.in][DEBUG ]  * extras: centos.mirror.net.in
    [ceph1.in][DEBUG ]  * updates: centos.mirror.net.in
    [ceph1.in][DEBUG ] 8 packages excluded due to repository priority protections
    [ceph1.in][DEBUG ] Resolving Dependencies
    [ceph1.in][DEBUG ] --> Running transaction check
    [ceph1.in][DEBUG ] ---> Package ceph.x86_64 2:13.2.10-0.el7 will be installed
    [ceph1.in][DEBUG ] --> Processing Dependency: ceph-mds = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: ceph-osd = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: ceph-mon = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: ceph-mgr = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] ---> Package ceph-radosgw.x86_64 2:13.2.10-0.el7 will be installed
    [ceph1.in][DEBUG ] --> Processing Dependency: ceph-base = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: ceph-selinux = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: librgw2 = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: librados2 = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: mailcap for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: librados.so.2()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: libtcmalloc.so.4()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: libibverbs.so.1()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: liboath.so.0()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: libceph-common.so.0()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Running transaction check
    [ceph1.in][DEBUG ] ---> Package ceph-base.x86_64 2:13.2.10-0.el7 will be installed
    [ceph1.in][DEBUG ] --> Processing Dependency: libcephfs2 = 2:13.2.10-0.el7 for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: librbd1 = 2:13.2.10-0.el7 for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: ceph-common = 2:13.2.10-0.el7 for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: gdisk for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: python-setuptools for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: psmisc for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: cryptsetup for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: python-requests for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: libleveldb.so.1()(64bit) for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: libfuse.so.2()(64bit) for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: liblttng-ust.so.0()(64bit) for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] ---> Package ceph-mds.x86_64 2:13.2.10-0.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package ceph-mgr.x86_64 2:13.2.10-0.el7 will be installed
    [ceph1.in][DEBUG ] --> Processing Dependency: python-cherrypy for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: python-werkzeug for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: python-six for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: python-routes for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: python-bcrypt for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: python-pecan for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: pyOpenSSL for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: python-jinja2 for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] ---> Package ceph-mon.x86_64 2:13.2.10-0.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package ceph-osd.x86_64 2:13.2.10-0.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package ceph-selinux.x86_64 2:13.2.10-0.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package gperftools-libs.x86_64 0:2.6.1-1.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package libibverbs.x86_64 0:22.4-6.el7_9 will be installed
    [ceph1.in][DEBUG ] --> Processing Dependency: rdma-core(x86-64) = 22.4-6.el7_9 for package: libibverbs-22.4-6.el7_9.x86_64
    [ceph1.in][DEBUG ] ---> Package liboath.x86_64 0:2.6.2-1.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package librados2.x86_64 2:13.2.10-0.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package librgw2.x86_64 2:13.2.10-0.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package mailcap.noarch 0:2.1.41-2.el7 will be installed
    [ceph1.in][DEBUG ] --> Running transaction check
    [ceph1.in][DEBUG ] ---> Package ceph-common.x86_64 2:13.2.10-0.el7 will be installed
    [ceph1.in][DEBUG ] --> Processing Dependency: python-cephfs = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: libradosstriper1 = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: python-rgw = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: python-rbd = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: python-rados = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: python-ceph-argparse = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: python-prettytable for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: libbabeltrace-ctf.so.1()(64bit) for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: libbabeltrace.so.1()(64bit) for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: libradosstriper.so.1()(64bit) for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph1.in][DEBUG ] ---> Package cryptsetup.x86_64 0:2.0.3-6.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package fuse-libs.x86_64 0:2.9.2-11.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package gdisk.x86_64 0:0.8.10-3.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package leveldb.x86_64 0:1.12.0-11.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package libcephfs2.x86_64 2:13.2.10-0.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package librbd1.x86_64 2:13.2.10-0.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package lttng-ust.x86_64 0:2.4.1-4.el7 will be installed
    [ceph1.in][DEBUG ] --> Processing Dependency: liburcu-bp.so.1()(64bit) for package: lttng-ust-2.4.1-4.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: liburcu-cds.so.1()(64bit) for package: lttng-ust-2.4.1-4.el7.x86_64
    [ceph1.in][DEBUG ] ---> Package psmisc.x86_64 0:22.20-17.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package pyOpenSSL.x86_64 0:0.13.1-4.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package python-cherrypy.noarch 0:3.2.2-4.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package python-jinja2.noarch 0:2.7.2-4.el7 will be installed
    [ceph1.in][DEBUG ] --> Processing Dependency: python-babel >= 0.8 for package: python-jinja2-2.7.2-4.el7.noarch
    [ceph1.in][DEBUG ] --> Processing Dependency: python-markupsafe for package: python-jinja2-2.7.2-4.el7.noarch
    [ceph1.in][DEBUG ] ---> Package python-pecan.noarch 0:0.4.5-2.el7 will be installed
    [ceph1.in][DEBUG ] --> Processing Dependency: python-mako >= 0.4.0 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph1.in][DEBUG ] --> Processing Dependency: python-simplegeneric >= 0.8 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph1.in][DEBUG ] --> Processing Dependency: python-webob >= 1.2 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph1.in][DEBUG ] --> Processing Dependency: python-webtest >= 1.3.1 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph1.in][DEBUG ] --> Processing Dependency: python-singledispatch for package: python-pecan-0.4.5-2.el7.noarch
    [ceph1.in][DEBUG ] ---> Package python-requests.noarch 0:2.6.0-10.el7 will be installed
    [ceph1.in][DEBUG ] --> Processing Dependency: python-urllib3 >= 1.10.2-1 for package: python-requests-2.6.0-10.el7.noarch
    [ceph1.in][DEBUG ] --> Processing Dependency: python-chardet >= 2.2.1-1 for package: python-requests-2.6.0-10.el7.noarch
    [ceph1.in][DEBUG ] ---> Package python-routes.noarch 0:1.13-2.el7 will be installed
    [ceph1.in][DEBUG ] --> Processing Dependency: python-repoze-lru for package: python-routes-1.13-2.el7.noarch
    [ceph1.in][DEBUG ] ---> Package python-setuptools.noarch 0:0.9.8-7.el7 will be installed
    [ceph1.in][DEBUG ] --> Processing Dependency: python-backports-ssl_match_hostname for package: python-setuptools-0.9.8-7.el7.noarch
    [ceph1.in][DEBUG ] ---> Package python-six.noarch 0:1.9.0-2.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package python-werkzeug.noarch 0:0.9.1-2.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package python2-bcrypt.x86_64 0:3.1.6-2.el7 will be installed
    [ceph1.in][DEBUG ] --> Processing Dependency: python-cffi for package: python2-bcrypt-3.1.6-2.el7.x86_64
    [ceph1.in][DEBUG ] --> Processing Dependency: python2-six for package: python2-bcrypt-3.1.6-2.el7.x86_64
    [ceph1.in][DEBUG ] ---> Package rdma-core.x86_64 0:22.4-6.el7_9 will be installed
    [ceph1.in][DEBUG ] --> Processing Dependency: pciutils for package: rdma-core-22.4-6.el7_9.x86_64
    [ceph1.in][DEBUG ] --> Running transaction check
    [ceph1.in][DEBUG ] ---> Package libbabeltrace.x86_64 0:1.2.4-3.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package libradosstriper1.x86_64 2:13.2.10-0.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package pciutils.x86_64 0:3.5.1-3.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package python-babel.noarch 0:0.9.6-8.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package python-backports-ssl_match_hostname.noarch 0:3.5.0.1-1.el7 will be installed
    [ceph1.in][DEBUG ] --> Processing Dependency: python-ipaddress for package: python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch
    [ceph1.in][DEBUG ] --> Processing Dependency: python-backports for package: python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch
    [ceph1.in][DEBUG ] ---> Package python-ceph-argparse.x86_64 2:13.2.10-0.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package python-cephfs.x86_64 2:13.2.10-0.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package python-cffi.x86_64 0:1.6.0-5.el7 will be installed
    [ceph1.in][DEBUG ] --> Processing Dependency: python-pycparser for package: python-cffi-1.6.0-5.el7.x86_64
    [ceph1.in][DEBUG ] ---> Package python-chardet.noarch 0:2.2.1-3.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package python-mako.noarch 0:0.8.1-2.el7 will be installed
    [ceph1.in][DEBUG ] --> Processing Dependency: python-beaker for package: python-mako-0.8.1-2.el7.noarch
    [ceph1.in][DEBUG ] ---> Package python-markupsafe.x86_64 0:0.11-10.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package python-prettytable.noarch 0:0.7.2-3.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package python-rados.x86_64 2:13.2.10-0.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package python-rbd.x86_64 2:13.2.10-0.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package python-repoze-lru.noarch 0:0.4-3.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package python-rgw.x86_64 2:13.2.10-0.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package python-simplegeneric.noarch 0:0.8-7.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package python-singledispatch.noarch 0:3.4.0.2-2.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package python-urllib3.noarch 0:1.10.2-7.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package python-webob.noarch 0:1.2.3-7.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package python-webtest.noarch 0:1.3.4-6.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package python2-six.noarch 0:1.9.0-0.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package userspace-rcu.x86_64 0:0.7.16-1.el7 will be installed
    [ceph1.in][DEBUG ] --> Running transaction check
    [ceph1.in][DEBUG ] ---> Package python-backports.x86_64 0:1.0-8.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package python-beaker.noarch 0:1.5.4-10.el7 will be installed
    [ceph1.in][DEBUG ] --> Processing Dependency: python-paste for package: python-beaker-1.5.4-10.el7.noarch
    [ceph1.in][DEBUG ] ---> Package python-ipaddress.noarch 0:1.0.16-2.el7 will be installed
    [ceph1.in][DEBUG ] ---> Package python-pycparser.noarch 0:2.14-1.el7 will be installed
    [ceph1.in][DEBUG ] --> Processing Dependency: python-ply for package: python-pycparser-2.14-1.el7.noarch
    [ceph1.in][DEBUG ] --> Running transaction check
    [ceph1.in][DEBUG ] ---> Package python-paste.noarch 0:1.7.5.1-9.20111221hg1498.el7 will be installed
    [ceph1.in][DEBUG ] --> Processing Dependency: python-tempita for package: python-paste-1.7.5.1-9.20111221hg1498.el7.noarch
    [ceph1.in][DEBUG ] ---> Package python-ply.noarch 0:3.4-11.el7 will be installed
    [ceph1.in][DEBUG ] --> Running transaction check
    [ceph1.in][DEBUG ] ---> Package python-tempita.noarch 0:0.5.1-6.el7 will be installed
    [ceph1.in][DEBUG ] --> Finished Dependency Resolution
    [ceph1.in][DEBUG ]
    [ceph1.in][DEBUG ] Dependencies Resolved
    [ceph1.in][DEBUG ]
    [ceph1.in][DEBUG ] ================================================================================
    [ceph1.in][DEBUG ]  Package                      Arch   Version                      Repository
    [ceph1.in][DEBUG ]                                                                            Size
    [ceph1.in][DEBUG ] ================================================================================
    [ceph1.in][DEBUG ] Installing:
    [ceph1.in][DEBUG ]  ceph                         x86_64 2:13.2.10-0.el7              Ceph    3.0 k
    [ceph1.in][DEBUG ]  ceph-radosgw                 x86_64 2:13.2.10-0.el7              Ceph    4.5 M
    [ceph1.in][DEBUG ] Installing for dependencies:
    [ceph1.in][DEBUG ]  ceph-base                    x86_64 2:13.2.10-0.el7              Ceph    4.8 M
    [ceph1.in][DEBUG ]  ceph-common                  x86_64 2:13.2.10-0.el7              Ceph     14 M
    [ceph1.in][DEBUG ]  ceph-mds                     x86_64 2:13.2.10-0.el7              Ceph    1.7 M
    [ceph1.in][DEBUG ]  ceph-mgr                     x86_64 2:13.2.10-0.el7              Ceph    3.5 M
    [ceph1.in][DEBUG ]  ceph-mon                     x86_64 2:13.2.10-0.el7              Ceph    3.9 M
    [ceph1.in][DEBUG ]  ceph-osd                     x86_64 2:13.2.10-0.el7              Ceph     13 M
    [ceph1.in][DEBUG ]  ceph-selinux                 x86_64 2:13.2.10-0.el7              Ceph     21 k
    [ceph1.in][DEBUG ]  cryptsetup                   x86_64 2.0.3-6.el7                  base    154 k
    [ceph1.in][DEBUG ]  fuse-libs                    x86_64 2.9.2-11.el7                 base     93 k
    [ceph1.in][DEBUG ]  gdisk                        x86_64 0.8.10-3.el7                 base    190 k
    [ceph1.in][DEBUG ]  gperftools-libs              x86_64 2.6.1-1.el7                  base    272 k
    [ceph1.in][DEBUG ]  leveldb                      x86_64 1.12.0-11.el7                epel    161 k
    [ceph1.in][DEBUG ]  libbabeltrace                x86_64 1.2.4-3.el7                  epel    147 k
    [ceph1.in][DEBUG ]  libcephfs2                   x86_64 2:13.2.10-0.el7              Ceph    434 k
    [ceph1.in][DEBUG ]  libibverbs                   x86_64 22.4-6.el7_9                 updates 269 k
    [ceph1.in][DEBUG ]  liboath                      x86_64 2.6.2-1.el7                  epel     51 k
    [ceph1.in][DEBUG ]  librados2                    x86_64 2:13.2.10-0.el7              Ceph    2.9 M
    [ceph1.in][DEBUG ]  libradosstriper1             x86_64 2:13.2.10-0.el7              Ceph    329 k
    [ceph1.in][DEBUG ]  librbd1                      x86_64 2:13.2.10-0.el7              Ceph    1.2 M
    [ceph1.in][DEBUG ]  librgw2                      x86_64 2:13.2.10-0.el7              Ceph    2.0 M
    [ceph1.in][DEBUG ]  lttng-ust                    x86_64 2.4.1-4.el7                  epel    176 k
    [ceph1.in][DEBUG ]  mailcap                      noarch 2.1.41-2.el7                 base     31 k
    [ceph1.in][DEBUG ]  pciutils                     x86_64 3.5.1-3.el7                  base     93 k
    [ceph1.in][DEBUG ]  psmisc                       x86_64 22.20-17.el7                 base    141 k
    [ceph1.in][DEBUG ]  pyOpenSSL                    x86_64 0.13.1-4.el7                 base    135 k
    [ceph1.in][DEBUG ]  python-babel                 noarch 0.9.6-8.el7                  base    1.4 M
    [ceph1.in][DEBUG ]  python-backports             x86_64 1.0-8.el7                    base    5.8 k
    [ceph1.in][DEBUG ]  python-backports-ssl_match_hostname
    [ceph1.in][DEBUG ]                               noarch 3.5.0.1-1.el7                base     13 k
    [ceph1.in][DEBUG ]  python-beaker                noarch 1.5.4-10.el7                 base     80 k
    [ceph1.in][DEBUG ]  python-ceph-argparse         x86_64 2:13.2.10-0.el7              Ceph     34 k
    [ceph1.in][DEBUG ]  python-cephfs                x86_64 2:13.2.10-0.el7              Ceph     87 k
    [ceph1.in][DEBUG ]  python-cffi                  x86_64 1.6.0-5.el7                  base    218 k
    [ceph1.in][DEBUG ]  python-chardet               noarch 2.2.1-3.el7                  base    227 k
    [ceph1.in][DEBUG ]  python-cherrypy              noarch 3.2.2-4.el7                  base    422 k
    [ceph1.in][DEBUG ]  python-ipaddress             noarch 1.0.16-2.el7                 base     34 k
    [ceph1.in][DEBUG ]  python-jinja2                noarch 2.7.2-4.el7                  base    519 k
    [ceph1.in][DEBUG ]  python-mako                  noarch 0.8.1-2.el7                  base    307 k
    [ceph1.in][DEBUG ]  python-markupsafe            x86_64 0.11-10.el7                  base     25 k
    [ceph1.in][DEBUG ]  python-paste                 noarch 1.7.5.1-9.20111221hg1498.el7 base    866 k
    [ceph1.in][DEBUG ]  python-pecan                 noarch 0.4.5-2.el7                  epel    255 k
    [ceph1.in][DEBUG ]  python-ply                   noarch 3.4-11.el7                   base    123 k
    [ceph1.in][DEBUG ]  python-prettytable           noarch 0.7.2-3.el7                  base     37 k
    [ceph1.in][DEBUG ]  python-pycparser             noarch 2.14-1.el7                   base    104 k
    [ceph1.in][DEBUG ]  python-rados                 x86_64 2:13.2.10-0.el7              Ceph    189 k
    [ceph1.in][DEBUG ]  python-rbd                   x86_64 2:13.2.10-0.el7              Ceph    132 k
    [ceph1.in][DEBUG ]  python-repoze-lru            noarch 0.4-3.el7                    epel     13 k
    [ceph1.in][DEBUG ]  python-requests              noarch 2.6.0-10.el7                 base     95 k
    [ceph1.in][DEBUG ]  python-rgw                   x86_64 2:13.2.10-0.el7              Ceph     76 k
    [ceph1.in][DEBUG ]  python-routes                noarch 1.13-2.el7                   epel    640 k
    [ceph1.in][DEBUG ]  python-setuptools            noarch 0.9.8-7.el7                  base    397 k
    [ceph1.in][DEBUG ]  python-simplegeneric         noarch 0.8-7.el7                    epel     12 k
    [ceph1.in][DEBUG ]  python-singledispatch        noarch 3.4.0.2-2.el7                epel     18 k
    [ceph1.in][DEBUG ]  python-six                   noarch 1.9.0-2.el7                  base     29 k
    [ceph1.in][DEBUG ]  python-tempita               noarch 0.5.1-6.el7                  base     33 k
    [ceph1.in][DEBUG ]  python-urllib3               noarch 1.10.2-7.el7                 base    103 k
    [ceph1.in][DEBUG ]  python-webob                 noarch 1.2.3-7.el7                  base    202 k
    [ceph1.in][DEBUG ]  python-webtest               noarch 1.3.4-6.el7                  base    102 k
    [ceph1.in][DEBUG ]  python-werkzeug              noarch 0.9.1-2.el7                  extras  562 k
    [ceph1.in][DEBUG ]  python2-bcrypt               x86_64 3.1.6-2.el7                  epel     39 k
    [ceph1.in][DEBUG ]  python2-six                  noarch 1.9.0-0.el7                  epel    2.9 k
    [ceph1.in][DEBUG ]  rdma-core                    x86_64 22.4-6.el7_9                 updates  51 k
    [ceph1.in][DEBUG ]  userspace-rcu                x86_64 0.7.16-1.el7                 epel     73 k
    [ceph1.in][DEBUG ]
    [ceph1.in][DEBUG ] Transaction Summary
    [ceph1.in][DEBUG ] ================================================================================
    [ceph1.in][DEBUG ] Install  2 Packages (+62 Dependent packages)
    [ceph1.in][DEBUG ]
    [ceph1.in][DEBUG ] Total download size: 61 M
    [ceph1.in][DEBUG ] Installed size: 210 M
    [ceph1.in][DEBUG ] Downloading packages:
    [ceph1.in][DEBUG ] Public key for leveldb-1.12.0-11.el7.x86_64.rpm is not installed
    [ceph1.in][WARNIN] warning: /var/cache/yum/x86_64/7/epel/packages/leveldb-1.12.0-11.el7.x86_64.rpm: Header V3 RSA/SHA256 Signature, key ID 352c64e5: NOKEY
    [ceph1.in][DEBUG ] --------------------------------------------------------------------------------
    [ceph1.in][DEBUG ] Total                                              4.2 MB/s |  61 MB  00:14
    [ceph1.in][DEBUG ] Retrieving key from file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
    [ceph1.in][WARNIN] Importing GPG key 0x352C64E5:
    [ceph1.in][WARNIN]  Userid     : "Fedora EPEL (7) <epel@fedoraproject.org>"
    [ceph1.in][WARNIN]  Fingerprint: 91e9 7d7c 4a5e 96f1 7f3e 888f 6a2f aea2 352c 64e5
    [ceph1.in][WARNIN]  Package    : epel-release-7-14.noarch (@/epel-release-latest-7.noarch)
    [ceph1.in][WARNIN]  From       : /etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
    [ceph1.in][DEBUG ] Running transaction check
    [ceph1.in][DEBUG ] Running transaction test
    [ceph1.in][DEBUG ] Transaction test succeeded
    [ceph1.in][DEBUG ] Running transaction
    [ceph1.in][DEBUG ]   Installing : gperftools-libs-2.6.1-1.el7.x86_64                          1/64
    [ceph1.in][DEBUG ]   Installing : leveldb-1.12.0-11.el7.x86_64                                2/64
    [ceph1.in][DEBUG ]   Installing : python-six-1.9.0-2.el7.noarch                               3/64
    [ceph1.in][DEBUG ]   Installing : fuse-libs-2.9.2-11.el7.x86_64                               4/64
    [ceph1.in][DEBUG ]   Installing : liboath-2.6.2-1.el7.x86_64                                  5/64
    [ceph1.in][DEBUG ]   Installing : python-ipaddress-1.0.16-2.el7.noarch                        6/64
    [ceph1.in][DEBUG ]   Installing : python-webob-1.2.3-7.el7.noarch                             7/64
    [ceph1.in][DEBUG ]   Installing : python-markupsafe-0.11-10.el7.x86_64                        8/64
    [ceph1.in][DEBUG ]   Installing : pyOpenSSL-0.13.1-4.el7.x86_64                               9/64
    [ceph1.in][DEBUG ]   Installing : 2:python-ceph-argparse-13.2.10-0.el7.x86_64                10/64
    [ceph1.in][DEBUG ]   Installing : python-webtest-1.3.4-6.el7.noarch                          11/64
    [ceph1.in][DEBUG ]   Installing : python2-six-1.9.0-0.el7.noarch                             12/64
    [ceph1.in][DEBUG ]   Installing : python-singledispatch-3.4.0.2-2.el7.noarch                 13/64
    [ceph1.in][DEBUG ]   Installing : psmisc-22.20-17.el7.x86_64                                 14/64
    [ceph1.in][DEBUG ]   Installing : pciutils-3.5.1-3.el7.x86_64                                15/64
    [ceph1.in][DEBUG ]   Installing : rdma-core-22.4-6.el7_9.x86_64                              16/64
    [ceph1.in][DEBUG ]   Installing : libibverbs-22.4-6.el7_9.x86_64                             17/64
    [ceph1.in][DEBUG ]   Installing : gdisk-0.8.10-3.el7.x86_64                                  18/64
    [ceph1.in][DEBUG ]   Installing : python-simplegeneric-0.8-7.el7.noarch                      19/64
    [ceph1.in][DEBUG ]   Installing : python-tempita-0.5.1-6.el7.noarch                          20/64
    [ceph1.in][DEBUG ]   Installing : python-cherrypy-3.2.2-4.el7.noarch                         21/64
    [ceph1.in][DEBUG ]   Installing : python-prettytable-0.7.2-3.el7.noarch                      22/64
    [ceph1.in][DEBUG ]   Installing : python-werkzeug-0.9.1-2.el7.noarch                         23/64
    [ceph1.in][DEBUG ]   Installing : python-repoze-lru-0.4-3.el7.noarch                         24/64
    [ceph1.in][DEBUG ]   Installing : python-routes-1.13-2.el7.noarch                            25/64
    [ceph1.in][DEBUG ]   Installing : python-backports-1.0-8.el7.x86_64                          26/64
    [ceph1.in][DEBUG ]   Installing : python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch   27/64
    [ceph1.in][DEBUG ]   Installing : python-setuptools-0.9.8-7.el7.noarch                       28/64
    [ceph1.in][DEBUG ]   Installing : python-paste-1.7.5.1-9.20111221hg1498.el7.noarch           29/64
    [ceph1.in][DEBUG ]   Installing : python-beaker-1.5.4-10.el7.noarch                          30/64
    [ceph1.in][DEBUG ]   Installing : python-mako-0.8.1-2.el7.noarch                             31/64
    [ceph1.in][DEBUG ]   Installing : python-pecan-0.4.5-2.el7.noarch                            32/64
    [ceph1.in][DEBUG ]   Installing : python-urllib3-1.10.2-7.el7.noarch                         33/64
    [ceph1.in][DEBUG ]   Installing : python-babel-0.9.6-8.el7.noarch                            34/64
    [ceph1.in][DEBUG ]   Installing : python-jinja2-2.7.2-4.el7.noarch                           35/64
    [ceph1.in][DEBUG ]   Installing : python-chardet-2.2.1-3.el7.noarch                          36/64
    [ceph1.in][DEBUG ]   Installing : python-requests-2.6.0-10.el7.noarch                        37/64
    [ceph1.in][DEBUG ]   Installing : cryptsetup-2.0.3-6.el7.x86_64                              38/64
    [ceph1.in][DEBUG ]   Installing : libbabeltrace-1.2.4-3.el7.x86_64                           39/64
    [ceph1.in][DEBUG ]   Installing : userspace-rcu-0.7.16-1.el7.x86_64                          40/64
    [ceph1.in][DEBUG ]   Installing : lttng-ust-2.4.1-4.el7.x86_64                               41/64
    [ceph1.in][DEBUG ]   Installing : 2:librados2-13.2.10-0.el7.x86_64                           42/64
    [ceph1.in][DEBUG ]   Installing : 2:python-rados-13.2.10-0.el7.x86_64                        43/64
    [ceph1.in][DEBUG ]   Installing : 2:librbd1-13.2.10-0.el7.x86_64                             44/64
    [ceph1.in][DEBUG ]   Installing : 2:libcephfs2-13.2.10-0.el7.x86_64                          45/64
    [ceph1.in][DEBUG ]   Installing : 2:librgw2-13.2.10-0.el7.x86_64                             46/64
    [ceph1.in][DEBUG ]   Installing : 2:python-rgw-13.2.10-0.el7.x86_64                          47/64
    [ceph1.in][DEBUG ]   Installing : 2:python-cephfs-13.2.10-0.el7.x86_64                       48/64
    [ceph1.in][DEBUG ]   Installing : 2:python-rbd-13.2.10-0.el7.x86_64                          49/64
    [ceph1.in][DEBUG ]   Installing : 2:libradosstriper1-13.2.10-0.el7.x86_64                    50/64
    [ceph1.in][DEBUG ]   Installing : 2:ceph-common-13.2.10-0.el7.x86_64                         51/64
    [ceph1.in][DEBUG ]   Installing : 2:ceph-base-13.2.10-0.el7.x86_64                           52/64
    [ceph1.in][DEBUG ]   Installing : 2:ceph-selinux-13.2.10-0.el7.x86_64                        53/64
    [ceph1.in][DEBUG ]   Installing : 2:ceph-osd-13.2.10-0.el7.x86_64                            54/64
    [ceph1.in][DEBUG ]   Installing : 2:ceph-mds-13.2.10-0.el7.x86_64                            55/64
    [ceph1.in][DEBUG ]   Installing : 2:ceph-mon-13.2.10-0.el7.x86_64                            56/64
    [ceph1.in][DEBUG ]   Installing : python-ply-3.4-11.el7.noarch                               57/64
    [ceph1.in][DEBUG ]   Installing : python-pycparser-2.14-1.el7.noarch                         58/64
    [ceph1.in][DEBUG ]   Installing : python-cffi-1.6.0-5.el7.x86_64                             59/64
    [ceph1.in][DEBUG ]   Installing : python2-bcrypt-3.1.6-2.el7.x86_64                          60/64
    [ceph1.in][DEBUG ]   Installing : 2:ceph-mgr-13.2.10-0.el7.x86_64                            61/64
    [ceph1.in][DEBUG ]   Installing : mailcap-2.1.41-2.el7.noarch                                62/64
    [ceph1.in][DEBUG ]   Installing : 2:ceph-radosgw-13.2.10-0.el7.x86_64                        63/64
    [ceph1.in][DEBUG ]   Installing : 2:ceph-13.2.10-0.el7.x86_64                                64/64
    [ceph1.in][DEBUG ]   Verifying  : liboath-2.6.2-1.el7.x86_64                                  1/64
    [ceph1.in][DEBUG ]   Verifying  : python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch    2/64
    [ceph1.in][DEBUG ]   Verifying  : 2:librbd1-13.2.10-0.el7.x86_64                              3/64
    [ceph1.in][DEBUG ]   Verifying  : 2:python-ceph-argparse-13.2.10-0.el7.x86_64                 4/64
    [ceph1.in][DEBUG ]   Verifying  : mailcap-2.1.41-2.el7.noarch                                 5/64
    [ceph1.in][DEBUG ]   Verifying  : pyOpenSSL-0.13.1-4.el7.x86_64                               6/64
    [ceph1.in][DEBUG ]   Verifying  : python2-bcrypt-3.1.6-2.el7.x86_64                           7/64
    [ceph1.in][DEBUG ]   Verifying  : python-ply-3.4-11.el7.noarch                                8/64
    [ceph1.in][DEBUG ]   Verifying  : userspace-rcu-0.7.16-1.el7.x86_64                           9/64
    [ceph1.in][DEBUG ]   Verifying  : libibverbs-22.4-6.el7_9.x86_64                             10/64
    [ceph1.in][DEBUG ]   Verifying  : rdma-core-22.4-6.el7_9.x86_64                              11/64
    [ceph1.in][DEBUG ]   Verifying  : fuse-libs-2.9.2-11.el7.x86_64                              12/64
    [ceph1.in][DEBUG ]   Verifying  : python-setuptools-0.9.8-7.el7.noarch                       13/64
    [ceph1.in][DEBUG ]   Verifying  : python-routes-1.13-2.el7.noarch                            14/64
    [ceph1.in][DEBUG ]   Verifying  : 2:libcephfs2-13.2.10-0.el7.x86_64                          15/64
    [ceph1.in][DEBUG ]   Verifying  : python-urllib3-1.10.2-7.el7.noarch                         16/64
    [ceph1.in][DEBUG ]   Verifying  : libbabeltrace-1.2.4-3.el7.x86_64                           17/64
    [ceph1.in][DEBUG ]   Verifying  : python-mako-0.8.1-2.el7.noarch                             18/64
    [ceph1.in][DEBUG ]   Verifying  : python2-six-1.9.0-0.el7.noarch                             19/64
    [ceph1.in][DEBUG ]   Verifying  : 2:ceph-mgr-13.2.10-0.el7.x86_64                            20/64
    [ceph1.in][DEBUG ]   Verifying  : 2:ceph-base-13.2.10-0.el7.x86_64                           21/64
    [ceph1.in][DEBUG ]   Verifying  : python-jinja2-2.7.2-4.el7.noarch                           22/64
    [ceph1.in][DEBUG ]   Verifying  : python-pecan-0.4.5-2.el7.noarch                            23/64
    [ceph1.in][DEBUG ]   Verifying  : python-six-1.9.0-2.el7.noarch                              24/64
    [ceph1.in][DEBUG ]   Verifying  : cryptsetup-2.0.3-6.el7.x86_64                              25/64
    [ceph1.in][DEBUG ]   Verifying  : leveldb-1.12.0-11.el7.x86_64                               26/64
    [ceph1.in][DEBUG ]   Verifying  : python-singledispatch-3.4.0.2-2.el7.noarch                 27/64
    [ceph1.in][DEBUG ]   Verifying  : python-markupsafe-0.11-10.el7.x86_64                       28/64
    [ceph1.in][DEBUG ]   Verifying  : 2:python-rados-13.2.10-0.el7.x86_64                        29/64
    [ceph1.in][DEBUG ]   Verifying  : 2:python-rgw-13.2.10-0.el7.x86_64                          30/64
    [ceph1.in][DEBUG ]   Verifying  : 2:ceph-radosgw-13.2.10-0.el7.x86_64                        31/64
    [ceph1.in][DEBUG ]   Verifying  : python-chardet-2.2.1-3.el7.noarch                          32/64
    [ceph1.in][DEBUG ]   Verifying  : python-babel-0.9.6-8.el7.noarch                            33/64
    [ceph1.in][DEBUG ]   Verifying  : 2:librados2-13.2.10-0.el7.x86_64                           34/64
    [ceph1.in][DEBUG ]   Verifying  : python-paste-1.7.5.1-9.20111221hg1498.el7.noarch           35/64
    [ceph1.in][DEBUG ]   Verifying  : 2:ceph-osd-13.2.10-0.el7.x86_64                            36/64
    [ceph1.in][DEBUG ]   Verifying  : python-backports-1.0-8.el7.x86_64                          37/64
    [ceph1.in][DEBUG ]   Verifying  : lttng-ust-2.4.1-4.el7.x86_64                               38/64
    [ceph1.in][DEBUG ]   Verifying  : python-webob-1.2.3-7.el7.noarch                            39/64
    [ceph1.in][DEBUG ]   Verifying  : 2:ceph-common-13.2.10-0.el7.x86_64                         40/64
    [ceph1.in][DEBUG ]   Verifying  : python-repoze-lru-0.4-3.el7.noarch                         41/64
    [ceph1.in][DEBUG ]   Verifying  : python-werkzeug-0.9.1-2.el7.noarch                         42/64
    [ceph1.in][DEBUG ]   Verifying  : python-beaker-1.5.4-10.el7.noarch                          43/64
    [ceph1.in][DEBUG ]   Verifying  : python-cffi-1.6.0-5.el7.x86_64                             44/64
    [ceph1.in][DEBUG ]   Verifying  : 2:ceph-selinux-13.2.10-0.el7.x86_64                        45/64
    [ceph1.in][DEBUG ]   Verifying  : python-requests-2.6.0-10.el7.noarch                        46/64
    [ceph1.in][DEBUG ]   Verifying  : python-pycparser-2.14-1.el7.noarch                         47/64
    [ceph1.in][DEBUG ]   Verifying  : python-prettytable-0.7.2-3.el7.noarch                      48/64
    [ceph1.in][DEBUG ]   Verifying  : 2:librgw2-13.2.10-0.el7.x86_64                             49/64
    [ceph1.in][DEBUG ]   Verifying  : 2:ceph-mds-13.2.10-0.el7.x86_64                            50/64
    [ceph1.in][DEBUG ]   Verifying  : python-cherrypy-3.2.2-4.el7.noarch                         51/64
    [ceph1.in][DEBUG ]   Verifying  : 2:python-cephfs-13.2.10-0.el7.x86_64                       52/64
    [ceph1.in][DEBUG ]   Verifying  : python-tempita-0.5.1-6.el7.noarch                          53/64
    [ceph1.in][DEBUG ]   Verifying  : 2:python-rbd-13.2.10-0.el7.x86_64                          54/64
    [ceph1.in][DEBUG ]   Verifying  : 2:ceph-mon-13.2.10-0.el7.x86_64                            55/64
    [ceph1.in][DEBUG ]   Verifying  : gperftools-libs-2.6.1-1.el7.x86_64                         56/64
    [ceph1.in][DEBUG ]   Verifying  : python-ipaddress-1.0.16-2.el7.noarch                       57/64
    [ceph1.in][DEBUG ]   Verifying  : python-webtest-1.3.4-6.el7.noarch                          58/64
    [ceph1.in][DEBUG ]   Verifying  : 2:ceph-13.2.10-0.el7.x86_64                                59/64
    [ceph1.in][DEBUG ]   Verifying  : python-simplegeneric-0.8-7.el7.noarch                      60/64
    [ceph1.in][DEBUG ]   Verifying  : gdisk-0.8.10-3.el7.x86_64                                  61/64
    [ceph1.in][DEBUG ]   Verifying  : 2:libradosstriper1-13.2.10-0.el7.x86_64                    62/64
    [ceph1.in][DEBUG ]   Verifying  : pciutils-3.5.1-3.el7.x86_64                                63/64
    [ceph1.in][DEBUG ]   Verifying  : psmisc-22.20-17.el7.x86_64                                 64/64
    [ceph1.in][DEBUG ]
    [ceph1.in][DEBUG ] Installed:
    [ceph1.in][DEBUG ]   ceph.x86_64 2:13.2.10-0.el7        ceph-radosgw.x86_64 2:13.2.10-0.el7
    [ceph1.in][DEBUG ]
    [ceph1.in][DEBUG ] Dependency Installed:
    [ceph1.in][DEBUG ]   ceph-base.x86_64 2:13.2.10-0.el7
    [ceph1.in][DEBUG ]   ceph-common.x86_64 2:13.2.10-0.el7
    [ceph1.in][DEBUG ]   ceph-mds.x86_64 2:13.2.10-0.el7
    [ceph1.in][DEBUG ]   ceph-mgr.x86_64 2:13.2.10-0.el7
    [ceph1.in][DEBUG ]   ceph-mon.x86_64 2:13.2.10-0.el7
    [ceph1.in][DEBUG ]   ceph-osd.x86_64 2:13.2.10-0.el7
    [ceph1.in][DEBUG ]   ceph-selinux.x86_64 2:13.2.10-0.el7
    [ceph1.in][DEBUG ]   cryptsetup.x86_64 0:2.0.3-6.el7
    [ceph1.in][DEBUG ]   fuse-libs.x86_64 0:2.9.2-11.el7
    [ceph1.in][DEBUG ]   gdisk.x86_64 0:0.8.10-3.el7
    [ceph1.in][DEBUG ]   gperftools-libs.x86_64 0:2.6.1-1.el7
    [ceph1.in][DEBUG ]   leveldb.x86_64 0:1.12.0-11.el7
    [ceph1.in][DEBUG ]   libbabeltrace.x86_64 0:1.2.4-3.el7
    [ceph1.in][DEBUG ]   libcephfs2.x86_64 2:13.2.10-0.el7
    [ceph1.in][DEBUG ]   libibverbs.x86_64 0:22.4-6.el7_9
    [ceph1.in][DEBUG ]   liboath.x86_64 0:2.6.2-1.el7
    [ceph1.in][DEBUG ]   librados2.x86_64 2:13.2.10-0.el7
    [ceph1.in][DEBUG ]   libradosstriper1.x86_64 2:13.2.10-0.el7
    [ceph1.in][DEBUG ]   librbd1.x86_64 2:13.2.10-0.el7
    [ceph1.in][DEBUG ]   librgw2.x86_64 2:13.2.10-0.el7
    [ceph1.in][DEBUG ]   lttng-ust.x86_64 0:2.4.1-4.el7
    [ceph1.in][DEBUG ]   mailcap.noarch 0:2.1.41-2.el7
    [ceph1.in][DEBUG ]   pciutils.x86_64 0:3.5.1-3.el7
    [ceph1.in][DEBUG ]   psmisc.x86_64 0:22.20-17.el7
    [ceph1.in][DEBUG ]   pyOpenSSL.x86_64 0:0.13.1-4.el7
    [ceph1.in][DEBUG ]   python-babel.noarch 0:0.9.6-8.el7
    [ceph1.in][DEBUG ]   python-backports.x86_64 0:1.0-8.el7
    [ceph1.in][DEBUG ]   python-backports-ssl_match_hostname.noarch 0:3.5.0.1-1.el7
    [ceph1.in][DEBUG ]   python-beaker.noarch 0:1.5.4-10.el7
    [ceph1.in][DEBUG ]   python-ceph-argparse.x86_64 2:13.2.10-0.el7
    [ceph1.in][DEBUG ]   python-cephfs.x86_64 2:13.2.10-0.el7
    [ceph1.in][DEBUG ]   python-cffi.x86_64 0:1.6.0-5.el7
    [ceph1.in][DEBUG ]   python-chardet.noarch 0:2.2.1-3.el7
    [ceph1.in][DEBUG ]   python-cherrypy.noarch 0:3.2.2-4.el7
    [ceph1.in][DEBUG ]   python-ipaddress.noarch 0:1.0.16-2.el7
    [ceph1.in][DEBUG ]   python-jinja2.noarch 0:2.7.2-4.el7
    [ceph1.in][DEBUG ]   python-mako.noarch 0:0.8.1-2.el7
    [ceph1.in][DEBUG ]   python-markupsafe.x86_64 0:0.11-10.el7
    [ceph1.in][DEBUG ]   python-paste.noarch 0:1.7.5.1-9.20111221hg1498.el7
    [ceph1.in][DEBUG ]   python-pecan.noarch 0:0.4.5-2.el7
    [ceph1.in][DEBUG ]   python-ply.noarch 0:3.4-11.el7
    [ceph1.in][DEBUG ]   python-prettytable.noarch 0:0.7.2-3.el7
    [ceph1.in][DEBUG ]   python-pycparser.noarch 0:2.14-1.el7
    [ceph1.in][DEBUG ]   python-rados.x86_64 2:13.2.10-0.el7
    [ceph1.in][DEBUG ]   python-rbd.x86_64 2:13.2.10-0.el7
    [ceph1.in][DEBUG ]   python-repoze-lru.noarch 0:0.4-3.el7
    [ceph1.in][DEBUG ]   python-requests.noarch 0:2.6.0-10.el7
    [ceph1.in][DEBUG ]   python-rgw.x86_64 2:13.2.10-0.el7
    [ceph1.in][DEBUG ]   python-routes.noarch 0:1.13-2.el7
    [ceph1.in][DEBUG ]   python-setuptools.noarch 0:0.9.8-7.el7
    [ceph1.in][DEBUG ]   python-simplegeneric.noarch 0:0.8-7.el7
    [ceph1.in][DEBUG ]   python-singledispatch.noarch 0:3.4.0.2-2.el7
    [ceph1.in][DEBUG ]   python-six.noarch 0:1.9.0-2.el7
    [ceph1.in][DEBUG ]   python-tempita.noarch 0:0.5.1-6.el7
    [ceph1.in][DEBUG ]   python-urllib3.noarch 0:1.10.2-7.el7
    [ceph1.in][DEBUG ]   python-webob.noarch 0:1.2.3-7.el7
    [ceph1.in][DEBUG ]   python-webtest.noarch 0:1.3.4-6.el7
    [ceph1.in][DEBUG ]   python-werkzeug.noarch 0:0.9.1-2.el7
    [ceph1.in][DEBUG ]   python2-bcrypt.x86_64 0:3.1.6-2.el7
    [ceph1.in][DEBUG ]   python2-six.noarch 0:1.9.0-0.el7
    [ceph1.in][DEBUG ]   rdma-core.x86_64 0:22.4-6.el7_9
    [ceph1.in][DEBUG ]   userspace-rcu.x86_64 0:0.7.16-1.el7
    [ceph1.in][DEBUG ]
    [ceph1.in][DEBUG ] Complete!
    [ceph1.in][INFO  ] Running command: sudo ceph --version
    [ceph1.in][DEBUG ] ceph version 13.2.10 (564bdc4ae87418a232fc901524470e1a0f76d641) mimic (stable)
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy mon create-initial
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy mon create-initial
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  subcommand                    : create-initial
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f9580715320>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  func                          : <function mon at 0x7f9580976500>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  keyrings                      : None
    [ceph_deploy.mon][DEBUG ] Deploying mon, cluster ceph hosts ceph1
    [ceph_deploy.mon][DEBUG ] detecting platform for host ceph1 ...
    ssh: Could not resolve hostname ceph1: Name or service not known
    [ceph_deploy.mon][ERROR ] connecting to host: ceph1 resulted in errors: HostNotFound ceph1
    [ceph_deploy][ERROR ] GenericError: Failed to create 1 monitors
    
    [cephadm@ceph2 ceph_cluster]$ vim ceph.conf
    [cephadm@ceph2 ceph_cluster]$ vim ~/.ssh/config
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy mon create-initial
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy mon create-initial
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  subcommand                    : create-initial
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7fa52a3af320>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  func                          : <function mon at 0x7fa52a610500>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  keyrings                      : None
    [ceph_deploy.mon][DEBUG ] Deploying mon, cluster ceph hosts ceph1
    [ceph_deploy.mon][DEBUG ] detecting platform for host ceph1 ...
    [ceph1][DEBUG ] connection detected need for sudo
    [ceph1][DEBUG ] connected to host: ceph1
    [ceph1][DEBUG ] detect platform information from remote host
    [ceph1][DEBUG ] detect machine type
    [ceph1][DEBUG ] find the location of an executable
    [ceph_deploy.mon][INFO  ] distro info: CentOS Linux 7.9.2009 Core
    [ceph1][DEBUG ] determining if provided host has same hostname in remote
    [ceph1][DEBUG ] get remote short hostname
    [ceph1][DEBUG ] deploying mon to ceph1
    [ceph1][DEBUG ] get remote short hostname
    [ceph1][DEBUG ] remote hostname: ceph1
    [ceph1][DEBUG ] write cluster configuration to /etc/ceph/{cluster}.conf
    [ceph1][DEBUG ] create the mon path if it does not exist
    [ceph1][DEBUG ] checking for done path: /var/lib/ceph/mon/ceph-ceph1/done
    [ceph1][DEBUG ] done path does not exist: /var/lib/ceph/mon/ceph-ceph1/done
    [ceph1][INFO  ] creating keyring file: /var/lib/ceph/tmp/ceph-ceph1.mon.keyring
    [ceph1][DEBUG ] create the monitor keyring file
    [ceph1][INFO  ] Running command: sudo ceph-mon --cluster ceph --mkfs -i ceph1 --keyring /var/lib/ceph/tmp/ceph-ceph1.mon.keyring --setuser 167 --setgroup 167
    [ceph1][INFO  ] unlinking keyring file /var/lib/ceph/tmp/ceph-ceph1.mon.keyring
    [ceph1][DEBUG ] create a done file to avoid re-doing the mon deployment
    [ceph1][DEBUG ] create the init path if it does not exist
    [ceph1][INFO  ] Running command: sudo systemctl enable ceph.target
    [ceph1][INFO  ] Running command: sudo systemctl enable ceph-mon@ceph1
    [ceph1][WARNIN] Created symlink from /etc/systemd/system/ceph-mon.target.wants/ceph-mon@ceph1.service to /usr/lib/systemd/system/ceph-mon@.service.
    [ceph1][INFO  ] Running command: sudo systemctl start ceph-mon@ceph1
    [ceph1][INFO  ] Running command: sudo ceph --cluster=ceph --admin-daemon /var/run/ceph/ceph-mon.ceph1.asok mon_status
    [ceph1][DEBUG ] ********************************************************************************
    [ceph1][DEBUG ] status for monitor: mon.ceph1
    [ceph1][DEBUG ] {
    [ceph1][DEBUG ]   "election_epoch": 3,
    [ceph1][DEBUG ]   "extra_probe_peers": [],
    [ceph1][DEBUG ]   "feature_map": {
    [ceph1][DEBUG ]     "mon": [
    [ceph1][DEBUG ]       {
    [ceph1][DEBUG ]         "features": "0x3ffddff8ffacfffb",
    [ceph1][DEBUG ]         "num": 1,
    [ceph1][DEBUG ]         "release": "luminous"
    [ceph1][DEBUG ]       }
    [ceph1][DEBUG ]     ]
    [ceph1][DEBUG ]   },
    [ceph1][DEBUG ]   "features": {
    [ceph1][DEBUG ]     "quorum_con": "4611087854031667195",
    [ceph1][DEBUG ]     "quorum_mon": [
    [ceph1][DEBUG ]       "kraken",
    [ceph1][DEBUG ]       "luminous",
    [ceph1][DEBUG ]       "mimic",
    [ceph1][DEBUG ]       "osdmap-prune"
    [ceph1][DEBUG ]     ],
    [ceph1][DEBUG ]     "required_con": "144115738102218752",
    [ceph1][DEBUG ]     "required_mon": [
    [ceph1][DEBUG ]       "kraken",
    [ceph1][DEBUG ]       "luminous",
    [ceph1][DEBUG ]       "mimic",
    [ceph1][DEBUG ]       "osdmap-prune"
    [ceph1][DEBUG ]     ]
    [ceph1][DEBUG ]   },
    [ceph1][DEBUG ]   "monmap": {
    [ceph1][DEBUG ]     "created": "2023-07-16 22:07:24.907995",
    [ceph1][DEBUG ]     "epoch": 1,
    [ceph1][DEBUG ]     "features": {
    [ceph1][DEBUG ]       "optional": [],
    [ceph1][DEBUG ]       "persistent": [
    [ceph1][DEBUG ]         "kraken",
    [ceph1][DEBUG ]         "luminous",
    [ceph1][DEBUG ]         "mimic",
    [ceph1][DEBUG ]         "osdmap-prune"
    [ceph1][DEBUG ]       ]
    [ceph1][DEBUG ]     },
    [ceph1][DEBUG ]     "fsid": "5cfc246a-5a14-4337-98b2-58d2a2e19b18",
    [ceph1][DEBUG ]     "modified": "2023-07-16 22:07:24.907995",
    [ceph1][DEBUG ]     "mons": [
    [ceph1][DEBUG ]       {
    [ceph1][DEBUG ]         "addr": "192.168.239.154:6789/0",
    [ceph1][DEBUG ]         "name": "ceph1",
    [ceph1][DEBUG ]         "public_addr": "192.168.239.154:6789/0",
    [ceph1][DEBUG ]         "rank": 0
    [ceph1][DEBUG ]       }
    [ceph1][DEBUG ]     ]
    [ceph1][DEBUG ]   },
    [ceph1][DEBUG ]   "name": "ceph1",
    [ceph1][DEBUG ]   "outside_quorum": [],
    [ceph1][DEBUG ]   "quorum": [
    [ceph1][DEBUG ]     0
    [ceph1][DEBUG ]   ],
    [ceph1][DEBUG ]   "rank": 0,
    [ceph1][DEBUG ]   "state": "leader",
    [ceph1][DEBUG ]   "sync_provider": []
    [ceph1][DEBUG ] }
    [ceph1][DEBUG ] ********************************************************************************
    [ceph1][INFO  ] monitor: mon.ceph1 is running
    [ceph1][INFO  ] Running command: sudo ceph --cluster=ceph --admin-daemon /var/run/ceph/ceph-mon.ceph1.asok mon_status
    [ceph_deploy.mon][INFO  ] processing monitor mon.ceph1
    [ceph1][DEBUG ] connection detected need for sudo
    [ceph1][DEBUG ] connected to host: ceph1
    [ceph1][DEBUG ] detect platform information from remote host
    [ceph1][DEBUG ] detect machine type
    [ceph1][DEBUG ] find the location of an executable
    [ceph1][INFO  ] Running command: sudo ceph --cluster=ceph --admin-daemon /var/run/ceph/ceph-mon.ceph1.asok mon_status
    [ceph_deploy.mon][INFO  ] mon.ceph1 monitor has reached quorum!
    [ceph_deploy.mon][INFO  ] all initial monitors are running and have formed quorum
    [ceph_deploy.mon][INFO  ] Running gatherkeys...
    [ceph_deploy.gatherkeys][INFO  ] Storing keys in temp directory /tmp/tmp6SBhet
    [ceph1][DEBUG ] connection detected need for sudo
    [ceph1][DEBUG ] connected to host: ceph1
    [ceph1][DEBUG ] detect platform information from remote host
    [ceph1][DEBUG ] detect machine type
    [ceph1][DEBUG ] get remote short hostname
    [ceph1][DEBUG ] fetch remote file
    [ceph1][INFO  ] Running command: sudo /usr/bin/ceph --connect-timeout=25 --cluster=ceph --admin-daemon=/var/run/ceph/ceph-mon.ceph1.asok mon_status
    [ceph1][INFO  ] Running command: sudo /usr/bin/ceph --connect-timeout=25 --cluster=ceph --name mon. --keyring=/var/lib/ceph/mon/ceph-ceph1/keyring auth get client.admin
    [ceph1][INFO  ] Running command: sudo /usr/bin/ceph --connect-timeout=25 --cluster=ceph --name mon. --keyring=/var/lib/ceph/mon/ceph-ceph1/keyring auth get client.bootstrap-mds
    [ceph1][INFO  ] Running command: sudo /usr/bin/ceph --connect-timeout=25 --cluster=ceph --name mon. --keyring=/var/lib/ceph/mon/ceph-ceph1/keyring auth get client.bootstrap-mgr
    [ceph1][INFO  ] Running command: sudo /usr/bin/ceph --connect-timeout=25 --cluster=ceph --name mon. --keyring=/var/lib/ceph/mon/ceph-ceph1/keyring auth get client.bootstrap-osd
    [ceph1][INFO  ] Running command: sudo /usr/bin/ceph --connect-timeout=25 --cluster=ceph --name mon. --keyring=/var/lib/ceph/mon/ceph-ceph1/keyring auth get client.bootstrap-rgw
    [ceph_deploy.gatherkeys][INFO  ] Storing ceph.client.admin.keyring
    [ceph_deploy.gatherkeys][INFO  ] Storing ceph.bootstrap-mds.keyring
    [ceph_deploy.gatherkeys][INFO  ] Storing ceph.bootstrap-mgr.keyring
    [ceph_deploy.gatherkeys][INFO  ] keyring 'ceph.mon.keyring' already exists
    [ceph_deploy.gatherkeys][INFO  ] Storing ceph.bootstrap-osd.keyring
    [ceph_deploy.gatherkeys][INFO  ] Storing ceph.bootstrap-rgw.keyring
    [ceph_deploy.gatherkeys][INFO  ] Destroy temp directory /tmp/tmp6SBhet
    [cephadm@ceph2 ceph_cluster]$ vim ~/.ssh/config
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy admin ceph2.in ceph3.in ceph4.in ceph1.in
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy admin ceph2.in ceph3.in ceph4.in ceph1.in
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f71baf53950>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  client                        : ['ceph2.in', 'ceph3.in', 'ceph4.in', 'ceph1.in']
    [ceph_deploy.cli][INFO  ]  func                          : <function admin at 0x7f71bb7eb320>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.admin][DEBUG ] Pushing admin keys and conf to ceph2.in
    [ceph2.in][DEBUG ] connection detected need for sudo
    [ceph2.in][DEBUG ] connected to host: ceph2.in
    [ceph2.in][DEBUG ] detect platform information from remote host
    [ceph2.in][DEBUG ] detect machine type
    [ceph2.in][DEBUG ] write cluster configuration to /etc/ceph/{cluster}.conf
    [ceph_deploy.admin][DEBUG ] Pushing admin keys and conf to ceph3.in
    [ceph3.in][DEBUG ] connection detected need for sudo
    [ceph3.in][DEBUG ] connected to host: ceph3.in
    [ceph3.in][DEBUG ] detect platform information from remote host
    [ceph3.in][DEBUG ] detect machine type
    [ceph3.in][DEBUG ] write cluster configuration to /etc/ceph/{cluster}.conf
    [ceph_deploy.admin][DEBUG ] Pushing admin keys and conf to ceph4.in
    [ceph4.in][DEBUG ] connection detected need for sudo
    [ceph4.in][DEBUG ] connected to host: ceph4.in
    [ceph4.in][DEBUG ] detect platform information from remote host
    [ceph4.in][DEBUG ] detect machine type
    [ceph4.in][DEBUG ] write cluster configuration to /etc/ceph/{cluster}.conf
    [ceph_deploy.admin][DEBUG ] Pushing admin keys and conf to ceph1.in
    [ceph1.in][DEBUG ] connection detected need for sudo
    [ceph1.in][DEBUG ] connected to host: ceph1.in
    [ceph1.in][DEBUG ] detect platform information from remote host
    [ceph1.in][DEBUG ] detect machine type
    [ceph1.in][DEBUG ] write cluster configuration to /etc/ceph/{cluster}.conf
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy mgr ceph3.in ceph4.in
    usage: ceph-deploy mgr [-h] {create} ...
    ceph-deploy mgr: error: argument subcommand: invalid choice: 'ceph3.in' (choose from 'create')
    [cephadm@ceph2 ceph_cluster]$ vim ~/.ssh/config
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy mgr ceph3.in ceph4.in
    usage: ceph-deploy mgr [-h] {create} ...
    ceph-deploy mgr: error: argument subcommand: invalid choice: 'ceph3.in' (choose from 'create')
    [cephadm@ceph2 ceph_cluster]$ vim ~/.ssh/config
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy mgr ceph3 ceph4
    usage: ceph-deploy mgr [-h] {create} ...
    ceph-deploy mgr: error: argument subcommand: invalid choice: 'ceph3' (choose from 'create')
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy mgr create ceph3.in ceph4.in
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy mgr create ceph3.in ceph4.in
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  mgr                           : [('ceph3.in', 'ceph3.in'), ('ceph4.in', 'ceph4.in')]
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  subcommand                    : create
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7fe65e951b90>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  func                          : <function mgr at 0x7fe65f23c230>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.mgr][DEBUG ] Deploying mgr, cluster ceph hosts ceph3.in:ceph3.in ceph4.in:ceph4.in
    [ceph3.in][DEBUG ] connection detected need for sudo
    [ceph3.in][DEBUG ] connected to host: ceph3.in
    [ceph3.in][DEBUG ] detect platform information from remote host
    [ceph3.in][DEBUG ] detect machine type
    [ceph_deploy.mgr][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph_deploy.mgr][DEBUG ] remote host will use systemd
    [ceph_deploy.mgr][DEBUG ] deploying mgr bootstrap to ceph3.in
    [ceph3.in][DEBUG ] write cluster configuration to /etc/ceph/{cluster}.conf
    [ceph3.in][WARNIN] mgr keyring does not exist yet, creating one
    [ceph3.in][DEBUG ] create a keyring file
    [ceph3.in][DEBUG ] create path recursively if it doesn't exist
    [ceph3.in][INFO  ] Running command: sudo ceph --cluster ceph --name client.bootstrap-mgr --keyring /var/lib/ceph/bootstrap-mgr/ceph.keyring auth get-or-create mgr.ceph3.in mon allow profile mgr osd allow * mds allow * -o /var/lib/ceph/mgr/ceph-ceph3.in/keyring
    [ceph3.in][INFO  ] Running command: sudo systemctl enable ceph-mgr@ceph3.in
    [ceph3.in][WARNIN] Created symlink from /etc/systemd/system/ceph-mgr.target.wants/ceph-mgr@ceph3.in.service to /usr/lib/systemd/system/ceph-mgr@.service.
    [ceph3.in][INFO  ] Running command: sudo systemctl start ceph-mgr@ceph3.in
    [ceph3.in][INFO  ] Running command: sudo systemctl enable ceph.target
    [ceph4.in][DEBUG ] connection detected need for sudo
    [ceph4.in][DEBUG ] connected to host: ceph4.in
    [ceph4.in][DEBUG ] detect platform information from remote host
    [ceph4.in][DEBUG ] detect machine type
    [ceph_deploy.mgr][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph_deploy.mgr][DEBUG ] remote host will use systemd
    [ceph_deploy.mgr][DEBUG ] deploying mgr bootstrap to ceph4.in
    [ceph4.in][DEBUG ] write cluster configuration to /etc/ceph/{cluster}.conf
    [ceph4.in][WARNIN] mgr keyring does not exist yet, creating one
    [ceph4.in][DEBUG ] create a keyring file
    [ceph4.in][DEBUG ] create path recursively if it doesn't exist
    [ceph4.in][INFO  ] Running command: sudo ceph --cluster ceph --name client.bootstrap-mgr --keyring /var/lib/ceph/bootstrap-mgr/ceph.keyring auth get-or-create mgr.ceph4.in mon allow profile mgr osd allow * mds allow * -o /var/lib/ceph/mgr/ceph-ceph4.in/keyring
    [ceph4.in][INFO  ] Running command: sudo systemctl enable ceph-mgr@ceph4.in
    [ceph4.in][WARNIN] Created symlink from /etc/systemd/system/ceph-mgr.target.wants/ceph-mgr@ceph4.in.service to /usr/lib/systemd/system/ceph-mgr@.service.
    [ceph4.in][INFO  ] Running command: sudo systemctl start ceph-mgr@ceph4.in
    [ceph4.in][INFO  ] Running command: sudo systemctl enable ceph.target
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy disk list  ceph3.in ceph4.in
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy disk list ceph3.in ceph4.in
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  debug                         : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  subcommand                    : list
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7fa2a79c97e8>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  host                          : ['ceph3.in', 'ceph4.in']
    [ceph_deploy.cli][INFO  ]  func                          : <function disk at 0x7fa2a7c17a28>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph3.in][DEBUG ] connection detected need for sudo
    [ceph3.in][DEBUG ] connected to host: ceph3.in
    [ceph3.in][DEBUG ] detect platform information from remote host
    [ceph3.in][DEBUG ] detect machine type
    [ceph3.in][DEBUG ] find the location of an executable
    [ceph3.in][INFO  ] Running command: sudo fdisk -l
    [ceph3.in][INFO  ] Disk /dev/sda: 21.5 GB, 21474836480 bytes, 41943040 sectors
    [ceph3.in][INFO  ] Disk /dev/sdb: 21.5 GB, 21474836480 bytes, 41943040 sectors
    [ceph3.in][INFO  ] Disk /dev/sdc: 21.5 GB, 21474836480 bytes, 41943040 sectors
    [ceph3.in][INFO  ] Disk /dev/sdd: 21.5 GB, 21474836480 bytes, 41943040 sectors
    [ceph3.in][INFO  ] Disk /dev/mapper/centos-root: 18.2 GB, 18249416704 bytes, 35643392 sectors
    [ceph3.in][INFO  ] Disk /dev/mapper/centos-swap: 2147 MB, 2147483648 bytes, 4194304 sectors
    [ceph4.in][DEBUG ] connection detected need for sudo
    [ceph4.in][DEBUG ] connected to host: ceph4.in
    [ceph4.in][DEBUG ] detect platform information from remote host
    [ceph4.in][DEBUG ] detect machine type
    [ceph4.in][DEBUG ] find the location of an executable
    [ceph4.in][INFO  ] Running command: sudo fdisk -l
    [ceph4.in][INFO  ] Disk /dev/sdb: 21.5 GB, 21474836480 bytes, 41943040 sectors
    [ceph4.in][INFO  ] Disk /dev/sdc: 21.5 GB, 21474836480 bytes, 41943040 sectors
    [ceph4.in][INFO  ] Disk /dev/sdd: 21.5 GB, 21474836480 bytes, 41943040 sectors
    [ceph4.in][INFO  ] Disk /dev/sda: 21.5 GB, 21474836480 bytes, 41943040 sectors
    [ceph4.in][INFO  ] Disk /dev/mapper/centos-root: 18.2 GB, 18249416704 bytes, 35643392 sectors
    [ceph4.in][INFO  ] Disk /dev/mapper/centos-swap: 2147 MB, 2147483648 bytes, 4194304 sectors
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy disk zap ceph3.in /dev/sdb
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy disk zap ceph3.in /dev/sdb
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  debug                         : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  subcommand                    : zap
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f8a6a8047e8>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  host                          : ceph3.in
    [ceph_deploy.cli][INFO  ]  func                          : <function disk at 0x7f8a6aa52a28>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  disk                          : ['/dev/sdb']
    [ceph_deploy.osd][DEBUG ] zapping /dev/sdb on ceph3.in
    [ceph3.in][DEBUG ] connection detected need for sudo
    [ceph3.in][DEBUG ] connected to host: ceph3.in
    [ceph3.in][DEBUG ] detect platform information from remote host
    [ceph3.in][DEBUG ] detect machine type
    [ceph3.in][DEBUG ] find the location of an executable
    [ceph_deploy.osd][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph3.in][DEBUG ] zeroing last few blocks of device
    [ceph3.in][DEBUG ] find the location of an executable
    [ceph3.in][INFO  ] Running command: sudo /usr/sbin/ceph-volume lvm zap /dev/sdb
    [ceph3.in][WARNIN] --> Zapping: /dev/sdb
    [ceph3.in][WARNIN] --> --destroy was not specified, but zapping a whole device will remove the partition table
    [ceph3.in][WARNIN] Running command: /bin/dd if=/dev/zero of=/dev/sdb bs=1M count=10 conv=fsync
    [ceph3.in][WARNIN]  stderr: 10+0 records in
    [ceph3.in][WARNIN] 10+0 records out
    [ceph3.in][WARNIN] 10485760 bytes (10 MB) copied, 0.0332592 s, 315 MB/s
    [ceph3.in][WARNIN] --> Zapping successful for: <Raw Device: /dev/sdb>
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy disk zap ceph3.in /dev/sdc
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy disk zap ceph3.in /dev/sdc
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  debug                         : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  subcommand                    : zap
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f5cae6207e8>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  host                          : ceph3.in
    [ceph_deploy.cli][INFO  ]  func                          : <function disk at 0x7f5cae86ea28>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  disk                          : ['/dev/sdc']
    [ceph_deploy.osd][DEBUG ] zapping /dev/sdc on ceph3.in
    [ceph3.in][DEBUG ] connection detected need for sudo
    [ceph3.in][DEBUG ] connected to host: ceph3.in
    [ceph3.in][DEBUG ] detect platform information from remote host
    [ceph3.in][DEBUG ] detect machine type
    [ceph3.in][DEBUG ] find the location of an executable
    [ceph_deploy.osd][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph3.in][DEBUG ] zeroing last few blocks of device
    [ceph3.in][DEBUG ] find the location of an executable
    [ceph3.in][INFO  ] Running command: sudo /usr/sbin/ceph-volume lvm zap /dev/sdc
    [ceph3.in][WARNIN] --> Zapping: /dev/sdc
    [ceph3.in][WARNIN] --> --destroy was not specified, but zapping a whole device will remove the partition table
    [ceph3.in][WARNIN] Running command: /bin/dd if=/dev/zero of=/dev/sdc bs=1M count=10 conv=fsync
    [ceph3.in][WARNIN]  stderr: 10+0 records in
    [ceph3.in][WARNIN] 10+0 records out
    [ceph3.in][WARNIN] 10485760 bytes (10 MB) copied, 0.0313767 s, 334 MB/s
    [ceph3.in][WARNIN] --> Zapping successful for: <Raw Device: /dev/sdc>
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy disk zap ceph3.in /dev/sdd
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy disk zap ceph3.in /dev/sdd
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  debug                         : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  subcommand                    : zap
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f5890fd37e8>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  host                          : ceph3.in
    [ceph_deploy.cli][INFO  ]  func                          : <function disk at 0x7f5891221a28>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  disk                          : ['/dev/sdd']
    [ceph_deploy.osd][DEBUG ] zapping /dev/sdd on ceph3.in
    [ceph3.in][DEBUG ] connection detected need for sudo
    [ceph3.in][DEBUG ] connected to host: ceph3.in
    [ceph3.in][DEBUG ] detect platform information from remote host
    [ceph3.in][DEBUG ] detect machine type
    [ceph3.in][DEBUG ] find the location of an executable
    [ceph_deploy.osd][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph3.in][DEBUG ] zeroing last few blocks of device
    [ceph3.in][DEBUG ] find the location of an executable
    [ceph3.in][INFO  ] Running command: sudo /usr/sbin/ceph-volume lvm zap /dev/sdd
    [ceph3.in][WARNIN] --> Zapping: /dev/sdd
    [ceph3.in][WARNIN] --> --destroy was not specified, but zapping a whole device will remove the partition table
    [ceph3.in][WARNIN] Running command: /bin/dd if=/dev/zero of=/dev/sdd bs=1M count=10 conv=fsync
    [ceph3.in][WARNIN] --> Zapping successful for: <Raw Device: /dev/sdd>
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy disk zap ceph4.in /dev/sdb
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy disk zap ceph4.in /dev/sdb
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  debug                         : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  subcommand                    : zap
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f993c79c7e8>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  host                          : ceph4.in
    [ceph_deploy.cli][INFO  ]  func                          : <function disk at 0x7f993c9eaa28>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  disk                          : ['/dev/sdb']
    [ceph_deploy.osd][DEBUG ] zapping /dev/sdb on ceph4.in
    [ceph4.in][DEBUG ] connection detected need for sudo
    [ceph4.in][DEBUG ] connected to host: ceph4.in
    [ceph4.in][DEBUG ] detect platform information from remote host
    [ceph4.in][DEBUG ] detect machine type
    [ceph4.in][DEBUG ] find the location of an executable
    [ceph_deploy.osd][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph4.in][DEBUG ] zeroing last few blocks of device
    [ceph4.in][DEBUG ] find the location of an executable
    [ceph4.in][INFO  ] Running command: sudo /usr/sbin/ceph-volume lvm zap /dev/sdb
    [ceph4.in][WARNIN] --> Zapping: /dev/sdb
    [ceph4.in][WARNIN] --> --destroy was not specified, but zapping a whole device will remove the partition table
    [ceph4.in][WARNIN] Running command: /bin/dd if=/dev/zero of=/dev/sdb bs=1M count=10 conv=fsync
    [ceph4.in][WARNIN] --> Zapping successful for: <Raw Device: /dev/sdb>
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy disk zap ceph4.in /dev/sdc
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy disk zap ceph4.in /dev/sdc
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  debug                         : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  subcommand                    : zap
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7fa7eeb8c7e8>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  host                          : ceph4.in
    [ceph_deploy.cli][INFO  ]  func                          : <function disk at 0x7fa7eeddaa28>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  disk                          : ['/dev/sdc']
    [ceph_deploy.osd][DEBUG ] zapping /dev/sdc on ceph4.in
    [ceph4.in][DEBUG ] connection detected need for sudo
    [ceph4.in][DEBUG ] connected to host: ceph4.in
    [ceph4.in][DEBUG ] detect platform information from remote host
    [ceph4.in][DEBUG ] detect machine type
    [ceph4.in][DEBUG ] find the location of an executable
    [ceph_deploy.osd][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph4.in][DEBUG ] zeroing last few blocks of device
    [ceph4.in][DEBUG ] find the location of an executable
    [ceph4.in][INFO  ] Running command: sudo /usr/sbin/ceph-volume lvm zap /dev/sdc
    [ceph4.in][WARNIN] --> Zapping: /dev/sdc
    [ceph4.in][WARNIN] --> --destroy was not specified, but zapping a whole device will remove the partition table
    [ceph4.in][WARNIN] Running command: /bin/dd if=/dev/zero of=/dev/sdc bs=1M count=10 conv=fsync
    [ceph4.in][WARNIN]  stderr: 10+0 records in
    [ceph4.in][WARNIN] 10+0 records out
    [ceph4.in][WARNIN] 10485760 bytes (10 MB) copied, 0.0320149 s, 328 MB/s
    [ceph4.in][WARNIN] --> Zapping successful for: <Raw Device: /dev/sdc>
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy disk zap ceph4.in /dev/sdd
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy disk zap ceph4.in /dev/sdd
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  debug                         : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  subcommand                    : zap
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f291d6977e8>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  host                          : ceph4.in
    [ceph_deploy.cli][INFO  ]  func                          : <function disk at 0x7f291d8e5a28>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  disk                          : ['/dev/sdd']
    [ceph_deploy.osd][DEBUG ] zapping /dev/sdd on ceph4.in
    [ceph4.in][DEBUG ] connection detected need for sudo
    [ceph4.in][DEBUG ] connected to host: ceph4.in
    [ceph4.in][DEBUG ] detect platform information from remote host
    [ceph4.in][DEBUG ] detect machine type
    [ceph4.in][DEBUG ] find the location of an executable
    [ceph_deploy.osd][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph4.in][DEBUG ] zeroing last few blocks of device
    [ceph4.in][DEBUG ] find the location of an executable
    [ceph4.in][INFO  ] Running command: sudo /usr/sbin/ceph-volume lvm zap /dev/sdd
    [ceph4.in][WARNIN] --> Zapping: /dev/sdd
    [ceph4.in][WARNIN] --> --destroy was not specified, but zapping a whole device will remove the partition table
    [ceph4.in][WARNIN] Running command: /bin/dd if=/dev/zero of=/dev/sdd bs=1M count=10 conv=fsync
    [ceph4.in][WARNIN]  stderr: 10+0 records in
    [ceph4.in][WARNIN] 10+0 records out
    [ceph4.in][WARNIN] 10485760 bytes (10 MB) copied, 0.00841474 s, 1.2 GB/s
    [ceph4.in][WARNIN] --> Zapping successful for: <Raw Device: /dev/sdd>
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy osd create --data /dev/sdb ceph3.in
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy osd create --data /dev/sdb ceph3.in
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  bluestore                     : None
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f6cca27f908>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  fs_type                       : xfs
    [ceph_deploy.cli][INFO  ]  block_wal                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  journal                       : None
    [ceph_deploy.cli][INFO  ]  subcommand                    : create
    [ceph_deploy.cli][INFO  ]  host                          : ceph3.in
    [ceph_deploy.cli][INFO  ]  filestore                     : None
    [ceph_deploy.cli][INFO  ]  func                          : <function osd at 0x7f6cca4c89b0>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  zap_disk                      : False
    [ceph_deploy.cli][INFO  ]  data                          : /dev/sdb
    [ceph_deploy.cli][INFO  ]  block_db                      : None
    [ceph_deploy.cli][INFO  ]  dmcrypt                       : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  dmcrypt_key_dir               : /etc/ceph/dmcrypt-keys
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  debug                         : False
    [ceph_deploy.osd][DEBUG ] Creating OSD on cluster ceph with data device /dev/sdb
    [ceph3.in][DEBUG ] connection detected need for sudo
    [ceph3.in][DEBUG ] connected to host: ceph3.in
    [ceph3.in][DEBUG ] detect platform information from remote host
    [ceph3.in][DEBUG ] detect machine type
    [ceph3.in][DEBUG ] find the location of an executable
    [ceph_deploy.osd][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph_deploy.osd][DEBUG ] Deploying osd to ceph3.in
    [ceph3.in][DEBUG ] write cluster configuration to /etc/ceph/{cluster}.conf
    [ceph3.in][WARNIN] osd keyring does not exist yet, creating one
    [ceph3.in][DEBUG ] create a keyring file
    [ceph3.in][DEBUG ] find the location of an executable
    [ceph3.in][INFO  ] Running command: sudo /usr/sbin/ceph-volume --cluster ceph lvm create --bluestore --data /dev/sdb
    [ceph3.in][WARNIN] Running command: /bin/ceph-authtool --gen-print-key
    [ceph3.in][WARNIN] Running command: /bin/ceph --cluster ceph --name client.bootstrap-osd --keyring /var/lib/ceph/bootstrap-osd/ceph.keyring -i - osd new d787705e-f3ac-4137-96b1-3a53f307ac16
    [ceph3.in][WARNIN] Running command: /sbin/vgcreate --force --yes ceph-d4f8dcba-5e3e-4149-b37f-7858202b5677 /dev/sdb
    [ceph3.in][WARNIN]  stdout: Physical volume "/dev/sdb" successfully created.
    [ceph3.in][WARNIN]  stdout: Volume group "ceph-d4f8dcba-5e3e-4149-b37f-7858202b5677" successfully created
    [ceph3.in][WARNIN] Running command: /sbin/lvcreate --yes -l 100%FREE -n osd-block-d787705e-f3ac-4137-96b1-3a53f307ac16 ceph-d4f8dcba-5e3e-4149-b37f-7858202b5677
    [ceph3.in][WARNIN]  stdout: Logical volume "osd-block-d787705e-f3ac-4137-96b1-3a53f307ac16" created.
    [ceph3.in][WARNIN] Running command: /bin/ceph-authtool --gen-print-key
    [ceph3.in][WARNIN] Running command: /bin/mount -t tmpfs tmpfs /var/lib/ceph/osd/ceph-0
    [ceph3.in][WARNIN] Running command: /bin/chown -h ceph:ceph /dev/ceph-d4f8dcba-5e3e-4149-b37f-7858202b5677/osd-block-d787705e-f3ac-4137-96b1-3a53f307ac16
    [ceph3.in][WARNIN] Running command: /bin/chown -R ceph:ceph /dev/dm-2
    [ceph3.in][WARNIN] Running command: /bin/ln -s /dev/ceph-d4f8dcba-5e3e-4149-b37f-7858202b5677/osd-block-d787705e-f3ac-4137-96b1-3a53f307ac16 /var/lib/ceph/osd/ceph-0/block
    [ceph3.in][WARNIN] Running command: /bin/ceph --cluster ceph --name client.bootstrap-osd --keyring /var/lib/ceph/bootstrap-osd/ceph.keyring mon getmap -o /var/lib/ceph/osd/ceph-0/activate.monmap
    [ceph3.in][WARNIN]  stderr: got monmap epoch 1
    [ceph3.in][WARNIN] Running command: /bin/ceph-authtool /var/lib/ceph/osd/ceph-0/keyring --create-keyring --name osd.0 --add-key AQD4HrRkY70FHhAAwcA3MKO/yMBNjAdzE7XuRA==
    [ceph3.in][WARNIN]  stdout: creating /var/lib/ceph/osd/ceph-0/keyring
    [ceph3.in][WARNIN] added entity osd.0 auth auth(auid = 18446744073709551615 key=AQD4HrRkY70FHhAAwcA3MKO/yMBNjAdzE7XuRA== with 0 caps)
    [ceph3.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-0/keyring
    [ceph3.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-0/
    [ceph3.in][WARNIN] Running command: /bin/ceph-osd --cluster ceph --osd-objectstore bluestore --mkfs -i 0 --monmap /var/lib/ceph/osd/ceph-0/activate.monmap --keyfile - --osd-data /var/lib/ceph/osd/ceph-0/ --osd-uuid d787705e-f3ac-4137-96b1-3a53f307ac16 --setuser ceph --setgroup ceph
    [ceph3.in][WARNIN] --> ceph-volume lvm prepare successful for: /dev/sdb
    [ceph3.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-0
    [ceph3.in][WARNIN] Running command: /bin/ceph-bluestore-tool --cluster=ceph prime-osd-dir --dev /dev/ceph-d4f8dcba-5e3e-4149-b37f-7858202b5677/osd-block-d787705e-f3ac-4137-96b1-3a53f307ac16 --path /var/lib/ceph/osd/ceph-0 --no-mon-config
    [ceph3.in][WARNIN] Running command: /bin/ln -snf /dev/ceph-d4f8dcba-5e3e-4149-b37f-7858202b5677/osd-block-d787705e-f3ac-4137-96b1-3a53f307ac16 /var/lib/ceph/osd/ceph-0/block
    [ceph3.in][WARNIN] Running command: /bin/chown -h ceph:ceph /var/lib/ceph/osd/ceph-0/block
    [ceph3.in][WARNIN] Running command: /bin/chown -R ceph:ceph /dev/dm-2
    [ceph3.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-0
    [ceph3.in][WARNIN] Running command: /bin/systemctl enable ceph-volume@lvm-0-d787705e-f3ac-4137-96b1-3a53f307ac16
    [ceph3.in][WARNIN]  stderr: Created symlink from /etc/systemd/system/multi-user.target.wants/ceph-volume@lvm-0-d787705e-f3ac-4137-96b1-3a53f307ac16.service to /usr/lib/systemd/system/ceph-volume@.service.
    [ceph3.in][WARNIN] Running command: /bin/systemctl enable --runtime ceph-osd@0
    [ceph3.in][WARNIN]  stderr: Created symlink from /run/systemd/system/ceph-osd.target.wants/ceph-osd@0.service to /usr/lib/systemd/system/ceph-osd@.service.
    [ceph3.in][WARNIN] Running command: /bin/systemctl start ceph-osd@0
    [ceph3.in][WARNIN] --> ceph-volume lvm activate successful for osd ID: 0
    [ceph3.in][WARNIN] --> ceph-volume lvm create successful for: /dev/sdb
    [ceph3.in][INFO  ] checking OSD status...
    [ceph3.in][DEBUG ] find the location of an executable
    [ceph3.in][INFO  ] Running command: sudo /bin/ceph --cluster=ceph osd stat --format=json
    [ceph_deploy.osd][DEBUG ] Host ceph3.in is now ready for osd use.
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy osd create --data /dev/sdc ceph3.in
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy osd create --data /dev/sdc ceph3.in
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  bluestore                     : None
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f4edd306908>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  fs_type                       : xfs
    [ceph_deploy.cli][INFO  ]  block_wal                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  journal                       : None
    [ceph_deploy.cli][INFO  ]  subcommand                    : create
    [ceph_deploy.cli][INFO  ]  host                          : ceph3.in
    [ceph_deploy.cli][INFO  ]  filestore                     : None
    [ceph_deploy.cli][INFO  ]  func                          : <function osd at 0x7f4edd54f9b0>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  zap_disk                      : False
    [ceph_deploy.cli][INFO  ]  data                          : /dev/sdc
    [ceph_deploy.cli][INFO  ]  block_db                      : None
    [ceph_deploy.cli][INFO  ]  dmcrypt                       : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  dmcrypt_key_dir               : /etc/ceph/dmcrypt-keys
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  debug                         : False
    [ceph_deploy.osd][DEBUG ] Creating OSD on cluster ceph with data device /dev/sdc
    [ceph3.in][DEBUG ] connection detected need for sudo
    [ceph3.in][DEBUG ] connected to host: ceph3.in
    [ceph3.in][DEBUG ] detect platform information from remote host
    [ceph3.in][DEBUG ] detect machine type
    [ceph3.in][DEBUG ] find the location of an executable
    [ceph_deploy.osd][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph_deploy.osd][DEBUG ] Deploying osd to ceph3.in
    [ceph3.in][DEBUG ] write cluster configuration to /etc/ceph/{cluster}.conf
    [ceph3.in][DEBUG ] find the location of an executable
    [ceph3.in][INFO  ] Running command: sudo /usr/sbin/ceph-volume --cluster ceph lvm create --bluestore --data /dev/sdc
    [ceph3.in][WARNIN] Running command: /bin/ceph-authtool --gen-print-key
    [ceph3.in][WARNIN] Running command: /bin/ceph --cluster ceph --name client.bootstrap-osd --keyring /var/lib/ceph/bootstrap-osd/ceph.keyring -i - osd new b2f2d528-3c6d-49dc-98e7-c05c880231a7
    [ceph3.in][WARNIN] Running command: /sbin/vgcreate --force --yes ceph-e511ccfa-7a42-4cdb-b21e-3591ece0589e /dev/sdc
    [ceph3.in][WARNIN]  stdout: Physical volume "/dev/sdc" successfully created.
    [ceph3.in][WARNIN]  stdout: Volume group "ceph-e511ccfa-7a42-4cdb-b21e-3591ece0589e" successfully created
    [ceph3.in][WARNIN] Running command: /sbin/lvcreate --yes -l 100%FREE -n osd-block-b2f2d528-3c6d-49dc-98e7-c05c880231a7 ceph-e511ccfa-7a42-4cdb-b21e-3591ece0589e
    [ceph3.in][WARNIN]  stdout: Logical volume "osd-block-b2f2d528-3c6d-49dc-98e7-c05c880231a7" created.
    [ceph3.in][WARNIN] Running command: /bin/ceph-authtool --gen-print-key
    [ceph3.in][WARNIN] Running command: /bin/mount -t tmpfs tmpfs /var/lib/ceph/osd/ceph-1
    [ceph3.in][WARNIN] Running command: /bin/chown -h ceph:ceph /dev/ceph-e511ccfa-7a42-4cdb-b21e-3591ece0589e/osd-block-b2f2d528-3c6d-49dc-98e7-c05c880231a7
    [ceph3.in][WARNIN] Running command: /bin/chown -R ceph:ceph /dev/dm-3
    [ceph3.in][WARNIN] Running command: /bin/ln -s /dev/ceph-e511ccfa-7a42-4cdb-b21e-3591ece0589e/osd-block-b2f2d528-3c6d-49dc-98e7-c05c880231a7 /var/lib/ceph/osd/ceph-1/block
    [ceph3.in][WARNIN] Running command: /bin/ceph --cluster ceph --name client.bootstrap-osd --keyring /var/lib/ceph/bootstrap-osd/ceph.keyring mon getmap -o /var/lib/ceph/osd/ceph-1/activate.monmap
    [ceph3.in][WARNIN]  stderr: got monmap epoch 1
    [ceph3.in][WARNIN] Running command: /bin/ceph-authtool /var/lib/ceph/osd/ceph-1/keyring --create-keyring --name osd.1 --add-key AQALH7RkBHeTMRAAdVU74W1Ad8QY19XmBNtLnQ==
    [ceph3.in][WARNIN]  stdout: creating /var/lib/ceph/osd/ceph-1/keyring
    [ceph3.in][WARNIN] added entity osd.1 auth auth(auid = 18446744073709551615 key=AQALH7RkBHeTMRAAdVU74W1Ad8QY19XmBNtLnQ== with 0 caps)
    [ceph3.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-1/keyring
    [ceph3.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-1/
    [ceph3.in][WARNIN] Running command: /bin/ceph-osd --cluster ceph --osd-objectstore bluestore --mkfs -i 1 --monmap /var/lib/ceph/osd/ceph-1/activate.monmap --keyfile - --osd-data /var/lib/ceph/osd/ceph-1/ --osd-uuid b2f2d528-3c6d-49dc-98e7-c05c880231a7 --setuser ceph --setgroup ceph
    [ceph3.in][WARNIN] --> ceph-volume lvm prepare successful for: /dev/sdc
    [ceph3.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-1
    [ceph3.in][WARNIN] Running command: /bin/ceph-bluestore-tool --cluster=ceph prime-osd-dir --dev /dev/ceph-e511ccfa-7a42-4cdb-b21e-3591ece0589e/osd-block-b2f2d528-3c6d-49dc-98e7-c05c880231a7 --path /var/lib/ceph/osd/ceph-1 --no-mon-config
    [ceph3.in][WARNIN] Running command: /bin/ln -snf /dev/ceph-e511ccfa-7a42-4cdb-b21e-3591ece0589e/osd-block-b2f2d528-3c6d-49dc-98e7-c05c880231a7 /var/lib/ceph/osd/ceph-1/block
    [ceph3.in][WARNIN] Running command: /bin/chown -h ceph:ceph /var/lib/ceph/osd/ceph-1/block
    [ceph3.in][WARNIN] Running command: /bin/chown -R ceph:ceph /dev/dm-3
    [ceph3.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-1
    [ceph3.in][WARNIN] Running command: /bin/systemctl enable ceph-volume@lvm-1-b2f2d528-3c6d-49dc-98e7-c05c880231a7
    [ceph3.in][WARNIN]  stderr: Created symlink from /etc/systemd/system/multi-user.target.wants/ceph-volume@lvm-1-b2f2d528-3c6d-49dc-98e7-c05c880231a7.service to /usr/lib/systemd/system/ceph-volume@.service.
    [ceph3.in][WARNIN] Running command: /bin/systemctl enable --runtime ceph-osd@1
    [ceph3.in][WARNIN]  stderr: Created symlink from /run/systemd/system/ceph-osd.target.wants/ceph-osd@1.service to /usr/lib/systemd/system/ceph-osd@.service.
    [ceph3.in][WARNIN] Running command: /bin/systemctl start ceph-osd@1
    [ceph3.in][WARNIN] --> ceph-volume lvm activate successful for osd ID: 1
    [ceph3.in][WARNIN] --> ceph-volume lvm create successful for: /dev/sdc
    [ceph3.in][INFO  ] checking OSD status...
    [ceph3.in][DEBUG ] find the location of an executable
    [ceph3.in][INFO  ] Running command: sudo /bin/ceph --cluster=ceph osd stat --format=json
    [ceph_deploy.osd][DEBUG ] Host ceph3.in is now ready for osd use.
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy osd create --data /dev/sdd ceph3.in
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy osd create --data /dev/sdd ceph3.in
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  bluestore                     : None
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7fa3f54af908>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  fs_type                       : xfs
    [ceph_deploy.cli][INFO  ]  block_wal                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  journal                       : None
    [ceph_deploy.cli][INFO  ]  subcommand                    : create
    [ceph_deploy.cli][INFO  ]  host                          : ceph3.in
    [ceph_deploy.cli][INFO  ]  filestore                     : None
    [ceph_deploy.cli][INFO  ]  func                          : <function osd at 0x7fa3f56f89b0>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  zap_disk                      : False
    [ceph_deploy.cli][INFO  ]  data                          : /dev/sdd
    [ceph_deploy.cli][INFO  ]  block_db                      : None
    [ceph_deploy.cli][INFO  ]  dmcrypt                       : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  dmcrypt_key_dir               : /etc/ceph/dmcrypt-keys
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  debug                         : False
    [ceph_deploy.osd][DEBUG ] Creating OSD on cluster ceph with data device /dev/sdd
    [ceph3.in][DEBUG ] connection detected need for sudo
    [ceph3.in][DEBUG ] connected to host: ceph3.in
    [ceph3.in][DEBUG ] detect platform information from remote host
    [ceph3.in][DEBUG ] detect machine type
    [ceph3.in][DEBUG ] find the location of an executable
    [ceph_deploy.osd][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph_deploy.osd][DEBUG ] Deploying osd to ceph3.in
    [ceph3.in][DEBUG ] write cluster configuration to /etc/ceph/{cluster}.conf
    [ceph3.in][DEBUG ] find the location of an executable
    [ceph3.in][INFO  ] Running command: sudo /usr/sbin/ceph-volume --cluster ceph lvm create --bluestore --data /dev/sdd
    [ceph3.in][WARNIN] Running command: /bin/ceph-authtool --gen-print-key
    [ceph3.in][WARNIN] Running command: /bin/ceph --cluster ceph --name client.bootstrap-osd --keyring /var/lib/ceph/bootstrap-osd/ceph.keyring -i - osd new fc75cec3-77bc-4f71-85f1-af593f45c4ae
    [ceph3.in][WARNIN] Running command: /sbin/vgcreate --force --yes ceph-f807e80d-10e2-4c9d-be99-6d44cb1d0a8a /dev/sdd
    [ceph3.in][WARNIN]  stdout: Physical volume "/dev/sdd" successfully created.
    [ceph3.in][WARNIN]  stdout: Volume group "ceph-f807e80d-10e2-4c9d-be99-6d44cb1d0a8a" successfully created
    [ceph3.in][WARNIN] Running command: /sbin/lvcreate --yes -l 100%FREE -n osd-block-fc75cec3-77bc-4f71-85f1-af593f45c4ae ceph-f807e80d-10e2-4c9d-be99-6d44cb1d0a8a
    [ceph3.in][WARNIN]  stdout: Logical volume "osd-block-fc75cec3-77bc-4f71-85f1-af593f45c4ae" created.
    [ceph3.in][WARNIN] Running command: /bin/ceph-authtool --gen-print-key
    [ceph3.in][WARNIN] Running command: /bin/mount -t tmpfs tmpfs /var/lib/ceph/osd/ceph-2
    [ceph3.in][WARNIN] Running command: /bin/chown -h ceph:ceph /dev/ceph-f807e80d-10e2-4c9d-be99-6d44cb1d0a8a/osd-block-fc75cec3-77bc-4f71-85f1-af593f45c4ae
    [ceph3.in][WARNIN] Running command: /bin/chown -R ceph:ceph /dev/dm-4
    [ceph3.in][WARNIN] Running command: /bin/ln -s /dev/ceph-f807e80d-10e2-4c9d-be99-6d44cb1d0a8a/osd-block-fc75cec3-77bc-4f71-85f1-af593f45c4ae /var/lib/ceph/osd/ceph-2/block
    [ceph3.in][WARNIN] Running command: /bin/ceph --cluster ceph --name client.bootstrap-osd --keyring /var/lib/ceph/bootstrap-osd/ceph.keyring mon getmap -o /var/lib/ceph/osd/ceph-2/activate.monmap
    [ceph3.in][WARNIN]  stderr: got monmap epoch 1
    [ceph3.in][WARNIN] Running command: /bin/ceph-authtool /var/lib/ceph/osd/ceph-2/keyring --create-keyring --name osd.2 --add-key AQAlH7RkALa0OhAAtwUapm9WrO1RM3DuZ6tPNA==
    [ceph3.in][WARNIN]  stdout: creating /var/lib/ceph/osd/ceph-2/keyring
    [ceph3.in][WARNIN] added entity osd.2 auth auth(auid = 18446744073709551615 key=AQAlH7RkALa0OhAAtwUapm9WrO1RM3DuZ6tPNA== with 0 caps)
    [ceph3.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-2/keyring
    [ceph3.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-2/
    [ceph3.in][WARNIN] Running command: /bin/ceph-osd --cluster ceph --osd-objectstore bluestore --mkfs -i 2 --monmap /var/lib/ceph/osd/ceph-2/activate.monmap --keyfile - --osd-data /var/lib/ceph/osd/ceph-2/ --osd-uuid fc75cec3-77bc-4f71-85f1-af593f45c4ae --setuser ceph --setgroup ceph
    [ceph3.in][WARNIN] --> ceph-volume lvm prepare successful for: /dev/sdd
    [ceph3.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-2
    [ceph3.in][WARNIN] Running command: /bin/ceph-bluestore-tool --cluster=ceph prime-osd-dir --dev /dev/ceph-f807e80d-10e2-4c9d-be99-6d44cb1d0a8a/osd-block-fc75cec3-77bc-4f71-85f1-af593f45c4ae --path /var/lib/ceph/osd/ceph-2 --no-mon-config
    [ceph3.in][WARNIN] Running command: /bin/ln -snf /dev/ceph-f807e80d-10e2-4c9d-be99-6d44cb1d0a8a/osd-block-fc75cec3-77bc-4f71-85f1-af593f45c4ae /var/lib/ceph/osd/ceph-2/block
    [ceph3.in][WARNIN] Running command: /bin/chown -h ceph:ceph /var/lib/ceph/osd/ceph-2/block
    [ceph3.in][WARNIN] Running command: /bin/chown -R ceph:ceph /dev/dm-4
    [ceph3.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-2
    [ceph3.in][WARNIN] Running command: /bin/systemctl enable ceph-volume@lvm-2-fc75cec3-77bc-4f71-85f1-af593f45c4ae
    [ceph3.in][WARNIN]  stderr: Created symlink from /etc/systemd/system/multi-user.target.wants/ceph-volume@lvm-2-fc75cec3-77bc-4f71-85f1-af593f45c4ae.service to /usr/lib/systemd/system/ceph-volume@.service.
    [ceph3.in][WARNIN] Running command: /bin/systemctl enable --runtime ceph-osd@2
    [ceph3.in][WARNIN]  stderr: Created symlink from /run/systemd/system/ceph-osd.target.wants/ceph-osd@2.service to /usr/lib/systemd/system/ceph-osd@.service.
    [ceph3.in][WARNIN] Running command: /bin/systemctl start ceph-osd@2
    [ceph3.in][WARNIN] --> ceph-volume lvm activate successful for osd ID: 2
    [ceph3.in][WARNIN] --> ceph-volume lvm create successful for: /dev/sdd
    [ceph3.in][INFO  ] checking OSD status...
    [ceph3.in][DEBUG ] find the location of an executable
    [ceph3.in][INFO  ] Running command: sudo /bin/ceph --cluster=ceph osd stat --format=json
    [ceph_deploy.osd][DEBUG ] Host ceph3.in is now ready for osd use.
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy osd create --data /dev/sdb ceph4.in
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy osd create --data /dev/sdb ceph4.in
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  bluestore                     : None
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f06a8e4c908>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  fs_type                       : xfs
    [ceph_deploy.cli][INFO  ]  block_wal                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  journal                       : None
    [ceph_deploy.cli][INFO  ]  subcommand                    : create
    [ceph_deploy.cli][INFO  ]  host                          : ceph4.in
    [ceph_deploy.cli][INFO  ]  filestore                     : None
    [ceph_deploy.cli][INFO  ]  func                          : <function osd at 0x7f06a90959b0>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  zap_disk                      : False
    [ceph_deploy.cli][INFO  ]  data                          : /dev/sdb
    [ceph_deploy.cli][INFO  ]  block_db                      : None
    [ceph_deploy.cli][INFO  ]  dmcrypt                       : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  dmcrypt_key_dir               : /etc/ceph/dmcrypt-keys
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  debug                         : False
    [ceph_deploy.osd][DEBUG ] Creating OSD on cluster ceph with data device /dev/sdb
    [ceph4.in][DEBUG ] connection detected need for sudo
    [ceph4.in][DEBUG ] connected to host: ceph4.in
    [ceph4.in][DEBUG ] detect platform information from remote host
    [ceph4.in][DEBUG ] detect machine type
    [ceph4.in][DEBUG ] find the location of an executable
    [ceph_deploy.osd][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph_deploy.osd][DEBUG ] Deploying osd to ceph4.in
    [ceph4.in][DEBUG ] write cluster configuration to /etc/ceph/{cluster}.conf
    [ceph4.in][WARNIN] osd keyring does not exist yet, creating one
    [ceph4.in][DEBUG ] create a keyring file
    [ceph4.in][DEBUG ] find the location of an executable
    [ceph4.in][INFO  ] Running command: sudo /usr/sbin/ceph-volume --cluster ceph lvm create --bluestore --data /dev/sdb
    [ceph4.in][WARNIN] Running command: /bin/ceph-authtool --gen-print-key
    [ceph4.in][WARNIN] Running command: /bin/ceph --cluster ceph --name client.bootstrap-osd --keyring /var/lib/ceph/bootstrap-osd/ceph.keyring -i - osd new 3192bcbe-b46f-445e-8000-cdd8b52edccb
    [ceph4.in][WARNIN] Running command: /sbin/vgcreate --force --yes ceph-841583ad-6d37-4cc1-99a4-a17148e47f47 /dev/sdb
    [ceph4.in][WARNIN]  stdout: Physical volume "/dev/sdb" successfully created.
    [ceph4.in][WARNIN]  stdout: Volume group "ceph-841583ad-6d37-4cc1-99a4-a17148e47f47" successfully created
    [ceph4.in][WARNIN] Running command: /sbin/lvcreate --yes -l 100%FREE -n osd-block-3192bcbe-b46f-445e-8000-cdd8b52edccb ceph-841583ad-6d37-4cc1-99a4-a17148e47f47
    [ceph4.in][WARNIN]  stdout: Logical volume "osd-block-3192bcbe-b46f-445e-8000-cdd8b52edccb" created.
    [ceph4.in][WARNIN] Running command: /bin/ceph-authtool --gen-print-key
    [ceph4.in][WARNIN] Running command: /bin/mount -t tmpfs tmpfs /var/lib/ceph/osd/ceph-3
    [ceph4.in][WARNIN] Running command: /bin/chown -h ceph:ceph /dev/ceph-841583ad-6d37-4cc1-99a4-a17148e47f47/osd-block-3192bcbe-b46f-445e-8000-cdd8b52edccb
    [ceph4.in][WARNIN] Running command: /bin/chown -R ceph:ceph /dev/dm-2
    [ceph4.in][WARNIN] Running command: /bin/ln -s /dev/ceph-841583ad-6d37-4cc1-99a4-a17148e47f47/osd-block-3192bcbe-b46f-445e-8000-cdd8b52edccb /var/lib/ceph/osd/ceph-3/block
    [ceph4.in][WARNIN] Running command: /bin/ceph --cluster ceph --name client.bootstrap-osd --keyring /var/lib/ceph/bootstrap-osd/ceph.keyring mon getmap -o /var/lib/ceph/osd/ceph-3/activate.monmap
    [ceph4.in][WARNIN]  stderr: got monmap epoch 1
    [ceph4.in][WARNIN] Running command: /bin/ceph-authtool /var/lib/ceph/osd/ceph-3/keyring --create-keyring --name osd.3 --add-key AQA9H7RkXLPAEhAA4rBgfRTPN6r3u02Tb0jAWg==
    [ceph4.in][WARNIN]  stdout: creating /var/lib/ceph/osd/ceph-3/keyring
    [ceph4.in][WARNIN] added entity osd.3 auth auth(auid = 18446744073709551615 key=AQA9H7RkXLPAEhAA4rBgfRTPN6r3u02Tb0jAWg== with 0 caps)
    [ceph4.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-3/keyring
    [ceph4.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-3/
    [ceph4.in][WARNIN] Running command: /bin/ceph-osd --cluster ceph --osd-objectstore bluestore --mkfs -i 3 --monmap /var/lib/ceph/osd/ceph-3/activate.monmap --keyfile - --osd-data /var/lib/ceph/osd/ceph-3/ --osd-uuid 3192bcbe-b46f-445e-8000-cdd8b52edccb --setuser ceph --setgroup ceph
    [ceph4.in][WARNIN] --> ceph-volume lvm prepare successful for: /dev/sdb
    [ceph4.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-3
    [ceph4.in][WARNIN] Running command: /bin/ceph-bluestore-tool --cluster=ceph prime-osd-dir --dev /dev/ceph-841583ad-6d37-4cc1-99a4-a17148e47f47/osd-block-3192bcbe-b46f-445e-8000-cdd8b52edccb --path /var/lib/ceph/osd/ceph-3 --no-mon-config
    [ceph4.in][WARNIN] Running command: /bin/ln -snf /dev/ceph-841583ad-6d37-4cc1-99a4-a17148e47f47/osd-block-3192bcbe-b46f-445e-8000-cdd8b52edccb /var/lib/ceph/osd/ceph-3/block
    [ceph4.in][WARNIN] Running command: /bin/chown -h ceph:ceph /var/lib/ceph/osd/ceph-3/block
    [ceph4.in][WARNIN] Running command: /bin/chown -R ceph:ceph /dev/dm-2
    [ceph4.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-3
    [ceph4.in][WARNIN] Running command: /bin/systemctl enable ceph-volume@lvm-3-3192bcbe-b46f-445e-8000-cdd8b52edccb
    [ceph4.in][WARNIN]  stderr: Created symlink from /etc/systemd/system/multi-user.target.wants/ceph-volume@lvm-3-3192bcbe-b46f-445e-8000-cdd8b52edccb.service to /usr/lib/systemd/system/ceph-volume@.service.
    [ceph4.in][WARNIN] Running command: /bin/systemctl enable --runtime ceph-osd@3
    [ceph4.in][WARNIN]  stderr: Created symlink from /run/systemd/system/ceph-osd.target.wants/ceph-osd@3.service to /usr/lib/systemd/system/ceph-osd@.service.
    [ceph4.in][WARNIN] Running command: /bin/systemctl start ceph-osd@3
    [ceph4.in][WARNIN] --> ceph-volume lvm activate successful for osd ID: 3
    [ceph4.in][WARNIN] --> ceph-volume lvm create successful for: /dev/sdb
    [ceph4.in][INFO  ] checking OSD status...
    [ceph4.in][DEBUG ] find the location of an executable
    [ceph4.in][INFO  ] Running command: sudo /bin/ceph --cluster=ceph osd stat --format=json
    [ceph_deploy.osd][DEBUG ] Host ceph4.in is now ready for osd use.
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy osd create --data /dev/sdc ceph4.in
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy osd create --data /dev/sdc ceph4.in
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  bluestore                     : None
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f1dd6605908>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  fs_type                       : xfs
    [ceph_deploy.cli][INFO  ]  block_wal                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  journal                       : None
    [ceph_deploy.cli][INFO  ]  subcommand                    : create
    [ceph_deploy.cli][INFO  ]  host                          : ceph4.in
    [ceph_deploy.cli][INFO  ]  filestore                     : None
    [ceph_deploy.cli][INFO  ]  func                          : <function osd at 0x7f1dd684e9b0>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  zap_disk                      : False
    [ceph_deploy.cli][INFO  ]  data                          : /dev/sdc
    [ceph_deploy.cli][INFO  ]  block_db                      : None
    [ceph_deploy.cli][INFO  ]  dmcrypt                       : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  dmcrypt_key_dir               : /etc/ceph/dmcrypt-keys
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  debug                         : False
    [ceph_deploy.osd][DEBUG ] Creating OSD on cluster ceph with data device /dev/sdc
    [ceph4.in][DEBUG ] connection detected need for sudo
    [ceph4.in][DEBUG ] connected to host: ceph4.in
    [ceph4.in][DEBUG ] detect platform information from remote host
    [ceph4.in][DEBUG ] detect machine type
    [ceph4.in][DEBUG ] find the location of an executable
    [ceph_deploy.osd][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph_deploy.osd][DEBUG ] Deploying osd to ceph4.in
    [ceph4.in][DEBUG ] write cluster configuration to /etc/ceph/{cluster}.conf
    [ceph4.in][DEBUG ] find the location of an executable
    [ceph4.in][INFO  ] Running command: sudo /usr/sbin/ceph-volume --cluster ceph lvm create --bluestore --data /dev/sdc
    [ceph4.in][WARNIN] Running command: /bin/ceph-authtool --gen-print-key
    [ceph4.in][WARNIN] Running command: /bin/ceph --cluster ceph --name client.bootstrap-osd --keyring /var/lib/ceph/bootstrap-osd/ceph.keyring -i - osd new 337748c0-eb0b-4894-a3df-784963069ce8
    [ceph4.in][WARNIN] Running command: /sbin/vgcreate --force --yes ceph-9fcf00bd-3680-4f0b-a2bc-a5586d5af937 /dev/sdc
    [ceph4.in][WARNIN]  stdout: Physical volume "/dev/sdc" successfully created.
    [ceph4.in][WARNIN]  stdout: Volume group "ceph-9fcf00bd-3680-4f0b-a2bc-a5586d5af937" successfully created
    [ceph4.in][WARNIN] Running command: /sbin/lvcreate --yes -l 100%FREE -n osd-block-337748c0-eb0b-4894-a3df-784963069ce8 ceph-9fcf00bd-3680-4f0b-a2bc-a5586d5af937
    [ceph4.in][WARNIN]  stdout: Logical volume "osd-block-337748c0-eb0b-4894-a3df-784963069ce8" created.
    [ceph4.in][WARNIN] Running command: /bin/ceph-authtool --gen-print-key
    [ceph4.in][WARNIN] Running command: /bin/mount -t tmpfs tmpfs /var/lib/ceph/osd/ceph-4
    [ceph4.in][WARNIN] Running command: /bin/chown -h ceph:ceph /dev/ceph-9fcf00bd-3680-4f0b-a2bc-a5586d5af937/osd-block-337748c0-eb0b-4894-a3df-784963069ce8
    [ceph4.in][WARNIN] Running command: /bin/chown -R ceph:ceph /dev/dm-3
    [ceph4.in][WARNIN] Running command: /bin/ln -s /dev/ceph-9fcf00bd-3680-4f0b-a2bc-a5586d5af937/osd-block-337748c0-eb0b-4894-a3df-784963069ce8 /var/lib/ceph/osd/ceph-4/block
    [ceph4.in][WARNIN] Running command: /bin/ceph --cluster ceph --name client.bootstrap-osd --keyring /var/lib/ceph/bootstrap-osd/ceph.keyring mon getmap -o /var/lib/ceph/osd/ceph-4/activate.monmap
    [ceph4.in][WARNIN]  stderr: got monmap epoch 1
    [ceph4.in][WARNIN] Running command: /bin/ceph-authtool /var/lib/ceph/osd/ceph-4/keyring --create-keyring --name osd.4 --add-key AQBNH7RkoGkqGhAADrmJGCtwfoyufW2AY0Eecw==
    [ceph4.in][WARNIN]  stdout: creating /var/lib/ceph/osd/ceph-4/keyring
    [ceph4.in][WARNIN] added entity osd.4 auth auth(auid = 18446744073709551615 key=AQBNH7RkoGkqGhAADrmJGCtwfoyufW2AY0Eecw== with 0 caps)
    [ceph4.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-4/keyring
    [ceph4.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-4/
    [ceph4.in][WARNIN] Running command: /bin/ceph-osd --cluster ceph --osd-objectstore bluestore --mkfs -i 4 --monmap /var/lib/ceph/osd/ceph-4/activate.monmap --keyfile - --osd-data /var/lib/ceph/osd/ceph-4/ --osd-uuid 337748c0-eb0b-4894-a3df-784963069ce8 --setuser ceph --setgroup ceph
    [ceph4.in][WARNIN] --> ceph-volume lvm prepare successful for: /dev/sdc
    [ceph4.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-4
    [ceph4.in][WARNIN] Running command: /bin/ceph-bluestore-tool --cluster=ceph prime-osd-dir --dev /dev/ceph-9fcf00bd-3680-4f0b-a2bc-a5586d5af937/osd-block-337748c0-eb0b-4894-a3df-784963069ce8 --path /var/lib/ceph/osd/ceph-4 --no-mon-config
    [ceph4.in][WARNIN] Running command: /bin/ln -snf /dev/ceph-9fcf00bd-3680-4f0b-a2bc-a5586d5af937/osd-block-337748c0-eb0b-4894-a3df-784963069ce8 /var/lib/ceph/osd/ceph-4/block
    [ceph4.in][WARNIN] Running command: /bin/chown -h ceph:ceph /var/lib/ceph/osd/ceph-4/block
    [ceph4.in][WARNIN] Running command: /bin/chown -R ceph:ceph /dev/dm-3
    [ceph4.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-4
    [ceph4.in][WARNIN] Running command: /bin/systemctl enable ceph-volume@lvm-4-337748c0-eb0b-4894-a3df-784963069ce8
    [ceph4.in][WARNIN]  stderr: Created symlink from /etc/systemd/system/multi-user.target.wants/ceph-volume@lvm-4-337748c0-eb0b-4894-a3df-784963069ce8.service to /usr/lib/systemd/system/ceph-volume@.service.
    [ceph4.in][WARNIN] Running command: /bin/systemctl enable --runtime ceph-osd@4
    [ceph4.in][WARNIN]  stderr: Created symlink from /run/systemd/system/ceph-osd.target.wants/ceph-osd@4.service to /usr/lib/systemd/system/ceph-osd@.service.
    [ceph4.in][WARNIN] Running command: /bin/systemctl start ceph-osd@4
    [ceph4.in][WARNIN] --> ceph-volume lvm activate successful for osd ID: 4
    [ceph4.in][WARNIN] --> ceph-volume lvm create successful for: /dev/sdc
    [ceph4.in][INFO  ] checking OSD status...
    [ceph4.in][DEBUG ] find the location of an executable
    [ceph4.in][INFO  ] Running command: sudo /bin/ceph --cluster=ceph osd stat --format=json
    [ceph_deploy.osd][DEBUG ] Host ceph4.in is now ready for osd use.
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy osd create --data /dev/sdd ceph4.in
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy osd create --data /dev/sdd ceph4.in
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  bluestore                     : None
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f4a8f79d908>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  fs_type                       : xfs
    [ceph_deploy.cli][INFO  ]  block_wal                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  journal                       : None
    [ceph_deploy.cli][INFO  ]  subcommand                    : create
    [ceph_deploy.cli][INFO  ]  host                          : ceph4.in
    [ceph_deploy.cli][INFO  ]  filestore                     : None
    [ceph_deploy.cli][INFO  ]  func                          : <function osd at 0x7f4a8f9e69b0>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  zap_disk                      : False
    [ceph_deploy.cli][INFO  ]  data                          : /dev/sdd
    [ceph_deploy.cli][INFO  ]  block_db                      : None
    [ceph_deploy.cli][INFO  ]  dmcrypt                       : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  dmcrypt_key_dir               : /etc/ceph/dmcrypt-keys
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  debug                         : False
    [ceph_deploy.osd][DEBUG ] Creating OSD on cluster ceph with data device /dev/sdd
    [ceph4.in][DEBUG ] connection detected need for sudo
    [ceph4.in][DEBUG ] connected to host: ceph4.in
    [ceph4.in][DEBUG ] detect platform information from remote host
    [ceph4.in][DEBUG ] detect machine type
    [ceph4.in][DEBUG ] find the location of an executable
    [ceph_deploy.osd][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph_deploy.osd][DEBUG ] Deploying osd to ceph4.in
    [ceph4.in][DEBUG ] write cluster configuration to /etc/ceph/{cluster}.conf
    [ceph4.in][DEBUG ] find the location of an executable
    [ceph4.in][INFO  ] Running command: sudo /usr/sbin/ceph-volume --cluster ceph lvm create --bluestore --data /dev/sdd
    [ceph4.in][WARNIN] Running command: /bin/ceph-authtool --gen-print-key
    [ceph4.in][WARNIN] Running command: /bin/ceph --cluster ceph --name client.bootstrap-osd --keyring /var/lib/ceph/bootstrap-osd/ceph.keyring -i - osd new 6a9a338f-2ce9-48e3-ba98-1b2363c0652d
    [ceph4.in][WARNIN] Running command: /sbin/vgcreate --force --yes ceph-8a118ba5-6373-48f0-807a-88d030de1441 /dev/sdd
    [ceph4.in][WARNIN]  stdout: Physical volume "/dev/sdd" successfully created.
    [ceph4.in][WARNIN]  stdout: Volume group "ceph-8a118ba5-6373-48f0-807a-88d030de1441" successfully created
    [ceph4.in][WARNIN] Running command: /sbin/lvcreate --yes -l 100%FREE -n osd-block-6a9a338f-2ce9-48e3-ba98-1b2363c0652d ceph-8a118ba5-6373-48f0-807a-88d030de1441
    [ceph4.in][WARNIN]  stdout: Logical volume "osd-block-6a9a338f-2ce9-48e3-ba98-1b2363c0652d" created.
    [ceph4.in][WARNIN] Running command: /bin/ceph-authtool --gen-print-key
    [ceph4.in][WARNIN] Running command: /bin/mount -t tmpfs tmpfs /var/lib/ceph/osd/ceph-5
    [ceph4.in][WARNIN] Running command: /bin/chown -h ceph:ceph /dev/ceph-8a118ba5-6373-48f0-807a-88d030de1441/osd-block-6a9a338f-2ce9-48e3-ba98-1b2363c0652d
    [ceph4.in][WARNIN] Running command: /bin/chown -R ceph:ceph /dev/dm-4
    [ceph4.in][WARNIN] Running command: /bin/ln -s /dev/ceph-8a118ba5-6373-48f0-807a-88d030de1441/osd-block-6a9a338f-2ce9-48e3-ba98-1b2363c0652d /var/lib/ceph/osd/ceph-5/block
    [ceph4.in][WARNIN] Running command: /bin/ceph --cluster ceph --name client.bootstrap-osd --keyring /var/lib/ceph/bootstrap-osd/ceph.keyring mon getmap -o /var/lib/ceph/osd/ceph-5/activate.monmap
    [ceph4.in][WARNIN]  stderr: got monmap epoch 1
    [ceph4.in][WARNIN] Running command: /bin/ceph-authtool /var/lib/ceph/osd/ceph-5/keyring --create-keyring --name osd.5 --add-key AQBbH7RkLxpoARAAeGEYFvwpUWpHSNEgQrsWvg==
    [ceph4.in][WARNIN]  stdout: creating /var/lib/ceph/osd/ceph-5/keyring
    [ceph4.in][WARNIN] added entity osd.5 auth auth(auid = 18446744073709551615 key=AQBbH7RkLxpoARAAeGEYFvwpUWpHSNEgQrsWvg== with 0 caps)
    [ceph4.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-5/keyring
    [ceph4.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-5/
    [ceph4.in][WARNIN] Running command: /bin/ceph-osd --cluster ceph --osd-objectstore bluestore --mkfs -i 5 --monmap /var/lib/ceph/osd/ceph-5/activate.monmap --keyfile - --osd-data /var/lib/ceph/osd/ceph-5/ --osd-uuid 6a9a338f-2ce9-48e3-ba98-1b2363c0652d --setuser ceph --setgroup ceph
    [ceph4.in][WARNIN] --> ceph-volume lvm prepare successful for: /dev/sdd
    [ceph4.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-5
    [ceph4.in][WARNIN] Running command: /bin/ceph-bluestore-tool --cluster=ceph prime-osd-dir --dev /dev/ceph-8a118ba5-6373-48f0-807a-88d030de1441/osd-block-6a9a338f-2ce9-48e3-ba98-1b2363c0652d --path /var/lib/ceph/osd/ceph-5 --no-mon-config
    [ceph4.in][WARNIN] Running command: /bin/ln -snf /dev/ceph-8a118ba5-6373-48f0-807a-88d030de1441/osd-block-6a9a338f-2ce9-48e3-ba98-1b2363c0652d /var/lib/ceph/osd/ceph-5/block
    [ceph4.in][WARNIN] Running command: /bin/chown -h ceph:ceph /var/lib/ceph/osd/ceph-5/block
    [ceph4.in][WARNIN] Running command: /bin/chown -R ceph:ceph /dev/dm-4
    [ceph4.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-5
    [ceph4.in][WARNIN] Running command: /bin/systemctl enable ceph-volume@lvm-5-6a9a338f-2ce9-48e3-ba98-1b2363c0652d
    [ceph4.in][WARNIN]  stderr: Created symlink from /etc/systemd/system/multi-user.target.wants/ceph-volume@lvm-5-6a9a338f-2ce9-48e3-ba98-1b2363c0652d.service to /usr/lib/systemd/system/ceph-volume@.service.
    [ceph4.in][WARNIN] Running command: /bin/systemctl enable --runtime ceph-osd@5
    [ceph4.in][WARNIN]  stderr: Created symlink from /run/systemd/system/ceph-osd.target.wants/ceph-osd@5.service to /usr/lib/systemd/system/ceph-osd@.service.
    [ceph4.in][WARNIN] Running command: /bin/systemctl start ceph-osd@5
    [ceph4.in][WARNIN] --> ceph-volume lvm activate successful for osd ID: 5
    [ceph4.in][WARNIN] --> ceph-volume lvm create successful for: /dev/sdd
    [ceph4.in][INFO  ] checking OSD status...
    [ceph4.in][DEBUG ] find the location of an executable
    [ceph4.in][INFO  ] Running command: sudo /bin/ceph --cluster=ceph osd stat --format=json
    [ceph_deploy.osd][DEBUG ] Host ceph4.in is now ready for osd use.
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy install ceph5.in
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy install ceph5.in
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  testing                       : None
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7ff2b4f3d5a8>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  dev_commit                    : None
    [ceph_deploy.cli][INFO  ]  install_mds                   : False
    [ceph_deploy.cli][INFO  ]  stable                        : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  adjust_repos                  : True
    [ceph_deploy.cli][INFO  ]  func                          : <function install at 0x7ff2b55896e0>
    [ceph_deploy.cli][INFO  ]  install_mgr                   : False
    [ceph_deploy.cli][INFO  ]  install_all                   : False
    [ceph_deploy.cli][INFO  ]  repo                          : False
    [ceph_deploy.cli][INFO  ]  host                          : ['ceph5.in']
    [ceph_deploy.cli][INFO  ]  install_rgw                   : False
    [ceph_deploy.cli][INFO  ]  install_tests                 : False
    [ceph_deploy.cli][INFO  ]  repo_url                      : None
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  install_osd                   : False
    [ceph_deploy.cli][INFO  ]  version_kind                  : stable
    [ceph_deploy.cli][INFO  ]  install_common                : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  dev                           : master
    [ceph_deploy.cli][INFO  ]  nogpgcheck                    : False
    [ceph_deploy.cli][INFO  ]  local_mirror                  : None
    [ceph_deploy.cli][INFO  ]  release                       : None
    [ceph_deploy.cli][INFO  ]  install_mon                   : False
    [ceph_deploy.cli][INFO  ]  gpg_url                       : None
    [ceph_deploy.install][DEBUG ] Installing stable version mimic on cluster ceph hosts ceph5.in
    [ceph_deploy.install][DEBUG ] Detecting platform for host ceph5.in ...
    [ceph5.in][DEBUG ] connection detected need for sudo
    [ceph5.in][DEBUG ] connected to host: ceph5.in
    [ceph5.in][DEBUG ] detect platform information from remote host
    [ceph5.in][DEBUG ] detect machine type
    [ceph_deploy.install][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph5.in][INFO  ] installing Ceph on ceph5.in
    [ceph5.in][INFO  ] Running command: sudo yum clean all
    [ceph5.in][DEBUG ] Loaded plugins: fastestmirror
    [ceph5.in][DEBUG ] Cleaning repos: base epel extras updates
    [ceph5.in][DEBUG ] Cleaning up list of fastest mirrors
    [ceph5.in][INFO  ] Running command: sudo yum -y install epel-release
    [ceph5.in][DEBUG ] Loaded plugins: fastestmirror
    [ceph5.in][DEBUG ] Determining fastest mirrors
    [ceph5.in][DEBUG ]  * base: centos.mirror.net.in
    [ceph5.in][DEBUG ]  * epel: epel.excellmedia.net
    [ceph5.in][DEBUG ]  * extras: centos.mirror.net.in
    [ceph5.in][DEBUG ]  * updates: centos.mirror.net.in
    [ceph5.in][DEBUG ] Package epel-release-7-14.noarch already installed and latest version
    [ceph5.in][DEBUG ] Nothing to do
    [ceph5.in][INFO  ] Running command: sudo yum -y install yum-plugin-priorities
    [ceph5.in][DEBUG ] Loaded plugins: fastestmirror
    [ceph5.in][DEBUG ] Loading mirror speeds from cached hostfile
    [ceph5.in][DEBUG ]  * base: centos.mirror.net.in
    [ceph5.in][DEBUG ]  * epel: epel.excellmedia.net
    [ceph5.in][DEBUG ]  * extras: centos.mirror.net.in
    [ceph5.in][DEBUG ]  * updates: centos.mirror.net.in
    [ceph5.in][DEBUG ] Resolving Dependencies
    [ceph5.in][DEBUG ] --> Running transaction check
    [ceph5.in][DEBUG ] ---> Package yum-plugin-priorities.noarch 0:1.1.31-54.el7_8 will be installed
    [ceph5.in][DEBUG ] --> Finished Dependency Resolution
    [ceph5.in][DEBUG ]
    [ceph5.in][DEBUG ] Dependencies Resolved
    [ceph5.in][DEBUG ]
    [ceph5.in][DEBUG ] ================================================================================
    [ceph5.in][DEBUG ]  Package                    Arch        Version                 Repository
    [ceph5.in][DEBUG ]                                                                            Size
    [ceph5.in][DEBUG ] ================================================================================
    [ceph5.in][DEBUG ] Installing:
    [ceph5.in][DEBUG ]  yum-plugin-priorities      noarch      1.1.31-54.el7_8         base       29 k
    [ceph5.in][DEBUG ]
    [ceph5.in][DEBUG ] Transaction Summary
    [ceph5.in][DEBUG ] ================================================================================
    [ceph5.in][DEBUG ] Install  1 Package
    [ceph5.in][DEBUG ]
    [ceph5.in][DEBUG ] Total download size: 29 k
    [ceph5.in][DEBUG ] Installed size: 28 k
    [ceph5.in][DEBUG ] Downloading packages:
    [ceph5.in][DEBUG ] Running transaction check
    [ceph5.in][DEBUG ] Running transaction test
    [ceph5.in][DEBUG ] Transaction test succeeded
    [ceph5.in][DEBUG ] Running transaction
    [ceph5.in][DEBUG ]   Installing : yum-plugin-priorities-1.1.31-54.el7_8.noarch                 1/1
    [ceph5.in][DEBUG ]   Verifying  : yum-plugin-priorities-1.1.31-54.el7_8.noarch                 1/1
    [ceph5.in][DEBUG ]
    [ceph5.in][DEBUG ] Installed:
    [ceph5.in][DEBUG ]   yum-plugin-priorities.noarch 0:1.1.31-54.el7_8
    [ceph5.in][DEBUG ]
    [ceph5.in][DEBUG ] Complete!
    [ceph5.in][DEBUG ] Configure Yum priorities to include obsoletes
    [ceph5.in][WARNIN] check_obsoletes has been enabled for Yum priorities plugin
    [ceph5.in][INFO  ] Running command: sudo rpm --import https://download.ceph.com/keys/release.asc
    [ceph5.in][INFO  ] Running command: sudo yum remove -y ceph-release
    [ceph5.in][DEBUG ] Loaded plugins: fastestmirror, priorities
    [ceph5.in][WARNIN] No Match for argument: ceph-release
    [ceph5.in][DEBUG ] No Packages marked for removal
    [ceph5.in][INFO  ] Running command: sudo yum install -y https://download.ceph.com/rpm-mimic/el7/noarch/ceph-release-1-0.el7.noarch.rpm
    [ceph5.in][DEBUG ] Loaded plugins: fastestmirror, priorities
    [ceph5.in][DEBUG ] Examining /var/tmp/yum-root-DmlpGq/ceph-release-1-0.el7.noarch.rpm: ceph-release-1-1.el7.noarch
    [ceph5.in][DEBUG ] Marking /var/tmp/yum-root-DmlpGq/ceph-release-1-0.el7.noarch.rpm to be installed
    [ceph5.in][DEBUG ] Resolving Dependencies
    [ceph5.in][DEBUG ] --> Running transaction check
    [ceph5.in][DEBUG ] ---> Package ceph-release.noarch 0:1-1.el7 will be installed
    [ceph5.in][DEBUG ] --> Finished Dependency Resolution
    [ceph5.in][DEBUG ]
    [ceph5.in][DEBUG ] Dependencies Resolved
    [ceph5.in][DEBUG ]
    [ceph5.in][DEBUG ] ================================================================================
    [ceph5.in][DEBUG ]  Package          Arch       Version     Repository                        Size
    [ceph5.in][DEBUG ] ================================================================================
    [ceph5.in][DEBUG ] Installing:
    [ceph5.in][DEBUG ]  ceph-release     noarch     1-1.el7     /ceph-release-1-0.el7.noarch     535
    [ceph5.in][DEBUG ]
    [ceph5.in][DEBUG ] Transaction Summary
    [ceph5.in][DEBUG ] ================================================================================
    [ceph5.in][DEBUG ] Install  1 Package
    [ceph5.in][DEBUG ]
    [ceph5.in][DEBUG ] Total size: 535
    [ceph5.in][DEBUG ] Installed size: 535
    [ceph5.in][DEBUG ] Downloading packages:
    [ceph5.in][DEBUG ] Running transaction check
    [ceph5.in][DEBUG ] Running transaction test
    [ceph5.in][DEBUG ] Transaction test succeeded
    [ceph5.in][DEBUG ] Running transaction
    [ceph5.in][DEBUG ]   Installing : ceph-release-1-1.el7.noarch                                  1/1
    [ceph5.in][DEBUG ]   Verifying  : ceph-release-1-1.el7.noarch                                  1/1
    [ceph5.in][DEBUG ]
    [ceph5.in][DEBUG ] Installed:
    [ceph5.in][DEBUG ]   ceph-release.noarch 0:1-1.el7
    [ceph5.in][DEBUG ]
    [ceph5.in][DEBUG ] Complete!
    [ceph5.in][WARNIN] ensuring that /etc/yum.repos.d/ceph.repo contains a high priority
    [ceph5.in][WARNIN] altered ceph.repo priorities to contain: priority=1
    [ceph5.in][INFO  ] Running command: sudo yum -y install ceph ceph-radosgw
    [ceph5.in][DEBUG ] Loaded plugins: fastestmirror, priorities
    [ceph5.in][DEBUG ] Loading mirror speeds from cached hostfile
    [ceph5.in][DEBUG ]  * base: centos.mirror.net.in
    [ceph5.in][DEBUG ]  * epel: epel.excellmedia.net
    [ceph5.in][DEBUG ]  * extras: centos.mirror.net.in
    [ceph5.in][DEBUG ]  * updates: centos.mirror.net.in
    [ceph5.in][DEBUG ] 8 packages excluded due to repository priority protections
    [ceph5.in][DEBUG ] Resolving Dependencies
    [ceph5.in][DEBUG ] --> Running transaction check
    [ceph5.in][DEBUG ] ---> Package ceph.x86_64 2:13.2.10-0.el7 will be installed
    [ceph5.in][DEBUG ] --> Processing Dependency: ceph-mds = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: ceph-osd = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: ceph-mon = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: ceph-mgr = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] ---> Package ceph-radosgw.x86_64 2:13.2.10-0.el7 will be installed
    [ceph5.in][DEBUG ] --> Processing Dependency: ceph-base = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: ceph-selinux = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: librgw2 = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: librados2 = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: mailcap for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: librados.so.2()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: libtcmalloc.so.4()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: libibverbs.so.1()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: liboath.so.0()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: libceph-common.so.0()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Running transaction check
    [ceph5.in][DEBUG ] ---> Package ceph-base.x86_64 2:13.2.10-0.el7 will be installed
    [ceph5.in][DEBUG ] --> Processing Dependency: libcephfs2 = 2:13.2.10-0.el7 for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: librbd1 = 2:13.2.10-0.el7 for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: ceph-common = 2:13.2.10-0.el7 for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: gdisk for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: python-setuptools for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: psmisc for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: cryptsetup for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: python-requests for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: libleveldb.so.1()(64bit) for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: libfuse.so.2()(64bit) for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: liblttng-ust.so.0()(64bit) for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] ---> Package ceph-mds.x86_64 2:13.2.10-0.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package ceph-mgr.x86_64 2:13.2.10-0.el7 will be installed
    [ceph5.in][DEBUG ] --> Processing Dependency: python-cherrypy for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: python-werkzeug for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: python-six for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: python-routes for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: python-bcrypt for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: python-pecan for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: pyOpenSSL for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: python-jinja2 for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] ---> Package ceph-mon.x86_64 2:13.2.10-0.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package ceph-osd.x86_64 2:13.2.10-0.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package ceph-selinux.x86_64 2:13.2.10-0.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package gperftools-libs.x86_64 0:2.6.1-1.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package libibverbs.x86_64 0:22.4-6.el7_9 will be installed
    [ceph5.in][DEBUG ] --> Processing Dependency: rdma-core(x86-64) = 22.4-6.el7_9 for package: libibverbs-22.4-6.el7_9.x86_64
    [ceph5.in][DEBUG ] ---> Package liboath.x86_64 0:2.6.2-1.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package librados2.x86_64 2:13.2.10-0.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package librgw2.x86_64 2:13.2.10-0.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package mailcap.noarch 0:2.1.41-2.el7 will be installed
    [ceph5.in][DEBUG ] --> Running transaction check
    [ceph5.in][DEBUG ] ---> Package ceph-common.x86_64 2:13.2.10-0.el7 will be installed
    [ceph5.in][DEBUG ] --> Processing Dependency: python-cephfs = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: libradosstriper1 = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: python-rgw = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: python-rbd = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: python-rados = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: python-ceph-argparse = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: python-prettytable for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: libbabeltrace-ctf.so.1()(64bit) for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: libbabeltrace.so.1()(64bit) for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: libradosstriper.so.1()(64bit) for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph5.in][DEBUG ] ---> Package cryptsetup.x86_64 0:2.0.3-6.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package fuse-libs.x86_64 0:2.9.2-11.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package gdisk.x86_64 0:0.8.10-3.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package leveldb.x86_64 0:1.12.0-11.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package libcephfs2.x86_64 2:13.2.10-0.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package librbd1.x86_64 2:13.2.10-0.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package lttng-ust.x86_64 0:2.4.1-4.el7 will be installed
    [ceph5.in][DEBUG ] --> Processing Dependency: liburcu-bp.so.1()(64bit) for package: lttng-ust-2.4.1-4.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: liburcu-cds.so.1()(64bit) for package: lttng-ust-2.4.1-4.el7.x86_64
    [ceph5.in][DEBUG ] ---> Package psmisc.x86_64 0:22.20-17.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package pyOpenSSL.x86_64 0:0.13.1-4.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package python-cherrypy.noarch 0:3.2.2-4.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package python-jinja2.noarch 0:2.7.2-4.el7 will be installed
    [ceph5.in][DEBUG ] --> Processing Dependency: python-babel >= 0.8 for package: python-jinja2-2.7.2-4.el7.noarch
    [ceph5.in][DEBUG ] --> Processing Dependency: python-markupsafe for package: python-jinja2-2.7.2-4.el7.noarch
    [ceph5.in][DEBUG ] ---> Package python-pecan.noarch 0:0.4.5-2.el7 will be installed
    [ceph5.in][DEBUG ] --> Processing Dependency: python-mako >= 0.4.0 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph5.in][DEBUG ] --> Processing Dependency: python-simplegeneric >= 0.8 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph5.in][DEBUG ] --> Processing Dependency: python-webob >= 1.2 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph5.in][DEBUG ] --> Processing Dependency: python-webtest >= 1.3.1 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph5.in][DEBUG ] --> Processing Dependency: python-singledispatch for package: python-pecan-0.4.5-2.el7.noarch
    [ceph5.in][DEBUG ] ---> Package python-requests.noarch 0:2.6.0-10.el7 will be installed
    [ceph5.in][DEBUG ] --> Processing Dependency: python-urllib3 >= 1.10.2-1 for package: python-requests-2.6.0-10.el7.noarch
    [ceph5.in][DEBUG ] --> Processing Dependency: python-chardet >= 2.2.1-1 for package: python-requests-2.6.0-10.el7.noarch
    [ceph5.in][DEBUG ] ---> Package python-routes.noarch 0:1.13-2.el7 will be installed
    [ceph5.in][DEBUG ] --> Processing Dependency: python-repoze-lru for package: python-routes-1.13-2.el7.noarch
    [ceph5.in][DEBUG ] ---> Package python-setuptools.noarch 0:0.9.8-7.el7 will be installed
    [ceph5.in][DEBUG ] --> Processing Dependency: python-backports-ssl_match_hostname for package: python-setuptools-0.9.8-7.el7.noarch
    [ceph5.in][DEBUG ] ---> Package python-six.noarch 0:1.9.0-2.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package python-werkzeug.noarch 0:0.9.1-2.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package python2-bcrypt.x86_64 0:3.1.6-2.el7 will be installed
    [ceph5.in][DEBUG ] --> Processing Dependency: python-cffi for package: python2-bcrypt-3.1.6-2.el7.x86_64
    [ceph5.in][DEBUG ] --> Processing Dependency: python2-six for package: python2-bcrypt-3.1.6-2.el7.x86_64
    [ceph5.in][DEBUG ] ---> Package rdma-core.x86_64 0:22.4-6.el7_9 will be installed
    [ceph5.in][DEBUG ] --> Processing Dependency: pciutils for package: rdma-core-22.4-6.el7_9.x86_64
    [ceph5.in][DEBUG ] --> Running transaction check
    [ceph5.in][DEBUG ] ---> Package libbabeltrace.x86_64 0:1.2.4-3.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package libradosstriper1.x86_64 2:13.2.10-0.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package pciutils.x86_64 0:3.5.1-3.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package python-babel.noarch 0:0.9.6-8.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package python-backports-ssl_match_hostname.noarch 0:3.5.0.1-1.el7 will be installed
    [ceph5.in][DEBUG ] --> Processing Dependency: python-ipaddress for package: python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch
    [ceph5.in][DEBUG ] --> Processing Dependency: python-backports for package: python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch
    [ceph5.in][DEBUG ] ---> Package python-ceph-argparse.x86_64 2:13.2.10-0.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package python-cephfs.x86_64 2:13.2.10-0.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package python-cffi.x86_64 0:1.6.0-5.el7 will be installed
    [ceph5.in][DEBUG ] --> Processing Dependency: python-pycparser for package: python-cffi-1.6.0-5.el7.x86_64
    [ceph5.in][DEBUG ] ---> Package python-chardet.noarch 0:2.2.1-3.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package python-mako.noarch 0:0.8.1-2.el7 will be installed
    [ceph5.in][DEBUG ] --> Processing Dependency: python-beaker for package: python-mako-0.8.1-2.el7.noarch
    [ceph5.in][DEBUG ] ---> Package python-markupsafe.x86_64 0:0.11-10.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package python-prettytable.noarch 0:0.7.2-3.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package python-rados.x86_64 2:13.2.10-0.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package python-rbd.x86_64 2:13.2.10-0.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package python-repoze-lru.noarch 0:0.4-3.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package python-rgw.x86_64 2:13.2.10-0.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package python-simplegeneric.noarch 0:0.8-7.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package python-singledispatch.noarch 0:3.4.0.2-2.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package python-urllib3.noarch 0:1.10.2-7.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package python-webob.noarch 0:1.2.3-7.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package python-webtest.noarch 0:1.3.4-6.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package python2-six.noarch 0:1.9.0-0.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package userspace-rcu.x86_64 0:0.7.16-1.el7 will be installed
    [ceph5.in][DEBUG ] --> Running transaction check
    [ceph5.in][DEBUG ] ---> Package python-backports.x86_64 0:1.0-8.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package python-beaker.noarch 0:1.5.4-10.el7 will be installed
    [ceph5.in][DEBUG ] --> Processing Dependency: python-paste for package: python-beaker-1.5.4-10.el7.noarch
    [ceph5.in][DEBUG ] ---> Package python-ipaddress.noarch 0:1.0.16-2.el7 will be installed
    [ceph5.in][DEBUG ] ---> Package python-pycparser.noarch 0:2.14-1.el7 will be installed
    [ceph5.in][DEBUG ] --> Processing Dependency: python-ply for package: python-pycparser-2.14-1.el7.noarch
    [ceph5.in][DEBUG ] --> Running transaction check
    [ceph5.in][DEBUG ] ---> Package python-paste.noarch 0:1.7.5.1-9.20111221hg1498.el7 will be installed
    [ceph5.in][DEBUG ] --> Processing Dependency: python-tempita for package: python-paste-1.7.5.1-9.20111221hg1498.el7.noarch
    [ceph5.in][DEBUG ] ---> Package python-ply.noarch 0:3.4-11.el7 will be installed
    [ceph5.in][DEBUG ] --> Running transaction check
    [ceph5.in][DEBUG ] ---> Package python-tempita.noarch 0:0.5.1-6.el7 will be installed
    [ceph5.in][DEBUG ] --> Finished Dependency Resolution
    [ceph5.in][DEBUG ]
    [ceph5.in][DEBUG ] Dependencies Resolved
    [ceph5.in][DEBUG ]
    [ceph5.in][DEBUG ] ================================================================================
    [ceph5.in][DEBUG ]  Package                      Arch   Version                      Repository
    [ceph5.in][DEBUG ]                                                                            Size
    [ceph5.in][DEBUG ] ================================================================================
    [ceph5.in][DEBUG ] Installing:
    [ceph5.in][DEBUG ]  ceph                         x86_64 2:13.2.10-0.el7              Ceph    3.0 k
    [ceph5.in][DEBUG ]  ceph-radosgw                 x86_64 2:13.2.10-0.el7              Ceph    4.5 M
    [ceph5.in][DEBUG ] Installing for dependencies:
    [ceph5.in][DEBUG ]  ceph-base                    x86_64 2:13.2.10-0.el7              Ceph    4.8 M
    [ceph5.in][DEBUG ]  ceph-common                  x86_64 2:13.2.10-0.el7              Ceph     14 M
    [ceph5.in][DEBUG ]  ceph-mds                     x86_64 2:13.2.10-0.el7              Ceph    1.7 M
    [ceph5.in][DEBUG ]  ceph-mgr                     x86_64 2:13.2.10-0.el7              Ceph    3.5 M
    [ceph5.in][DEBUG ]  ceph-mon                     x86_64 2:13.2.10-0.el7              Ceph    3.9 M
    [ceph5.in][DEBUG ]  ceph-osd                     x86_64 2:13.2.10-0.el7              Ceph     13 M
    [ceph5.in][DEBUG ]  ceph-selinux                 x86_64 2:13.2.10-0.el7              Ceph     21 k
    [ceph5.in][DEBUG ]  cryptsetup                   x86_64 2.0.3-6.el7                  base    154 k
    [ceph5.in][DEBUG ]  fuse-libs                    x86_64 2.9.2-11.el7                 base     93 k
    [ceph5.in][DEBUG ]  gdisk                        x86_64 0.8.10-3.el7                 base    190 k
    [ceph5.in][DEBUG ]  gperftools-libs              x86_64 2.6.1-1.el7                  base    272 k
    [ceph5.in][DEBUG ]  leveldb                      x86_64 1.12.0-11.el7                epel    161 k
    [ceph5.in][DEBUG ]  libbabeltrace                x86_64 1.2.4-3.el7                  epel    147 k
    [ceph5.in][DEBUG ]  libcephfs2                   x86_64 2:13.2.10-0.el7              Ceph    434 k
    [ceph5.in][DEBUG ]  libibverbs                   x86_64 22.4-6.el7_9                 updates 269 k
    [ceph5.in][DEBUG ]  liboath                      x86_64 2.6.2-1.el7                  epel     51 k
    [ceph5.in][DEBUG ]  librados2                    x86_64 2:13.2.10-0.el7              Ceph    2.9 M
    [ceph5.in][DEBUG ]  libradosstriper1             x86_64 2:13.2.10-0.el7              Ceph    329 k
    [ceph5.in][DEBUG ]  librbd1                      x86_64 2:13.2.10-0.el7              Ceph    1.2 M
    [ceph5.in][DEBUG ]  librgw2                      x86_64 2:13.2.10-0.el7              Ceph    2.0 M
    [ceph5.in][DEBUG ]  lttng-ust                    x86_64 2.4.1-4.el7                  epel    176 k
    [ceph5.in][DEBUG ]  mailcap                      noarch 2.1.41-2.el7                 base     31 k
    [ceph5.in][DEBUG ]  pciutils                     x86_64 3.5.1-3.el7                  base     93 k
    [ceph5.in][DEBUG ]  psmisc                       x86_64 22.20-17.el7                 base    141 k
    [ceph5.in][DEBUG ]  pyOpenSSL                    x86_64 0.13.1-4.el7                 base    135 k
    [ceph5.in][DEBUG ]  python-babel                 noarch 0.9.6-8.el7                  base    1.4 M
    [ceph5.in][DEBUG ]  python-backports             x86_64 1.0-8.el7                    base    5.8 k
    [ceph5.in][DEBUG ]  python-backports-ssl_match_hostname
    [ceph5.in][DEBUG ]                               noarch 3.5.0.1-1.el7                base     13 k
    [ceph5.in][DEBUG ]  python-beaker                noarch 1.5.4-10.el7                 base     80 k
    [ceph5.in][DEBUG ]  python-ceph-argparse         x86_64 2:13.2.10-0.el7              Ceph     34 k
    [ceph5.in][DEBUG ]  python-cephfs                x86_64 2:13.2.10-0.el7              Ceph     87 k
    [ceph5.in][DEBUG ]  python-cffi                  x86_64 1.6.0-5.el7                  base    218 k
    [ceph5.in][DEBUG ]  python-chardet               noarch 2.2.1-3.el7                  base    227 k
    [ceph5.in][DEBUG ]  python-cherrypy              noarch 3.2.2-4.el7                  base    422 k
    [ceph5.in][DEBUG ]  python-ipaddress             noarch 1.0.16-2.el7                 base     34 k
    [ceph5.in][DEBUG ]  python-jinja2                noarch 2.7.2-4.el7                  base    519 k
    [ceph5.in][DEBUG ]  python-mako                  noarch 0.8.1-2.el7                  base    307 k
    [ceph5.in][DEBUG ]  python-markupsafe            x86_64 0.11-10.el7                  base     25 k
    [ceph5.in][DEBUG ]  python-paste                 noarch 1.7.5.1-9.20111221hg1498.el7 base    866 k
    [ceph5.in][DEBUG ]  python-pecan                 noarch 0.4.5-2.el7                  epel    255 k
    [ceph5.in][DEBUG ]  python-ply                   noarch 3.4-11.el7                   base    123 k
    [ceph5.in][DEBUG ]  python-prettytable           noarch 0.7.2-3.el7                  base     37 k
    [ceph5.in][DEBUG ]  python-pycparser             noarch 2.14-1.el7                   base    104 k
    [ceph5.in][DEBUG ]  python-rados                 x86_64 2:13.2.10-0.el7              Ceph    189 k
    [ceph5.in][DEBUG ]  python-rbd                   x86_64 2:13.2.10-0.el7              Ceph    132 k
    [ceph5.in][DEBUG ]  python-repoze-lru            noarch 0.4-3.el7                    epel     13 k
    [ceph5.in][DEBUG ]  python-requests              noarch 2.6.0-10.el7                 base     95 k
    [ceph5.in][DEBUG ]  python-rgw                   x86_64 2:13.2.10-0.el7              Ceph     76 k
    [ceph5.in][DEBUG ]  python-routes                noarch 1.13-2.el7                   epel    640 k
    [ceph5.in][DEBUG ]  python-setuptools            noarch 0.9.8-7.el7                  base    397 k
    [ceph5.in][DEBUG ]  python-simplegeneric         noarch 0.8-7.el7                    epel     12 k
    [ceph5.in][DEBUG ]  python-singledispatch        noarch 3.4.0.2-2.el7                epel     18 k
    [ceph5.in][DEBUG ]  python-six                   noarch 1.9.0-2.el7                  base     29 k
    [ceph5.in][DEBUG ]  python-tempita               noarch 0.5.1-6.el7                  base     33 k
    [ceph5.in][DEBUG ]  python-urllib3               noarch 1.10.2-7.el7                 base    103 k
    [ceph5.in][DEBUG ]  python-webob                 noarch 1.2.3-7.el7                  base    202 k
    [ceph5.in][DEBUG ]  python-webtest               noarch 1.3.4-6.el7                  base    102 k
    [ceph5.in][DEBUG ]  python-werkzeug              noarch 0.9.1-2.el7                  extras  562 k
    [ceph5.in][DEBUG ]  python2-bcrypt               x86_64 3.1.6-2.el7                  epel     39 k
    [ceph5.in][DEBUG ]  python2-six                  noarch 1.9.0-0.el7                  epel    2.9 k
    [ceph5.in][DEBUG ]  rdma-core                    x86_64 22.4-6.el7_9                 updates  51 k
    [ceph5.in][DEBUG ]  userspace-rcu                x86_64 0.7.16-1.el7                 epel     73 k
    [ceph5.in][DEBUG ]
    [ceph5.in][DEBUG ] Transaction Summary
    [ceph5.in][DEBUG ] ================================================================================
    [ceph5.in][DEBUG ] Install  2 Packages (+62 Dependent packages)
    [ceph5.in][DEBUG ]
    [ceph5.in][DEBUG ] Total download size: 61 M
    [ceph5.in][DEBUG ] Installed size: 210 M
    [ceph5.in][DEBUG ] Downloading packages:
    [ceph5.in][DEBUG ] Public key for leveldb-1.12.0-11.el7.x86_64.rpm is not installed
    [ceph5.in][WARNIN] warning: /var/cache/yum/x86_64/7/epel/packages/leveldb-1.12.0-11.el7.x86_64.rpm: Header V3 RSA/SHA256 Signature, key ID 352c64e5: NOKEY
    [ceph5.in][DEBUG ] --------------------------------------------------------------------------------
    [ceph5.in][DEBUG ] Total                                              6.1 MB/s |  61 MB  00:10
    [ceph5.in][DEBUG ] Retrieving key from file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
    [ceph5.in][WARNIN] Importing GPG key 0x352C64E5:
    [ceph5.in][WARNIN]  Userid     : "Fedora EPEL (7) <epel@fedoraproject.org>"
    [ceph5.in][WARNIN]  Fingerprint: 91e9 7d7c 4a5e 96f1 7f3e 888f 6a2f aea2 352c 64e5
    [ceph5.in][WARNIN]  Package    : epel-release-7-14.noarch (@/epel-release-latest-7.noarch)
    [ceph5.in][WARNIN]  From       : /etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
    [ceph5.in][DEBUG ] Running transaction check
    [ceph5.in][DEBUG ] Running transaction test
    [ceph5.in][DEBUG ] Transaction test succeeded
    [ceph5.in][DEBUG ] Running transaction
    [ceph5.in][DEBUG ]   Installing : gperftools-libs-2.6.1-1.el7.x86_64                          1/64
    [ceph5.in][DEBUG ]   Installing : leveldb-1.12.0-11.el7.x86_64                                2/64
    [ceph5.in][DEBUG ]   Installing : python-six-1.9.0-2.el7.noarch                               3/64
    [ceph5.in][DEBUG ]   Installing : fuse-libs-2.9.2-11.el7.x86_64                               4/64
    [ceph5.in][DEBUG ]   Installing : liboath-2.6.2-1.el7.x86_64                                  5/64
    [ceph5.in][DEBUG ]   Installing : python-ipaddress-1.0.16-2.el7.noarch                        6/64
    [ceph5.in][DEBUG ]   Installing : python-webob-1.2.3-7.el7.noarch                             7/64
    [ceph5.in][DEBUG ]   Installing : python-markupsafe-0.11-10.el7.x86_64                        8/64
    [ceph5.in][DEBUG ]   Installing : pyOpenSSL-0.13.1-4.el7.x86_64                               9/64
    [ceph5.in][DEBUG ]   Installing : 2:python-ceph-argparse-13.2.10-0.el7.x86_64                10/64
    [ceph5.in][DEBUG ]   Installing : python-webtest-1.3.4-6.el7.noarch                          11/64
    [ceph5.in][DEBUG ]   Installing : python2-six-1.9.0-0.el7.noarch                             12/64
    [ceph5.in][DEBUG ]   Installing : python-singledispatch-3.4.0.2-2.el7.noarch                 13/64
    [ceph5.in][DEBUG ]   Installing : psmisc-22.20-17.el7.x86_64                                 14/64
    [ceph5.in][DEBUG ]   Installing : pciutils-3.5.1-3.el7.x86_64                                15/64
    [ceph5.in][DEBUG ]   Installing : rdma-core-22.4-6.el7_9.x86_64                              16/64
    [ceph5.in][DEBUG ]   Installing : libibverbs-22.4-6.el7_9.x86_64                             17/64
    [ceph5.in][DEBUG ]   Installing : gdisk-0.8.10-3.el7.x86_64                                  18/64
    [ceph5.in][DEBUG ]   Installing : python-simplegeneric-0.8-7.el7.noarch                      19/64
    [ceph5.in][DEBUG ]   Installing : python-tempita-0.5.1-6.el7.noarch                          20/64
    [ceph5.in][DEBUG ]   Installing : python-cherrypy-3.2.2-4.el7.noarch                         21/64
    [ceph5.in][DEBUG ]   Installing : python-prettytable-0.7.2-3.el7.noarch                      22/64
    [ceph5.in][DEBUG ]   Installing : python-werkzeug-0.9.1-2.el7.noarch                         23/64
    [ceph5.in][DEBUG ]   Installing : python-repoze-lru-0.4-3.el7.noarch                         24/64
    [ceph5.in][DEBUG ]   Installing : python-routes-1.13-2.el7.noarch                            25/64
    [ceph5.in][DEBUG ]   Installing : python-backports-1.0-8.el7.x86_64                          26/64
    [ceph5.in][DEBUG ]   Installing : python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch   27/64
    [ceph5.in][DEBUG ]   Installing : python-setuptools-0.9.8-7.el7.noarch                       28/64
    [ceph5.in][DEBUG ]   Installing : python-paste-1.7.5.1-9.20111221hg1498.el7.noarch           29/64
    [ceph5.in][DEBUG ]   Installing : python-beaker-1.5.4-10.el7.noarch                          30/64
    [ceph5.in][DEBUG ]   Installing : python-mako-0.8.1-2.el7.noarch                             31/64
    [ceph5.in][DEBUG ]   Installing : python-pecan-0.4.5-2.el7.noarch                            32/64
    [ceph5.in][DEBUG ]   Installing : python-urllib3-1.10.2-7.el7.noarch                         33/64
    [ceph5.in][DEBUG ]   Installing : python-babel-0.9.6-8.el7.noarch                            34/64
    [ceph5.in][DEBUG ]   Installing : python-jinja2-2.7.2-4.el7.noarch                           35/64
    [ceph5.in][DEBUG ]   Installing : python-chardet-2.2.1-3.el7.noarch                          36/64
    [ceph5.in][DEBUG ]   Installing : python-requests-2.6.0-10.el7.noarch                        37/64
    [ceph5.in][DEBUG ]   Installing : cryptsetup-2.0.3-6.el7.x86_64                              38/64
    [ceph5.in][DEBUG ]   Installing : libbabeltrace-1.2.4-3.el7.x86_64                           39/64
    [ceph5.in][DEBUG ]   Installing : userspace-rcu-0.7.16-1.el7.x86_64                          40/64
    [ceph5.in][DEBUG ]   Installing : lttng-ust-2.4.1-4.el7.x86_64                               41/64
    [ceph5.in][DEBUG ]   Installing : 2:librados2-13.2.10-0.el7.x86_64                           42/64
    [ceph5.in][DEBUG ]   Installing : 2:python-rados-13.2.10-0.el7.x86_64                        43/64
    [ceph5.in][DEBUG ]   Installing : 2:librbd1-13.2.10-0.el7.x86_64                             44/64
    [ceph5.in][DEBUG ]   Installing : 2:libcephfs2-13.2.10-0.el7.x86_64                          45/64
    [ceph5.in][DEBUG ]   Installing : 2:librgw2-13.2.10-0.el7.x86_64                             46/64
    [ceph5.in][DEBUG ]   Installing : 2:python-rgw-13.2.10-0.el7.x86_64                          47/64
    [ceph5.in][DEBUG ]   Installing : 2:python-cephfs-13.2.10-0.el7.x86_64                       48/64
    [ceph5.in][DEBUG ]   Installing : 2:python-rbd-13.2.10-0.el7.x86_64                          49/64
    [ceph5.in][DEBUG ]   Installing : 2:libradosstriper1-13.2.10-0.el7.x86_64                    50/64
    [ceph5.in][DEBUG ]   Installing : 2:ceph-common-13.2.10-0.el7.x86_64                         51/64
    [ceph5.in][DEBUG ]   Installing : 2:ceph-base-13.2.10-0.el7.x86_64                           52/64
    [ceph5.in][DEBUG ]   Installing : 2:ceph-selinux-13.2.10-0.el7.x86_64                        53/64
    [ceph5.in][DEBUG ]   Installing : 2:ceph-osd-13.2.10-0.el7.x86_64                            54/64
    [ceph5.in][DEBUG ]   Installing : 2:ceph-mds-13.2.10-0.el7.x86_64                            55/64
    [ceph5.in][DEBUG ]   Installing : 2:ceph-mon-13.2.10-0.el7.x86_64                            56/64
    [ceph5.in][DEBUG ]   Installing : python-ply-3.4-11.el7.noarch                               57/64
    [ceph5.in][DEBUG ]   Installing : python-pycparser-2.14-1.el7.noarch                         58/64
    [ceph5.in][DEBUG ]   Installing : python-cffi-1.6.0-5.el7.x86_64                             59/64
    [ceph5.in][DEBUG ]   Installing : python2-bcrypt-3.1.6-2.el7.x86_64                          60/64
    [ceph5.in][DEBUG ]   Installing : 2:ceph-mgr-13.2.10-0.el7.x86_64                            61/64
    [ceph5.in][DEBUG ]   Installing : mailcap-2.1.41-2.el7.noarch                                62/64
    [ceph5.in][DEBUG ]   Installing : 2:ceph-radosgw-13.2.10-0.el7.x86_64                        63/64
    [ceph5.in][DEBUG ]   Installing : 2:ceph-13.2.10-0.el7.x86_64                                64/64
    [ceph5.in][DEBUG ]   Verifying  : liboath-2.6.2-1.el7.x86_64                                  1/64
    [ceph5.in][DEBUG ]   Verifying  : python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch    2/64
    [ceph5.in][DEBUG ]   Verifying  : 2:librbd1-13.2.10-0.el7.x86_64                              3/64
    [ceph5.in][DEBUG ]   Verifying  : 2:python-ceph-argparse-13.2.10-0.el7.x86_64                 4/64
    [ceph5.in][DEBUG ]   Verifying  : mailcap-2.1.41-2.el7.noarch                                 5/64
    [ceph5.in][DEBUG ]   Verifying  : pyOpenSSL-0.13.1-4.el7.x86_64                               6/64
    [ceph5.in][DEBUG ]   Verifying  : python2-bcrypt-3.1.6-2.el7.x86_64                           7/64
    [ceph5.in][DEBUG ]   Verifying  : python-ply-3.4-11.el7.noarch                                8/64
    [ceph5.in][DEBUG ]   Verifying  : userspace-rcu-0.7.16-1.el7.x86_64                           9/64
    [ceph5.in][DEBUG ]   Verifying  : libibverbs-22.4-6.el7_9.x86_64                             10/64
    [ceph5.in][DEBUG ]   Verifying  : rdma-core-22.4-6.el7_9.x86_64                              11/64
    [ceph5.in][DEBUG ]   Verifying  : fuse-libs-2.9.2-11.el7.x86_64                              12/64
    [ceph5.in][DEBUG ]   Verifying  : python-setuptools-0.9.8-7.el7.noarch                       13/64
    [ceph5.in][DEBUG ]   Verifying  : python-routes-1.13-2.el7.noarch                            14/64
    [ceph5.in][DEBUG ]   Verifying  : 2:libcephfs2-13.2.10-0.el7.x86_64                          15/64
    [ceph5.in][DEBUG ]   Verifying  : python-urllib3-1.10.2-7.el7.noarch                         16/64
    [ceph5.in][DEBUG ]   Verifying  : libbabeltrace-1.2.4-3.el7.x86_64                           17/64
    [ceph5.in][DEBUG ]   Verifying  : python-mako-0.8.1-2.el7.noarch                             18/64
    [ceph5.in][DEBUG ]   Verifying  : python2-six-1.9.0-0.el7.noarch                             19/64
    [ceph5.in][DEBUG ]   Verifying  : 2:ceph-mgr-13.2.10-0.el7.x86_64                            20/64
    [ceph5.in][DEBUG ]   Verifying  : 2:ceph-base-13.2.10-0.el7.x86_64                           21/64
    [ceph5.in][DEBUG ]   Verifying  : python-jinja2-2.7.2-4.el7.noarch                           22/64
    [ceph5.in][DEBUG ]   Verifying  : python-pecan-0.4.5-2.el7.noarch                            23/64
    [ceph5.in][DEBUG ]   Verifying  : python-six-1.9.0-2.el7.noarch                              24/64
    [ceph5.in][DEBUG ]   Verifying  : cryptsetup-2.0.3-6.el7.x86_64                              25/64
    [ceph5.in][DEBUG ]   Verifying  : leveldb-1.12.0-11.el7.x86_64                               26/64
    [ceph5.in][DEBUG ]   Verifying  : python-singledispatch-3.4.0.2-2.el7.noarch                 27/64
    [ceph5.in][DEBUG ]   Verifying  : python-markupsafe-0.11-10.el7.x86_64                       28/64
    [ceph5.in][DEBUG ]   Verifying  : 2:python-rados-13.2.10-0.el7.x86_64                        29/64
    [ceph5.in][DEBUG ]   Verifying  : 2:python-rgw-13.2.10-0.el7.x86_64                          30/64
    [ceph5.in][DEBUG ]   Verifying  : 2:ceph-radosgw-13.2.10-0.el7.x86_64                        31/64
    [ceph5.in][DEBUG ]   Verifying  : python-chardet-2.2.1-3.el7.noarch                          32/64
    [ceph5.in][DEBUG ]   Verifying  : python-babel-0.9.6-8.el7.noarch                            33/64
    [ceph5.in][DEBUG ]   Verifying  : 2:librados2-13.2.10-0.el7.x86_64                           34/64
    [ceph5.in][DEBUG ]   Verifying  : python-paste-1.7.5.1-9.20111221hg1498.el7.noarch           35/64
    [ceph5.in][DEBUG ]   Verifying  : 2:ceph-osd-13.2.10-0.el7.x86_64                            36/64
    [ceph5.in][DEBUG ]   Verifying  : python-backports-1.0-8.el7.x86_64                          37/64
    [ceph5.in][DEBUG ]   Verifying  : lttng-ust-2.4.1-4.el7.x86_64                               38/64
    [ceph5.in][DEBUG ]   Verifying  : python-webob-1.2.3-7.el7.noarch                            39/64
    [ceph5.in][DEBUG ]   Verifying  : 2:ceph-common-13.2.10-0.el7.x86_64                         40/64
    [ceph5.in][DEBUG ]   Verifying  : python-repoze-lru-0.4-3.el7.noarch                         41/64
    [ceph5.in][DEBUG ]   Verifying  : python-werkzeug-0.9.1-2.el7.noarch                         42/64
    [ceph5.in][DEBUG ]   Verifying  : python-beaker-1.5.4-10.el7.noarch                          43/64
    [ceph5.in][DEBUG ]   Verifying  : python-cffi-1.6.0-5.el7.x86_64                             44/64
    [ceph5.in][DEBUG ]   Verifying  : 2:ceph-selinux-13.2.10-0.el7.x86_64                        45/64
    [ceph5.in][DEBUG ]   Verifying  : python-requests-2.6.0-10.el7.noarch                        46/64
    [ceph5.in][DEBUG ]   Verifying  : python-pycparser-2.14-1.el7.noarch                         47/64
    [ceph5.in][DEBUG ]   Verifying  : python-prettytable-0.7.2-3.el7.noarch                      48/64
    [ceph5.in][DEBUG ]   Verifying  : 2:librgw2-13.2.10-0.el7.x86_64                             49/64
    [ceph5.in][DEBUG ]   Verifying  : 2:ceph-mds-13.2.10-0.el7.x86_64                            50/64
    [ceph5.in][DEBUG ]   Verifying  : python-cherrypy-3.2.2-4.el7.noarch                         51/64
    [ceph5.in][DEBUG ]   Verifying  : 2:python-cephfs-13.2.10-0.el7.x86_64                       52/64
    [ceph5.in][DEBUG ]   Verifying  : python-tempita-0.5.1-6.el7.noarch                          53/64
    [ceph5.in][DEBUG ]   Verifying  : 2:python-rbd-13.2.10-0.el7.x86_64                          54/64
    [ceph5.in][DEBUG ]   Verifying  : 2:ceph-mon-13.2.10-0.el7.x86_64                            55/64
    [ceph5.in][DEBUG ]   Verifying  : gperftools-libs-2.6.1-1.el7.x86_64                         56/64
    [ceph5.in][DEBUG ]   Verifying  : python-ipaddress-1.0.16-2.el7.noarch                       57/64
    [ceph5.in][DEBUG ]   Verifying  : python-webtest-1.3.4-6.el7.noarch                          58/64
    [ceph5.in][DEBUG ]   Verifying  : 2:ceph-13.2.10-0.el7.x86_64                                59/64
    [ceph5.in][DEBUG ]   Verifying  : python-simplegeneric-0.8-7.el7.noarch                      60/64
    [ceph5.in][DEBUG ]   Verifying  : gdisk-0.8.10-3.el7.x86_64                                  61/64
    [ceph5.in][DEBUG ]   Verifying  : 2:libradosstriper1-13.2.10-0.el7.x86_64                    62/64
    [ceph5.in][DEBUG ]   Verifying  : pciutils-3.5.1-3.el7.x86_64                                63/64
    [ceph5.in][DEBUG ]   Verifying  : psmisc-22.20-17.el7.x86_64                                 64/64
    [ceph5.in][DEBUG ]
    [ceph5.in][DEBUG ] Installed:
    [ceph5.in][DEBUG ]   ceph.x86_64 2:13.2.10-0.el7        ceph-radosgw.x86_64 2:13.2.10-0.el7
    [ceph5.in][DEBUG ]
    [ceph5.in][DEBUG ] Dependency Installed:
    [ceph5.in][DEBUG ]   ceph-base.x86_64 2:13.2.10-0.el7
    [ceph5.in][DEBUG ]   ceph-common.x86_64 2:13.2.10-0.el7
    [ceph5.in][DEBUG ]   ceph-mds.x86_64 2:13.2.10-0.el7
    [ceph5.in][DEBUG ]   ceph-mgr.x86_64 2:13.2.10-0.el7
    [ceph5.in][DEBUG ]   ceph-mon.x86_64 2:13.2.10-0.el7
    [ceph5.in][DEBUG ]   ceph-osd.x86_64 2:13.2.10-0.el7
    [ceph5.in][DEBUG ]   ceph-selinux.x86_64 2:13.2.10-0.el7
    [ceph5.in][DEBUG ]   cryptsetup.x86_64 0:2.0.3-6.el7
    [ceph5.in][DEBUG ]   fuse-libs.x86_64 0:2.9.2-11.el7
    [ceph5.in][DEBUG ]   gdisk.x86_64 0:0.8.10-3.el7
    [ceph5.in][DEBUG ]   gperftools-libs.x86_64 0:2.6.1-1.el7
    [ceph5.in][DEBUG ]   leveldb.x86_64 0:1.12.0-11.el7
    [ceph5.in][DEBUG ]   libbabeltrace.x86_64 0:1.2.4-3.el7
    [ceph5.in][DEBUG ]   libcephfs2.x86_64 2:13.2.10-0.el7
    [ceph5.in][DEBUG ]   libibverbs.x86_64 0:22.4-6.el7_9
    [ceph5.in][DEBUG ]   liboath.x86_64 0:2.6.2-1.el7
    [ceph5.in][DEBUG ]   librados2.x86_64 2:13.2.10-0.el7
    [ceph5.in][DEBUG ]   libradosstriper1.x86_64 2:13.2.10-0.el7
    [ceph5.in][DEBUG ]   librbd1.x86_64 2:13.2.10-0.el7
    [ceph5.in][DEBUG ]   librgw2.x86_64 2:13.2.10-0.el7
    [ceph5.in][DEBUG ]   lttng-ust.x86_64 0:2.4.1-4.el7
    [ceph5.in][DEBUG ]   mailcap.noarch 0:2.1.41-2.el7
    [ceph5.in][DEBUG ]   pciutils.x86_64 0:3.5.1-3.el7
    [ceph5.in][DEBUG ]   psmisc.x86_64 0:22.20-17.el7
    [ceph5.in][DEBUG ]   pyOpenSSL.x86_64 0:0.13.1-4.el7
    [ceph5.in][DEBUG ]   python-babel.noarch 0:0.9.6-8.el7
    [ceph5.in][DEBUG ]   python-backports.x86_64 0:1.0-8.el7
    [ceph5.in][DEBUG ]   python-backports-ssl_match_hostname.noarch 0:3.5.0.1-1.el7
    [ceph5.in][DEBUG ]   python-beaker.noarch 0:1.5.4-10.el7
    [ceph5.in][DEBUG ]   python-ceph-argparse.x86_64 2:13.2.10-0.el7
    [ceph5.in][DEBUG ]   python-cephfs.x86_64 2:13.2.10-0.el7
    [ceph5.in][DEBUG ]   python-cffi.x86_64 0:1.6.0-5.el7
    [ceph5.in][DEBUG ]   python-chardet.noarch 0:2.2.1-3.el7
    [ceph5.in][DEBUG ]   python-cherrypy.noarch 0:3.2.2-4.el7
    [ceph5.in][DEBUG ]   python-ipaddress.noarch 0:1.0.16-2.el7
    [ceph5.in][DEBUG ]   python-jinja2.noarch 0:2.7.2-4.el7
    [ceph5.in][DEBUG ]   python-mako.noarch 0:0.8.1-2.el7
    [ceph5.in][DEBUG ]   python-markupsafe.x86_64 0:0.11-10.el7
    [ceph5.in][DEBUG ]   python-paste.noarch 0:1.7.5.1-9.20111221hg1498.el7
    [ceph5.in][DEBUG ]   python-pecan.noarch 0:0.4.5-2.el7
    [ceph5.in][DEBUG ]   python-ply.noarch 0:3.4-11.el7
    [ceph5.in][DEBUG ]   python-prettytable.noarch 0:0.7.2-3.el7
    [ceph5.in][DEBUG ]   python-pycparser.noarch 0:2.14-1.el7
    [ceph5.in][DEBUG ]   python-rados.x86_64 2:13.2.10-0.el7
    [ceph5.in][DEBUG ]   python-rbd.x86_64 2:13.2.10-0.el7
    [ceph5.in][DEBUG ]   python-repoze-lru.noarch 0:0.4-3.el7
    [ceph5.in][DEBUG ]   python-requests.noarch 0:2.6.0-10.el7
    [ceph5.in][DEBUG ]   python-rgw.x86_64 2:13.2.10-0.el7
    [ceph5.in][DEBUG ]   python-routes.noarch 0:1.13-2.el7
    [ceph5.in][DEBUG ]   python-setuptools.noarch 0:0.9.8-7.el7
    [ceph5.in][DEBUG ]   python-simplegeneric.noarch 0:0.8-7.el7
    [ceph5.in][DEBUG ]   python-singledispatch.noarch 0:3.4.0.2-2.el7
    [ceph5.in][DEBUG ]   python-six.noarch 0:1.9.0-2.el7
    [ceph5.in][DEBUG ]   python-tempita.noarch 0:0.5.1-6.el7
    [ceph5.in][DEBUG ]   python-urllib3.noarch 0:1.10.2-7.el7
    [ceph5.in][DEBUG ]   python-webob.noarch 0:1.2.3-7.el7
    [ceph5.in][DEBUG ]   python-webtest.noarch 0:1.3.4-6.el7
    [ceph5.in][DEBUG ]   python-werkzeug.noarch 0:0.9.1-2.el7
    [ceph5.in][DEBUG ]   python2-bcrypt.x86_64 0:3.1.6-2.el7
    [ceph5.in][DEBUG ]   python2-six.noarch 0:1.9.0-0.el7
    [ceph5.in][DEBUG ]   rdma-core.x86_64 0:22.4-6.el7_9
    [ceph5.in][DEBUG ]   userspace-rcu.x86_64 0:0.7.16-1.el7
    [ceph5.in][DEBUG ]
    [ceph5.in][DEBUG ] Complete!
    [ceph5.in][INFO  ] Running command: sudo ceph --version
    [ceph5.in][DEBUG ] ceph version 13.2.10 (564bdc4ae87418a232fc901524470e1a0f76d641) mimic (stable)
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy admin ceph5.in
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy admin ceph5.in
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f2af0ce2950>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  client                        : ['ceph5.in']
    [ceph_deploy.cli][INFO  ]  func                          : <function admin at 0x7f2af157a320>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.admin][DEBUG ] Pushing admin keys and conf to ceph5.in
    [ceph5.in][DEBUG ] connection detected need for sudo
    [ceph5.in][DEBUG ] connected to host: ceph5.in
    [ceph5.in][DEBUG ] detect platform information from remote host
    [ceph5.in][DEBUG ] detect machine type
    [ceph5.in][DEBUG ] write cluster configuration to /etc/ceph/{cluster}.conf
    [cephadm@ceph2 ceph_cluster]$ exit
    logout
    [root@ceph2 ~]# ceph health
    HEALTH_OK
    [root@ceph2 ~]# ceph health detail
    HEALTH_OK
    [root@ceph2 ~]# ceph -s
      cluster:
        id:     5cfc246a-5a14-4337-98b2-58d2a2e19b18
        health: HEALTH_OK
    
      services:
        mon: 1 daemons, quorum ceph1
        mgr: ceph3.in(active), standbys: ceph4.in
        osd: 6 osds: 6 up, 6 in
    
      data:
        pools:   0 pools, 0 pgs
        objects: 0  objects, 0 B
        usage:   6.0 GiB used, 114 GiB / 120 GiB avail
        pgs:
    
    [root@ceph2 ~]# ceph osd pool create rbd 200 3
    pool 'rbd' created
    [root@ceph2 ~]# vim /etc/hosts
    [root@ceph2 ~]# systemctl restart chronyd
    [root@ceph2 ~]# ssh-copy-id cephadm@ceph6.in
    
    /usr/bin/ssh-copy-id: ERROR: failed to open ID file '/root/.pub': No such file or directory
            (to install the contents of '/root/.pub' anyway, look at the -f option)
    [root@ceph2 ~]# su - cephadm
    Last login: Sun Jul 16 21:26:19 IST 2023 on pts/0
    [cephadm@ceph2 ~]$ ssh-copy-id cephadm@ceph6.in
    /bin/ssh-copy-id: INFO: Source of key(s) to be installed: "/home/cephadm/.ssh/id_rsa.pub"
    The authenticity of host 'ceph6.in (192.168.239.159)' can't be established.
    ECDSA key fingerprint is SHA256:JbQFp/4SaYFpszIjBlpttyXEMGiNiL5rz5A+HcTkXQo.
    ECDSA key fingerprint is MD5:9c:7c:9f:fd:38:b0:70:5c:20:ab:69:3b:07:05:3f:1c.
    Are you sure you want to continue connecting (yes/no)? yes
    /bin/ssh-copy-id: INFO: attempting to log in with the new key(s), to filter out any that are already installed
    /bin/ssh-copy-id: INFO: 1 key(s) remain to be installed -- if you are prompted now it is to install the new keys
    cephadm@ceph6.in's password:
    
    Number of key(s) added: 1
    
    Now try logging into the machine, with:   "ssh 'cephadm@ceph6.in'"
    and check to make sure that only the key(s) you wanted were added.
    
    [cephadm@ceph2 ~]$ vim ~/.ssh/config
    [cephadm@ceph2 ~]$ ssh cephadm@ceph6.in
    [cephadm@ceph6 ~]$ exit
    logout
    Connection to ceph6.in closed.
    [cephadm@ceph2 ~]$ cd ceph_cluster/
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy install ceph6.in
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy install ceph6.in
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  testing                       : None
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7fda667aa5a8>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  dev_commit                    : None
    [ceph_deploy.cli][INFO  ]  install_mds                   : False
    [ceph_deploy.cli][INFO  ]  stable                        : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  adjust_repos                  : True
    [ceph_deploy.cli][INFO  ]  func                          : <function install at 0x7fda66df66e0>
    [ceph_deploy.cli][INFO  ]  install_mgr                   : False
    [ceph_deploy.cli][INFO  ]  install_all                   : False
    [ceph_deploy.cli][INFO  ]  repo                          : False
    [ceph_deploy.cli][INFO  ]  host                          : ['ceph6.in']
    [ceph_deploy.cli][INFO  ]  install_rgw                   : False
    [ceph_deploy.cli][INFO  ]  install_tests                 : False
    [ceph_deploy.cli][INFO  ]  repo_url                      : None
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  install_osd                   : False
    [ceph_deploy.cli][INFO  ]  version_kind                  : stable
    [ceph_deploy.cli][INFO  ]  install_common                : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  dev                           : master
    [ceph_deploy.cli][INFO  ]  nogpgcheck                    : False
    [ceph_deploy.cli][INFO  ]  local_mirror                  : None
    [ceph_deploy.cli][INFO  ]  release                       : None
    [ceph_deploy.cli][INFO  ]  install_mon                   : False
    [ceph_deploy.cli][INFO  ]  gpg_url                       : None
    [ceph_deploy.install][DEBUG ] Installing stable version mimic on cluster ceph hosts ceph6.in
    [ceph_deploy.install][DEBUG ] Detecting platform for host ceph6.in ...
    [ceph6.in][DEBUG ] connection detected need for sudo
    [ceph6.in][DEBUG ] connected to host: ceph6.in
    [ceph6.in][DEBUG ] detect platform information from remote host
    [ceph6.in][DEBUG ] detect machine type
    [ceph_deploy.install][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph6.in][INFO  ] installing Ceph on ceph6.in
    [ceph6.in][INFO  ] Running command: sudo yum clean all
    [ceph6.in][DEBUG ] Loaded plugins: fastestmirror
    [ceph6.in][DEBUG ] Cleaning repos: base epel extras updates
    [ceph6.in][DEBUG ] Cleaning up list of fastest mirrors
    [ceph6.in][INFO  ] Running command: sudo yum -y install epel-release
    [ceph6.in][DEBUG ] Loaded plugins: fastestmirror
    [ceph6.in][DEBUG ] Determining fastest mirrors
    [ceph6.in][DEBUG ]  * base: centos.mirror.net.in
    [ceph6.in][DEBUG ]  * epel: repo.extreme-ix.org
    [ceph6.in][DEBUG ]  * extras: centos.mirror.net.in
    [ceph6.in][DEBUG ]  * updates: centos.mirror.net.in
    [ceph6.in][DEBUG ] Resolving Dependencies
    [ceph6.in][DEBUG ] --> Running transaction check
    [ceph6.in][DEBUG ] ---> Package epel-release.noarch 0:7-11 will be updated
    [ceph6.in][DEBUG ] ---> Package epel-release.noarch 0:7-14 will be an update
    [ceph6.in][DEBUG ] --> Finished Dependency Resolution
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] Dependencies Resolved
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] ================================================================================
    [ceph6.in][DEBUG ]  Package                Arch             Version           Repository      Size
    [ceph6.in][DEBUG ] ================================================================================
    [ceph6.in][DEBUG ] Updating:
    [ceph6.in][DEBUG ]  epel-release           noarch           7-14              epel            15 k
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] Transaction Summary
    [ceph6.in][DEBUG ] ================================================================================
    [ceph6.in][DEBUG ] Upgrade  1 Package
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] Total download size: 15 k
    [ceph6.in][DEBUG ] Downloading packages:
    [ceph6.in][DEBUG ] Delta RPMs disabled because /usr/bin/applydeltarpm not installed.
    [ceph6.in][DEBUG ] Public key for epel-release-7-14.noarch.rpm is not installed
    [ceph6.in][WARNIN] warning: /var/cache/yum/x86_64/7/epel/packages/epel-release-7-14.noarch.rpm: Header V4 RSA/SHA256 Signature, key ID 352c64e5: NOKEY
    [ceph6.in][DEBUG ] Retrieving key from file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
    [ceph6.in][WARNIN] Importing GPG key 0x352C64E5:
    [ceph6.in][WARNIN]  Userid     : "Fedora EPEL (7) <epel@fedoraproject.org>"
    [ceph6.in][WARNIN]  Fingerprint: 91e9 7d7c 4a5e 96f1 7f3e 888f 6a2f aea2 352c 64e5
    [ceph6.in][WARNIN]  Package    : epel-release-7-11.noarch (@extras)
    [ceph6.in][WARNIN]  From       : /etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
    [ceph6.in][DEBUG ] Running transaction check
    [ceph6.in][DEBUG ] Running transaction test
    [ceph6.in][DEBUG ] Transaction test succeeded
    [ceph6.in][DEBUG ] Running transaction
    [ceph6.in][DEBUG ]   Updating   : epel-release-7-14.noarch                                     1/2
    [ceph6.in][DEBUG ]   Cleanup    : epel-release-7-11.noarch                                     2/2
    [ceph6.in][DEBUG ]   Verifying  : epel-release-7-14.noarch                                     1/2
    [ceph6.in][DEBUG ]   Verifying  : epel-release-7-11.noarch                                     2/2
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] Updated:
    [ceph6.in][DEBUG ]   epel-release.noarch 0:7-14
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] Complete!
    [ceph6.in][INFO  ] Running command: sudo yum -y install yum-plugin-priorities
    [ceph6.in][DEBUG ] Loaded plugins: fastestmirror
    [ceph6.in][DEBUG ] Loading mirror speeds from cached hostfile
    [ceph6.in][DEBUG ]  * base: centos.mirror.net.in
    [ceph6.in][DEBUG ]  * epel: repo.extreme-ix.org
    [ceph6.in][DEBUG ]  * extras: centos.mirror.net.in
    [ceph6.in][DEBUG ]  * updates: centos.mirror.net.in
    [ceph6.in][DEBUG ] Resolving Dependencies
    [ceph6.in][DEBUG ] --> Running transaction check
    [ceph6.in][DEBUG ] ---> Package yum-plugin-priorities.noarch 0:1.1.31-54.el7_8 will be installed
    [ceph6.in][DEBUG ] --> Finished Dependency Resolution
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] Dependencies Resolved
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] ================================================================================
    [ceph6.in][DEBUG ]  Package                    Arch        Version                 Repository
    [ceph6.in][DEBUG ]                                                                            Size
    [ceph6.in][DEBUG ] ================================================================================
    [ceph6.in][DEBUG ] Installing:
    [ceph6.in][DEBUG ]  yum-plugin-priorities      noarch      1.1.31-54.el7_8         base       29 k
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] Transaction Summary
    [ceph6.in][DEBUG ] ================================================================================
    [ceph6.in][DEBUG ] Install  1 Package
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] Total download size: 29 k
    [ceph6.in][DEBUG ] Installed size: 28 k
    [ceph6.in][DEBUG ] Downloading packages:
    [ceph6.in][DEBUG ] Running transaction check
    [ceph6.in][DEBUG ] Running transaction test
    [ceph6.in][DEBUG ] Transaction test succeeded
    [ceph6.in][DEBUG ] Running transaction
    [ceph6.in][DEBUG ]   Installing : yum-plugin-priorities-1.1.31-54.el7_8.noarch                 1/1
    [ceph6.in][DEBUG ]   Verifying  : yum-plugin-priorities-1.1.31-54.el7_8.noarch                 1/1
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] Installed:
    [ceph6.in][DEBUG ]   yum-plugin-priorities.noarch 0:1.1.31-54.el7_8
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] Complete!
    [ceph6.in][DEBUG ] Configure Yum priorities to include obsoletes
    [ceph6.in][WARNIN] check_obsoletes has been enabled for Yum priorities plugin
    [ceph6.in][INFO  ] Running command: sudo rpm --import https://download.ceph.com/keys/release.asc
    [ceph6.in][INFO  ] Running command: sudo yum remove -y ceph-release
    [ceph6.in][DEBUG ] Loaded plugins: fastestmirror, priorities
    [ceph6.in][WARNIN] No Match for argument: ceph-release
    [ceph6.in][DEBUG ] No Packages marked for removal
    [ceph6.in][INFO  ] Running command: sudo yum install -y https://download.ceph.com/rpm-mimic/el7/noarch/ceph-release-1-0.el7.noarch.rpm
    [ceph6.in][DEBUG ] Loaded plugins: fastestmirror, priorities
    [ceph6.in][DEBUG ] Examining /var/tmp/yum-root-MEn1Cw/ceph-release-1-0.el7.noarch.rpm: ceph-release-1-1.el7.noarch
    [ceph6.in][DEBUG ] Marking /var/tmp/yum-root-MEn1Cw/ceph-release-1-0.el7.noarch.rpm to be installed
    [ceph6.in][DEBUG ] Resolving Dependencies
    [ceph6.in][DEBUG ] --> Running transaction check
    [ceph6.in][DEBUG ] ---> Package ceph-release.noarch 0:1-1.el7 will be installed
    [ceph6.in][DEBUG ] --> Finished Dependency Resolution
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] Dependencies Resolved
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] ================================================================================
    [ceph6.in][DEBUG ]  Package          Arch       Version     Repository                        Size
    [ceph6.in][DEBUG ] ================================================================================
    [ceph6.in][DEBUG ] Installing:
    [ceph6.in][DEBUG ]  ceph-release     noarch     1-1.el7     /ceph-release-1-0.el7.noarch     535
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] Transaction Summary
    [ceph6.in][DEBUG ] ================================================================================
    [ceph6.in][DEBUG ] Install  1 Package
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] Total size: 535
    [ceph6.in][DEBUG ] Installed size: 535
    [ceph6.in][DEBUG ] Downloading packages:
    [ceph6.in][DEBUG ] Running transaction check
    [ceph6.in][DEBUG ] Running transaction test
    [ceph6.in][DEBUG ] Transaction test succeeded
    [ceph6.in][DEBUG ] Running transaction
    [ceph6.in][DEBUG ]   Installing : ceph-release-1-1.el7.noarch                                  1/1
    [ceph6.in][DEBUG ]   Verifying  : ceph-release-1-1.el7.noarch                                  1/1
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] Installed:
    [ceph6.in][DEBUG ]   ceph-release.noarch 0:1-1.el7
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] Complete!
    [ceph6.in][WARNIN] ensuring that /etc/yum.repos.d/ceph.repo contains a high priority
    [ceph6.in][WARNIN] altered ceph.repo priorities to contain: priority=1
    [ceph6.in][INFO  ] Running command: sudo yum -y install ceph ceph-radosgw
    [ceph6.in][DEBUG ] Loaded plugins: fastestmirror, priorities
    [ceph6.in][DEBUG ] Loading mirror speeds from cached hostfile
    [ceph6.in][DEBUG ]  * base: centos.mirror.net.in
    [ceph6.in][DEBUG ]  * epel: repo.extreme-ix.org
    [ceph6.in][DEBUG ]  * extras: centos.mirror.net.in
    [ceph6.in][DEBUG ]  * updates: centos.mirror.net.in
    [ceph6.in][DEBUG ] 8 packages excluded due to repository priority protections
    [ceph6.in][DEBUG ] Resolving Dependencies
    [ceph6.in][DEBUG ] --> Running transaction check
    [ceph6.in][DEBUG ] ---> Package ceph.x86_64 2:13.2.10-0.el7 will be installed
    [ceph6.in][DEBUG ] --> Processing Dependency: ceph-mds = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: ceph-osd = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: ceph-mon = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: ceph-mgr = 2:13.2.10-0.el7 for package: 2:ceph-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] ---> Package ceph-radosgw.x86_64 2:13.2.10-0.el7 will be installed
    [ceph6.in][DEBUG ] --> Processing Dependency: ceph-base = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: ceph-selinux = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: librgw2 = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: librados2 = 2:13.2.10-0.el7 for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: mailcap for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: librados.so.2()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: libtcmalloc.so.4()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: libibverbs.so.1()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: liboath.so.0()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: libceph-common.so.0()(64bit) for package: 2:ceph-radosgw-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Running transaction check
    [ceph6.in][DEBUG ] ---> Package ceph-base.x86_64 2:13.2.10-0.el7 will be installed
    [ceph6.in][DEBUG ] --> Processing Dependency: libcephfs2 = 2:13.2.10-0.el7 for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: librbd1 = 2:13.2.10-0.el7 for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: ceph-common = 2:13.2.10-0.el7 for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: gdisk for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: python-setuptools for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: psmisc for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: cryptsetup for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: python-requests for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: libleveldb.so.1()(64bit) for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: libfuse.so.2()(64bit) for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: liblttng-ust.so.0()(64bit) for package: 2:ceph-base-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] ---> Package ceph-mds.x86_64 2:13.2.10-0.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package ceph-mgr.x86_64 2:13.2.10-0.el7 will be installed
    [ceph6.in][DEBUG ] --> Processing Dependency: python-cherrypy for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: python-werkzeug for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: python-six for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: python-routes for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: python-bcrypt for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: python-pecan for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: pyOpenSSL for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: python-jinja2 for package: 2:ceph-mgr-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] ---> Package ceph-mon.x86_64 2:13.2.10-0.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package ceph-osd.x86_64 2:13.2.10-0.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package ceph-selinux.x86_64 2:13.2.10-0.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package gperftools-libs.x86_64 0:2.6.1-1.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package libibverbs.x86_64 0:22.4-6.el7_9 will be installed
    [ceph6.in][DEBUG ] --> Processing Dependency: rdma-core(x86-64) = 22.4-6.el7_9 for package: libibverbs-22.4-6.el7_9.x86_64
    [ceph6.in][DEBUG ] ---> Package liboath.x86_64 0:2.6.2-1.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package librados2.x86_64 2:13.2.10-0.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package librgw2.x86_64 2:13.2.10-0.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package mailcap.noarch 0:2.1.41-2.el7 will be installed
    [ceph6.in][DEBUG ] --> Running transaction check
    [ceph6.in][DEBUG ] ---> Package ceph-common.x86_64 2:13.2.10-0.el7 will be installed
    [ceph6.in][DEBUG ] --> Processing Dependency: python-cephfs = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: libradosstriper1 = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: python-rgw = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: python-rbd = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: python-rados = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: python-ceph-argparse = 2:13.2.10-0.el7 for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: python-prettytable for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: libbabeltrace-ctf.so.1()(64bit) for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: libbabeltrace.so.1()(64bit) for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: libradosstriper.so.1()(64bit) for package: 2:ceph-common-13.2.10-0.el7.x86_64
    [ceph6.in][DEBUG ] ---> Package cryptsetup.x86_64 0:2.0.3-6.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package fuse-libs.x86_64 0:2.9.2-11.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package gdisk.x86_64 0:0.8.10-3.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package leveldb.x86_64 0:1.12.0-11.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package libcephfs2.x86_64 2:13.2.10-0.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package librbd1.x86_64 2:13.2.10-0.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package lttng-ust.x86_64 0:2.4.1-4.el7 will be installed
    [ceph6.in][DEBUG ] --> Processing Dependency: liburcu-bp.so.1()(64bit) for package: lttng-ust-2.4.1-4.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: liburcu-cds.so.1()(64bit) for package: lttng-ust-2.4.1-4.el7.x86_64
    [ceph6.in][DEBUG ] ---> Package psmisc.x86_64 0:22.20-17.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package pyOpenSSL.x86_64 0:0.13.1-4.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package python-cherrypy.noarch 0:3.2.2-4.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package python-jinja2.noarch 0:2.7.2-4.el7 will be installed
    [ceph6.in][DEBUG ] --> Processing Dependency: python-babel >= 0.8 for package: python-jinja2-2.7.2-4.el7.noarch
    [ceph6.in][DEBUG ] --> Processing Dependency: python-markupsafe for package: python-jinja2-2.7.2-4.el7.noarch
    [ceph6.in][DEBUG ] ---> Package python-pecan.noarch 0:0.4.5-2.el7 will be installed
    [ceph6.in][DEBUG ] --> Processing Dependency: python-mako >= 0.4.0 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph6.in][DEBUG ] --> Processing Dependency: python-simplegeneric >= 0.8 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph6.in][DEBUG ] --> Processing Dependency: python-webob >= 1.2 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph6.in][DEBUG ] --> Processing Dependency: python-webtest >= 1.3.1 for package: python-pecan-0.4.5-2.el7.noarch
    [ceph6.in][DEBUG ] --> Processing Dependency: python-singledispatch for package: python-pecan-0.4.5-2.el7.noarch
    [ceph6.in][DEBUG ] ---> Package python-requests.noarch 0:2.6.0-10.el7 will be installed
    [ceph6.in][DEBUG ] --> Processing Dependency: python-urllib3 >= 1.10.2-1 for package: python-requests-2.6.0-10.el7.noarch
    [ceph6.in][DEBUG ] --> Processing Dependency: python-chardet >= 2.2.1-1 for package: python-requests-2.6.0-10.el7.noarch
    [ceph6.in][DEBUG ] ---> Package python-routes.noarch 0:1.13-2.el7 will be installed
    [ceph6.in][DEBUG ] --> Processing Dependency: python-repoze-lru for package: python-routes-1.13-2.el7.noarch
    [ceph6.in][DEBUG ] ---> Package python-setuptools.noarch 0:0.9.8-7.el7 will be installed
    [ceph6.in][DEBUG ] --> Processing Dependency: python-backports-ssl_match_hostname for package: python-setuptools-0.9.8-7.el7.noarch
    [ceph6.in][DEBUG ] ---> Package python-six.noarch 0:1.9.0-2.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package python-werkzeug.noarch 0:0.9.1-2.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package python2-bcrypt.x86_64 0:3.1.6-2.el7 will be installed
    [ceph6.in][DEBUG ] --> Processing Dependency: python-cffi for package: python2-bcrypt-3.1.6-2.el7.x86_64
    [ceph6.in][DEBUG ] --> Processing Dependency: python2-six for package: python2-bcrypt-3.1.6-2.el7.x86_64
    [ceph6.in][DEBUG ] ---> Package rdma-core.x86_64 0:22.4-6.el7_9 will be installed
    [ceph6.in][DEBUG ] --> Processing Dependency: pciutils for package: rdma-core-22.4-6.el7_9.x86_64
    [ceph6.in][DEBUG ] --> Running transaction check
    [ceph6.in][DEBUG ] ---> Package libbabeltrace.x86_64 0:1.2.4-3.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package libradosstriper1.x86_64 2:13.2.10-0.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package pciutils.x86_64 0:3.5.1-3.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package python-babel.noarch 0:0.9.6-8.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package python-backports-ssl_match_hostname.noarch 0:3.5.0.1-1.el7 will be installed
    [ceph6.in][DEBUG ] --> Processing Dependency: python-ipaddress for package: python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch
    [ceph6.in][DEBUG ] --> Processing Dependency: python-backports for package: python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch
    [ceph6.in][DEBUG ] ---> Package python-ceph-argparse.x86_64 2:13.2.10-0.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package python-cephfs.x86_64 2:13.2.10-0.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package python-cffi.x86_64 0:1.6.0-5.el7 will be installed
    [ceph6.in][DEBUG ] --> Processing Dependency: python-pycparser for package: python-cffi-1.6.0-5.el7.x86_64
    [ceph6.in][DEBUG ] ---> Package python-chardet.noarch 0:2.2.1-3.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package python-mako.noarch 0:0.8.1-2.el7 will be installed
    [ceph6.in][DEBUG ] --> Processing Dependency: python-beaker for package: python-mako-0.8.1-2.el7.noarch
    [ceph6.in][DEBUG ] ---> Package python-markupsafe.x86_64 0:0.11-10.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package python-prettytable.noarch 0:0.7.2-3.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package python-rados.x86_64 2:13.2.10-0.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package python-rbd.x86_64 2:13.2.10-0.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package python-repoze-lru.noarch 0:0.4-3.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package python-rgw.x86_64 2:13.2.10-0.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package python-simplegeneric.noarch 0:0.8-7.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package python-singledispatch.noarch 0:3.4.0.2-2.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package python-urllib3.noarch 0:1.10.2-7.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package python-webob.noarch 0:1.2.3-7.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package python-webtest.noarch 0:1.3.4-6.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package python2-six.noarch 0:1.9.0-0.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package userspace-rcu.x86_64 0:0.7.16-1.el7 will be installed
    [ceph6.in][DEBUG ] --> Running transaction check
    [ceph6.in][DEBUG ] ---> Package python-backports.x86_64 0:1.0-8.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package python-beaker.noarch 0:1.5.4-10.el7 will be installed
    [ceph6.in][DEBUG ] --> Processing Dependency: python-paste for package: python-beaker-1.5.4-10.el7.noarch
    [ceph6.in][DEBUG ] ---> Package python-ipaddress.noarch 0:1.0.16-2.el7 will be installed
    [ceph6.in][DEBUG ] ---> Package python-pycparser.noarch 0:2.14-1.el7 will be installed
    [ceph6.in][DEBUG ] --> Processing Dependency: python-ply for package: python-pycparser-2.14-1.el7.noarch
    [ceph6.in][DEBUG ] --> Running transaction check
    [ceph6.in][DEBUG ] ---> Package python-paste.noarch 0:1.7.5.1-9.20111221hg1498.el7 will be installed
    [ceph6.in][DEBUG ] --> Processing Dependency: python-tempita for package: python-paste-1.7.5.1-9.20111221hg1498.el7.noarch
    [ceph6.in][DEBUG ] ---> Package python-ply.noarch 0:3.4-11.el7 will be installed
    [ceph6.in][DEBUG ] --> Running transaction check
    [ceph6.in][DEBUG ] ---> Package python-tempita.noarch 0:0.5.1-6.el7 will be installed
    [ceph6.in][DEBUG ] --> Finished Dependency Resolution
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] Dependencies Resolved
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] ================================================================================
    [ceph6.in][DEBUG ]  Package                      Arch   Version                      Repository
    [ceph6.in][DEBUG ]                                                                            Size
    [ceph6.in][DEBUG ] ================================================================================
    [ceph6.in][DEBUG ] Installing:
    [ceph6.in][DEBUG ]  ceph                         x86_64 2:13.2.10-0.el7              Ceph    3.0 k
    [ceph6.in][DEBUG ]  ceph-radosgw                 x86_64 2:13.2.10-0.el7              Ceph    4.5 M
    [ceph6.in][DEBUG ] Installing for dependencies:
    [ceph6.in][DEBUG ]  ceph-base                    x86_64 2:13.2.10-0.el7              Ceph    4.8 M
    [ceph6.in][DEBUG ]  ceph-common                  x86_64 2:13.2.10-0.el7              Ceph     14 M
    [ceph6.in][DEBUG ]  ceph-mds                     x86_64 2:13.2.10-0.el7              Ceph    1.7 M
    [ceph6.in][DEBUG ]  ceph-mgr                     x86_64 2:13.2.10-0.el7              Ceph    3.5 M
    [ceph6.in][DEBUG ]  ceph-mon                     x86_64 2:13.2.10-0.el7              Ceph    3.9 M
    [ceph6.in][DEBUG ]  ceph-osd                     x86_64 2:13.2.10-0.el7              Ceph     13 M
    [ceph6.in][DEBUG ]  ceph-selinux                 x86_64 2:13.2.10-0.el7              Ceph     21 k
    [ceph6.in][DEBUG ]  cryptsetup                   x86_64 2.0.3-6.el7                  base    154 k
    [ceph6.in][DEBUG ]  fuse-libs                    x86_64 2.9.2-11.el7                 base     93 k
    [ceph6.in][DEBUG ]  gdisk                        x86_64 0.8.10-3.el7                 base    190 k
    [ceph6.in][DEBUG ]  gperftools-libs              x86_64 2.6.1-1.el7                  base    272 k
    [ceph6.in][DEBUG ]  leveldb                      x86_64 1.12.0-11.el7                epel    161 k
    [ceph6.in][DEBUG ]  libbabeltrace                x86_64 1.2.4-3.el7                  epel    147 k
    [ceph6.in][DEBUG ]  libcephfs2                   x86_64 2:13.2.10-0.el7              Ceph    434 k
    [ceph6.in][DEBUG ]  libibverbs                   x86_64 22.4-6.el7_9                 updates 269 k
    [ceph6.in][DEBUG ]  liboath                      x86_64 2.6.2-1.el7                  epel     51 k
    [ceph6.in][DEBUG ]  librados2                    x86_64 2:13.2.10-0.el7              Ceph    2.9 M
    [ceph6.in][DEBUG ]  libradosstriper1             x86_64 2:13.2.10-0.el7              Ceph    329 k
    [ceph6.in][DEBUG ]  librbd1                      x86_64 2:13.2.10-0.el7              Ceph    1.2 M
    [ceph6.in][DEBUG ]  librgw2                      x86_64 2:13.2.10-0.el7              Ceph    2.0 M
    [ceph6.in][DEBUG ]  lttng-ust                    x86_64 2.4.1-4.el7                  epel    176 k
    [ceph6.in][DEBUG ]  mailcap                      noarch 2.1.41-2.el7                 base     31 k
    [ceph6.in][DEBUG ]  pciutils                     x86_64 3.5.1-3.el7                  base     93 k
    [ceph6.in][DEBUG ]  psmisc                       x86_64 22.20-17.el7                 base    141 k
    [ceph6.in][DEBUG ]  pyOpenSSL                    x86_64 0.13.1-4.el7                 base    135 k
    [ceph6.in][DEBUG ]  python-babel                 noarch 0.9.6-8.el7                  base    1.4 M
    [ceph6.in][DEBUG ]  python-backports             x86_64 1.0-8.el7                    base    5.8 k
    [ceph6.in][DEBUG ]  python-backports-ssl_match_hostname
    [ceph6.in][DEBUG ]                               noarch 3.5.0.1-1.el7                base     13 k
    [ceph6.in][DEBUG ]  python-beaker                noarch 1.5.4-10.el7                 base     80 k
    [ceph6.in][DEBUG ]  python-ceph-argparse         x86_64 2:13.2.10-0.el7              Ceph     34 k
    [ceph6.in][DEBUG ]  python-cephfs                x86_64 2:13.2.10-0.el7              Ceph     87 k
    [ceph6.in][DEBUG ]  python-cffi                  x86_64 1.6.0-5.el7                  base    218 k
    [ceph6.in][DEBUG ]  python-chardet               noarch 2.2.1-3.el7                  base    227 k
    [ceph6.in][DEBUG ]  python-cherrypy              noarch 3.2.2-4.el7                  base    422 k
    [ceph6.in][DEBUG ]  python-ipaddress             noarch 1.0.16-2.el7                 base     34 k
    [ceph6.in][DEBUG ]  python-jinja2                noarch 2.7.2-4.el7                  base    519 k
    [ceph6.in][DEBUG ]  python-mako                  noarch 0.8.1-2.el7                  base    307 k
    [ceph6.in][DEBUG ]  python-markupsafe            x86_64 0.11-10.el7                  base     25 k
    [ceph6.in][DEBUG ]  python-paste                 noarch 1.7.5.1-9.20111221hg1498.el7 base    866 k
    [ceph6.in][DEBUG ]  python-pecan                 noarch 0.4.5-2.el7                  epel    255 k
    [ceph6.in][DEBUG ]  python-ply                   noarch 3.4-11.el7                   base    123 k
    [ceph6.in][DEBUG ]  python-prettytable           noarch 0.7.2-3.el7                  base     37 k
    [ceph6.in][DEBUG ]  python-pycparser             noarch 2.14-1.el7                   base    104 k
    [ceph6.in][DEBUG ]  python-rados                 x86_64 2:13.2.10-0.el7              Ceph    189 k
    [ceph6.in][DEBUG ]  python-rbd                   x86_64 2:13.2.10-0.el7              Ceph    132 k
    [ceph6.in][DEBUG ]  python-repoze-lru            noarch 0.4-3.el7                    epel     13 k
    [ceph6.in][DEBUG ]  python-requests              noarch 2.6.0-10.el7                 base     95 k
    [ceph6.in][DEBUG ]  python-rgw                   x86_64 2:13.2.10-0.el7              Ceph     76 k
    [ceph6.in][DEBUG ]  python-routes                noarch 1.13-2.el7                   epel    640 k
    [ceph6.in][DEBUG ]  python-setuptools            noarch 0.9.8-7.el7                  base    397 k
    [ceph6.in][DEBUG ]  python-simplegeneric         noarch 0.8-7.el7                    epel     12 k
    [ceph6.in][DEBUG ]  python-singledispatch        noarch 3.4.0.2-2.el7                epel     18 k
    [ceph6.in][DEBUG ]  python-six                   noarch 1.9.0-2.el7                  base     29 k
    [ceph6.in][DEBUG ]  python-tempita               noarch 0.5.1-6.el7                  base     33 k
    [ceph6.in][DEBUG ]  python-urllib3               noarch 1.10.2-7.el7                 base    103 k
    [ceph6.in][DEBUG ]  python-webob                 noarch 1.2.3-7.el7                  base    202 k
    [ceph6.in][DEBUG ]  python-webtest               noarch 1.3.4-6.el7                  base    102 k
    [ceph6.in][DEBUG ]  python-werkzeug              noarch 0.9.1-2.el7                  extras  562 k
    [ceph6.in][DEBUG ]  python2-bcrypt               x86_64 3.1.6-2.el7                  epel     39 k
    [ceph6.in][DEBUG ]  python2-six                  noarch 1.9.0-0.el7                  epel    2.9 k
    [ceph6.in][DEBUG ]  rdma-core                    x86_64 22.4-6.el7_9                 updates  51 k
    [ceph6.in][DEBUG ]  userspace-rcu                x86_64 0.7.16-1.el7                 epel     73 k
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] Transaction Summary
    [ceph6.in][DEBUG ] ================================================================================
    [ceph6.in][DEBUG ] Install  2 Packages (+62 Dependent packages)
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] Total download size: 61 M
    [ceph6.in][DEBUG ] Installed size: 210 M
    [ceph6.in][DEBUG ] Downloading packages:
    [ceph6.in][DEBUG ] --------------------------------------------------------------------------------
    [ceph6.in][DEBUG ] Total                                              5.9 MB/s |  61 MB  00:10
    [ceph6.in][DEBUG ] Running transaction check
    [ceph6.in][DEBUG ] Running transaction test
    [ceph6.in][DEBUG ] Transaction test succeeded
    [ceph6.in][DEBUG ] Running transaction
    [ceph6.in][DEBUG ]   Installing : gperftools-libs-2.6.1-1.el7.x86_64                          1/64
    [ceph6.in][DEBUG ]   Installing : leveldb-1.12.0-11.el7.x86_64                                2/64
    [ceph6.in][DEBUG ]   Installing : python-six-1.9.0-2.el7.noarch                               3/64
    [ceph6.in][DEBUG ]   Installing : fuse-libs-2.9.2-11.el7.x86_64                               4/64
    [ceph6.in][DEBUG ]   Installing : liboath-2.6.2-1.el7.x86_64                                  5/64
    [ceph6.in][DEBUG ]   Installing : python-ipaddress-1.0.16-2.el7.noarch                        6/64
    [ceph6.in][DEBUG ]   Installing : python-webob-1.2.3-7.el7.noarch                             7/64
    [ceph6.in][DEBUG ]   Installing : python-markupsafe-0.11-10.el7.x86_64                        8/64
    [ceph6.in][DEBUG ]   Installing : pyOpenSSL-0.13.1-4.el7.x86_64                               9/64
    [ceph6.in][DEBUG ]   Installing : 2:python-ceph-argparse-13.2.10-0.el7.x86_64                10/64
    [ceph6.in][DEBUG ]   Installing : python-webtest-1.3.4-6.el7.noarch                          11/64
    [ceph6.in][DEBUG ]   Installing : python2-six-1.9.0-0.el7.noarch                             12/64
    [ceph6.in][DEBUG ]   Installing : python-singledispatch-3.4.0.2-2.el7.noarch                 13/64
    [ceph6.in][DEBUG ]   Installing : psmisc-22.20-17.el7.x86_64                                 14/64
    [ceph6.in][DEBUG ]   Installing : pciutils-3.5.1-3.el7.x86_64                                15/64
    [ceph6.in][DEBUG ]   Installing : rdma-core-22.4-6.el7_9.x86_64                              16/64
    [ceph6.in][DEBUG ]   Installing : libibverbs-22.4-6.el7_9.x86_64                             17/64
    [ceph6.in][DEBUG ]   Installing : gdisk-0.8.10-3.el7.x86_64                                  18/64
    [ceph6.in][DEBUG ]   Installing : python-simplegeneric-0.8-7.el7.noarch                      19/64
    [ceph6.in][DEBUG ]   Installing : python-tempita-0.5.1-6.el7.noarch                          20/64
    [ceph6.in][DEBUG ]   Installing : python-cherrypy-3.2.2-4.el7.noarch                         21/64
    [ceph6.in][DEBUG ]   Installing : python-prettytable-0.7.2-3.el7.noarch                      22/64
    [ceph6.in][DEBUG ]   Installing : python-werkzeug-0.9.1-2.el7.noarch                         23/64
    [ceph6.in][DEBUG ]   Installing : python-repoze-lru-0.4-3.el7.noarch                         24/64
    [ceph6.in][DEBUG ]   Installing : python-routes-1.13-2.el7.noarch                            25/64
    [ceph6.in][DEBUG ]   Installing : python-backports-1.0-8.el7.x86_64                          26/64
    [ceph6.in][DEBUG ]   Installing : python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch   27/64
    [ceph6.in][DEBUG ]   Installing : python-setuptools-0.9.8-7.el7.noarch                       28/64
    [ceph6.in][DEBUG ]   Installing : python-paste-1.7.5.1-9.20111221hg1498.el7.noarch           29/64
    [ceph6.in][DEBUG ]   Installing : python-beaker-1.5.4-10.el7.noarch                          30/64
    [ceph6.in][DEBUG ]   Installing : python-mako-0.8.1-2.el7.noarch                             31/64
    [ceph6.in][DEBUG ]   Installing : python-pecan-0.4.5-2.el7.noarch                            32/64
    [ceph6.in][DEBUG ]   Installing : python-urllib3-1.10.2-7.el7.noarch                         33/64
    [ceph6.in][DEBUG ]   Installing : python-babel-0.9.6-8.el7.noarch                            34/64
    [ceph6.in][DEBUG ]   Installing : python-jinja2-2.7.2-4.el7.noarch                           35/64
    [ceph6.in][DEBUG ]   Installing : python-chardet-2.2.1-3.el7.noarch                          36/64
    [ceph6.in][DEBUG ]   Installing : python-requests-2.6.0-10.el7.noarch                        37/64
    [ceph6.in][DEBUG ]   Installing : cryptsetup-2.0.3-6.el7.x86_64                              38/64
    [ceph6.in][DEBUG ]   Installing : libbabeltrace-1.2.4-3.el7.x86_64                           39/64
    [ceph6.in][DEBUG ]   Installing : userspace-rcu-0.7.16-1.el7.x86_64                          40/64
    [ceph6.in][DEBUG ]   Installing : lttng-ust-2.4.1-4.el7.x86_64                               41/64
    [ceph6.in][DEBUG ]   Installing : 2:librados2-13.2.10-0.el7.x86_64                           42/64
    [ceph6.in][DEBUG ]   Installing : 2:python-rados-13.2.10-0.el7.x86_64                        43/64
    [ceph6.in][DEBUG ]   Installing : 2:librbd1-13.2.10-0.el7.x86_64                             44/64
    [ceph6.in][DEBUG ]   Installing : 2:libcephfs2-13.2.10-0.el7.x86_64                          45/64
    [ceph6.in][DEBUG ]   Installing : 2:librgw2-13.2.10-0.el7.x86_64                             46/64
    [ceph6.in][DEBUG ]   Installing : 2:python-rgw-13.2.10-0.el7.x86_64                          47/64
    [ceph6.in][DEBUG ]   Installing : 2:python-cephfs-13.2.10-0.el7.x86_64                       48/64
    [ceph6.in][DEBUG ]   Installing : 2:python-rbd-13.2.10-0.el7.x86_64                          49/64
    [ceph6.in][DEBUG ]   Installing : 2:libradosstriper1-13.2.10-0.el7.x86_64                    50/64
    [ceph6.in][DEBUG ]   Installing : 2:ceph-common-13.2.10-0.el7.x86_64                         51/64
    [ceph6.in][DEBUG ]   Installing : 2:ceph-base-13.2.10-0.el7.x86_64                           52/64
    [ceph6.in][DEBUG ]   Installing : 2:ceph-selinux-13.2.10-0.el7.x86_64                        53/64
    [ceph6.in][DEBUG ]   Installing : 2:ceph-osd-13.2.10-0.el7.x86_64                            54/64
    [ceph6.in][DEBUG ]   Installing : 2:ceph-mds-13.2.10-0.el7.x86_64                            55/64
    [ceph6.in][DEBUG ]   Installing : 2:ceph-mon-13.2.10-0.el7.x86_64                            56/64
    [ceph6.in][DEBUG ]   Installing : python-ply-3.4-11.el7.noarch                               57/64
    [ceph6.in][DEBUG ]   Installing : python-pycparser-2.14-1.el7.noarch                         58/64
    [ceph6.in][DEBUG ]   Installing : python-cffi-1.6.0-5.el7.x86_64                             59/64
    [ceph6.in][DEBUG ]   Installing : python2-bcrypt-3.1.6-2.el7.x86_64                          60/64
    [ceph6.in][DEBUG ]   Installing : 2:ceph-mgr-13.2.10-0.el7.x86_64                            61/64
    [ceph6.in][DEBUG ]   Installing : mailcap-2.1.41-2.el7.noarch                                62/64
    [ceph6.in][DEBUG ]   Installing : 2:ceph-radosgw-13.2.10-0.el7.x86_64                        63/64
    [ceph6.in][DEBUG ]   Installing : 2:ceph-13.2.10-0.el7.x86_64                                64/64
    [ceph6.in][DEBUG ]   Verifying  : liboath-2.6.2-1.el7.x86_64                                  1/64
    [ceph6.in][DEBUG ]   Verifying  : python-backports-ssl_match_hostname-3.5.0.1-1.el7.noarch    2/64
    [ceph6.in][DEBUG ]   Verifying  : 2:librbd1-13.2.10-0.el7.x86_64                              3/64
    [ceph6.in][DEBUG ]   Verifying  : 2:python-ceph-argparse-13.2.10-0.el7.x86_64                 4/64
    [ceph6.in][DEBUG ]   Verifying  : mailcap-2.1.41-2.el7.noarch                                 5/64
    [ceph6.in][DEBUG ]   Verifying  : pyOpenSSL-0.13.1-4.el7.x86_64                               6/64
    [ceph6.in][DEBUG ]   Verifying  : python2-bcrypt-3.1.6-2.el7.x86_64                           7/64
    [ceph6.in][DEBUG ]   Verifying  : python-ply-3.4-11.el7.noarch                                8/64
    [ceph6.in][DEBUG ]   Verifying  : userspace-rcu-0.7.16-1.el7.x86_64                           9/64
    [ceph6.in][DEBUG ]   Verifying  : libibverbs-22.4-6.el7_9.x86_64                             10/64
    [ceph6.in][DEBUG ]   Verifying  : rdma-core-22.4-6.el7_9.x86_64                              11/64
    [ceph6.in][DEBUG ]   Verifying  : fuse-libs-2.9.2-11.el7.x86_64                              12/64
    [ceph6.in][DEBUG ]   Verifying  : python-setuptools-0.9.8-7.el7.noarch                       13/64
    [ceph6.in][DEBUG ]   Verifying  : python-routes-1.13-2.el7.noarch                            14/64
    [ceph6.in][DEBUG ]   Verifying  : 2:libcephfs2-13.2.10-0.el7.x86_64                          15/64
    [ceph6.in][DEBUG ]   Verifying  : python-urllib3-1.10.2-7.el7.noarch                         16/64
    [ceph6.in][DEBUG ]   Verifying  : libbabeltrace-1.2.4-3.el7.x86_64                           17/64
    [ceph6.in][DEBUG ]   Verifying  : python-mako-0.8.1-2.el7.noarch                             18/64
    [ceph6.in][DEBUG ]   Verifying  : python2-six-1.9.0-0.el7.noarch                             19/64
    [ceph6.in][DEBUG ]   Verifying  : 2:ceph-mgr-13.2.10-0.el7.x86_64                            20/64
    [ceph6.in][DEBUG ]   Verifying  : 2:ceph-base-13.2.10-0.el7.x86_64                           21/64
    [ceph6.in][DEBUG ]   Verifying  : python-jinja2-2.7.2-4.el7.noarch                           22/64
    [ceph6.in][DEBUG ]   Verifying  : python-pecan-0.4.5-2.el7.noarch                            23/64
    [ceph6.in][DEBUG ]   Verifying  : python-six-1.9.0-2.el7.noarch                              24/64
    [ceph6.in][DEBUG ]   Verifying  : cryptsetup-2.0.3-6.el7.x86_64                              25/64
    [ceph6.in][DEBUG ]   Verifying  : leveldb-1.12.0-11.el7.x86_64                               26/64
    [ceph6.in][DEBUG ]   Verifying  : python-singledispatch-3.4.0.2-2.el7.noarch                 27/64
    [ceph6.in][DEBUG ]   Verifying  : python-markupsafe-0.11-10.el7.x86_64                       28/64
    [ceph6.in][DEBUG ]   Verifying  : 2:python-rados-13.2.10-0.el7.x86_64                        29/64
    [ceph6.in][DEBUG ]   Verifying  : 2:python-rgw-13.2.10-0.el7.x86_64                          30/64
    [ceph6.in][DEBUG ]   Verifying  : 2:ceph-radosgw-13.2.10-0.el7.x86_64                        31/64
    [ceph6.in][DEBUG ]   Verifying  : python-chardet-2.2.1-3.el7.noarch                          32/64
    [ceph6.in][DEBUG ]   Verifying  : python-babel-0.9.6-8.el7.noarch                            33/64
    [ceph6.in][DEBUG ]   Verifying  : 2:librados2-13.2.10-0.el7.x86_64                           34/64
    [ceph6.in][DEBUG ]   Verifying  : python-paste-1.7.5.1-9.20111221hg1498.el7.noarch           35/64
    [ceph6.in][DEBUG ]   Verifying  : 2:ceph-osd-13.2.10-0.el7.x86_64                            36/64
    [ceph6.in][DEBUG ]   Verifying  : python-backports-1.0-8.el7.x86_64                          37/64
    [ceph6.in][DEBUG ]   Verifying  : lttng-ust-2.4.1-4.el7.x86_64                               38/64
    [ceph6.in][DEBUG ]   Verifying  : python-webob-1.2.3-7.el7.noarch                            39/64
    [ceph6.in][DEBUG ]   Verifying  : 2:ceph-common-13.2.10-0.el7.x86_64                         40/64
    [ceph6.in][DEBUG ]   Verifying  : python-repoze-lru-0.4-3.el7.noarch                         41/64
    [ceph6.in][DEBUG ]   Verifying  : python-werkzeug-0.9.1-2.el7.noarch                         42/64
    [ceph6.in][DEBUG ]   Verifying  : python-beaker-1.5.4-10.el7.noarch                          43/64
    [ceph6.in][DEBUG ]   Verifying  : python-cffi-1.6.0-5.el7.x86_64                             44/64
    [ceph6.in][DEBUG ]   Verifying  : 2:ceph-selinux-13.2.10-0.el7.x86_64                        45/64
    [ceph6.in][DEBUG ]   Verifying  : python-requests-2.6.0-10.el7.noarch                        46/64
    [ceph6.in][DEBUG ]   Verifying  : python-pycparser-2.14-1.el7.noarch                         47/64
    [ceph6.in][DEBUG ]   Verifying  : python-prettytable-0.7.2-3.el7.noarch                      48/64
    [ceph6.in][DEBUG ]   Verifying  : 2:librgw2-13.2.10-0.el7.x86_64                             49/64
    [ceph6.in][DEBUG ]   Verifying  : 2:ceph-mds-13.2.10-0.el7.x86_64                            50/64
    [ceph6.in][DEBUG ]   Verifying  : python-cherrypy-3.2.2-4.el7.noarch                         51/64
    [ceph6.in][DEBUG ]   Verifying  : 2:python-cephfs-13.2.10-0.el7.x86_64                       52/64
    [ceph6.in][DEBUG ]   Verifying  : python-tempita-0.5.1-6.el7.noarch                          53/64
    [ceph6.in][DEBUG ]   Verifying  : 2:python-rbd-13.2.10-0.el7.x86_64                          54/64
    [ceph6.in][DEBUG ]   Verifying  : 2:ceph-mon-13.2.10-0.el7.x86_64                            55/64
    [ceph6.in][DEBUG ]   Verifying  : gperftools-libs-2.6.1-1.el7.x86_64                         56/64
    [ceph6.in][DEBUG ]   Verifying  : python-ipaddress-1.0.16-2.el7.noarch                       57/64
    [ceph6.in][DEBUG ]   Verifying  : python-webtest-1.3.4-6.el7.noarch                          58/64
    [ceph6.in][DEBUG ]   Verifying  : 2:ceph-13.2.10-0.el7.x86_64                                59/64
    [ceph6.in][DEBUG ]   Verifying  : python-simplegeneric-0.8-7.el7.noarch                      60/64
    [ceph6.in][DEBUG ]   Verifying  : gdisk-0.8.10-3.el7.x86_64                                  61/64
    [ceph6.in][DEBUG ]   Verifying  : 2:libradosstriper1-13.2.10-0.el7.x86_64                    62/64
    [ceph6.in][DEBUG ]   Verifying  : pciutils-3.5.1-3.el7.x86_64                                63/64
    [ceph6.in][DEBUG ]   Verifying  : psmisc-22.20-17.el7.x86_64                                 64/64
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] Installed:
    [ceph6.in][DEBUG ]   ceph.x86_64 2:13.2.10-0.el7        ceph-radosgw.x86_64 2:13.2.10-0.el7
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] Dependency Installed:
    [ceph6.in][DEBUG ]   ceph-base.x86_64 2:13.2.10-0.el7
    [ceph6.in][DEBUG ]   ceph-common.x86_64 2:13.2.10-0.el7
    [ceph6.in][DEBUG ]   ceph-mds.x86_64 2:13.2.10-0.el7
    [ceph6.in][DEBUG ]   ceph-mgr.x86_64 2:13.2.10-0.el7
    [ceph6.in][DEBUG ]   ceph-mon.x86_64 2:13.2.10-0.el7
    [ceph6.in][DEBUG ]   ceph-osd.x86_64 2:13.2.10-0.el7
    [ceph6.in][DEBUG ]   ceph-selinux.x86_64 2:13.2.10-0.el7
    [ceph6.in][DEBUG ]   cryptsetup.x86_64 0:2.0.3-6.el7
    [ceph6.in][DEBUG ]   fuse-libs.x86_64 0:2.9.2-11.el7
    [ceph6.in][DEBUG ]   gdisk.x86_64 0:0.8.10-3.el7
    [ceph6.in][DEBUG ]   gperftools-libs.x86_64 0:2.6.1-1.el7
    [ceph6.in][DEBUG ]   leveldb.x86_64 0:1.12.0-11.el7
    [ceph6.in][DEBUG ]   libbabeltrace.x86_64 0:1.2.4-3.el7
    [ceph6.in][DEBUG ]   libcephfs2.x86_64 2:13.2.10-0.el7
    [ceph6.in][DEBUG ]   libibverbs.x86_64 0:22.4-6.el7_9
    [ceph6.in][DEBUG ]   liboath.x86_64 0:2.6.2-1.el7
    [ceph6.in][DEBUG ]   librados2.x86_64 2:13.2.10-0.el7
    [ceph6.in][DEBUG ]   libradosstriper1.x86_64 2:13.2.10-0.el7
    [ceph6.in][DEBUG ]   librbd1.x86_64 2:13.2.10-0.el7
    [ceph6.in][DEBUG ]   librgw2.x86_64 2:13.2.10-0.el7
    [ceph6.in][DEBUG ]   lttng-ust.x86_64 0:2.4.1-4.el7
    [ceph6.in][DEBUG ]   mailcap.noarch 0:2.1.41-2.el7
    [ceph6.in][DEBUG ]   pciutils.x86_64 0:3.5.1-3.el7
    [ceph6.in][DEBUG ]   psmisc.x86_64 0:22.20-17.el7
    [ceph6.in][DEBUG ]   pyOpenSSL.x86_64 0:0.13.1-4.el7
    [ceph6.in][DEBUG ]   python-babel.noarch 0:0.9.6-8.el7
    [ceph6.in][DEBUG ]   python-backports.x86_64 0:1.0-8.el7
    [ceph6.in][DEBUG ]   python-backports-ssl_match_hostname.noarch 0:3.5.0.1-1.el7
    [ceph6.in][DEBUG ]   python-beaker.noarch 0:1.5.4-10.el7
    [ceph6.in][DEBUG ]   python-ceph-argparse.x86_64 2:13.2.10-0.el7
    [ceph6.in][DEBUG ]   python-cephfs.x86_64 2:13.2.10-0.el7
    [ceph6.in][DEBUG ]   python-cffi.x86_64 0:1.6.0-5.el7
    [ceph6.in][DEBUG ]   python-chardet.noarch 0:2.2.1-3.el7
    [ceph6.in][DEBUG ]   python-cherrypy.noarch 0:3.2.2-4.el7
    [ceph6.in][DEBUG ]   python-ipaddress.noarch 0:1.0.16-2.el7
    [ceph6.in][DEBUG ]   python-jinja2.noarch 0:2.7.2-4.el7
    [ceph6.in][DEBUG ]   python-mako.noarch 0:0.8.1-2.el7
    [ceph6.in][DEBUG ]   python-markupsafe.x86_64 0:0.11-10.el7
    [ceph6.in][DEBUG ]   python-paste.noarch 0:1.7.5.1-9.20111221hg1498.el7
    [ceph6.in][DEBUG ]   python-pecan.noarch 0:0.4.5-2.el7
    [ceph6.in][DEBUG ]   python-ply.noarch 0:3.4-11.el7
    [ceph6.in][DEBUG ]   python-prettytable.noarch 0:0.7.2-3.el7
    [ceph6.in][DEBUG ]   python-pycparser.noarch 0:2.14-1.el7
    [ceph6.in][DEBUG ]   python-rados.x86_64 2:13.2.10-0.el7
    [ceph6.in][DEBUG ]   python-rbd.x86_64 2:13.2.10-0.el7
    [ceph6.in][DEBUG ]   python-repoze-lru.noarch 0:0.4-3.el7
    [ceph6.in][DEBUG ]   python-requests.noarch 0:2.6.0-10.el7
    [ceph6.in][DEBUG ]   python-rgw.x86_64 2:13.2.10-0.el7
    [ceph6.in][DEBUG ]   python-routes.noarch 0:1.13-2.el7
    [ceph6.in][DEBUG ]   python-setuptools.noarch 0:0.9.8-7.el7
    [ceph6.in][DEBUG ]   python-simplegeneric.noarch 0:0.8-7.el7
    [ceph6.in][DEBUG ]   python-singledispatch.noarch 0:3.4.0.2-2.el7
    [ceph6.in][DEBUG ]   python-six.noarch 0:1.9.0-2.el7
    [ceph6.in][DEBUG ]   python-tempita.noarch 0:0.5.1-6.el7
    [ceph6.in][DEBUG ]   python-urllib3.noarch 0:1.10.2-7.el7
    [ceph6.in][DEBUG ]   python-webob.noarch 0:1.2.3-7.el7
    [ceph6.in][DEBUG ]   python-webtest.noarch 0:1.3.4-6.el7
    [ceph6.in][DEBUG ]   python-werkzeug.noarch 0:0.9.1-2.el7
    [ceph6.in][DEBUG ]   python2-bcrypt.x86_64 0:3.1.6-2.el7
    [ceph6.in][DEBUG ]   python2-six.noarch 0:1.9.0-0.el7
    [ceph6.in][DEBUG ]   rdma-core.x86_64 0:22.4-6.el7_9
    [ceph6.in][DEBUG ]   userspace-rcu.x86_64 0:0.7.16-1.el7
    [ceph6.in][DEBUG ]
    [ceph6.in][DEBUG ] Complete!
    [ceph6.in][INFO  ] Running command: sudo ceph --version
    [ceph6.in][DEBUG ] ceph version 13.2.10 (564bdc4ae87418a232fc901524470e1a0f76d641) mimic (stable)
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy admin ceph6.in
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy admin ceph6.in
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f1a56872950>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  client                        : ['ceph6.in']
    [ceph_deploy.cli][INFO  ]  func                          : <function admin at 0x7f1a5710a320>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.admin][DEBUG ] Pushing admin keys and conf to ceph6.in
    [ceph6.in][DEBUG ] connection detected need for sudo
    [ceph6.in][DEBUG ] connected to host: ceph6.in
    [ceph6.in][DEBUG ] detect platform information from remote host
    [ceph6.in][DEBUG ] detect machine type
    [ceph6.in][DEBUG ] write cluster configuration to /etc/ceph/{cluster}.conf
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy mgr create ceph6.in
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy mgr create ceph6.in
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  mgr                           : [('ceph6.in', 'ceph6.in')]
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  subcommand                    : create
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f36f13c1b90>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  func                          : <function mgr at 0x7f36f1cac230>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.mgr][DEBUG ] Deploying mgr, cluster ceph hosts ceph6.in:ceph6.in
    [ceph6.in][DEBUG ] connection detected need for sudo
    [ceph6.in][DEBUG ] connected to host: ceph6.in
    [ceph6.in][DEBUG ] detect platform information from remote host
    [ceph6.in][DEBUG ] detect machine type
    [ceph_deploy.mgr][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph_deploy.mgr][DEBUG ] remote host will use systemd
    [ceph_deploy.mgr][DEBUG ] deploying mgr bootstrap to ceph6.in
    [ceph6.in][DEBUG ] write cluster configuration to /etc/ceph/{cluster}.conf
    [ceph6.in][WARNIN] mgr keyring does not exist yet, creating one
    [ceph6.in][DEBUG ] create a keyring file
    [ceph6.in][DEBUG ] create path recursively if it doesn't exist
    [ceph6.in][INFO  ] Running command: sudo ceph --cluster ceph --name client.bootstrap-mgr --keyring /var/lib/ceph/bootstrap-mgr/ceph.keyring auth get-or-create mgr.ceph6.in mon allow profile mgr osd allow * mds allow * -o /var/lib/ceph/mgr/ceph-ceph6.in/keyring
    [ceph6.in][INFO  ] Running command: sudo systemctl enable ceph-mgr@ceph6.in
    [ceph6.in][WARNIN] Created symlink from /etc/systemd/system/ceph-mgr.target.wants/ceph-mgr@ceph6.in.service to /usr/lib/systemd/system/ceph-mgr@.service.
    [ceph6.in][INFO  ] Running command: sudo systemctl start ceph-mgr@ceph6.in
    [ceph6.in][INFO  ] Running command: sudo systemctl enable ceph.target
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy disk list ceph6.in
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy disk list ceph6.in
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  debug                         : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  subcommand                    : list
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f9c8fbb07e8>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  host                          : ['ceph6.in']
    [ceph_deploy.cli][INFO  ]  func                          : <function disk at 0x7f9c8fdfea28>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph6.in][DEBUG ] connection detected need for sudo
    [ceph6.in][DEBUG ] connected to host: ceph6.in
    [ceph6.in][DEBUG ] detect platform information from remote host
    [ceph6.in][DEBUG ] detect machine type
    [ceph6.in][DEBUG ] find the location of an executable
    [ceph6.in][INFO  ] Running command: sudo fdisk -l
    [ceph6.in][INFO  ] Disk /dev/sda: 21.5 GB, 21474836480 bytes, 41943040 sectors
    [ceph6.in][INFO  ] Disk /dev/sdb: 21.5 GB, 21474836480 bytes, 41943040 sectors
    [ceph6.in][INFO  ] Disk /dev/sdd: 21.5 GB, 21474836480 bytes, 41943040 sectors
    [ceph6.in][INFO  ] Disk /dev/sdc: 21.5 GB, 21474836480 bytes, 41943040 sectors
    [ceph6.in][INFO  ] Disk /dev/mapper/centos-root: 18.2 GB, 18249416704 bytes, 35643392 sectors
    [ceph6.in][INFO  ] Disk /dev/mapper/centos-swap: 2147 MB, 2147483648 bytes, 4194304 sectors
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy disk zap ceph6.in /dev/sdb
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy disk zap ceph6.in /dev/sdb
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  debug                         : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  subcommand                    : zap
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f598f4467e8>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  host                          : ceph6.in
    [ceph_deploy.cli][INFO  ]  func                          : <function disk at 0x7f598f694a28>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  disk                          : ['/dev/sdb']
    [ceph_deploy.osd][DEBUG ] zapping /dev/sdb on ceph6.in
    [ceph6.in][DEBUG ] connection detected need for sudo
    [ceph6.in][DEBUG ] connected to host: ceph6.in
    [ceph6.in][DEBUG ] detect platform information from remote host
    [ceph6.in][DEBUG ] detect machine type
    [ceph6.in][DEBUG ] find the location of an executable
    [ceph_deploy.osd][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph6.in][DEBUG ] zeroing last few blocks of device
    [ceph6.in][DEBUG ] find the location of an executable
    [ceph6.in][INFO  ] Running command: sudo /usr/sbin/ceph-volume lvm zap /dev/sdb
    [ceph6.in][WARNIN] --> Zapping: /dev/sdb
    [ceph6.in][WARNIN] --> --destroy was not specified, but zapping a whole device will remove the partition table
    [ceph6.in][WARNIN] Running command: /bin/dd if=/dev/zero of=/dev/sdb bs=1M count=10 conv=fsync
    [ceph6.in][WARNIN]  stderr: 10+0 records in
    [ceph6.in][WARNIN] 10+0 records out
    [ceph6.in][WARNIN] 10485760 bytes (10 MB) copied, 0.00613356 s, 1.7 GB/s
    [ceph6.in][WARNIN] --> Zapping successful for: <Raw Device: /dev/sdb>
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy disk zap ceph6.in /dev/sdc
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy disk zap ceph6.in /dev/sdc
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  debug                         : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  subcommand                    : zap
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f4042df77e8>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  host                          : ceph6.in
    [ceph_deploy.cli][INFO  ]  func                          : <function disk at 0x7f4043045a28>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  disk                          : ['/dev/sdc']
    [ceph_deploy.osd][DEBUG ] zapping /dev/sdc on ceph6.in
    [ceph6.in][DEBUG ] connection detected need for sudo
    [ceph6.in][DEBUG ] connected to host: ceph6.in
    [ceph6.in][DEBUG ] detect platform information from remote host
    [ceph6.in][DEBUG ] detect machine type
    [ceph6.in][DEBUG ] find the location of an executable
    [ceph_deploy.osd][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph6.in][DEBUG ] zeroing last few blocks of device
    [ceph6.in][DEBUG ] find the location of an executable
    [ceph6.in][INFO  ] Running command: sudo /usr/sbin/ceph-volume lvm zap /dev/sdc
    [ceph6.in][WARNIN] --> Zapping: /dev/sdc
    [ceph6.in][WARNIN] --> --destroy was not specified, but zapping a whole device will remove the partition table
    [ceph6.in][WARNIN] Running command: /bin/dd if=/dev/zero of=/dev/sdc bs=1M count=10 conv=fsync
    [ceph6.in][WARNIN]  stderr: 10+0 records in
    [ceph6.in][WARNIN] 10+0 records out
    [ceph6.in][WARNIN] 10485760 bytes (10 MB) copied, 0.00553697 s, 1.9 GB/s
    [ceph6.in][WARNIN] --> Zapping successful for: <Raw Device: /dev/sdc>
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy disk zap ceph6.in /dev/sdd
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy disk zap ceph6.in /dev/sdd
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  debug                         : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  subcommand                    : zap
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f808f6477e8>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  host                          : ceph6.in
    [ceph_deploy.cli][INFO  ]  func                          : <function disk at 0x7f808f895a28>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  disk                          : ['/dev/sdd']
    [ceph_deploy.osd][DEBUG ] zapping /dev/sdd on ceph6.in
    [ceph6.in][DEBUG ] connection detected need for sudo
    [ceph6.in][DEBUG ] connected to host: ceph6.in
    [ceph6.in][DEBUG ] detect platform information from remote host
    [ceph6.in][DEBUG ] detect machine type
    [ceph6.in][DEBUG ] find the location of an executable
    [ceph_deploy.osd][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph6.in][DEBUG ] zeroing last few blocks of device
    [ceph6.in][DEBUG ] find the location of an executable
    [ceph6.in][INFO  ] Running command: sudo /usr/sbin/ceph-volume lvm zap /dev/sdd
    [ceph6.in][WARNIN] --> Zapping: /dev/sdd
    [ceph6.in][WARNIN] --> --destroy was not specified, but zapping a whole device will remove the partition table
    [ceph6.in][WARNIN] Running command: /bin/dd if=/dev/zero of=/dev/sdd bs=1M count=10 conv=fsync
    [ceph6.in][WARNIN]  stderr: 10+0 records in
    [ceph6.in][WARNIN] 10+0 records out
    [ceph6.in][WARNIN] 10485760 bytes (10 MB) copied, 0.00639854 s, 1.6 GB/s
    [ceph6.in][WARNIN] --> Zapping successful for: <Raw Device: /dev/sdd>
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy osd create --data /dev/sdb ceph6.in
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy osd create --data /dev/sdb ceph6.in
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  bluestore                     : None
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7fa604b01908>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  fs_type                       : xfs
    [ceph_deploy.cli][INFO  ]  block_wal                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  journal                       : None
    [ceph_deploy.cli][INFO  ]  subcommand                    : create
    [ceph_deploy.cli][INFO  ]  host                          : ceph6.in
    [ceph_deploy.cli][INFO  ]  filestore                     : None
    [ceph_deploy.cli][INFO  ]  func                          : <function osd at 0x7fa604d4a9b0>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  zap_disk                      : False
    [ceph_deploy.cli][INFO  ]  data                          : /dev/sdb
    [ceph_deploy.cli][INFO  ]  block_db                      : None
    [ceph_deploy.cli][INFO  ]  dmcrypt                       : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  dmcrypt_key_dir               : /etc/ceph/dmcrypt-keys
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  debug                         : False
    [ceph_deploy.osd][DEBUG ] Creating OSD on cluster ceph with data device /dev/sdb
    [ceph6.in][DEBUG ] connection detected need for sudo
    [ceph6.in][DEBUG ] connected to host: ceph6.in
    [ceph6.in][DEBUG ] detect platform information from remote host
    [ceph6.in][DEBUG ] detect machine type
    [ceph6.in][DEBUG ] find the location of an executable
    [ceph_deploy.osd][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph_deploy.osd][DEBUG ] Deploying osd to ceph6.in
    [ceph6.in][DEBUG ] write cluster configuration to /etc/ceph/{cluster}.conf
    [ceph6.in][WARNIN] osd keyring does not exist yet, creating one
    [ceph6.in][DEBUG ] create a keyring file
    [ceph6.in][DEBUG ] find the location of an executable
    [ceph6.in][INFO  ] Running command: sudo /usr/sbin/ceph-volume --cluster ceph lvm create --bluestore --data /dev/sdb
    [ceph6.in][WARNIN] Running command: /bin/ceph-authtool --gen-print-key
    [ceph6.in][WARNIN] Running command: /bin/ceph --cluster ceph --name client.bootstrap-osd --keyring /var/lib/ceph/bootstrap-osd/ceph.keyring -i - osd new 8d12084f-1991-477d-90ed-378617ec861f
    [ceph6.in][WARNIN] Running command: /sbin/vgcreate --force --yes ceph-43ef347e-04c4-41cf-9b3e-ea5b1751fb52 /dev/sdb
    [ceph6.in][WARNIN]  stdout: Physical volume "/dev/sdb" successfully created.
    [ceph6.in][WARNIN]  stdout: Volume group "ceph-43ef347e-04c4-41cf-9b3e-ea5b1751fb52" successfully created
    [ceph6.in][WARNIN] Running command: /sbin/lvcreate --yes -l 100%FREE -n osd-block-8d12084f-1991-477d-90ed-378617ec861f ceph-43ef347e-04c4-41cf-9b3e-ea5b1751fb52
    [ceph6.in][WARNIN]  stdout: Logical volume "osd-block-8d12084f-1991-477d-90ed-378617ec861f" created.
    [ceph6.in][WARNIN] Running command: /bin/ceph-authtool --gen-print-key
    [ceph6.in][WARNIN] Running command: /bin/mount -t tmpfs tmpfs /var/lib/ceph/osd/ceph-6
    [ceph6.in][WARNIN] Running command: /bin/chown -h ceph:ceph /dev/ceph-43ef347e-04c4-41cf-9b3e-ea5b1751fb52/osd-block-8d12084f-1991-477d-90ed-378617ec861f
    [ceph6.in][WARNIN] Running command: /bin/chown -R ceph:ceph /dev/dm-2
    [ceph6.in][WARNIN] Running command: /bin/ln -s /dev/ceph-43ef347e-04c4-41cf-9b3e-ea5b1751fb52/osd-block-8d12084f-1991-477d-90ed-378617ec861f /var/lib/ceph/osd/ceph-6/block
    [ceph6.in][WARNIN] Running command: /bin/ceph --cluster ceph --name client.bootstrap-osd --keyring /var/lib/ceph/bootstrap-osd/ceph.keyring mon getmap -o /var/lib/ceph/osd/ceph-6/activate.monmap
    [ceph6.in][WARNIN]  stderr: got monmap epoch 1
    [ceph6.in][WARNIN] Running command: /bin/ceph-authtool /var/lib/ceph/osd/ceph-6/keyring --create-keyring --name osd.6 --add-key AQDcLLRkq0DFLhAAJ/wfKV1bU57M0bnxR1D+wQ==
    [ceph6.in][WARNIN]  stdout: creating /var/lib/ceph/osd/ceph-6/keyring
    [ceph6.in][WARNIN] added entity osd.6 auth auth(auid = 18446744073709551615 key=AQDcLLRkq0DFLhAAJ/wfKV1bU57M0bnxR1D+wQ== with 0 caps)
    [ceph6.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-6/keyring
    [ceph6.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-6/
    [ceph6.in][WARNIN] Running command: /bin/ceph-osd --cluster ceph --osd-objectstore bluestore --mkfs -i 6 --monmap /var/lib/ceph/osd/ceph-6/activate.monmap --keyfile - --osd-data /var/lib/ceph/osd/ceph-6/ --osd-uuid 8d12084f-1991-477d-90ed-378617ec861f --setuser ceph --setgroup ceph
    [ceph6.in][WARNIN] --> ceph-volume lvm prepare successful for: /dev/sdb
    [ceph6.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-6
    [ceph6.in][WARNIN] Running command: /bin/ceph-bluestore-tool --cluster=ceph prime-osd-dir --dev /dev/ceph-43ef347e-04c4-41cf-9b3e-ea5b1751fb52/osd-block-8d12084f-1991-477d-90ed-378617ec861f --path /var/lib/ceph/osd/ceph-6 --no-mon-config
    [ceph6.in][WARNIN] Running command: /bin/ln -snf /dev/ceph-43ef347e-04c4-41cf-9b3e-ea5b1751fb52/osd-block-8d12084f-1991-477d-90ed-378617ec861f /var/lib/ceph/osd/ceph-6/block
    [ceph6.in][WARNIN] Running command: /bin/chown -h ceph:ceph /var/lib/ceph/osd/ceph-6/block
    [ceph6.in][WARNIN] Running command: /bin/chown -R ceph:ceph /dev/dm-2
    [ceph6.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-6
    [ceph6.in][WARNIN] Running command: /bin/systemctl enable ceph-volume@lvm-6-8d12084f-1991-477d-90ed-378617ec861f
    [ceph6.in][WARNIN]  stderr: Created symlink from /etc/systemd/system/multi-user.target.wants/ceph-volume@lvm-6-8d12084f-1991-477d-90ed-378617ec861f.service to /usr/lib/systemd/system/ceph-volume@.service.
    [ceph6.in][WARNIN] Running command: /bin/systemctl enable --runtime ceph-osd@6
    [ceph6.in][WARNIN]  stderr: Created symlink from /run/systemd/system/ceph-osd.target.wants/ceph-osd@6.service to /usr/lib/systemd/system/ceph-osd@.service.
    [ceph6.in][WARNIN] Running command: /bin/systemctl start ceph-osd@6
    [ceph6.in][WARNIN] --> ceph-volume lvm activate successful for osd ID: 6
    [ceph6.in][WARNIN] --> ceph-volume lvm create successful for: /dev/sdb
    [ceph6.in][INFO  ] checking OSD status...
    [ceph6.in][DEBUG ] find the location of an executable
    [ceph6.in][INFO  ] Running command: sudo /bin/ceph --cluster=ceph osd stat --format=json
    [ceph_deploy.osd][DEBUG ] Host ceph6.in is now ready for osd use.
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy osd create --data /dev/sdc ceph6.in
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy osd create --data /dev/sdc ceph6.in
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  bluestore                     : None
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7f9d13b96908>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  fs_type                       : xfs
    [ceph_deploy.cli][INFO  ]  block_wal                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  journal                       : None
    [ceph_deploy.cli][INFO  ]  subcommand                    : create
    [ceph_deploy.cli][INFO  ]  host                          : ceph6.in
    [ceph_deploy.cli][INFO  ]  filestore                     : None
    [ceph_deploy.cli][INFO  ]  func                          : <function osd at 0x7f9d13ddf9b0>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  zap_disk                      : False
    [ceph_deploy.cli][INFO  ]  data                          : /dev/sdc
    [ceph_deploy.cli][INFO  ]  block_db                      : None
    [ceph_deploy.cli][INFO  ]  dmcrypt                       : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  dmcrypt_key_dir               : /etc/ceph/dmcrypt-keys
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  debug                         : False
    [ceph_deploy.osd][DEBUG ] Creating OSD on cluster ceph with data device /dev/sdc
    [ceph6.in][DEBUG ] connection detected need for sudo
    [ceph6.in][DEBUG ] connected to host: ceph6.in
    [ceph6.in][DEBUG ] detect platform information from remote host
    [ceph6.in][DEBUG ] detect machine type
    [ceph6.in][DEBUG ] find the location of an executable
    [ceph_deploy.osd][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph_deploy.osd][DEBUG ] Deploying osd to ceph6.in
    [ceph6.in][DEBUG ] write cluster configuration to /etc/ceph/{cluster}.conf
    [ceph6.in][DEBUG ] find the location of an executable
    [ceph6.in][INFO  ] Running command: sudo /usr/sbin/ceph-volume --cluster ceph lvm create --bluestore --data /dev/sdc
    [ceph6.in][WARNIN] Running command: /bin/ceph-authtool --gen-print-key
    [ceph6.in][WARNIN] Running command: /bin/ceph --cluster ceph --name client.bootstrap-osd --keyring /var/lib/ceph/bootstrap-osd/ceph.keyring -i - osd new e593f28f-55ef-455a-be95-aee0c5543540
    [ceph6.in][WARNIN] Running command: /sbin/vgcreate --force --yes ceph-9de75551-0b02-4435-8443-95bc02e334a5 /dev/sdc
    [ceph6.in][WARNIN]  stdout: Physical volume "/dev/sdc" successfully created.
    [ceph6.in][WARNIN]  stdout: Volume group "ceph-9de75551-0b02-4435-8443-95bc02e334a5" successfully created
    [ceph6.in][WARNIN] Running command: /sbin/lvcreate --yes -l 100%FREE -n osd-block-e593f28f-55ef-455a-be95-aee0c5543540 ceph-9de75551-0b02-4435-8443-95bc02e334a5
    [ceph6.in][WARNIN]  stdout: Logical volume "osd-block-e593f28f-55ef-455a-be95-aee0c5543540" created.
    [ceph6.in][WARNIN] Running command: /bin/ceph-authtool --gen-print-key
    [ceph6.in][WARNIN] Running command: /bin/mount -t tmpfs tmpfs /var/lib/ceph/osd/ceph-7
    [ceph6.in][WARNIN] Running command: /bin/chown -h ceph:ceph /dev/ceph-9de75551-0b02-4435-8443-95bc02e334a5/osd-block-e593f28f-55ef-455a-be95-aee0c5543540
    [ceph6.in][WARNIN] Running command: /bin/chown -R ceph:ceph /dev/dm-3
    [ceph6.in][WARNIN] Running command: /bin/ln -s /dev/ceph-9de75551-0b02-4435-8443-95bc02e334a5/osd-block-e593f28f-55ef-455a-be95-aee0c5543540 /var/lib/ceph/osd/ceph-7/block
    [ceph6.in][WARNIN] Running command: /bin/ceph --cluster ceph --name client.bootstrap-osd --keyring /var/lib/ceph/bootstrap-osd/ceph.keyring mon getmap -o /var/lib/ceph/osd/ceph-7/activate.monmap
    [ceph6.in][WARNIN]  stderr: got monmap epoch 1
    [ceph6.in][WARNIN] Running command: /bin/ceph-authtool /var/lib/ceph/osd/ceph-7/keyring --create-keyring --name osd.7 --add-key AQDyLLRk85/5LRAA2+UNucd2RKi/qrpXUl0qag==
    [ceph6.in][WARNIN]  stdout: creating /var/lib/ceph/osd/ceph-7/keyring
    [ceph6.in][WARNIN] added entity osd.7 auth auth(auid = 18446744073709551615 key=AQDyLLRk85/5LRAA2+UNucd2RKi/qrpXUl0qag== with 0 caps)
    [ceph6.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-7/keyring
    [ceph6.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-7/
    [ceph6.in][WARNIN] Running command: /bin/ceph-osd --cluster ceph --osd-objectstore bluestore --mkfs -i 7 --monmap /var/lib/ceph/osd/ceph-7/activate.monmap --keyfile - --osd-data /var/lib/ceph/osd/ceph-7/ --osd-uuid e593f28f-55ef-455a-be95-aee0c5543540 --setuser ceph --setgroup ceph
    [ceph6.in][WARNIN] --> ceph-volume lvm prepare successful for: /dev/sdc
    [ceph6.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-7
    [ceph6.in][WARNIN] Running command: /bin/ceph-bluestore-tool --cluster=ceph prime-osd-dir --dev /dev/ceph-9de75551-0b02-4435-8443-95bc02e334a5/osd-block-e593f28f-55ef-455a-be95-aee0c5543540 --path /var/lib/ceph/osd/ceph-7 --no-mon-config
    [ceph6.in][WARNIN] Running command: /bin/ln -snf /dev/ceph-9de75551-0b02-4435-8443-95bc02e334a5/osd-block-e593f28f-55ef-455a-be95-aee0c5543540 /var/lib/ceph/osd/ceph-7/block
    [ceph6.in][WARNIN] Running command: /bin/chown -h ceph:ceph /var/lib/ceph/osd/ceph-7/block
    [ceph6.in][WARNIN] Running command: /bin/chown -R ceph:ceph /dev/dm-3
    [ceph6.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-7
    [ceph6.in][WARNIN] Running command: /bin/systemctl enable ceph-volume@lvm-7-e593f28f-55ef-455a-be95-aee0c5543540
    [ceph6.in][WARNIN]  stderr: Created symlink from /etc/systemd/system/multi-user.target.wants/ceph-volume@lvm-7-e593f28f-55ef-455a-be95-aee0c5543540.service to /usr/lib/systemd/system/ceph-volume@.service.
    [ceph6.in][WARNIN] Running command: /bin/systemctl enable --runtime ceph-osd@7
    [ceph6.in][WARNIN]  stderr: Created symlink from /run/systemd/system/ceph-osd.target.wants/ceph-osd@7.service to /usr/lib/systemd/system/ceph-osd@.service.
    [ceph6.in][WARNIN] Running command: /bin/systemctl start ceph-osd@7
    [ceph6.in][WARNIN] --> ceph-volume lvm activate successful for osd ID: 7
    [ceph6.in][WARNIN] --> ceph-volume lvm create successful for: /dev/sdc
    [ceph6.in][INFO  ] checking OSD status...
    [ceph6.in][DEBUG ] find the location of an executable
    [ceph6.in][INFO  ] Running command: sudo /bin/ceph --cluster=ceph osd stat --format=json
    [ceph_deploy.osd][DEBUG ] Host ceph6.in is now ready for osd use.
    [cephadm@ceph2 ceph_cluster]$ ceph-deploy osd create --data /dev/sdd ceph6.in
    [ceph_deploy.conf][DEBUG ] found configuration file at: /home/cephadm/.cephdeploy.conf
    [ceph_deploy.cli][INFO  ] Invoked (2.0.1): /bin/ceph-deploy osd create --data /dev/sdd ceph6.in
    [ceph_deploy.cli][INFO  ] ceph-deploy options:
    [ceph_deploy.cli][INFO  ]  verbose                       : False
    [ceph_deploy.cli][INFO  ]  bluestore                     : None
    [ceph_deploy.cli][INFO  ]  cd_conf                       : <ceph_deploy.conf.cephdeploy.Conf instance at 0x7fc36f109908>
    [ceph_deploy.cli][INFO  ]  cluster                       : ceph
    [ceph_deploy.cli][INFO  ]  fs_type                       : xfs
    [ceph_deploy.cli][INFO  ]  block_wal                     : None
    [ceph_deploy.cli][INFO  ]  default_release               : False
    [ceph_deploy.cli][INFO  ]  username                      : None
    [ceph_deploy.cli][INFO  ]  journal                       : None
    [ceph_deploy.cli][INFO  ]  subcommand                    : create
    [ceph_deploy.cli][INFO  ]  host                          : ceph6.in
    [ceph_deploy.cli][INFO  ]  filestore                     : None
    [ceph_deploy.cli][INFO  ]  func                          : <function osd at 0x7fc36f3529b0>
    [ceph_deploy.cli][INFO  ]  ceph_conf                     : None
    [ceph_deploy.cli][INFO  ]  zap_disk                      : False
    [ceph_deploy.cli][INFO  ]  data                          : /dev/sdd
    [ceph_deploy.cli][INFO  ]  block_db                      : None
    [ceph_deploy.cli][INFO  ]  dmcrypt                       : False
    [ceph_deploy.cli][INFO  ]  overwrite_conf                : False
    [ceph_deploy.cli][INFO  ]  dmcrypt_key_dir               : /etc/ceph/dmcrypt-keys
    [ceph_deploy.cli][INFO  ]  quiet                         : False
    [ceph_deploy.cli][INFO  ]  debug                         : False
    [ceph_deploy.osd][DEBUG ] Creating OSD on cluster ceph with data device /dev/sdd
    [ceph6.in][DEBUG ] connection detected need for sudo
    [ceph6.in][DEBUG ] connected to host: ceph6.in
    [ceph6.in][DEBUG ] detect platform information from remote host
    [ceph6.in][DEBUG ] detect machine type
    [ceph6.in][DEBUG ] find the location of an executable
    [ceph_deploy.osd][INFO  ] Distro info: CentOS Linux 7.9.2009 Core
    [ceph_deploy.osd][DEBUG ] Deploying osd to ceph6.in
    [ceph6.in][DEBUG ] write cluster configuration to /etc/ceph/{cluster}.conf
    [ceph6.in][DEBUG ] find the location of an executable
    [ceph6.in][INFO  ] Running command: sudo /usr/sbin/ceph-volume --cluster ceph lvm create --bluestore --data /dev/sdd
    [ceph6.in][WARNIN] Running command: /bin/ceph-authtool --gen-print-key
    [ceph6.in][WARNIN] Running command: /bin/ceph --cluster ceph --name client.bootstrap-osd --keyring /var/lib/ceph/bootstrap-osd/ceph.keyring -i - osd new 8b2d981d-7572-437d-bbd1-049ae951f380
    [ceph6.in][WARNIN] Running command: /sbin/vgcreate --force --yes ceph-00a340ce-bff3-461b-b377-f065bbded035 /dev/sdd
    [ceph6.in][WARNIN]  stdout: Physical volume "/dev/sdd" successfully created.
    [ceph6.in][WARNIN]  stdout: Volume group "ceph-00a340ce-bff3-461b-b377-f065bbded035" successfully created
    [ceph6.in][WARNIN] Running command: /sbin/lvcreate --yes -l 100%FREE -n osd-block-8b2d981d-7572-437d-bbd1-049ae951f380 ceph-00a340ce-bff3-461b-b377-f065bbded035
    [ceph6.in][WARNIN]  stdout: Logical volume "osd-block-8b2d981d-7572-437d-bbd1-049ae951f380" created.
    [ceph6.in][WARNIN] Running command: /bin/ceph-authtool --gen-print-key
    [ceph6.in][WARNIN] Running command: /bin/mount -t tmpfs tmpfs /var/lib/ceph/osd/ceph-8
    [ceph6.in][WARNIN] Running command: /bin/chown -h ceph:ceph /dev/ceph-00a340ce-bff3-461b-b377-f065bbded035/osd-block-8b2d981d-7572-437d-bbd1-049ae951f380
    [ceph6.in][WARNIN] Running command: /bin/chown -R ceph:ceph /dev/dm-4
    [ceph6.in][WARNIN] Running command: /bin/ln -s /dev/ceph-00a340ce-bff3-461b-b377-f065bbded035/osd-block-8b2d981d-7572-437d-bbd1-049ae951f380 /var/lib/ceph/osd/ceph-8/block
    [ceph6.in][WARNIN] Running command: /bin/ceph --cluster ceph --name client.bootstrap-osd --keyring /var/lib/ceph/bootstrap-osd/ceph.keyring mon getmap -o /var/lib/ceph/osd/ceph-8/activate.monmap
    [ceph6.in][WARNIN]  stderr: got monmap epoch 1
    [ceph6.in][WARNIN] Running command: /bin/ceph-authtool /var/lib/ceph/osd/ceph-8/keyring --create-keyring --name osd.8 --add-key AQAALbRkwHVGExAABzBVLHPJfFMZgZ1BGrsJbw==
    [ceph6.in][WARNIN]  stdout: creating /var/lib/ceph/osd/ceph-8/keyring
    [ceph6.in][WARNIN] added entity osd.8 auth auth(auid = 18446744073709551615 key=AQAALbRkwHVGExAABzBVLHPJfFMZgZ1BGrsJbw== with 0 caps)
    [ceph6.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-8/keyring
    [ceph6.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-8/
    [ceph6.in][WARNIN] Running command: /bin/ceph-osd --cluster ceph --osd-objectstore bluestore --mkfs -i 8 --monmap /var/lib/ceph/osd/ceph-8/activate.monmap --keyfile - --osd-data /var/lib/ceph/osd/ceph-8/ --osd-uuid 8b2d981d-7572-437d-bbd1-049ae951f380 --setuser ceph --setgroup ceph
    [ceph6.in][WARNIN] --> ceph-volume lvm prepare successful for: /dev/sdd
    [ceph6.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-8
    [ceph6.in][WARNIN] Running command: /bin/ceph-bluestore-tool --cluster=ceph prime-osd-dir --dev /dev/ceph-00a340ce-bff3-461b-b377-f065bbded035/osd-block-8b2d981d-7572-437d-bbd1-049ae951f380 --path /var/lib/ceph/osd/ceph-8 --no-mon-config
    [ceph6.in][WARNIN] Running command: /bin/ln -snf /dev/ceph-00a340ce-bff3-461b-b377-f065bbded035/osd-block-8b2d981d-7572-437d-bbd1-049ae951f380 /var/lib/ceph/osd/ceph-8/block
    [ceph6.in][WARNIN] Running command: /bin/chown -h ceph:ceph /var/lib/ceph/osd/ceph-8/block
    [ceph6.in][WARNIN] Running command: /bin/chown -R ceph:ceph /dev/dm-4
    [ceph6.in][WARNIN] Running command: /bin/chown -R ceph:ceph /var/lib/ceph/osd/ceph-8
    [ceph6.in][WARNIN] Running command: /bin/systemctl enable ceph-volume@lvm-8-8b2d981d-7572-437d-bbd1-049ae951f380
    [ceph6.in][WARNIN]  stderr: Created symlink from /etc/systemd/system/multi-user.target.wants/ceph-volume@lvm-8-8b2d981d-7572-437d-bbd1-049ae951f380.service to /usr/lib/systemd/system/ceph-volume@.service.
    [ceph6.in][WARNIN] Running command: /bin/systemctl enable --runtime ceph-osd@8
    [ceph6.in][WARNIN]  stderr: Created symlink from /run/systemd/system/ceph-osd.target.wants/ceph-osd@8.service to /usr/lib/systemd/system/ceph-osd@.service.
    [ceph6.in][WARNIN] Running command: /bin/systemctl start ceph-osd@8
    [ceph6.in][WARNIN] --> ceph-volume lvm activate successful for osd ID: 8
    [ceph6.in][WARNIN] --> ceph-volume lvm create successful for: /dev/sdd
    [ceph6.in][INFO  ] checking OSD status...
    [ceph6.in][DEBUG ] find the location of an executable
    [ceph6.in][INFO  ] Running command: sudo /bin/ceph --cluster=ceph osd stat --format=json
    [ceph_deploy.osd][DEBUG ] Host ceph6.in is now ready for osd use.
    [cephadm@ceph2 ceph_cluster]$ sudo ceph -s
      cluster:
        id:     5cfc246a-5a14-4337-98b2-58d2a2e19b18
        health: HEALTH_WARN
                application not enabled on 1 pool(s)
                1 pools have pg_num > pgp_num
    
      services:
        mon: 1 daemons, quorum ceph1
        mgr: ceph3.in(active), standbys: ceph4.in, ceph6.in
        osd: 9 osds: 9 up, 9 in
    
      data:
        pools:   1 pools, 200 pgs
        objects: 16  objects, 14 MiB
        usage:   9.1 GiB used, 171 GiB / 180 GiB avail
        pgs:     200 active+clean
    
    [cephadm@ceph2 ceph_cluster]$ sudo ceph osd tree
    ID CLASS WEIGHT  TYPE NAME      STATUS REWEIGHT PRI-AFF
    -1       0.17537 root default
    -3       0.05846     host ceph3
     0   hdd 0.01949         osd.0      up  1.00000 1.00000
     1   hdd 0.01949         osd.1      up  1.00000 1.00000
     2   hdd 0.01949         osd.2      up  1.00000 1.00000
    -5       0.05846     host ceph4
     3   hdd 0.01949         osd.3      up  1.00000 1.00000
     4   hdd 0.01949         osd.4      up  1.00000 1.00000
     5   hdd 0.01949         osd.5      up  1.00000 1.00000
    -7       0.05846     host ceph6
     6   hdd 0.01949         osd.6      up  1.00000 1.00000
     7   hdd 0.01949         osd.7      up  1.00000 1.00000
     8   hdd 0.01949         osd.8      up  1.00000 1.00000
    [cephadm@ceph2 ceph_cluster]$ ceph osd pool ls
    2023-07-16 23:21:40.750 7feac6dcd700 -1 auth: unable to find a keyring on /etc/ceph/ceph.client.admin.keyring,/etc/ceph/ceph.keyring,/etc/ceph/keyring,/etc/ceph/keyring.bin,: (2) No such file or directory
    2023-07-16 23:21:40.750 7feac6dcd700 -1 monclient: ERROR: missing keyring, cannot use cephx for authentication
    [errno 2] error connecting to the cluster
    [cephadm@ceph2 ceph_cluster]$ sudo ceph osd pool ls
    rbd
    [cephadm@ceph2 ceph_cluster]$
