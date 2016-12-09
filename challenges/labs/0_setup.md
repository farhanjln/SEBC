 instance-1	us-central1-c	CentOS 7
 instance-2	us-central1-c	CentOS 7
 instance-3	us-central1-c	CentOS 7
 instance-4	us-central1-c	CentOS 7
 instance-5	us-central1-c	CentOS 7


///DISK VOLUME EACH NODE/// 
 [root@instance-1 hinotamashi94]# df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/sda1        30G  1.3G   29G   5% /
devtmpfs        7.9G     0  7.9G   0% /dev
tmpfs           7.9G     0  7.9G   0% /dev/shm
tmpfs           7.9G  8.2M  7.9G   1% /run
tmpfs           7.9G     0  7.9G   0% /sys/fs/cgroup
tmpfs           1.6G     0  1.6G   0% /run/user/1000
[root@instance-1 hinotamashi94]# sfdisk -l -uM
Disk /dev/sda: 3916 cylinders, 255 heads, 63 sectors/track
Units: 1MiB = 1024*1024 bytes, blocks of 1024 bytes, counting from 0
   Device Boot Start   End    MiB    #blocks   Id  System
/dev/sda1   *     1  30718- 30718-  31454246   83  Linux
/dev/sda2         0      -      0          0    0  Empty
/dev/sda3         0      -      0          0    0  Empty
/dev/sda4         0      -      0          0    0  Empty
[root@instance-1 hinotamashi94]# 

[hinotamashi94@instance-2 ~]$ sudo su
[root@instance-2 hinotamashi94]# df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/sda1        30G  1.3G   29G   5% /
devtmpfs        7.9G     0  7.9G   0% /dev
tmpfs           7.9G     0  7.9G   0% /dev/shm
tmpfs           7.9G  8.2M  7.9G   1% /run
tmpfs           7.9G     0  7.9G   0% /sys/fs/cgroup
tmpfs           1.6G     0  1.6G   0% /run/user/1000
[root@instance-2 hinotamashi94]# sfdisk -l -uM
Disk /dev/sda: 3916 cylinders, 255 heads, 63 sectors/track
Units: 1MiB = 1024*1024 bytes, blocks of 1024 bytes, counting from 0
   Device Boot Start   End    MiB    #blocks   Id  System
/dev/sda1   *     1  30718- 30718-  31454246   83  Linux
/dev/sda2         0      -      0          0    0  Empty
/dev/sda3         0      -      0          0    0  Empty
/dev/sda4         0      -      0          0    0  Empty
[root@instance-2 hinotamashi94]# 


[hinotamashi94@instance-3 ~]$ sudo su
[root@instance-3 hinotamashi94]# df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/sda1        30G  1.3G   29G   5% /
devtmpfs        7.9G     0  7.9G   0% /dev
tmpfs           7.9G     0  7.9G   0% /dev/shm
tmpfs           7.9G  8.2M  7.9G   1% /run
tmpfs           7.9G     0  7.9G   0% /sys/fs/cgroup
tmpfs           1.6G     0  1.6G   0% /run/user/1000
[root@instance-3 hinotamashi94]# sfdisk -l -UM
Disk /dev/sda: 3916 cylinders, 255 heads, 63 sectors/track
Units: cylinders of 8225280 bytes, blocks of 1024 bytes, counting from 0
   Device Boot Start     End   #cyls    #blocks   Id  System
/dev/sda1   *      0+   3915    3916-  31454246   83  Linux
/dev/sda2          0       -       0          0    0  Empty
/dev/sda3          0       -       0          0    0  Empty
/dev/sda4          0       -       0          0    0  Empty
[root@instance-3 hinotamashi94]# 


[hinotamashi94@instance-4 ~]$ sudo su
[root@instance-4 hinotamashi94]# df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/sda1        30G  1.3G   29G   5% /
devtmpfs        7.9G     0  7.9G   0% /dev
tmpfs           7.9G     0  7.9G   0% /dev/shm
tmpfs           7.9G  8.2M  7.9G   1% /run
tmpfs           7.9G     0  7.9G   0% /sys/fs/cgroup
tmpfs           1.6G     0  1.6G   0% /run/user/1000
[root@instance-4 hinotamashi94]# sfdisk -l -uM
Disk /dev/sda: 3916 cylinders, 255 heads, 63 sectors/track
Units: 1MiB = 1024*1024 bytes, blocks of 1024 bytes, counting from 0
   Device Boot Start   End    MiB    #blocks   Id  System
/dev/sda1   *     1  30718- 30718-  31454246   83  Linux
/dev/sda2         0      -      0          0    0  Empty
/dev/sda3         0      -      0          0    0  Empty
/dev/sda4         0      -      0          0    0  Empty
[root@instance-4 hinotamashi94]# 

