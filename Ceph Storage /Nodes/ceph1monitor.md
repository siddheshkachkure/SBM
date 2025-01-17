    ┌──────────────────────────────────────────────────────────────────────┐
    │                 • MobaXterm Personal Edition v23.1 •                 │
    │               (SSH client, X server and network tools)               │
    │                                                                      │
    │ ⮞ SSH session to root@192.168.239.154                                │
    │   • Direct SSH      :  ✓                                             │
    │   • SSH compression :  ✓                                             │
    │   • SSH-browser     :  ✓                                             │
    │   • X11-forwarding  :  ✗  (disabled or not supported by server)      │
    │                                                                      │
    │ ⮞ For more info, ctrl+click on help or visit our website.            │
    └──────────────────────────────────────────────────────────────────────┘

    Last login: Sun Jul 16 21:12:39 2023
    [root@ceph1 ~]# vim /etc/chrony.conf
    [root@ceph1 ~]# systemctl restart chronyd
    [root@ceph1 ~]# ceph-deploy install ceph-controller ceph-compute01 ceph-compute02 ceph-monitor
    -bash: ceph-deploy: command not found
    [root@ceph1 ~]# ceph-deploy mon create-initial
    -bash: ceph-deploy: command not found
    [root@ceph1 ~]# vim /etc/hosts
    [root@ceph1 ~]# cat /etc/hosts
    127.0.0.1   localhost localhost.localdomain localhost4 localhost4.localdomain4
    ::1         localhost localhost.localdomain localhost6 localhost6.localdomain6
    192.168.239.154 ceph1.in
    192.168.239.155 ceph2.in
    192.168.239.156 ceph3.in
    192.168.239.157 ceph4.in
    192.168.239.158 ceph5.in
    192.168.239.159 ceph6.in
    [root@ceph1 ~]# systemctl restart chronyd
