<code><b> Local RPMs </b></code><br>

<code><b>[root@host1 CDH5]# ls /etc/yum.repos.d</b></code><br>
public-yum-ol7.repo<br>


<code><b>[root@host1 CDH5]# yum localinstall cloudera-manager-* -y</b></code><br>
<code><b>[root@host1 CDH5]# yum localinstall oracle-j2sdk1.7-1.7.0+update67-1.x86_64.rpm </b></code><br>


[root@host1 CDH5]# cat /etc/cloudera-scm-server/db.properties <br>
 Copyright (c) 2012 Cloudera, Inc. All rights reserved.<br>

This file describes the database connection.<br>


The database type <br>
Currently 'mysql', 'postgresql' and 'oracle' are valid databases.<br>
com.cloudera.cmf.db.type=mysql<br>

The database host<br>
If a non standard port is needed, use 'hostname:port'<br>
com.cloudera.cmf.db.host=sserverjq.northcentralus.cloudapp.azure.com<br>

The database name<br>
com.cloudera.cmf.db.name=scm<br>
<br>
The database user<br>
com.cloudera.cmf.db.user=scm<br>

The database user's password<br>
com.cloudera.cmf.db.password=Raken.2017<br>

The db setup type<br>
By default, it is set to INIT<br>
If scm-server uses Embedded DB then it is set to EMBEDDED<br>
If scm-server uses External DB then it is set to EXTERNAL<br>
com.cloudera.cmf.db.setupType=EXTERNAL<br>