[hinotamashi94@instance-5 ~]$ sudo su
[root@instance-5 hinotamashi94]# df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/sda1        30G  1.3G   29G   5% /
devtmpfs        7.9G     0  7.9G   0% /dev
tmpfs           7.9G     0  7.9G   0% /dev/shm
tmpfs           7.9G  8.2M  7.9G   1% /run
tmpfs           7.9G     0  7.9G   0% /sys/fs/cgroup
tmpfs           1.6G     0  1.6G   0% /run/user/1000
[root@instance-5 hinotamashi94]# sfdisk -l -uM
Disk /dev/sda: 3916 cylinders, 255 heads, 63 sectors/track
Units: 1MiB = 1024*1024 bytes, blocks of 1024 bytes, counting from 0
   Device Boot Start   End    MiB    #blocks   Id  System
/dev/sda1   *     1  30718- 30718-  31454246   83  Linux
/dev/sda2         0      -      0          0    0  Empty
/dev/sda3         0      -      0          0    0  Empty
/dev/sda4         0      -      0          0    0  Empty
[root@instance-5 hinotamashi94]# 

/// yum repolist///
[root@instance-1 hinotamashi94]# yum repolist enabled
Loaded plugins: fastestmirror
base                                                                                                                                               | 3.6 kB  00:00:00     
extras                                                                                                                                             | 3.4 kB  00:00:00     
google-cloud-compute/signature                                                                                                                     |  454 B  00:00:00     
google-cloud-compute/signature                                                                                                                     | 1.4 kB  00:00:00 !!! 
google-cloud-sdk/signature                                                                                                                         |  454 B  00:00:00     
google-cloud-sdk/signature                                                                                                                         | 1.4 kB  00:00:00 !!! 
updates                                                                                                                                            | 3.4 kB  00:00:00     
(1/6): google-cloud-compute/primary                                                                                                                | 1.9 kB  00:00:00     
(2/6): extras/7/x86_64/primary_db                                                                                                                  | 166 kB  00:00:00     
(3/6): google-cloud-sdk/primary                                                                                                                    | 2.8 kB  00:00:00     
(4/6): base/7/x86_64/group_gz                                                                                                                      | 155 kB  00:00:00     
(5/6): base/7/x86_64/primary_db                                                                                                                    | 5.3 MB  00:00:01     
(6/6): updates/7/x86_64/primary_db                                                                                                                 | 9.1 MB  00:00:00     
Determining fastest mirrors
 * base: mirrors.gigenet.com
 * extras: mirror.tzulo.com
 * updates: mirrors.gigenet.com
google-cloud-compute                                                                                                                                                  4/4
google-cloud-sdk                                                                                                                                                      7/7
repo id                                                                           repo name                                                                         status
base/7/x86_64                                                                     CentOS-7 - Base                                                                   9,007
extras/7/x86_64                                                                   CentOS-7 - Extras                                                                   393
google-cloud-compute                                                              Google Cloud Compute                                                                  4
google-cloud-sdk                                                                  Google Cloud SDK                                                                      7
updates/7/x86_64                                                                  CentOS-7 - Updates                                                                2,560
repolist: 11,971
[root@instance-1 hinotamashi94]# 



[root@instance-2 hinotamashi94]# yum repolist enabled
Loaded plugins: fastestmirror
base                                                                                     | 3.6 kB  00:00:00     
extras                                                                                   | 3.4 kB  00:00:00     
google-cloud-compute/signature                                                           |  454 B  00:00:00     
google-cloud-compute/signature                                                           | 1.4 kB  00:00:00 !!! 
google-cloud-sdk/signature                                                               |  454 B  00:00:00     
google-cloud-sdk/signature                                                               | 1.4 kB  00:00:00 !!! 
updates                                                                                  | 3.4 kB  00:00:00     
(1/6): google-cloud-compute/primary                                                      | 1.9 kB  00:00:00     
(2/6): extras/7/x86_64/primary_db                                                        | 166 kB  00:00:00     
(3/6): google-cloud-sdk/primary                                                          | 2.8 kB  00:00:00     
(4/6): base/7/x86_64/group_gz                                                            | 155 kB  00:00:00     
(5/6): updates/7/x86_64/primary_db                                                       | 9.1 MB  00:00:00     
(6/6): base/7/x86_64/primary_db                                                          | 5.3 MB  00:00:00     
Determining fastest mirrors
 * base: centos.mirrors.tds.net
 * extras: mirror.tzulo.com
 * updates: mirror.eboundhost.com
google-cloud-compute                                                                                        4/4
google-cloud-sdk                                                                                            7/7
repo id                                              repo name                                            status
base/7/x86_64                                        CentOS-7 - Base                                      9,007
extras/7/x86_64                                      CentOS-7 - Extras                                      393
google-cloud-compute                                 Google Cloud Compute                                     4
google-cloud-sdk                                     Google Cloud SDK                                         7
updates/7/x86_64                                     CentOS-7 - Updates                                   2,560
repolist: 11,971
[root@instance-2 hinotamashi94]#



