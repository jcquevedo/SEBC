<code><b> Check HIVE Status </b></code><br>
<code><b>[raken@hdp1 ~]$ curl -u jcquevedo:cloudera   'http://localhost:7180/api/v14/cluters/jcquevedo/services/hive'</b></code><br>
{<br>
  "name" : "hive",<br>
  "type" : "HIVE",<br>
  "clusterRef" : {<br>
    "clusterName" : "cluster"<br>
  },<br>
  "serviceUrl" : "http://hdp1.northcentralus.cloudapp.azure.com:7180/cmf/serviceRedirect/hive",<br>
  "roleInstancesUrl" : "http://hdp1.northcentralus.cloudapp.azure.com:7180/cmf/serviceRedirect/hive/instances",<br>
  "serviceState" : "STARTED",<br>
  "healthSummary" : "GOOD",<br>
  "healthChecks" : [ {<br>
    "name" : "HIVE_HIVEMETASTORES_HEALTHY",<br>
    "summary" : "GOOD",<br>
    "suppressed" : false<br>
  }, {<br>
    "name" : "HIVE_HIVESERVER2S_HEALTHY",<br>
    "summary" : "GOOD",<br>
    "suppressed" : false<br>
  } ],<br>
  "configStalenessStatus" : "FRESH",<br>
  "clientConfigStalenessStatus" : "FRESH",<br>
  "maintenanceMode" : false,<br>
  "maintenanceOwners" : [ ],<br>
  "displayName" : "Hive",<br>
  "entityStatus" : "GOOD_HEALTH"<br>
}<br>
<br>
<code><b> Stop Hive Service </b></code><br>
<code><b>[raken@hdp1 ~]$ curl -X POST -u jcquevedo:cloudera \ </b></code><br>
  'http://localhost:7180/api/v14/clusters/jcquevedo/services/hive/commands/stop' <br>
{ <br>
  "id" : 1206,<br>
  "name" : "Stop",<br>
  "startTime" : "2017-11-30T18:15:08.390Z",
  "active" : true,<br>
  "serviceRef" : {<br>
    "clusterName" : "cluster",<br>
    "serviceName" : "hive"<br>
  }<br>

<code><b> Sart Hive Service </b></code><br>
<code><b>[raken@hdp1 ~]$ curl -X POST -u jcquevedo:cloudera \ </b></code><br>
  'http://localhost:7180/api/v14/clusters/jcquevedo/services/hive/commands/start'<br>
{<br>
  "id" : 1212,<br>
  "name" : "Start",<br>
  "startTime" : "2017-11-30T18:20:05.275Z",<br>
  "active" : true,<br>
  "serviceRef" : {<br>
    "clusterName" : "cluster",<br>
    "serviceName" : "hive"<br>
  }<br>
}<br>
