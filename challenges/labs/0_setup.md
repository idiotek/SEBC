* List the cloud provider you are using (AWS, GCE, Azure, other)
<code>AWS</code>

* List the nodes you are using by IP address and name
```
Name | IP
---- | --
ip-172-31-28-115 | 172.31.28.115
ip-172-31-19-216 | 172.31.19.216
ip-172-31-22-166 | 172.31.22.166
ip-172-31-26-40 | 172.31.26.40
ip-172-31-23-151 | 172.31.23.151
```

* List the Linux release you are using
```
cat /etc/redhat-release 
CentOS release 6.8 (Final)
```

* Demonstrate the disk capacity available on each node is >= 30 GB
```
df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvde        20G  678M   19G   4% /
tmpfs           7.4G     0  7.4G   0% /dev/shm
/dev/xvdf1      9.9G  198M  9.2G   3% /var
/dev/xvdf2       20G  172M   19G   1% /opt
```

* List the command and output for yum repolist enabled
```
yum repolist enabled
Loaded plugins: fastestmirror, presto
Loading mirror speeds from cached hostfile
 * base: mirror.centos.org
 * extras: mirror.centos.org
 * updates: mirror.centos.org
repo id                                                                                          repo name                                                                                                   status
base                                                                                             CentOS-6 - Base                                                                                             6,706
extras                                                                                           CentOS-6 - Extras                                                                                              64
updates                                                                                          CentOS-6 - Updates                                                                                            252
repolist: 7,022
```

* Add users and groups
```
groupadd -g 2300 aussies
groupadd -g 2900 kiwis
useradd -u 2300 -g 2300 cate
useradd -u 2900 -g 2900 jemaine
passwd cate
passwd jemaine
```

* List the /etc/passwd and /etc/group
```
cat /etc/passwd | egrep -E "cate|jemaine"; cat /etc/group | egrep -E "aussies|kiwis"
cate:x:2300:2300::/home/cate:/bin/bash
jemaine:x:2900:2900::/home/jemaine:/bin/bash
aussies:x:2300:
kiwis:x:2900:
```