[root@instance-3 hinotamashi94]# yum repolist enabled
Loaded plugins: fastestmirror
base                                                                                     | 3.6 kB  00:00:00     
extras                                                                                   | 3.4 kB  00:00:00     
google-cloud-compute/signature                                                           |  454 B  00:00:00     
google-cloud-compute/signature                                                           | 1.4 kB  00:00:00 !!! 
google-cloud-sdk/signature                                                               |  454 B  00:00:00     
google-cloud-sdk/signature                                                               | 1.4 kB  00:00:00 !!! 
updates                                                                                  | 3.4 kB  00:00:00     
(1/6): google-cloud-compute/primary                                                      | 1.9 kB  00:00:00     
(2/6): extras/7/x86_64/primary_db                                                        | 166 kB  00:00:00     
(3/6): google-cloud-sdk/primary                                                          | 2.8 kB  00:00:00     
(4/6): base/7/x86_64/group_gz                                                            | 155 kB  00:00:00     
(5/6): updates/7/x86_64/primary_db                                                       | 9.1 MB  00:00:00     
(6/6): base/7/x86_64/primary_db                                                          | 5.3 MB  00:00:00     
Determining fastest mirrors
 * base: mirrors.gigenet.com
 * extras: mirror.tzulo.com
 * updates: mirrors.gigenet.com
google-cloud-compute                                                                                        4/4
google-cloud-sdk                                                                                            7/7
repo id                                              repo name                                            status
base/7/x86_64                                        CentOS-7 - Base                                      9,007
extras/7/x86_64                                      CentOS-7 - Extras                                      393
google-cloud-compute                                 Google Cloud Compute                                     4
google-cloud-sdk                                     Google Cloud SDK                                         7
updates/7/x86_64                                     CentOS-7 - Updates                                   2,560
repolist: 11,971
[root@instance-3 hinotamashi94]# 



[root@instance-4 hinotamashi94]# yum repolist enabled
Loaded plugins: fastestmirror
base                                                                                     | 3.6 kB  00:00:00     
extras                                                                                   | 3.4 kB  00:00:00     
google-cloud-compute/signature                                                           |  454 B  00:00:00     
google-cloud-compute/signature                                                           | 1.4 kB  00:00:00 !!! 
google-cloud-sdk/signature                                                               |  454 B  00:00:00     
google-cloud-sdk/signature                                                               | 1.4 kB  00:00:00 !!! 
updates                                                                                  | 3.4 kB  00:00:00     
(1/6): google-cloud-compute/primary                                                      | 1.9 kB  00:00:00     
(2/6): extras/7/x86_64/primary_db                                                        | 166 kB  00:00:00     
(3/6): google-cloud-sdk/primary                                                          | 2.8 kB  00:00:00     
(4/6): base/7/x86_64/group_gz                                                            | 155 kB  00:00:00     
(5/6): updates/7/x86_64/primary_db                                                       | 9.1 MB  00:00:00     
(6/6): base/7/x86_64/primary_db                                                          | 5.3 MB  00:00:00     
Determining fastest mirrors
 * base: mirrors.gigenet.com
 * extras: mirror.tzulo.com
 * updates: mirrors.gigenet.com
google-cloud-compute                                                                                        4/4
google-cloud-sdk                                                                                            7/7
repo id                                              repo name                                            status
base/7/x86_64                                        CentOS-7 - Base                                      9,007
extras/7/x86_64                                      CentOS-7 - Extras                                      393
google-cloud-compute                                 Google Cloud Compute                                     4
google-cloud-sdk                                     Google Cloud SDK                                         7
updates/7/x86_64                                     CentOS-7 - Updates                                   2,560
repolist: 11,971
[root@instance-4 hinotamashi94]# 



[root@instance-5 hinotamashi94]# yum repolist enabled
Loaded plugins: fastestmirror
base                                                                                     | 3.6 kB  00:00:00     
extras                                                                                   | 3.4 kB  00:00:00     
google-cloud-compute/signature                                                           |  454 B  00:00:00     
google-cloud-compute/signature                                                           | 1.4 kB  00:00:00 !!! 
google-cloud-sdk/signature                                                               |  454 B  00:00:00     
google-cloud-sdk/signature                                                               | 1.4 kB  00:00:00 !!! 
updates                                                                                  | 3.4 kB  00:00:00     
(1/6): google-cloud-compute/primary                                                      | 1.9 kB  00:00:00     
(2/6): extras/7/x86_64/primary_db                                                        | 166 kB  00:00:00     
(3/6): google-cloud-sdk/primary                                                          | 2.8 kB  00:00:00     
(4/6): base/7/x86_64/group_gz                                                            | 155 kB  00:00:00     
(5/6): updates/7/x86_64/primary_db                                                       | 9.1 MB  00:00:00     
(6/6): base/7/x86_64/primary_db                                                          | 5.3 MB  00:00:00     
Determining fastest mirrors
 * base: mirrors.gigenet.com
 * extras: mirrors.liquidweb.com
 * updates: mirror.eboundhost.com
