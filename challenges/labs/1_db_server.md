<code><b> MySQL Local Install </b></code><br>
<code><b>[root@sserverjq raken]# yum localinstall mysql-community-common-5.7.20-1.el7.x86_64.rpm mysql-community-libs-* mysql-community-client-5.7.20-1.el7.x86_64.rpm mysql-community-server-5.7.20-1.el7.x86_64.rpm</b></code><br>

<code><b> Show the database hostname </b></code><br>
<b>[root@sserverjq raken]# hostname</b><br>
sserverjq<br>
<br>

<code><b> Show the database version </b></code><br>
<b>[root@sserverjq raken]# mysql --version</b><br>
mysql  Ver 14.14 Distrib 5.7.20, for Linux (x86_64) using  EditLine wrapper<br>

<code><b> Show the databases </b></code><br>
<b>mysql> show databases;</b><br>
+--------------------+<br>
| Database           |<br>
+--------------------+<br>
| information_schema |<br>
| hive               |<br>
| hue                |<br>
| mysql              |<br>
| oozie              |<br>
| performance_schema |<br>
| rman               |<br>
| scm                |<br>
| sys                |<br>
+--------------------+<br>
9 rows in set (0.00 sec)<br>
<br>
mysql> <br>
<br>






