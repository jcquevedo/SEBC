{
  "timestamp" : "2017-11-30T17:01:53.643Z",
  "clusters" : [ {
    "name" : "jcquevedo",
    "version" : "CDH5",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HIVEMETASTORE",
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "6026166272"
          }, {
            "name" : "hive_metastore_server_max_message_size",
            "value" : "602616627"
          } ]
        }, {
          "roleType" : "HIVESERVER2",
          "items" : [ {
            "name" : "hiveserver2_enable_impersonation",
            "value" : "false"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "4801377075"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "808"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "stdalonejq.northcentralus.cloudapp.azure.com"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "Raken.2017"
        }, {
          "name" : "hive_proxy_user_groups_list",
          "value" : "hue,hive,sentry"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "sentry_service",
          "value" : "sentry"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-0606538f948d493a297260707d78d635",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "781ae094-3759-4653-8657-da3682878391"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-193d65d588027c655cefab96da5feb37",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "7dae7d03-866d-4638-877a-39de4cfb5485"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-54de5a68a1c4c7dc1cd2ef6ecbbec893",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "2182c8eb-e19d-447d-a9e9-df43e23bfbb2"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-6d4b72313ca639207efafcd082d1e8e3",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-54de5a68a1c4c7dc1cd2ef6ecbbec893",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "2182c8eb-e19d-447d-a9e9-df43e23bfbb2"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6obfyr7rxhrdp959x40smaa78"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-54de5a68a1c4c7dc1cd2ef6ecbbec893",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "2182c8eb-e19d-447d-a9e9-df43e23bfbb2"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ej8bthvr041xkyzl7599o3svn"
          } ]
        }
      } ],
      "displayName" : "Hive"
    }, {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ {
          "name" : "enableSecurity",
          "value" : "true"
        } ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-0606538f948d493a297260707d78d635",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "781ae094-3759-4653-8657-da3682878391"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "e0g3hn04si9hjy890727xc675"
          }, {
            "name" : "serverId",
            "value" : "1"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-193d65d588027c655cefab96da5feb37",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "7dae7d03-866d-4638-877a-39de4cfb5485"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8y66mhza4cxtkfuxsrvahtojt"
          }, {
            "name" : "serverId",
            "value" : "2"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-6d4b72313ca639207efafcd082d1e8e3",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "fjce7txnjx0uh227hlxl3lg9"
          }, {
            "name" : "serverId",
            "value" : "3"
          } ]
        }
      } ],
      "displayName" : "ZooKeeper"
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HUE_SERVER",
          "items" : [ {
            "name" : "hue_server_bind_wildcard",
            "value" : "true"
          } ]
        } ],
        "items" : [ {
          "name" : "database_host",
          "value" : "stdalonejq.northcentralus.cloudapp.azure.com"
        }, {
          "name" : "database_password",
          "value" : "Raken.2017"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-NAMENODE-6d4b72313ca639207efafcd082d1e8e3"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "sentry_service",
          "value" : "sentry"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-193d65d588027c655cefab96da5feb37",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "7dae7d03-866d-4638-877a-39de4cfb5485"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2qln5lg0imc2sf9j9k0qpiy1v"
          }, {
            "name" : "secret_key",
            "value" : "OQBNFBaE0UUjDPDQ425j2ZyKgpjAZz"
          } ]
        }
      }, {
        "name" : "hue-KT_RENEWER-193d65d588027c655cefab96da5feb37",
        "type" : "KT_RENEWER",
        "hostRef" : {
          "hostId" : "7dae7d03-866d-4638-877a-39de4cfb5485"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "aeghmmvszbanxayrueon0fpeg"
          } ]
        }
      } ],
      "displayName" : "Hue"
    }, {
      "name" : "oozie",
      "type" : "OOZIE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "OOZIE_SERVER",
          "items" : [ {
            "name" : "oozie_database_host",
            "value" : "stdalonejq.northcentralus.cloudapp.azure.com"
          }, {
            "name" : "oozie_database_password",
            "value" : "Raken.2017"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-54de5a68a1c4c7dc1cd2ef6ecbbec893",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "2182c8eb-e19d-447d-a9e9-df43e23bfbb2"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "arf21j4n8lz7yaelq9vs7ddmw"
          } ]
        }
      } ],
      "displayName" : "Oozie"
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "mapred_reduce_tasks",
            "value" : "12"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "1"
          } ]
        }, {
          "roleType" : "NODEMANAGER",
          "items" : [ {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/mnt/resource/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/mnt/resource/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "9776"
          } ]
        }, {
          "roleType" : "RESOURCEMANAGER",
          "items" : [ {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "16508"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "6"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "80"
        }, {
          "name" : "yarn_service_cgroups",
          "value" : "false"
        }, {
          "name" : "yarn_service_lce_always",
          "value" : "false"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "TaNWXESFPc0T3S3r7qOYNkqtkIoqMD"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-6d4b72313ca639207efafcd082d1e8e3",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "23uocofb173wjanjoyqm1io7h"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-0606538f948d493a297260707d78d635",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "781ae094-3759-4653-8657-da3682878391"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4ij5z8fghfch9sml2rn5545rn"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-193d65d588027c655cefab96da5feb37",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "7dae7d03-866d-4638-877a-39de4cfb5485"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "46se3znplz3uo20ainzmcjouj"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-54de5a68a1c4c7dc1cd2ef6ecbbec893",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "2182c8eb-e19d-447d-a9e9-df43e23bfbb2"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "9acxvsmc5u0qap8ozah3zgckz"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-0606538f948d493a297260707d78d635",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "781ae094-3759-4653-8657-da3682878391"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "48"
          }, {
            "name" : "role_jceks_password",
            "value" : "x330b5qfv1y8ase42x59hspw"
          } ]
        }
      } ],
      "displayName" : "YARN (MR2 Included)"
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "DATANODE",
          "items" : [ {
            "name" : "datanode_java_heapsize",
            "value" : "1073741824"
          }, {
            "name" : "dfs_data_dir_list",
            "value" : "/mnt/resource/dfs/dn"
          }, {
            "name" : "dfs_datanode_data_dir_perm",
            "value" : "700"
          }, {
            "name" : "dfs_datanode_http_port",
            "value" : "1006"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "4294967296"
          }, {
            "name" : "dfs_datanode_port",
            "value" : "1004"
          }, {
            "name" : "rm_cpu_shares",
            "value" : "400"
          }, {
            "name" : "rm_io_weight",
            "value" : "200"
          } ]
        }, {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }, {
          "roleType" : "JOURNALNODE",
          "items" : [ {
            "name" : "dfs_journalnode_edits_dir",
            "value" : "/mnt/resource/jn"
          } ]
        }, {
          "roleType" : "NAMENODE",
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/mnt/resource/dfs/nn"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          } ]
        }, {
          "roleType" : "SECONDARYNAMENODE",
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/mnt/resource/dfs/snn"
          } ]
        } ],
        "items" : [ {
          "name" : "dfs_encrypt_data_transfer_algorithm",
          "value" : "AES/CTR/NoPadding"
        }, {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "psPgnRB4dbjeJpBZhTaJbGdRP4gNBr"
        }, {
          "name" : "dfs_ha_fencing_methods",
          "value" : "shell(true)"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "x96bchl3ePMfWat4NrRM5xezJnc0Up"
        }, {
          "name" : "hadoop_security_authentication",
          "value" : "kerberos"
        }, {
          "name" : "hadoop_security_authorization",
          "value" : "true"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "JVYcQJ2wg1bwsb7nu6qYE7e7BE1nMz"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "20"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-6d4b72313ca639207efafcd082d1e8e3",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-0606538f948d493a297260707d78d635",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "781ae094-3759-4653-8657-da3682878391"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dzx6qjxsgqw0jfc1kcuo2d5ax"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-193d65d588027c655cefab96da5feb37",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "7dae7d03-866d-4638-877a-39de4cfb5485"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7hjxk493wqq0bl1y8yx0hcetb"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-54de5a68a1c4c7dc1cd2ef6ecbbec893",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "2182c8eb-e19d-447d-a9e9-df43e23bfbb2"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ad7tnhsencafgenxp5jhf6px8"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-0606538f948d493a297260707d78d635",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "781ae094-3759-4653-8657-da3682878391"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "fnwmfhz6wsypg92liq1sx3rh"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-6d4b72313ca639207efafcd082d1e8e3",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6m0n5pxbqn1ucjojni2nq688t"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-0606538f948d493a297260707d78d635",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "781ae094-3759-4653-8657-da3682878391"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "3gtaxlxozpf7s388p3xqnyn1m"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-193d65d588027c655cefab96da5feb37",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "7dae7d03-866d-4638-877a-39de4cfb5485"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "3e5tw39akxnzwmop3tqrx35i"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-54de5a68a1c4c7dc1cd2ef6ecbbec893",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "2182c8eb-e19d-447d-a9e9-df43e23bfbb2"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2usxwux0gf7ruwm6g8bnov9hp"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-0606538f948d493a297260707d78d635",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "781ae094-3759-4653-8657-da3682878391"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservice1"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservice1"
          }, {
            "name" : "namenode_id",
            "value" : "55"
          }, {
            "name" : "role_jceks_password",
            "value" : "386n30s8a0uelr8ktce5j5vy8"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-6d4b72313ca639207efafcd082d1e8e3",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservice1"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservice1"
          }, {
            "name" : "namenode_id",
            "value" : "50"
          }, {
            "name" : "role_jceks_password",
            "value" : "5jdydp0hq46hago6la27xeps4"
          } ]
        }
      } ],
      "displayName" : "HDFS"
    }, {
      "name" : "sentry",
      "type" : "SENTRY",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "SENTRY_SERVER",
          "items" : [ {
            "name" : "sentry_server_java_heapsize",
            "value" : "268435456"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "sentry_server_database_host",
          "value" : "stdalonejq.northcentralus.cloudapp.azure.com"
        }, {
          "name" : "sentry_server_database_password",
          "value" : "Raken.2017"
        }, {
          "name" : "sentry_service_admin_group",
          "value" : "hive,impala,hue,solr,kafka,jcquevedo"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "sentry-GATEWAY-0606538f948d493a297260707d78d635",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "781ae094-3759-4653-8657-da3682878391"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "sentry-GATEWAY-193d65d588027c655cefab96da5feb37",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "7dae7d03-866d-4638-877a-39de4cfb5485"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "sentry-GATEWAY-54de5a68a1c4c7dc1cd2ef6ecbbec893",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "2182c8eb-e19d-447d-a9e9-df43e23bfbb2"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "sentry-GATEWAY-6d4b72313ca639207efafcd082d1e8e3",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "sentry-SENTRY_SERVER-54de5a68a1c4c7dc1cd2ef6ecbbec893",
        "type" : "SENTRY_SERVER",
        "hostRef" : {
          "hostId" : "2182c8eb-e19d-447d-a9e9-df43e23bfbb2"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "40264zvmf260zh8lvnzivq2xt"
          } ]
        }
      } ],
      "displayName" : "Sentry"
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f",
    "ipAddress" : "10.0.0.5",
    "hostname" : "hdp1.northcentralus.cloudapp.azure.com",
    "rackId" : "/default",
    "config" : {
      "items" : [ {
        "name" : "memory_overcommit_threshold",
        "value" : "0.95"
      } ]
    }
  }, {
    "hostId" : "781ae094-3759-4653-8657-da3682878391",
    "ipAddress" : "10.0.0.6",
    "hostname" : "hdp2.northcentralus.cloudapp.azure.com",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "7dae7d03-866d-4638-877a-39de4cfb5485",
    "ipAddress" : "10.0.0.7",
    "hostname" : "hdp3.northcentralus.cloudapp.azure.com",
    "rackId" : "/default",
    "config" : {
      "items" : [ {
        "name" : "memory_overcommit_threshold",
        "value" : "0.95"
      } ]
    }
  }, {
    "hostId" : "2182c8eb-e19d-447d-a9e9-df43e23bfbb2",
    "ipAddress" : "10.0.0.8",
    "hostname" : "hdp4.northcentralus.cloudapp.azure.com",
    "rackId" : "/default",
    "config" : {
      "items" : [ {
        "name" : "memory_overcommit_threshold",
        "value" : "0.95"
      } ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-6d4b72313ca639207efafcd082d1e8e3",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "eaf44f9462f0df27b384881ce7777eaf671ea3b9ad05f65ea79ec8db498b34da",
    "pwSalt" : -2373169864744697506,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-6d4b72313ca639207efafcd082d1e8e3",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "342e197e0134af3be5316a8b53094b78af8baca3f685247ef166bc51d8aa696c",
    "pwSalt" : 5631694952982674857,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-6d4b72313ca639207efafcd082d1e8e3",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "43b676be9be44dad70ed5afdbaae307c26e1d76d6eea2e8c7a7c2dc7c31b7c7b",
    "pwSalt" : -8632549585653729165,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-6d4b72313ca639207efafcd082d1e8e3",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "14fde2e9e5545c499f2e6273fb622d6ef3af04238b767a14132e02b98fa7a1ba",
    "pwSalt" : -457909825541318944,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ],
    "pwHash" : "73b73e3b3595b358ece1d5399cd95249d7995f809a8e2e8ca40aba131ca1e244",
    "pwSalt" : -3249067716897620933,
    "pwLogin" : true
  }, {
    "name" : "jcquevedo",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "fddf0f92bacd3dcd1411cb3e5da5d9088342b8de24dcfa0aebe62681fdee802c",
    "pwSalt" : -4047757178806164821,
    "pwLogin" : true
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ],
    "pwHash" : "ae2265528c30d1353723af45dddb2d8294532904c14d51fca3f18204af2a73c7",
    "pwSalt" : -8523854381113412111,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.9.1",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20170112-1158",
    "gitHash" : "a66d8bbdbe8bc3ee54235e55423f2f76c7d9f3b1",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "roleTypeConfigs" : [ {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1610612736"
        } ]
      }, {
        "roleType" : "REPORTSMANAGER",
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "stdalonejq.northcentralus.cloudapp.azure.com"
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_password",
          "value" : "Raken.2017"
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman"
        } ]
      }, {
        "roleType" : "SERVICEMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1610612736"
        } ]
      } ],
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ALERTPUBLISHER-6d4b72313ca639207efafcd082d1e8e3",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "cet3nrl181jn3m9wt9ks1eew"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-6d4b72313ca639207efafcd082d1e8e3",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "6xv9xg0dqz2s0e49ndg7ix8t1"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-6d4b72313ca639207efafcd082d1e8e3",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "2csaxisvujqksob2af2l176hb"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-6d4b72313ca639207efafcd082d1e8e3",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "8mg5vjuffwuhrap5gb94uehbb"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-6d4b72313ca639207efafcd082d1e8e3",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "fccd90f8-c88e-4418-87fe-75b386b77c7f"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "d0yit74p3ge9bk6rebvxq1sgy"
        } ]
      }
    } ],
    "displayName" : "Cloudera Management Service"
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "AD_USE_SIMPLE_AUTH",
      "value" : "false"
    }, {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/23/2012 7:20"
    }, {
      "name" : "KDC_ADMIN_PASSWORD",
      "value" : "BQIAAAA/AAEADFJBS0VOSERQLkNPTQAMY2xvdWRlcmEtc2NtAAAAAVofDAcBABcAEOiX/BhZDvIkN04fZL/YVbUAAAAB"
    }, {
      "name" : "KDC_ADMIN_USER",
      "value" : "cloudera-scm@RAKENHDP.COM"
    }, {
      "name" : "KDC_HOST",
      "value" : "stdalonejq.northcentralus.cloudapp.azure.com"
    }, {
      "name" : "KRB_ENC_TYPES",
      "value" : "arcfour-hmac"
    }, {
      "name" : "KRB_MANAGE_KRB5_CONF",
      "value" : "true"
    }, {
      "name" : "MAX_RENEW_LIFE",
      "value" : "604800"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "NOT_ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,http://10.0.0.4:8000,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/"
    }, {
      "name" : "SECURITY_REALM",
      "value" : "RAKENHDP.COM"
    } ]
  }
}