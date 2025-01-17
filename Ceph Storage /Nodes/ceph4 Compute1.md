        ┌──────────────────────────────────────────────────────────────────────┐
        │                 • MobaXterm Personal Edition v23.1 •                 │
        │               (SSH client, X server and network tools)               │
        │                                                                      │
        │ ⮞ SSH session to root@192.168.239.157                               |
        │   • Direct SSH      :  ✓                                             │
        │   • SSH compression :  ✓                                             │
        │   • SSH-browser     :  ✓                                            |
        │   • X11-forwarding  :  ✗  (disabled or not supported by server)      │
        │                                                                      │
        │ ⮞ For more info, ctrl+click on help or visit our website.            │
        └──────────────────────────────────────────────────────────────────────┘
    
    Last login: Sun Jul 16 21:13:48 2023
    [root@ceph4 ~]# vim /etc/chrony.conf
    [root@ceph4 ~]# systemctl restart chronyd
    [root@ceph4 ~]# vim /etc/hosts
    [root@ceph4 ~]# systemctl restart chronyd
    [root@ceph4 ~]#