google-cloud-compute                                                                                        4/4
google-cloud-sdk                                                                                            7/7
repo id                                              repo name                                            status
base/7/x86_64                                        CentOS-7 - Base                                      9,007
extras/7/x86_64                                      CentOS-7 - Extras                                      393
google-cloud-compute                                 Google Cloud Compute                                     4
google-cloud-sdk                                     Google Cloud SDK                                         7
updates/7/x86_64                                     CentOS-7 - Updates                                   2,560
repolist: 11,971
[root@instance-5 hinotamashi94]# 



///useradd orchard and raffles///
[root@instance-1 hinotamashi94]# useradd raffles -u 2700
[root@instance-1 hinotamashi94]# useradd orchard -u 2800

[root@instance-2 hinotamashi94]# useradd raffles -u 2700
[root@instance-2 hinotamashi94]# useradd orchard -u 2800

[root@instance-3 hinotamashi94]# useradd raffles -u 2700
[root@instance-3 hinotamashi94]# useradd orchard -u 2800

[root@instance-4 hinotamashi94]# useradd raffles -u 2700
[root@instance-4 hinotamashi94]# useradd orchard -u 2800

[root@instance-5 hinotamashi94]# useradd raffles -u 2700
[root@instance-5 hinotamashi94]# useradd orchard -u 2800


///etc/passwd ///
[root@instance-1 hinotamashi94]# cat /etc/passwd |grep orchard
orchard:x:2800:2800::/home/orchard:/bin/bash
[root@instance-1 hinotamashi94]# cat /etc/passwd |grep raffles
raffles:x:2700:2700::/home/raffles:/bin/bash
[root@instance-1 hinotamashi94]# 

[root@instance-2 hinotamashi94]# cat /etc/passwd |grep orchard
orchard:x:2800:2800::/home/orchard:/bin/bash
[root@instance-2 hinotamashi94]# cat /etc/passwd |grep raffles
raffles:x:2700:2700::/home/raffles:/bin/bash
[root@instance-2 hinotamashi94]# 

[root@instance-3 hinotamashi94]# cat /etc/passwd |grep orchard
orchard:x:2800:2800::/home/orchard:/bin/bash
[root@instance-3 hinotamashi94]# cat /etc/passwd |grep raffles
raffles:x:2700:2700::/home/raffles:/bin/bash
[root@instance-3 hinotamashi94]# 

[root@instance-4 hinotamashi94]# cat /etc/passwd |grep orchard
orchard:x:2800:2800::/home/orchard:/bin/bash
[root@instance-4 hinotamashi94]# cat /etc/passwd |grep raffles
raffles:x:2700:2700::/home/raffles:/bin/bash
[root@instance-4 hinotamashi94]# 

[root@instance-5 hinotamashi94]# cat /etc/passwd |grep orchard
orchard:x:2800:2800::/home/orchard:/bin/bash
[root@instance-5 hinotamashi94]# cat /etc/passwd |grep raffles
raffles:x:2700:2700::/home/raffles:/bin/bash
[root@instance-5 hinotamashi94]# 

[root@instance-1 hinotamashi94]# cat /etc/group |grep shops
shops:x:2801:orchard
[root@instance-1 hinotamashi94]# cat /etc/group |grep walks
walks:x:2802:raffles

[root@instance-2 hinotamashi94]# cat /etc/group| grep shops
shops:x:2801:orchard
[root@instance-2 hinotamashi94]# cat /etc/group| grep raffles
raffles:x:2700:
walks:x:2802:raffles
[root@instance-2 hinotamashi94]#

[root@instance-3 hinotamashi94]# cat /etc/group |grep shops
shops:x:2801:orchard
[root@instance-3 hinotamashi94]# cat /etc/group |grep walks
walks:x:2802:raffles
[root@instance-3 hinotamashi94]# 

[root@instance-4 hinotamashi94]# cat /etc/group |grep shops
shops:x:2801:orchard
[root@instance-4 hinotamashi94]# cat /etc/group |grep walks
walks:x:2802:raffles
[root@instance-4 hinotamashi94]# 

[root@instance-5 hinotamashi94]# cat /etc/group |grep shops
shops:x:2801:orchard
[root@instance-5 hinotamashi94]# cat /etc/group |grep walks
walks:x:2802:raffles
