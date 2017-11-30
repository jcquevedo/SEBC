{<br>
  "timestamp" : "2017-11-30T17:01:53.643Z",<br>
  "clusters" : [ {<br>
    "name" : "jcquevedo",<br>
    "version" : "CDH5",<br>
    "services" : [ {<br>
      "name" : "hive",<br>
      "type" : "HIVE",<br>
      "config" : {<br>
        "roleTypeConfigs" : [ {<br>
          "roleType" : "HIVEMETASTORE",<br>
          "items" : [ {<br>
            "name" : "hive_metastore_java_heapsize",<br>
            "value" : "6026166272"<br>
          }, {<br>
            "name" : "hive_metastore_server_max_message_size",<br>
            "value" : "602616627"<br>
          } ]<br>
        }, {<br>
          "roleType" : "HIVESERVER2",<br>
          "items" : [ {<br>
            "name" : "hiveserver2_enable_impersonation",<br>
            "value" : "false"<br>
          }, {<br>
            "name" : "hiveserver2_spark_driver_memory",<br>
            "value" : "966367641"<br>
          }, {<br>
            "name" : "hiveserver2_spark_executor_cores",<br>
            "value" : "4"<br>
          }, {<br>
            "name" : "hiveserver2_spark_executor_memory",<br>
            "value" : "4801377075"<br>
          }, {<br>
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",<br>
            "value" : "102"<br>
          }, {<br>
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",<br>
            "value" : "808"<br>
          } ]<br>
        } ],<br>
        "items" : [ {<br>
          "name" : "hive_metastore_database_host",<br>
          "value" : "stdalonejq.northcentralus.cloudapp.azure.com"<br>
        }, {<br>
          "name" : "hive_metastore_database_password",<br>
          "value" : "Raken.2017"<br>
        }, {<br>
          "name" : "hive_proxy_user_groups_list",<br>
          "value" : "hue,hive,sentry"<br>
        }, {<br>
          "name" : "mapreduce_yarn_service",<br>
          "value" : "yarn"<br>
        }, {<br>
          "name" : "sentry_service",<br>
          "value" : "sentry"<br>
        }, {<br>
          "name" : "zookeeper_service",<br>
          "value" : "zookeeper"<br>
        } ]<br>
      },<br>
      "roles" : [ {<br>
        "name" : "hive-GATEWAY-0606538f948d493a297260707d78d635",<br>
        "type" : "GATEWAY",<br>
        "hostRef" : {<br>
          "hostId" : "781ae094-3759-4653-8657-da3682878391"<br>
        },<br>
        "config" : {<br>
          "items" : [ ]<br>
        }<br>
      }, {<br>
        "name" : "hive-GATEWAY-193d65d588027c655cefab96da5feb37",<br>
        "type" : "GATEWAY",<br>
        "hostRef" : {<br>
          "hostId" : "7dae7d03-866d-4638-877a-39de4cfb5485"<br>
        },<br>
        "config" : {<br>
          "items" : [ ]<br>
        }<br>
      }, {<br>
        "name" : "hive-GATEWAY-54de5a68a1c4c7dc1cd2ef6ecbbec893",<br>
        "type" : "GATEWAY",<br>
        "hostRef" : {<br>
          "hostId" : "2182c8eb-e19d-447d-a9e9-df43e23bfbb2"<br>
        },<br>
        "config" : {<br>
          "items" : [ ]<br>
        }<br>
      }, {<br>
        "name" : "hive-GATEWAY-6d4b72313ca639207efafcd082d1e8e3",<br>
        "type" : "GATEWAY",<br>
        "hostRef" : {<br>
          "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"<br>
        },<br>
        "config" : {<br>
          "items" : [ ]<br>
        }<br>
      }, {<br>
        "name" : "hive-HIVEMETASTORE-54de5a68a1c4c7dc1cd2ef6ecbbec893",<br>
        "type" : "HIVEMETASTORE",<br>
        "hostRef" : {<br>
          "hostId" : "2182c8eb-e19d-447d-a9e9-df43e23bfbb2"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "6obfyr7rxhrdp959x40smaa78"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "hive-HIVESERVER2-54de5a68a1c4c7dc1cd2ef6ecbbec893",<br>
        "type" : "HIVESERVER2",<br>
        "hostRef" : {<br>
          "hostId" : "2182c8eb-e19d-447d-a9e9-df43e23bfbb2"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "ej8bthvr041xkyzl7599o3svn"<br>
          } ]<br>
        }<br>
      } ],<br>
      "displayName" : "Hive"<br>
    }, {<br>
      "name" : "zookeeper",<br>
      "type" : "ZOOKEEPER",<br>
      "config" : {<br>
        "roleTypeConfigs" : [ ],<br>
        "items" : [ {<br>
          "name" : "enableSecurity",<br>
          "value" : "true"<br>
        } ]<br>
      },<br>
      "roles" : [ {<br>
        "name" : "zookeeper-SERVER-0606538f948d493a297260707d78d635",<br>
        "type" : "SERVER",<br>
        "hostRef" : {<br>
          "hostId" : "781ae094-3759-4653-8657-da3682878391"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "e0g3hn04si9hjy890727xc675"<br>
          }, {<br>
            "name" : "serverId",<br>
            "value" : "1"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "zookeeper-SERVER-193d65d588027c655cefab96da5feb37",<br>
        "type" : "SERVER",<br>
        "hostRef" : {<br>
          "hostId" : "7dae7d03-866d-4638-877a-39de4cfb5485"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "8y66mhza4cxtkfuxsrvahtojt"<br>
          }, {<br>
            "name" : "serverId",<br>
            "value" : "2"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "zookeeper-SERVER-6d4b72313ca639207efafcd082d1e8e3",<br>
        "type" : "SERVER",<br>
        "hostRef" : {<br>
          "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "fjce7txnjx0uh227hlxl3lg9"<br>
          }, {<br>
            "name" : "serverId",<br>
            "value" : "3"<br>
          } ]<br>
        }<br>
      } ],<br>
      "displayName" : "ZooKeeper"<br>
    }, {<br>
      "name" : "hue",<br>
      "type" : "HUE",<br>
      "config" : {<br>
        "roleTypeConfigs" : [ {<br>
          "roleType" : "HUE_SERVER",<br>
          "items" : [ {<br>
            "name" : "hue_server_bind_wildcard",<br>
            "value" : "true"<br>
          } ]<br>
        } ],<br>
        "items" : [ {<br>
          "name" : "database_host",<br>
          "value" : "stdalonejq.northcentralus.cloudapp.azure.com"<br>
        }, {<br>
          "name" : "database_password",<br>
          "value" : "Raken.2017"<br>
        }, {<br>
          "name" : "database_type",<br>
          "value" : "mysql"<br>
        }, {<br>
          "name" : "hive_service",<br>
          "value" : "hive"<br>
        }, {<br>
          "name" : "hue_webhdfs",<br>
          "value" : "hdfs-NAMENODE-6d4b72313ca639207efafcd082d1e8e3"<br>
        }, {<br>
          "name" : "oozie_service",<br>
          "value" : "oozie"<br>
        }, {<br>
          "name" : "sentry_service",<br>
          "value" : "sentry"<br>
        }, {<br>
          "name" : "zookeeper_service",<br>
          "value" : "zookeeper"<br>
        } ]<br>
      },<br>
      "roles" : [ {<br>
        "name" : "hue-HUE_SERVER-193d65d588027c655cefab96da5feb37",<br>
        "type" : "HUE_SERVER",<br>
        "hostRef" : {<br>
          "hostId" : "7dae7d03-866d-4638-877a-39de4cfb5485"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "2qln5lg0imc2sf9j9k0qpiy1v"<br>
          }, {<br>
            "name" : "secret_key",<br>
            "value" : "OQBNFBaE0UUjDPDQ425j2ZyKgpjAZz"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "hue-KT_RENEWER-193d65d588027c655cefab96da5feb37",<br>
        "type" : "KT_RENEWER",<br>
        "hostRef" : {<br>
          "hostId" : "7dae7d03-866d-4638-877a-39de4cfb5485"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "aeghmmvszbanxayrueon0fpeg"<br>
          } ]<br>
        }<br>
      } ],<br>
      "displayName" : "Hue"<br>
    }, {<br>
      "name" : "oozie",<br>
      "type" : "OOZIE",<br>
      "config" : {<br>
        "roleTypeConfigs" : [ {<br>
          "roleType" : "OOZIE_SERVER",<br>
          "items" : [ {<br>
            "name" : "oozie_database_host",<br>
            "value" : "stdalonejq.northcentralus.cloudapp.azure.com"<br>
          }, {<br>
            "name" : "oozie_database_password",<br>
            "value" : "Raken.2017"<br>
          }, {<br>
            "name" : "oozie_database_type",<br>
            "value" : "mysql"<br>
          }, {<br>
            "name" : "oozie_database_user",<br>
            "value" : "oozie"<br>
          } ]<br>
        } ],<br>
        "items" : [ {<br>
          "name" : "hive_service",<br>
          "value" : "hive"<br>
        }, {<br>
          "name" : "mapreduce_yarn_service",<br>
          "value" : "yarn"<br>
        }, {<br>
          "name" : "zookeeper_service",<br>
          "value" : "zookeeper"<br>
        } ]<br>
      },<br>
      "roles" : [ {<br>
        "name" : "oozie-OOZIE_SERVER-54de5a68a1c4c7dc1cd2ef6ecbbec893",<br>
        "type" : "OOZIE_SERVER",<br>
        "hostRef" : {<br>
          "hostId" : "2182c8eb-e19d-447d-a9e9-df43e23bfbb2"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "arf21j4n8lz7yaelq9vs7ddmw"<br>
          } ]<br>
        }<br>
      } ],<br>
      "displayName" : "Oozie"<br>
    }, {<br>
      "name" : "yarn",<br>
      "type" : "YARN",<br>
      "config" : {<br>
        "roleTypeConfigs" : [ {<br>
          "roleType" : "GATEWAY",<br>
          "items" : [ {<br>
            "name" : "mapred_reduce_tasks",<br>
            "value" : "12"<br>
          }, {<br>
            "name" : "mapred_submit_replication",<br>
            "value" : "1"<br>
          } ]<br>
        }, {<br>
          "roleType" : "NODEMANAGER",<br>
          "items" : [ {<br>
            "name" : "yarn_nodemanager_heartbeat_interval_ms",<br>
            "value" : "100"<br>
          }, {<br>
            "name" : "yarn_nodemanager_local_dirs",<br>
            "value" : "/mnt/resource/yarn/nm"<br>
          }, {<br>
            "name" : "yarn_nodemanager_log_dirs",<br>
            "value" : "/mnt/resource/yarn/container-logs"<br>
          }, {<br>
            "name" : "yarn_nodemanager_resource_memory_mb",<br>
            "value" : "9776"<br>
          } ]<br>
        }, {<br>
          "roleType" : "RESOURCEMANAGER",<br>
          "items" : [ {<br>
            "name" : "yarn_scheduler_maximum_allocation_mb",<br>
            "value" : "16508"<br>
          }, {<br>
            "name" : "yarn_scheduler_maximum_allocation_vcores",<br>
            "value" : "6"<br>
          } ]<br>
        } ],<br>
        "items" : [ {<br>
          "name" : "hdfs_service",<br>
          "value" : "hdfs"<br>
        }, {<br>
          "name" : "rm_dirty",<br>
          "value" : "false"<br>
        }, {<br>
          "name" : "rm_last_allocation_percentage",<br>
          "value" : "80"<br>
        }, {<br>
          "name" : "yarn_service_cgroups",<br>
          "value" : "false"<br>
        }, {<br>
          "name" : "yarn_service_lce_always",<br>
          "value" : "false"<br>
        }, {<br>
          "name" : "zk_authorization_secret_key",<br>
          "value" : "TaNWXESFPc0T3S3r7qOYNkqtkIoqMD"<br>
        }, {<br>
          "name" : "zookeeper_service",<br>
          "value" : "zookeeper"<br>
        } ]<br>
      },<br>
      "roles" : [ {<br>
        "name" : "yarn-JOBHISTORY-6d4b72313ca639207efafcd082d1e8e3",<br>
        "type" : "JOBHISTORY",<br>
        "hostRef" : {<br>
          "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "23uocofb173wjanjoyqm1io7h"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "yarn-NODEMANAGER-0606538f948d493a297260707d78d635",<br>
        "type" : "NODEMANAGER",<br>
        "hostRef" : {<br>
          "hostId" : "781ae094-3759-4653-8657-da3682878391"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "4ij5z8fghfch9sml2rn5545rn"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "yarn-NODEMANAGER-193d65d588027c655cefab96da5feb37",<br>
        "type" : "NODEMANAGER",<br>
        "hostRef" : {<br>
          "hostId" : "7dae7d03-866d-4638-877a-39de4cfb5485"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "46se3znplz3uo20ainzmcjouj"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "yarn-NODEMANAGER-54de5a68a1c4c7dc1cd2ef6ecbbec893",<br>
        "type" : "NODEMANAGER",<br>
        "hostRef" : {<br>
          "hostId" : "2182c8eb-e19d-447d-a9e9-df43e23bfbb2"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "9acxvsmc5u0qap8ozah3zgckz"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "yarn-RESOURCEMANAGER-0606538f948d493a297260707d78d635",<br>
        "type" : "RESOURCEMANAGER",<br>
        "hostRef" : {<br>
          "hostId" : "781ae094-3759-4653-8657-da3682878391"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "rm_id",<br>
            "value" : "48"<br>
          }, {<br>
            "name" : "role_jceks_password",<br>
            "value" : "x330b5qfv1y8ase42x59hspw"<br>
          } ]<br>
        }<br>
      } ],<br>
      "displayName" : "YARN (MR2 Included)"<br>
    }, {<br>
      "name" : "hdfs",<br>
      "type" : "HDFS",<br>
      "config" : {<br>
        "roleTypeConfigs" : [ {<br>
          "roleType" : "DATANODE",<br>
          "items" : [ {<br>
            "name" : "datanode_java_heapsize",<br>
            "value" : "1073741824"<br>
          }, {<br>
            "name" : "dfs_data_dir_list",<br>
            "value" : "/mnt/resource/dfs/dn"<br>
          }, {<br>
            "name" : "dfs_datanode_data_dir_perm",<br>
            "value" : "700"<br>
          }, {<br>
            "name" : "dfs_datanode_http_port",<br>
            "value" : "1006"<br>
          }, {<br>
            "name" : "dfs_datanode_max_locked_memory",<br>
            "value" : "4294967296"<br>
          }, {<br>
            "name" : "dfs_datanode_port",<br>
            "value" : "1004"<br>
          }, {<br>
            "name" : "rm_cpu_shares",<br>
            "value" : "400"<br>
          }, {<br>
            "name" : "rm_io_weight",<br>
            "value" : "200"<br>
          } ]<br>
        }, {<br>
          "roleType" : "GATEWAY",<br>
          "items" : [ {<br>
            "name" : "dfs_client_use_trash",<br>
            "value" : "true"<br>
          } ]<br>
        }, {<br>
          "roleType" : "JOURNALNODE",<br>
          "items" : [ {<br>
            "name" : "dfs_journalnode_edits_dir",<br>
            "value" : "/mnt/resource/jn"<br>
          } ]<br>
        }, {<br>
          "roleType" : "NAMENODE",<br>
          "items" : [ {<br>
            "name" : "dfs_name_dir_list",<br>
            "value" : "/mnt/resource/dfs/nn"<br>
          }, {<br>
            "name" : "dfs_namenode_servicerpc_address",<br>
            "value" : "8022"<br>
          } ]<br>
        }, {<br>
          "roleType" : "SECONDARYNAMENODE",<br>
          "items" : [ {<br>
            "name" : "fs_checkpoint_dir_list",<br>
            "value" : "/mnt/resource/dfs/snn"<br>
          } ]<br>
        } ],<br>
        "items" : [ {<br>
          "name" : "dfs_encrypt_data_transfer_algorithm",<br>
          "value" : "AES/CTR/NoPadding"<br>
        }, {<br>
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",<br>
          "value" : "psPgnRB4dbjeJpBZhTaJbGdRP4gNBr"<br>
        }, {<br>
          "name" : "dfs_ha_fencing_methods",<br>
          "value" : "shell(true)"<br>
        }, {<br>
          "name" : "fc_authorization_secret_key",<br>
          "value" : "x96bchl3ePMfWat4NrRM5xezJnc0Up"<br>
        }, {<br>
          "name" : "hadoop_security_authentication",<br>
          "value" : "kerberos"<br>
        }, {<br>
          "name" : "hadoop_security_authorization",<br>
          "value" : "true"<br>
        }, {<br>
          "name" : "http_auth_signature_secret",<br>
          "value" : "JVYcQJ2wg1bwsb7nu6qYE7e7BE1nMz"<br>
        }, {<br>
          "name" : "rm_dirty",<br>
          "value" : "false"<br>
        }, {<br>
          "name" : "rm_last_allocation_percentage",<br>
          "value" : "20"<br>
        }, {<br>
          "name" : "zookeeper_service",<br>
          "value" : "zookeeper"<br>
        } ]<br>
      },<br>
      "roles" : [ {<br>
        "name" : "hdfs-BALANCER-6d4b72313ca639207efafcd082d1e8e3",<br>
        "type" : "BALANCER",<br>
        "hostRef" : {<br>
          "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"<br>
        },<br>
        "config" : {<br>
          "items" : [ ]<br>
        }<br>
      }, {<br>
        "name" : "hdfs-DATANODE-0606538f948d493a297260707d78d635",<br>
        "type" : "DATANODE",<br>
        "hostRef" : {<br>
          "hostId" : "781ae094-3759-4653-8657-da3682878391"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "dzx6qjxsgqw0jfc1kcuo2d5ax"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "hdfs-DATANODE-193d65d588027c655cefab96da5feb37",<br>
        "type" : "DATANODE",<br>
        "hostRef" : {<br>
          "hostId" : "7dae7d03-866d-4638-877a-39de4cfb5485"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "7hjxk493wqq0bl1y8yx0hcetb"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "hdfs-DATANODE-54de5a68a1c4c7dc1cd2ef6ecbbec893",<br>
        "type" : "DATANODE",<br>
        "hostRef" : {<br>
          "hostId" : "2182c8eb-e19d-447d-a9e9-df43e23bfbb2"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "ad7tnhsencafgenxp5jhf6px8"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "hdfs-FAILOVERCONTROLLER-0606538f948d493a297260707d78d635",<br>
        "type" : "FAILOVERCONTROLLER",<br>
        "hostRef" : {<br>
          "hostId" : "781ae094-3759-4653-8657-da3682878391"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "fnwmfhz6wsypg92liq1sx3rh"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "hdfs-FAILOVERCONTROLLER-6d4b72313ca639207efafcd082d1e8e3",<br>
        "type" : "FAILOVERCONTROLLER",<br>
        "hostRef" : {<br>
          "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "6m0n5pxbqn1ucjojni2nq688t"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "hdfs-JOURNALNODE-0606538f948d493a297260707d78d635",<br>
        "type" : "JOURNALNODE",<br>
        "hostRef" : {<br>
          "hostId" : "781ae094-3759-4653-8657-da3682878391"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "3gtaxlxozpf7s388p3xqnyn1m"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "hdfs-JOURNALNODE-193d65d588027c655cefab96da5feb37",<br>
        "type" : "JOURNALNODE",<br>
        "hostRef" : {<br>
          "hostId" : "7dae7d03-866d-4638-877a-39de4cfb5485"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "3e5tw39akxnzwmop3tqrx35i"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "hdfs-JOURNALNODE-54de5a68a1c4c7dc1cd2ef6ecbbec893",<br>
        "type" : "JOURNALNODE",<br>
        "hostRef" : {<br>
          "hostId" : "2182c8eb-e19d-447d-a9e9-df43e23bfbb2"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "2usxwux0gf7ruwm6g8bnov9hp"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "hdfs-NAMENODE-0606538f948d493a297260707d78d635",<br>
        "type" : "NAMENODE",<br>
        "hostRef" : {<br>
          "hostId" : "781ae094-3759-4653-8657-da3682878391"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "autofailover_enabled",<br>
            "value" : "true"<br>
          }, {<br>
            "name" : "dfs_federation_namenode_nameservice",<br>
            "value" : "nameservice1"<br>
          }, {<br>
            "name" : "dfs_namenode_quorum_journal_name",<br>
            "value" : "nameservice1"<br>
          }, {<br>
            "name" : "namenode_id",<br>
            "value" : "55"<br>
          }, {<br>
            "name" : "role_jceks_password",<br>
            "value" : "386n30s8a0uelr8ktce5j5vy8"<br>
          } ]<br>
        }<br>
      }, {<br>
        "name" : "hdfs-NAMENODE-6d4b72313ca639207efafcd082d1e8e3",<br>
        "type" : "NAMENODE",<br>
        "hostRef" : {<br>
          "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "autofailover_enabled",<br>
            "value" : "true"<br>
          }, {<br>
            "name" : "dfs_federation_namenode_nameservice",<br>
            "value" : "nameservice1"<br>
          }, {<br>
            "name" : "dfs_namenode_quorum_journal_name",<br>
            "value" : "nameservice1"<br>
          }, {<br>
            "name" : "namenode_id",<br>
            "value" : "50"<br>
          }, {<br>
            "name" : "role_jceks_password",<br>
            "value" : "5jdydp0hq46hago6la27xeps4"<br>
          } ]<br>
        }<br>
      } ],<br>
      "displayName" : "HDFS"<br>
    }, {<br>
      "name" : "sentry",<br>
      "type" : "SENTRY",<br>
      "config" : {<br>
        "roleTypeConfigs" : [ {<br>
          "roleType" : "SENTRY_SERVER",<br>
          "items" : [ {<br>
            "name" : "sentry_server_java_heapsize",<br>
            "value" : "268435456"<br>
          } ]<br>
        } ],<br>
        "items" : [ {<br>
          "name" : "hdfs_service",<br>
          "value" : "hdfs"<br>
        }, {<br>
          "name" : "sentry_server_database_host",<br>
          "value" : "stdalonejq.northcentralus.cloudapp.azure.com"<br>
        }, {<br>
          "name" : "sentry_server_database_password",<br>
          "value" : "Raken.2017"<br>
        }, {<br>
          "name" : "sentry_service_admin_group",<br>
          "value" : "hive,impala,hue,solr,kafka,jcquevedo"<br>
        }, {<br>
          "name" : "zookeeper_service",<br>
          "value" : "zookeeper"<br>
        } ]<br>
      },<br>
      "roles" : [ {<br>
        "name" : "sentry-GATEWAY-0606538f948d493a297260707d78d635",<br>
        "type" : "GATEWAY",<br>
        "hostRef" : {<br>
          "hostId" : "781ae094-3759-4653-8657-da3682878391"<br>
        },<br>
        "config" : {<br>
          "items" : [ ]<br>
        }<br>
      }, {<br>
        "name" : "sentry-GATEWAY-193d65d588027c655cefab96da5feb37",<br>
        "type" : "GATEWAY",<br>
        "hostRef" : {<br>
          "hostId" : "7dae7d03-866d-4638-877a-39de4cfb5485"<br>
        },<br>
        "config" : {<br>
          "items" : [ ]<br>
        }<br>
      }, {<br>
        "name" : "sentry-GATEWAY-54de5a68a1c4c7dc1cd2ef6ecbbec893",<br>
        "type" : "GATEWAY",<br>
        "hostRef" : {<br>
          "hostId" : "2182c8eb-e19d-447d-a9e9-df43e23bfbb2"<br>
        },<br>
        "config" : {<br>
          "items" : [ ]<br>
        }<br>
      }, {<br>
        "name" : "sentry-GATEWAY-6d4b72313ca639207efafcd082d1e8e3",<br>
        "type" : "GATEWAY",<br>
        "hostRef" : {<br>
          "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"<br>
        },<br>
        "config" : {<br>
          "items" : [ ]<br>
        }<br>
      }, {<br>
        "name" : "sentry-SENTRY_SERVER-54de5a68a1c4c7dc1cd2ef6ecbbec893",<br>
        "type" : "SENTRY_SERVER",<br>
        "hostRef" : {<br>
          "hostId" : "2182c8eb-e19d-447d-a9e9-df43e23bfbb2"<br>
        },<br>
        "config" : {<br>
          "items" : [ {<br>
            "name" : "role_jceks_password",<br>
            "value" : "40264zvmf260zh8lvnzivq2xt"<br>
          } ]<br>
        }<br>
      } ],<br>
      "displayName" : "Sentry"<br>
    } ]<br>
  } ],<br>
  "hosts" : [ {<br>
    "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f",<br>
    "ipAddress" : "10.0.0.5",<br>
    "hostname" : "hdp1.northcentralus.cloudapp.azure.com",<br>
    "rackId" : "/default",<br>
    "config" : {<br>
      "items" : [ {<br>
        "name" : "memory_overcommit_threshold",<br>
        "value" : "0.95"<br>
      } ]<br>
    }<br>
  }, {<br>
    "hostId" : "781ae094-3759-4653-8657-da3682878391",<br>
    "ipAddress" : "10.0.0.6",<br>
    "hostname" : "hdp2.northcentralus.cloudapp.azure.com",<br>
    "rackId" : "/default",<br>
    "config" : {<br>
      "items" : [ ]<br>
    }<br>
  }, {<br>
    "hostId" : "7dae7d03-866d-4638-877a-39de4cfb5485",<br>
    "ipAddress" : "10.0.0.7",<br>
    "hostname" : "hdp3.northcentralus.cloudapp.azure.com",<br>
    "rackId" : "/default",<br>
    "config" : {<br>
      "items" : [ {<br>
        "name" : "memory_overcommit_threshold",<br>
        "value" : "0.95"<br>
      } ]<br>
    }<br>
  }, {<br>
    "hostId" : "2182c8eb-e19d-447d-a9e9-df43e23bfbb2",<br>
    "ipAddress" : "10.0.0.8",<br>
    "hostname" : "hdp4.northcentralus.cloudapp.azure.com",<br>
    "rackId" : "/default",<br>
    "config" : {<br>
      "items" : [ {<br>
        "name" : "memory_overcommit_threshold",<br>
        "value" : "0.95"<br>
      } ]<br>
    }<br>
  } ],<br>
  "users" : [ {<br>
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-6d4b72313ca639207efafcd082d1e8e3",<br>
    "roles" : [ "ROLE_USER" ],<br>
    "pwHash" : "eaf44f9462f0df27b384881ce7777eaf671ea3b9ad05f65ea79ec8db498b34da",<br>
    "pwSalt" : -2373169864744697506,<br>
    "pwLogin" : true<br>
  }, {<br>
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-6d4b72313ca639207efafcd082d1e8e3",<br>
    "roles" : [ "ROLE_USER" ],<br>
    "pwHash" : "342e197e0134af3be5316a8b53094b78af8baca3f685247ef166bc51d8aa696c",<br>
    "pwSalt" : 5631694952982674857,<br>
    "pwLogin" : true<br>
  }, {<br>
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-6d4b72313ca639207efafcd082d1e8e3",<br>
    "roles" : [ "ROLE_USER" ],<br>
    "pwHash" : "43b676be9be44dad70ed5afdbaae307c26e1d76d6eea2e8c7a7c2dc7c31b7c7b",<br>
    "pwSalt" : -8632549585653729165,<br>
    "pwLogin" : true<br>
  }, {<br>
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-6d4b72313ca639207efafcd082d1e8e3",<br>
    "roles" : [ "ROLE_USER" ],<br>
    "pwHash" : "14fde2e9e5545c499f2e6273fb622d6ef3af04238b767a14132e02b98fa7a1ba",<br>
    "pwSalt" : -457909825541318944,<br>
    "pwLogin" : true<br>
  }, {<br>
    "name" : "admin",<br>
    "roles" : [ "ROLE_LIMITED" ],<br>
    "pwHash" : "73b73e3b3595b358ece1d5399cd95249d7995f809a8e2e8ca40aba131ca1e244",<br>
    "pwSalt" : -3249067716897620933,<br>
    "pwLogin" : true<br>
  }, {<br>
    "name" : "jcquevedo",<br>
    "roles" : [ "ROLE_ADMIN" ],<br>
    "pwHash" : "fddf0f92bacd3dcd1411cb3e5da5d9088342b8de24dcfa0aebe62681fdee802c",<br>
    "pwSalt" : -4047757178806164821,<br>
    "pwLogin" : true<br>
  }, {<br>
    "name" : "minotaur",<br>
    "roles" : [ "ROLE_CONFIGURATOR" ],<br>
    "pwHash" : "ae2265528c30d1353723af45dddb2d8294532904c14d51fca3f18204af2a73c7",<br>
    "pwSalt" : -8523854381113412111,<br>
    "pwLogin" : true<br>
  } ],<br>
  "versionInfo" : {<br>
    "version" : "5.9.1",<br>
    "buildUser" : "jenkins",<br>
    "buildTimestamp" : "20170112-1158",<br>
    "gitHash" : "a66d8bbdbe8bc3ee54235e55423f2f76c7d9f3b1",<br>
    "snapshot" : false<br>
  },<br>
  "managementService" : {<br>
    "name" : "mgmt",<br>
    "type" : "MGMT",<br>
    "config" : {<br>
      "roleTypeConfigs" : [ {<br>
        "roleType" : "HOSTMONITOR",<br>
        "items" : [ {<br>
          "name" : "firehose_non_java_memory_bytes",<br>
          "value" : "1610612736"<br>
        } ]<br>
      }, {<br>
        "roleType" : "REPORTSMANAGER",<br>
        "items" : [ {<br>
          "name" : "headlamp_database_host",<br>
          "value" : "stdalonejq.northcentralus.cloudapp.azure.com"<br>
        }, {<br>
          "name" : "headlamp_database_name",<br>
          "value" : "rman"<br>
        }, {<br>
          "name" : "headlamp_database_password",<br>
          "value" : "Raken.2017"<br>
        }, {<br>
          "name" : "headlamp_database_user",<br>
          "value" : "rman"<br>
        } ]<br>
      }, {<br>
        "roleType" : "SERVICEMONITOR",<br>
        "items" : [ {<br>
          "name" : "firehose_non_java_memory_bytes",<br>
          "value" : "1610612736"<br>
        } ]<br>
      } ],<br>
      "items" : [ ]<br>
    },<br>
    "roles" : [ {<br>
      "name" : "mgmt-ALERTPUBLISHER-6d4b72313ca639207efafcd082d1e8e3",<br>
      "type" : "ALERTPUBLISHER",<br>
      "hostRef" : {<br>
        "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"<br>
      },<br>
      "config" : {<br>
        "items" : [ {<br>
          "name" : "role_jceks_password",<br>
          "value" : "cet3nrl181jn3m9wt9ks1eew"<br>
        } ]<br>
      }<br>
    }, {<br>
      "name" : "mgmt-EVENTSERVER-6d4b72313ca639207efafcd082d1e8e3",<br>
      "type" : "EVENTSERVER",<br>
      "hostRef" : {<br>
        "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"<br>
      },<br>
      "config" : {<br>
        "items" : [ {<br>
          "name" : "role_jceks_password",<br>
          "value" : "6xv9xg0dqz2s0e49ndg7ix8t1"<br>
        } ]<br>
      }<br>
    }, {<br>
      "name" : "mgmt-HOSTMONITOR-6d4b72313ca639207efafcd082d1e8e3",<br>
      "type" : "HOSTMONITOR",<br>
      "hostRef" : {<br>
        "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"<br>
      },<br>
      "config" : {<br>
        "items" : [ {<br>
          "name" : "role_jceks_password",<br>
          "value" : "2csaxisvujqksob2af2l176hb"<br>
        } ]<br>
      }<br>
    }, {<br>
      "name" : "mgmt-REPORTSMANAGER-6d4b72313ca639207efafcd082d1e8e3",<br>
      "type" : "REPORTSMANAGER",<br>
      "hostRef" : {<br>
        "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"<br>
      },<br>
      "config" : {<br>
        "items" : [ {<br>
          "name" : "role_jceks_password",<br>
          "value" : "8mg5vjuffwuhrap5gb94uehbb"<br>
        } ]<br>
      }<br>
    }, {<br>
      "name" : "mgmt-SERVICEMONITOR-6d4b72313ca639207efafcd082d1e8e3",<br>
      "type" : "SERVICEMONITOR",<br>
      "hostRef" : {<br>
        "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"<br>
      },<br>
      "config" : {<br>
        "items" : [ {<br>
          "name" : "role_jceks_password",<br>
          "value" : "d0yit74p3ge9bk6rebvxq1sgy"<br>
        } ]<br>
      }<br>
    } ],<br>
    "displayName" : "Cloudera Management Service"<br>
  },<br>
  "managerSettings" : {<br>
    "items" : [ {<br>
      "name" : "AD_USE_SIMPLE_AUTH",<br>
      "value" : "false"<br>
    }, {<br>
      "name" : "CLUSTER_STATS_START",<br>
      "value" : "10/23/2012 7:20"<br>
    }, {<br>
      "name" : "KDC_ADMIN_PASSWORD",<br>
      "value" : "BQIAAAA/AAEADFJBS0VOSERQLkNPTQAMY2xvdWRlcmEtc2NtAAAAAVofDAcBABcAEOiX/BhZDvIkN04fZL/YVbUAAAAB"<br>
    }, {<br>
      "name" : "KDC_ADMIN_USER",<br>
      "value" : "cloudera-scm@RAKENHDP.COM"<br>
    }, {<br>
      "name" : "KDC_HOST",<br>
      "value" : "stdalonejq.northcentralus.cloudapp.azure.com"<br>
    }, {<br>
      "name" : "KRB_ENC_TYPES",<br>
      "value" : "arcfour-hmac"<br>
    }, {<br>
      "name" : "KRB_MANAGE_KRB5_CONF",<br>
      "value" : "true"<br>
    }, {<br>
      "name" : "MAX_RENEW_LIFE",<br>
      "value" : "604800"<br>
    }, {<br>
      "name" : "PUBLIC_CLOUD_STATUS",<br>
      "value" : "NOT_ON_PUBLIC_CLOUD"<br>
    }, {<br>
      "name" : "REMOTE_PARCEL_REPO_URLS",<br>
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,http://10.0.0.4:8000,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/"<br>
    }, {<br>
      "name" : "SECURITY_REALM",<br>
      "value" : "RAKENHDP.COM"<br>
    } ]<br>
  }<br>
}<br>