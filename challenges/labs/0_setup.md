<b> List the cloud provider you are using (AWS, GCE, Azure, CloudCat, other) </b> <br>
<code><b>Azure</b></code><br>

<b>List your instances by IP address and DNS name (don't use /etc/hosts for this)</b><br>
PING sserverjq.northcentralus.cloudapp.azure.com (10.0.0.5)<br>
PING host1.northcentralus.cloudapp.azure.com (10.0.0.9) <br>
PING hosts2.northcentralus.cloudapp.azure.com (10.0.0.10)<br>
PING hosts3.northcentralus.cloudapp.azure.com (10.0.0.11)<br>
PING host4.northcentralus.cloudapp.azure.com (10.0.0.12)<br>

<b>List the Linux release you are using</b><br>
<code><b>O[raken@host1 ~]$ cat /etc/*release</b></code><br>
Oracle Linux Server release 7.3<br>
NAME="Oracle Linux Server"<br>
VERSION="7.3"<br>
ID="ol"<br>
VERSION_ID="7.3"<br>
PRETTY_NAME="Oracle Linux Server 7.3"<br>
ANSI_COLOR="0;31"<br>
CPE_NAME="cpe:/o:oracle:linux:7:3:server"<br>
HOME_URL="https://linux.oracle.com/"<br>
BUG_REPORT_URL="https://bugzilla.oracle.com/"<br>

ORACLE_BUGZILLA_PRODUCT="Oracle Linux 7"<br>
ORACLE_BUGZILLA_PRODUCT_VERSION=7.3<br>
ORACLE_SUPPORT_PRODUCT="Oracle Linux"<br>
ORACLE_SUPPORT_PRODUCT_VERSION=7.3<br>
Red Hat Enterprise Linux Server release 7.3 (Maipo)<br>
Oracle Linux Server release 7.3<br>

<b>List the file system capacity for the first node</b><br>
<code><b>[raken@host1 ~]$ df -h</b></code><br>
Filesystem      Size  Used Avail Use% Mounted on<br>
devtmpfs         16G     0   16G   0% /dev<br>
tmpfs            16G     0   16G   0% /dev/shm<br>
tmpfs            16G  8.3M   16G   1% /run<br>
tmpfs            16G     0   16G   0% /sys/fs/cgroup<br>
/dev/sda2        30G  1.8G   26G   7% /<br>
/dev/sda1       497M  112M  386M  23% /boot<br>
/dev/sdb1       197G  2.1G  185G   2% /mnt/resource<br>
tmpfs           3.2G     0  3.2G   0% /run/user/1000<br>

<b>List the command and output for yum repolist enabled </b><br>
<code><b>[raken@host1 ~]$ sudo yum list enabled</b></code><br>
Failed to set locale, defaulting to C<br>
Loaded plugins: ulninfo<br>
ol7_UEKR4                                                | 1.2 kB     00:00     <br>
ol7_addons                                               | 1.2 kB     00:00     <br>
ol7_latest                                               | 1.4 kB     00:00     <br>
(1/7): ol7_addons/x86_64/updateinfo                        |  39 kB   00:00     <br>
(2/7): ol7_addons/x86_64/primary                           |  78 kB   00:00     <br>
(3/7): ol7_UEKR4/x86_64/updateinfo                         | 133 kB   00:00     <br>
(4/7): ol7_latest/x86_64/group                             | 681 kB   00:00     <br>
(5/7): ol7_latest/x86_64/updateinfo                        | 1.6 MB   00:00     <br>
(6/7): ol7_UEKR4/x86_64/primary                            |  25 MB   00:02     <br>
(7/7): ol7_latest/x86_64/primary                           |  31 MB   00:03     <br>
ol7_UEKR4                                                               499/499<br>
ol7_addons                                                              249/249<br>
ol7_latest                                                          23409/23409<br>
Error: No matching Packages to list<br>
[raken@host1 ~]$ <br>

<b>Add the following Linux accounts to all nodes</b><br>
<b>User saturn with a UID of 2800</b><br>
[root@hosts2 raken]# useradd -u 2800 saturn<br>

<b>User haley with a UID of 2900</b><br>
[root@hosts2 raken]# useradd -u 2900 haley<br>

<b>Create the group comets and add haley to it</b><br>
[root@hosts2 raken]# groupadd comets<br>
[root@hosts2 raken]# usermod -g comets haley<br>

<b>Create the group planets and add saturn to it</b><br>
[root@hosts2 raken]# groupadd planets<br>
[root@hosts2 raken]# usermod -g planets saturn<br>


<b>List the /etc/passwd entries for saturn and haley</b>
<b>Do not list the entire file</b><<br>
[root@host1 raken]# cat /etc/passwd |grep 'haley' <br>
haley:x:2900:2901::/home/haley:/bin/bash<br>
[root@host1 raken]# cat /etc/passwd |grep 'saturn' <br>
saturn:x:2800:2902::/home/saturn:/bin/bash<br>

<b>List the /etc/group entries for comets and planets</b><br>
<b>Do not list the entire file</b><br>
[root@host1 raken]# cat /etc/group |grep 'comets'<br>
comets:x:2901:<br>
[root@host1 raken]# cat /etc/group |grep 'planets'<br>
planets:x:2902:<br>

<b> INSTALL MYSQL </b>
<code><b>[root@sserverjq raken]# yum localinstall mysql-community-common-5.7.20-1.el7.x86_64.rpm mysql-community-libs-* mysql-community-client-5.7.20-1.el7.x86_64.rpm mysql-community-server-5.7.20-1.el7.x86_64.rpm</b></code><br>



