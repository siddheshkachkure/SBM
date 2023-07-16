    ┌──────────────────────────────────────────────────────────────────────┐
    │                 • MobaXterm Personal Edition v23.1 •                 │
    │               (SSH client, X server and network tools)               │
    │                                                                      │
    │ ⮞ SSH session to root@192.168.239.156                                │
    │   • Direct SSH      :  ✓                                             │
    │   • SSH compression :  ✓                                             │
    │   • SSH-browser     :  ✓                                             │
    │   • X11-forwarding  :  ✗  (disabled or not supported by server)      │
    │                                                                      │
    │ ⮞ For more info, ctrl+click on help or visit our website.            │
    └──────────────────────────────────────────────────────────────────────┘

    Last login: Sun Jul 16 21:13:07 2023
    [root@ceph3 ~]# vim /etc/chrony.conf
    [root@ceph3 ~]# systemctl restart chronyd
    [root@ceph3 ~]# cat /etc/chrony.conf
    # Use public servers from the pool.ntp.org project.
    # Please consider joining the pool (http://www.pool.ntp.org/join.html).
    #server 0.centos.pool.ntp.org iburst
    #server 1.centos.pool.ntp.org iburst
    #server 2.centos.pool.ntp.org iburst
    #server 3.centos.pool.ntp.org iburst
    server ceph2.in
    # Record the rate at which the system clock gains/losses time.
    driftfile /var/lib/chrony/drift
    
    # Allow the system clock to be stepped in the first three updates
    # if its offset is larger than 1 second.
    makestep 1.0 3
    
    # Enable kernel synchronization of the real-time clock (RTC).
    rtcsync
    
    # Enable hardware timestamping on all interfaces that support it.
    #hwtimestamp *
    
    # Increase the minimum number of selectable sources required to adjust
    # the system clock.
    #minsources 2
    
    # Allow NTP client access from local network.
    #allow 192.168.0.0/16
    
    # Serve time even if not synchronized to a time source.
    #local stratum 10
    
    # Specify file containing keys for NTP authentication.
    #keyfile /etc/chrony.keys
    
    # Specify directory for log files.
    logdir /var/log/chrony

    # Select which information is logged.
    #log measurements statistics tracking
    [root@ceph3 ~]# vim /etc/hosts
    [root@ceph3 ~]# systemctl restart chronyd
    [root@ceph3 ~]#