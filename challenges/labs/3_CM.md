
<code><b>The command and output for</b></code><br>
hdfs dfs -ls /user<br>
[raken@host4 ~]$ hdfs dfs -ls /user<br>
Found 7 items<br>
drwxr-xr-x   - hdfs   supergroup          0 2017-12-01 14:00 /user/haley<br>
drwxrwxrwx   - mapred hadoop              0 2017-12-01 13:49 /user/history<br>
drwxrwxr-t   - hive   hive                0 2017-12-01 13:51 /user/hive<br>
drwxrwxr-x   - hue    hue                 0 2017-12-01 13:51 /user/hue<br>
drwxrwxr-x   - oozie  oozie               0 2017-12-01 13:52 /user/oozie<br>
drwxr-xr-x   - hdfs   supergroup          0 2017-12-01 14:00 /user/saturn<br>
drwxr-x--x   - spark  spark               0 2017-12-01 13:49 /user/spark<br>
[raken@host4 ~]$ <br>

<code><b>The command and output from the CM API call ../api/v14/hosts</b></code><br>
curl -u jcquevedo:cloudera \ <br>
 'http://localhost:7180/api/v14/hosts'<br>
{<br>
  "items" : [ {<br>
    "hostId" : "8905d6c7-cd78-4d45-ad7b-a8a934c12e09",<br>
    "ipAddress" : "10.0.0.9",<br>
    "hostname" : "host1.northcentralus.cloudapp.azure.com",<br>
    "rackId" : "/default",<br>
    "hostUrl" : "http://host1.northcentralus.cloudapp.azure.com:7180/cmf/hostRedirect/8905d6c7-cd78-4d45-ad7b-a8a934c12e09",<br>
    "maintenanceMode" : false,<br>
    "maintenanceOwners" : [ ],<br>
    "commissionState" : "COMMISSIONED",<br>
    "numCores" : 8,<br>
    "numPhysicalCores" : 4,<br>
    "totalPhysMemBytes" : 33449582592<br>
  }, {<br>
    "hostId" : "197382d9-ea0b-41a8-972f-1bdb3b1aa2b7",<br>
    "ipAddress" : "10.0.0.12",<br>
    "hostname" : "host4.northcentralus.cloudapp.azure.com",<br>
    "rackId" : "/default",<br>
    "hostUrl" : "http://host1.northcentralus.cloudapp.azure.com:7180/cmf/hostRedirect/197382d9-ea0b-41a8-972f-1bdb3b1aa2b7",<br>
    "maintenanceMode" : false,<br>
    "maintenanceOwners" : [ ],<br>
    "commissionState" : "COMMISSIONED",<br>
    "numCores" : 8,<br>
    "numPhysicalCores" : 4,<br>
    "totalPhysMemBytes" : 33449582592<br>
  }, {<br>
    "hostId" : "01073da5-0d60-467c-b980-4c32ea47345b",<br>
    "ipAddress" : "10.0.0.10",<br>
    "hostname" : "hosts2.northcentralus.cloudapp.azure.com",<br>
    "rackId" : "/default",<br>
    "hostUrl" : "http://host1.northcentralus.cloudapp.azure.com:7180/cmf/hostRedirect/01073da5-0d60-467c-b980-4c32ea47345b",<br>
    "maintenanceMode" : false,<br>
    "maintenanceOwners" : [ ],<br>
    "commissionState" : "COMMISSIONED",<br>
    "numCores" : 8,<br>
    "numPhysicalCores" : 4,<br>
    "totalPhysMemBytes" : 33449582592<br>
  }, {<br>
    "hostId" : "12a3b359-63cc-4080-879b-90206d9a9753",<br>
    "ipAddress" : "10.0.0.11",<br>
    "hostname" : "hosts3.northcentralus.cloudapp.azure.com",<br>
    "rackId" : "/default",<br>
    "hostUrl" : "http://host1.northcentralus.cloudapp.azure.com:7180/cmf/hostRedirect/12a3b359-63cc-4080-879b-90206d9a9753",<br>
    "maintenanceMode" : false,<br>
    "maintenanceOwners" : [ ],<br>
    "commissionState" : "COMMISSIONED",<br>
    "numCores" : 8,<br>
    "numPhysicalCores" : 4,<br>
    "totalPhysMemBytes" : 33449582592<br>
  } ]<br>


<code><b>The command and output from the CM API call ../api/v8/clusters/jcquevedo/services</b></code><br>
curl -u jcquevedo:cloudera \ <br>
 'http://localhost:7180/api/v8/clusters/jcquevedo/services'<br>
{<br>
  "items" : [ {<br>
    "hostId" : "8905d6c7-cd78-4d45-ad7b-a8a934c12e09",<br>
    "ipAddress" : "10.0.0.9",<br>
    "hostname" : "host1.northcentralus.cloudapp.azure.com",<br>
    "rackId" : "/default",<br>
    "hostUrl" : "http://host1.northcentralus.cloudapp.azure.com:7180/cmf/hostRedirect/8905d6c7-cd78-4d45-ad7b-a8a934c12e09",<br>
    "maintenanceMode" : false,<br>
    "maintenanceOwners" : [ ],<br>
    "commissionState" : "COMMISSIONED",<br>
    "numCores" : 8,<br>
    "numPhysicalCores" : 4,<br>
    "totalPhysMemBytes" : 33449582592<br>
  }, {<br>
    "hostId" : "197382d9-ea0b-41a8-972f-1bdb3b1aa2b7",<br>
    "ipAddress" : "10.0.0.12",<br>
    "hostname" : "host4.northcentralus.cloudapp.azure.com",<br>
    "rackId" : "/default",<br>
    "hostUrl" : "http://host1.northcentralus.cloudapp.azure.com:7180/cmf/hostRedirect/197382d9-ea0b-41a8-972f-1bdb3b1aa2b7",<br>
    "maintenanceMode" : false,<br>
    "maintenanceOwners" : [ ],<br>
    "commissionState" : "COMMISSIONED",<br>
    "numCores" : 8,<br>
    "numPhysicalCores" : 4,<br>
    "totalPhysMemBytes" : 33449582592<br>
  }, {<br>
    "hostId" : "01073da5-0d60-467c-b980-4c32ea47345b",<br>
    "ipAddress" : "10.0.0.10",<br>
    "hostname" : "hosts2.northcentralus.cloudapp.azure.com",<br>
    "rackId" : "/default",<br>
    "hostUrl" : "http://host1.northcentralus.cloudapp.azure.com:7180/cmf/hostRedirect/01073da5-0d60-467c-b980-4c32ea47345b",<br>
    "maintenanceMode" : false,<br>
    "maintenanceOwners" : [ ],<br>
    "commissionState" : "COMMISSIONED",<br>
    "numCores" : 8,<br>
    "numPhysicalCores" : 4,<br>
    "totalPhysMemBytes" : 33449582592<br>
  }, {<br>
    "hostId" : "12a3b359-63cc-4080-879b-90206d9a9753",<br>
    "ipAddress" : "10.0.0.11",<br>
    "hostname" : "hosts3.northcentralus.cloudapp.azure.com",<br>
    "rackId" : "/default",<br>
    "hostUrl" : "http://host1.northcentralus.cloudapp.azure.com:7180/cmf/hostRedirect/12a3b359-63cc-4080-879b-90206d9a9753",<br>
    "maintenanceMode" : false,<br>
    "maintenanceOwners" : [ ],<br>
    "commissionState" : "COMMISSIONED",<br>
    "numCores" : 8,<br>
    "numPhysicalCores" : 4,<br>
    "totalPhysMemBytes" : 33449582592<br>
  } ]<br>
}[root@host1 CDH5]# curl -u jcquevedo:cloudera \<br>
 'http://localhost:7180/api/v8/clusters/jcquevedo/services'<br>
{<br>
  "items" : [ {<br>
    "name" : "hive",<br>
    "type" : "HIVE",<br>
    "clusterRef" : {<br>
      "clusterName" : "cluster"<br>
    },<br>
    "serviceUrl" : "http://host1.northcentralus.cloudapp.azure.com:7180/cmf/serviceRedirect/hive",<br>
    "serviceState" : "STARTED",<br>
    "healthSummary" : "BAD",<br>
    "healthChecks" : [ {<br>
      "name" : "HIVE_HIVEMETASTORES_HEALTHY",<br>
      "summary" : "BAD"<br>
    }, {<br>
      "name" : "HIVE_HIVESERVER2S_HEALTHY",<br>
      "summary" : "BAD"<br>
    } ],<br>
    "configStalenessStatus" : "FRESH",<br>
    "clientConfigStalenessStatus" : "FRESH",<br>
    "maintenanceMode" : false,<br>
    "maintenanceOwners" : [ ],<br>
    "displayName" : "Hive"<br>
  }, {<br>
    "name" : "zookeeper",<br>
    "type" : "ZOOKEEPER",<br>
    "clusterRef" : {<br>
      "clusterName" : "cluster"<br>
    },<br>
    "serviceUrl" : "http://host1.northcentralus.cloudapp.azure.com:7180/cmf/serviceRedirect/zookeeper",<br>
    "serviceState" : "STARTED",<br>
    "healthSummary" : "BAD",<br>
    "healthChecks" : [ {<br>
      "name" : "ZOOKEEPER_CANARY_HEALTH",<br>
      "summary" : "GOOD"<br>
    }, {<br>
      "name" : "ZOOKEEPER_SERVERS_HEALTHY",<br>
      "summary" : "BAD"<br>
    } ],<br>
    "configStalenessStatus" : "FRESH",<br>
    "clientConfigStalenessStatus" : "FRESH",<br>
    "maintenanceMode" : false,<br>
    "maintenanceOwners" : [ ],<br>
    "displayName" : "ZooKeeper"<br>
  }, {<br>
    "name" : "hue",<br>
    "type" : "HUE",<br>
    "clusterRef" : {<br>
      "clusterName" : "cluster"<br>
    },<br>
    "serviceUrl" : "http://host1.northcentralus.cloudapp.azure.com:7180/cmf/serviceRedirect/hue",<br>
    "serviceState" : "STARTED",<br>
    "healthSummary" : "BAD",<br>
    "healthChecks" : [ {<br>
      "name" : "HUE_HUE_SERVERS_HEALTHY",<br>
      "summary" : "BAD"<br>
    } ],<br>
    "configStalenessStatus" : "FRESH",<br>
    "clientConfigStalenessStatus" : "FRESH",<br>
    "maintenanceMode" : false,<br>
    "maintenanceOwners" : [ ],<br>
    "displayName" : "Hue"<br>
  }, {<br>
    "name" : "oozie",<br>
    "type" : "OOZIE",<br>
    "clusterRef" : {<br>
      "clusterName" : "cluster"<br>
    },<br>
    "serviceUrl" : "http://host1.northcentralus.cloudapp.azure.com:7180/cmf/serviceRedirect/oozie",<br>
    "serviceState" : "STARTED",<br>
    "healthSummary" : "BAD",<br>
    "healthChecks" : [ {<br>
      "name" : "OOZIE_OOZIE_SERVERS_HEALTHY",<br>
      "summary" : "BAD"<br>
    } ],<br>
    "configStalenessStatus" : "FRESH",<br>
    "clientConfigStalenessStatus" : "FRESH",<br>
    "maintenanceMode" : false,<br>
    "maintenanceOwners" : [ ],<br>
    "displayName" : "Oozie"<br>
  }, {<br>
    "name" : "yarn",<br>
    "type" : "YARN",<br>
    "clusterRef" : {<br>
      "clusterName" : "cluster"<br>
    },<br>
    "serviceUrl" : "http://host1.northcentralus.cloudapp.azure.com:7180/cmf/serviceRedirect/yarn",<br>
    "serviceState" : "STARTED",<br>
    "healthSummary" : "BAD",<br>
    "healthChecks" : [ {<br>
      "name" : "YARN_JOBHISTORY_HEALTH",<br>
      "summary" : "BAD"<br>
    }, {<br>
      "name" : "YARN_NODE_MANAGERS_HEALTHY",<br>
      "summary" : "BAD"<br>
    }, {<br>
      "name" : "YARN_RESOURCEMANAGERS_HEALTH",<br>
      "summary" : "BAD"<br>
    }, {<br>
      "name" : "YARN_USAGE_AGGREGATION_HEALTH",<br>
      "summary" : "DISABLED"<br>
    } ],<br>
    "configStalenessStatus" : "FRESH",<br>
    "clientConfigStalenessStatus" : "FRESH",<br>
    "maintenanceMode" : false,<br>
    "maintenanceOwners" : [ ],<br>
    "displayName" : "YARN (MR2 Included)"<br>
  }, {<br>
    "name" : "spark_on_yarn",<br>
    "type" : "SPARK_ON_YARN",<br>
    "clusterRef" : {<br>
      "clusterName" : "cluster"<br>
    },<br>
    "serviceUrl" : "http://host1.northcentralus.cloudapp.azure.com:7180/cmf/serviceRedirect/spark_on_yarn",<br>
    "serviceState" : "STARTED",<br>
    "healthSummary" : "GOOD",<br>
    "healthChecks" : [ ],<br>
    "configStalenessStatus" : "FRESH",<br>
    "clientConfigStalenessStatus" : "FRESH",<br>
    "maintenanceMode" : false,<br>
    "maintenanceOwners" : [ ],<br>
    "displayName" : "Spark"<br>
  }, {<br>
    "name" : "hdfs",<br>
    "type" : "HDFS",<br>
    "clusterRef" : {<br>
      "clusterName" : "cluster"<br>
    },<br>
    "serviceUrl" : "http://host1.northcentralus.cloudapp.azure.com:7180/cmf/serviceRedirect/hdfs",<br>
    "serviceState" : "STARTED",<br>
    "healthSummary" : "BAD",<br>
    "healthChecks" : [ {<br>
      "name" : "HDFS_BLOCKS_WITH_CORRUPT_REPLICAS",<br>
      "summary" : "GOOD"<br>
    }, {<br>
      "name" : "HDFS_CANARY_HEALTH",<br>
      "summary" : "GOOD"<br>
    }, {<br>
      "name" : "HDFS_DATA_NODES_HEALTHY",<br>
      "summary" : "BAD"<br>
    }, {<br>
      "name" : "HDFS_FREE_SPACE_REMAINING",<br>
      "summary" : "GOOD"<br>
    }, {<br>
      "name" : "HDFS_HA_NAMENODE_HEALTH",<br>
      "summary" : "BAD"<br>
    }, {<br>
      "name" : "HDFS_MISSING_BLOCKS",<br>
      "summary" : "GOOD"<br>
    }, {<br>
      "name" : "HDFS_UNDER_REPLICATED_BLOCKS",<br>
      "summary" : "GOOD"<br>
    } ],<br>
    "configStalenessStatus" : "FRESH",<br>
    "clientConfigStalenessStatus" : "FRESH",<br>
    "maintenanceMode" : false,<br>
    "maintenanceOwners" : [ ],<br>
    "displayName" : "HDFS"<br>
  } ]<br>
}<br>


<br>