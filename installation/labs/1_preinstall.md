
~~~~
1.Check vm.swappiness on all your nodes

[root@cdh01 ansible]# cat  /etc/sysctl.conf |grep  swap
vm.swappiness = 1

~~~~
~~~~
2.Show the mount attributes of all volumes
[root@cdh01 ansible]# cat  /etc/fstab

#
# /etc/fstab
# Created by anaconda on Mon Feb 22 17:08:22 2016
#
# Accessible filesystems, by reference, are maintained under '/dev/disk'
# See man pages fstab(5), findfs(8), mount(8) and/or blkid(8) for more info
#
UUID=ef6ba050-6cdc-416a-9380-c14304d0d206 /                       xfs     defaults        0 0
~~~~~~~~
~~~~~~~
3.Show the reserve space of any non-root, ext-based volumes

N/A : because / is XFS.
[root@cdh01 ansible]# tune2fs  -l  /dev/xvda1
tune2fs 1.42.9 (28-Dec-2013)
tune2fs: Bad magic number in super-block while trying to open /dev/xvda1
Couldn't find valid filesystem superblock.
~~~~~

~~~~~~
4.Show that transparent hugepages is disabled
[root@cdh01 ansible]# cat /sys/kernel/mm/transparent_hugepage/defrag
always madvise [never]

~~~~~~~~
~~~~~
5.Report the network interface attributes
[root@cdh01 ansible]# ip  a
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host
       valid_lft forever preferred_lft forever
2: eth0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 9001 qdisc pfifo_fast state UP qlen 1000
    link/ether 02:3d:45:fe:98:fb brd ff:ff:ff:ff:ff:ff
    inet 172.31.3.200/20 brd 172.31.15.255 scope global dynamic eth0
       valid_lft 3335sec preferred_lft 3335sec
    inet6 fe80::3d:45ff:fefe:98fb/64 scope link
       valid_lft forever preferred_lft forever

~~~~~~
~~~~~
6.Show forward and reverse host lookups using getent and nslookup

[root@cdh01 ansible]# ping  cdh03
PING cdh03 (172.31.3.45) 56(84) bytes of data.
64 bytes from cdh03 (172.31.3.45): icmp_seq=1 ttl=64 time=0.252 ms
64 bytes from cdh03 (172.31.3.45): icmp_seq=2 ttl=64 time=0.289 ms
^X64 bytes from cdh03 (172.31.3.45): icmp_seq=3 ttl=64 time=0.278 ms

[root@cdh01 ansible]# getent  hosts 172.31.3.45
172.31.3.45     cdh03 ip-172-31-3-45.ap-southeast-1.compute.internal


[root@cdh01 ansible]# nslookup  172.31.3.45
Server:		172.31.0.2
Address:	172.31.0.2#53

Non-authoritative answer:
45.3.31.172.in-addr.arpa	name = ip-172-31-3-45.ap-southeast-1.compute.internal.

Authoritative answers can be found from:
~~~~~
~~~~~~
7.Verify the nscd service is running
[root@cdh01 ansible]# service nscd status
Redirecting to /bin/systemctl status  nscd.service
● nscd.service - Name Service Cache Daemon
   Loaded: loaded (/usr/lib/systemd/system/nscd.service; enabled; vendor preset: disabled)
   Active: active (running) since Mon 2016-12-05 08:24:12 UTC; 14min ago
 Main PID: 19051 (nscd)
   CGroup: /system.slice/nscd.service
           └─19051 /usr/sbin/nscd
~~~~~
~~~~~
8.Verify the ntpd service is running
[root@cdh01 ansible]# service ntpd status
Redirecting to /bin/systemctl status  ntpd.service
● ntpd.service - Network Time Service
   Loaded: loaded (/usr/lib/systemd/system/ntpd.service; enabled; vendor preset: disabled)
   Active: active (running) since Mon 2016-12-05 08:24:58 UTC; 12min ago
 Main PID: 19258 (ntpd)
   CGroup: /system.slice/ntpd.service
           └─19258 /usr/sbin/ntpd -u ntp:ntp -g
~~~~~~~
~~~
