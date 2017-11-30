<code><b>Report the latest available version of the API</b></code><br>
[root@hdp1 instaladores]# curl -u jcquevedo:cloudera  'http://localhost:7180/api/version'
v18


<code><b> Report the CM version </b></code><br>
<b>[root@hdp1 instaladores]# curl -u jcquevedo:cloudera \ </b><br>
  'http://localhost:7180/api/v18/cm/version'<br>
{<br>
  "version" : "5.13.0",<br>
  "buildUser" : "jenkins",<br>
  "buildTimestamp" : "20171002-1719",<br>
  "gitHash" : "bd657e597e6743c458ee2c9aabe808b7c972981c",<br>
  "snapshot" : false<br>
}[root@hdp1 instaladores]# <br>

<code><b> List all CM users </b></code><br>
<b>[root@hdp1 instaladores]# curl -u jcquevedo:cloudera \</b><br>
  'http://localhost:7180/api/v18/users'<br>
{<br>
  "items" : [ {<br>
    "name" : "admin",<br>
    "roles" : [ "ROLE_LIMITED" ]<br>
  }, {<br>
    "name" : "jcquevedo",<br>
    "roles" : [ "ROLE_ADMIN" ]<br>
  }, {<br>
    "name" : "minotaur",<br>
    "roles" : [ "ROLE_CONFIGURATOR" ]<br>
  } ]<br>
}[root@hdp1 instaladores]# <br>

<code><b> Report the database server in use by CM </b></code><br>
<b>[root@hdp1 instaladores]# curl -u jcquevedo:cloudera \ </b><br>
<b>  'http://localhost:7180/api/v18/cm/scmDbInfo'</b><br>
{<br>
  "scmDbType" : "MYSQL",<br>
  "embeddedDbUsed" : false<br>
}<br>


