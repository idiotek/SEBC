* Check vm.swapiness
<code>cat /proc/sys/vm/swappiness</code>
```
# cat /proc/sys/vm/swappiness 
1
```
* Show the mount attributes of your volume(s)
<code>cat /proc/mounts | grep "ext4"</code>
```
# cat /proc/mounts | grep "ext4"
/dev/xvde / ext4 rw,seclabel,relatime,barrier=1,data=ordered 0 0
```
* List the reserve space setting for ext-based volumes
<code>tune2fs -l /dev/xvde | grep "Reserved block count"</code>
```
# tune2fs -l /dev/xvde | grep "Reserved block count"
Reserved block count:     524185
```
* Disable transparent hugepage support
<code>grep -i HugePages_Total /proc/meminfo</code>
```
[mfernest: Not quite I had in mind. This shows the facility is not in use. You want to show the setting that proves it's disabled]

# grep -i HugePages_Total /proc/meminfo
HugePages_Total:       0
```
* List your network interface configuration
<code>ifconfig</code>
```
# ifconfig
eth0      Link encap:Ethernet  HWaddr 02:C8:75:4D:9F:6F  
          inet addr:172.31.10.189  Bcast:172.31.15.255  Mask:255.255.240.0
          inet6 addr: fe80::c8:75ff:fe4d:9f6f/64 Scope:Link
          UP BROADCAST RUNNING MULTICAST  MTU:9001  Metric:1
          RX packets:109411 errors:0 dropped:0 overruns:0 frame:0
          TX packets:17540 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:1000 
          RX bytes:154481409 (147.3 MiB)  TX bytes:1631295 (1.5 MiB)
          Interrupt:24 

lo        Link encap:Local Loopback  
          inet addr:127.0.0.1  Mask:255.0.0.0
          inet6 addr: ::1/128 Scope:Host
          UP LOOPBACK RUNNING  MTU:16436  Metric:1
          RX packets:8 errors:0 dropped:0 overruns:0 frame:0
          TX packets:8 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:0 
          RX bytes:672 (672.0 b)  TX bytes:672 (672.0 b)
```
* Show correct forward and reverse host lookups
<code>getent hosts</code>
```
# getent hosts
127.0.0.1       localhost.localdomain localhost
127.0.0.1       localhost6.localdomain6 localhost6
172.31.10.189   ip-172-31-10-189 sebc01
172.31.2.85     ip-172-31-2-85 sebc02
172.31.8.175    ip-172-31-8-175 sebc03
172.31.4.126    ip-172-31-4-126 sebc04
172.31.10.43    ip-172-31-10-43 sebc05
```
* Show the nscd service is running
<code>service nscd status</code>
```
# service nscd status
nscd (pid 4602) is running...
```
* Show the ntpd service is running
<code>service ntpd status</code>
```
# service ntpd status
ntpd (pid  4625) is running...
```
