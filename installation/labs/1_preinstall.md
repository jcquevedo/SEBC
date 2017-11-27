[raken@hdp1 ~]$ sudo systemctl stop chronyd
[sudo] password for raken: 
[raken@hdp1 ~]$ sudo systemctl disable chronyd
Removed symlink /etc/systemd/system/multi-user.target.wants/chronyd.service.



<code>[raken@hdp1 ~]$ sudo systemctl stop firewalld
Failed to stop firewalld.service: Unit firewalld.service not loaded.
[raken@hdp1 ~]$ sudo systemctl status firewalld
Unit firewalld.service could not be found.</code>



Check vm.swappiness on all your nodes
Set the value to 1 if necessary
	<code>echo "vm.swappiness = 1" >> /etc/sysctl.conf</code>

Show the mount attributes of your volume(s)
If you have ext-based volumes, list the reserve space setting
XFS volumes do not support reserve space
<code>[root@hdp4 raken]# cat /etc/fstab

#
# /etc/fstab
# Created by anaconda on Mon Mar 20 18:26:52 2017
#
# Accessible filesystems, by reference, are maintained under '/dev/disk'
# See man pages fstab(5), findfs(8), mount(8) and/or blkid(8) for more info
#
UUID=e2bd018e-fe97-4848-80fd-5ba60aafef7e /                       btrfs   subvol=root     0 0
UUID=ce15c4e7-9c1f-4f07-93a6-b0f5e30f2acd /boot                   xfs     defaults        0 0</code>


Disable transparent hugepage support
<code>echo never > /sys/kernel/mm/transparent_hugepage/defrag</code>

List your network interface configuration
<code>[root@hdp4 raken]# ifconfig
eth0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        inet 10.0.0.8  netmask 255.255.255.0  broadcast 10.0.0.255
        inet6 fe80::20d:3aff:fe61:aca8  prefixlen 64  scopeid 0x20<link>
        ether 00:0d:3a:61:ac:a8  txqueuelen 1000  (Ethernet)
        RX packets 114224  bytes 80266984 (76.5 MiB)
        RX errors 0  dropped 4  overruns 0  frame 0
        TX packets 97266  bytes 16984877 (16.1 MiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536
        inet 127.0.0.1  netmask 255.0.0.0
        inet6 ::1  prefixlen 128  scopeid 0x10<host>
        loop  txqueuelen 0  (Local Loopback)
        RX packets 0  bytes 0 (0.0 B)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 0  bytes 0 (0.0 B)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0</code>


Show that forward and reverse host lookups are correctly resolved
For /etc/hosts, use getent
For DNS, use nslookup
<code>[root@hdp4 raken]# nslookup hdp1
Server:		168.63.129.16
Address:	168.63.129.16#53

Non-authoritative answer:
Name:	hdp1.northcentralus.cloudapp.azure.com
Address: 52.237.157.87</code>


Show the nscd service is running
<code>[root@hdp4 raken]# service nscd start
Redirecting to /bin/systemctl start  nscd.service
[root@hdp4 raken]# chkconfig nscd on
Note: Forwarding request to 'systemctl enable nscd.service'.
Created symlink from /etc/systemd/system/multi-user.target.wants/nscd.service to /usr/lib/systemd/system/nscd.service.
Created symlink from /etc/systemd/system/sockets.target.wants/nscd.socket to /usr/lib/systemd/system/nscd.socket.
[root@hdp4 raken]# time nslookup www.google.com
Server:   168.63.129.16
Address:  168.63.129.16#53

Name: www.google.com
Address: 172.217.3.164


real  0m0.022s
user  0m0.002s
sys 0m0.006s</code>

Show the ntpd service is running
<code>[root@hdp4 raken]# sudo systemctl status ntpd.service
● ntpd.service - Network Time Service
   Loaded: loaded (/usr/lib/systemd/system/ntpd.service; enabled; vendor preset: disabled)
   Active: active (running) since Mon 2017-11-27 13:45:29 EST; 1h 26min ago
  Process: 12769 ExecStart=/usr/sbin/ntpd -u ntp:ntp $OPTIONS (code=exited, status=0/SUCCESS)
 Main PID: 12770 (ntpd)
   CGroup: /system.slice/ntpd.service
           └─12770 /usr/sbin/ntpd -u ntp:ntp -g

Nov 27 13:45:29 hdp4.northcentralus.cloudapp.azure.com ntpd[12770]: Listen normally on 4 lo ::1 U...3
Nov 27 13:45:29 hdp4.northcentralus.cloudapp.azure.com ntpd[12770]: Listen normally on 5 eth0 fe8...3
Nov 27 13:45:29 hdp4.northcentralus.cloudapp.azure.com ntpd[12770]: Listening on routing socket o...s
Nov 27 13:45:29 hdp4.northcentralus.cloudapp.azure.com systemd[1]: Started Network Time Service.
Nov 27 13:45:29 hdp4.northcentralus.cloudapp.azure.com ntpd[12770]: 0.0.0.0 c016 06 restart
Nov 27 13:45:29 hdp4.northcentralus.cloudapp.azure.com ntpd[12770]: 0.0.0.0 c012 02 freq_set kern...M
Nov 27 13:45:29 hdp4.northcentralus.cloudapp.azure.com ntpd[12770]: 0.0.0.0 c011 01 freq_not_set
Nov 27 13:45:36 hdp4.northcentralus.cloudapp.azure.com ntpd[12770]: 0.0.0.0 c614 04 freq_mode
Nov 27 14:01:26 hdp4.northcentralus.cloudapp.azure.com ntpd[12770]: 0.0.0.0 0612 02 freq_set kern...M
Nov 27 14:01:26 hdp4.northcentralus.cloudapp.azure.com ntpd[12770]: 0.0.0.0 0615 05 clock_sync
Hint: Some lines were ellipsized, use -l to show in full.</code>