```
{
  "timestamp" : "2017-05-03T11:31:54.443Z",
  "clusters" : [ {
    "name" : "idiotek",
    "version" : "CDH5",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HIVEMETASTORE",
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "751828992"
          } ]
        }, {
          "roleType" : "HIVESERVER2",
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "1610612736"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "1984901939"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "334"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "ip-172-31-10-189"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "Hive4#sebc"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-03d57ed8122e3fe4d8a37b86d27e4790",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-03d36711045309233"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-0e531dbdcf20f47272f591972b5c4a14",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-08454d9d1e8134e76"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-6f1d0e131507241a3823727fa85c07bb",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-0aced0f2b7544a4bc"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-a3d2ce38c7cd8dfeabf9888444e1ff66",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-061d6b74a4bc73dd1"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-bb5a5ad83a834dbb38f237a6f06ce741",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-0d2420c5a3a883b92"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-03d57ed8122e3fe4d8a37b86d27e4790",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "i-03d36711045309233"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8t1aab7etsra84b44vn0lxi1h"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-6f1d0e131507241a3823727fa85c07bb",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "i-0aced0f2b7544a4bc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dnjr6cuov2o96uxq674icc4t3"
          } ]
        }
      } ],
      "displayName" : "Hive"
    }, {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "SERVER",
          "items" : [ {
            "name" : "zookeeper_server_java_heapsize",
            "value" : "805306368"
          } ]
        } ],
        "items" : [ ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-0e531dbdcf20f47272f591972b5c4a14",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-08454d9d1e8134e76"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6b8v45p2ylw31vrayot6w31aw"
          }, {
            "name" : "serverId",
            "value" : "2"
          }, {
            "name" : "zookeeper_server_java_heapsize",
            "value" : "805306368"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-6f1d0e131507241a3823727fa85c07bb",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-0aced0f2b7544a4bc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "e33gw56dpclgag7inylfxcx1c"
          }, {
            "name" : "serverId",
            "value" : "3"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-bb5a5ad83a834dbb38f237a6f06ce741",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-0d2420c5a3a883b92"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "9x6qudwiaq0u66bchjuh2gw6k"
          }, {
            "name" : "serverId",
            "value" : "1"
          } ]
        }
      } ],
      "displayName" : "ZooKeeper"
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ {
          "name" : "database_host",
          "value" : "ip-172-31-10-189"
        }, {
          "name" : "database_password",
          "value" : "Hue4#sebc"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-HTTPFS-bb5a5ad83a834dbb38f237a6f06ce741"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-03d57ed8122e3fe4d8a37b86d27e4790",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "i-03d36711045309233"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "c2nyofnkzbm5m67y71gjs4980"
          }, {
            "name" : "secret_key",
            "value" : "dA8Sq6dHnABtVCtadBTH5VRGg6jYU3"
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
            "value" : "ip-172-31-10-189"
          }, {
            "name" : "oozie_database_password",
            "value" : "Oozie4#sebc"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie"
          }, {
            "name" : "oozie_java_heapsize",
            "value" : "751828992"
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
        "name" : "oozie-OOZIE_SERVER-03d57ed8122e3fe4d8a37b86d27e4790",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "i-03d36711045309233"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "93k76hw5dtisn4ytt65de9er5"
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
            "value" : "8"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "2"
          } ]
        }, {
          "roleType" : "JOBHISTORY",
          "items" : [ {
            "name" : "mr2_jobhistory_java_heapsize",
            "value" : "805306368"
          }, {
            "name" : "rm_io_weight",
            "value" : "1000"
          } ]
        }, {
          "roleType" : "NODEMANAGER",
          "items" : [ {
            "name" : "node_manager_java_heapsize",
            "value" : "805306368"
          }, {
            "name" : "rm_io_weight",
            "value" : "1000"
          }, {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "3"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "1024"
          } ]
        }, {
          "roleType" : "RESOURCEMANAGER",
          "items" : [ {
            "name" : "resource_manager_java_heapsize",
            "value" : "805306368"
          }, {
            "name" : "rm_io_weight",
            "value" : "1000"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "4096"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "3"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "true"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "90"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "OGf6vLHdATpykjwekiqnUWkwPTc4ta"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-a3d2ce38c7cd8dfeabf9888444e1ff66",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "i-061d6b74a4bc73dd1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4znbg383xwx5u7z1j81d5ris8"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-0e531dbdcf20f47272f591972b5c4a14",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-08454d9d1e8134e76"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "92iseat6z06w985kogex2x3zw"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "1024"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-6f1d0e131507241a3823727fa85c07bb",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-0aced0f2b7544a4bc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2m5y0a2of0vuerjgzg08ky3y6"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-a3d2ce38c7cd8dfeabf9888444e1ff66",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-061d6b74a4bc73dd1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "uni9vg3yfoiwyr2qxm7sqq7d"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-bb5a5ad83a834dbb38f237a6f06ce741",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-0d2420c5a3a883b92"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ut6kmyo8w09byzcu15fy0tw4"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-a3d2ce38c7cd8dfeabf9888444e1ff66",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "i-061d6b74a4bc73dd1"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "55"
          }, {
            "name" : "role_jceks_password",
            "value" : "8qpyache5rswiinvzc438yr1d"
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
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "4214154854"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "1073741824"
          }, {
            "name" : "rm_io_weight",
            "value" : "1000"
          } ]
        }, {
          "roleType" : "FAILOVERCONTROLLER",
          "items" : [ {
            "name" : "rm_io_weight",
            "value" : "1000"
          } ]
        }, {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }, {
          "roleType" : "HTTPFS",
          "items" : [ {
            "name" : "rm_io_weight",
            "value" : "1000"
          } ]
        }, {
          "roleType" : "JOURNALNODE",
          "items" : [ {
            "name" : "dfs_journalnode_edits_dir",
            "value" : "/dfs/jn"
          }, {
            "name" : "rm_io_weight",
            "value" : "1000"
          } ]
        }, {
          "roleType" : "NAMENODE",
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/dfs/nn"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          }, {
            "name" : "namenode_java_heapsize",
            "value" : "2684354560"
          }, {
            "name" : "rm_io_weight",
            "value" : "1000"
          }, {
            "name" : "role_config_suppression_namenode_java_heapsize_minimum_validator",
            "value" : "true"
          } ]
        }, {
          "roleType" : "NFSGATEWAY",
          "items" : [ {
            "name" : "rm_io_weight",
            "value" : "1000"
          } ]
        }, {
          "roleType" : "SECONDARYNAMENODE",
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/dfs/snn"
          }, {
            "name" : "rm_io_weight",
            "value" : "1000"
          }, {
            "name" : "secondary_namenode_java_heapsize",
            "value" : "2684354560"
          } ]
        } ],
        "items" : [ {
          "name" : "core_site_safety_valve",
          "value" : ""
        }, {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "9TJJMrBhuW6zReeGCELTlhIshapOif"
        }, {
          "name" : "dfs_ha_fencing_methods",
          "value" : "shell(true)"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "eF8l6hXSesbOcpKwSvqi5onFuPTyOB"
        }, {
          "name" : "hdfs_service_config_safety_valve",
          "value" : ""
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "iTmWTWqvzWUG18vqSUohV24ukR4qgs"
        }, {
          "name" : "rm_dirty",
          "value" : "true"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "10"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-bb5a5ad83a834dbb38f237a6f06ce741",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "i-0d2420c5a3a883b92"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-0e531dbdcf20f47272f591972b5c4a14",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-08454d9d1e8134e76"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dby7o7ly7vhlduw6dnobazqa0"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-6f1d0e131507241a3823727fa85c07bb",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-0aced0f2b7544a4bc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4ifrhhkajghnvhsyf7kdf8irh"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-a3d2ce38c7cd8dfeabf9888444e1ff66",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-061d6b74a4bc73dd1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7i0a0dvwelx0j1g1mrzgivf89"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-bb5a5ad83a834dbb38f237a6f06ce741",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-0d2420c5a3a883b92"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "75etckkhzl0hlludkibeul9pl"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-6f1d0e131507241a3823727fa85c07bb",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "i-0aced0f2b7544a4bc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "cnbrfm3gv5dvjyuc5g125ojy3"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-a3d2ce38c7cd8dfeabf9888444e1ff66",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "i-061d6b74a4bc73dd1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "607yq3eq7vs9prbfsjbywfbjs"
          } ]
        }
      }, {
        "name" : "hdfs-HTTPFS-bb5a5ad83a834dbb38f237a6f06ce741",
        "type" : "HTTPFS",
        "hostRef" : {
          "hostId" : "i-0d2420c5a3a883b92"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6cvwc2e03xai6qxt1pwwj463e"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-0e531dbdcf20f47272f591972b5c4a14",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "i-08454d9d1e8134e76"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ay7jp2ysd7lhjmengctry9tc0"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-6f1d0e131507241a3823727fa85c07bb",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "i-0aced0f2b7544a4bc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8z41odn2fsksfehwand85ipnw"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-bb5a5ad83a834dbb38f237a6f06ce741",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "i-0d2420c5a3a883b92"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "rl0dixcy00xyoymvh4f3rnqs"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-6f1d0e131507241a3823727fa85c07bb",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "i-0aced0f2b7544a4bc"
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
            "value" : "71"
          }, {
            "name" : "role_jceks_password",
            "value" : "3ihaos0fv4p5am4j239hnddjz"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-a3d2ce38c7cd8dfeabf9888444e1ff66",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "i-061d6b74a4bc73dd1"
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
            "value" : "57"
          }, {
            "name" : "role_jceks_password",
            "value" : "bryml8y4wu1lji1mp8g9l3b86"
          } ]
        }
      } ],
      "displayName" : "HDFS"
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "i-03d36711045309233",
    "ipAddress" : "172.31.10.189",
    "hostname" : "ip-172-31-10-189",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-0d2420c5a3a883b92",
    "ipAddress" : "172.31.10.43",
    "hostname" : "ip-172-31-10-43",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-061d6b74a4bc73dd1",
    "ipAddress" : "172.31.2.85",
    "hostname" : "ip-172-31-2-85",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-0aced0f2b7544a4bc",
    "ipAddress" : "172.31.4.126",
    "hostname" : "ip-172-31-4-126",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-08454d9d1e8134e76",
    "ipAddress" : "172.31.8.175",
    "hostname" : "ip-172-31-8-175",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__mgmt-ACTIVITYMONITOR-03d57ed8122e3fe4d8a37b86d27e4790",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "d067aa710bc3d960da86dd90ce00bb56af8619e00f1db120ad482ba1070c8b28",
    "pwSalt" : 8055494862672910416,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-03d57ed8122e3fe4d8a37b86d27e4790",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "5fec7d5275a098585ac3548c9055f80e0d3f1f33e480104626af62ee17aaf61f",
    "pwSalt" : 5652443883862000645,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-03d57ed8122e3fe4d8a37b86d27e4790",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "30716aab907aab3f96a3d4afdf7ededf914251688c738f36fe7689054411c524",
    "pwSalt" : 61849955374674558,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-03d57ed8122e3fe4d8a37b86d27e4790",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "af553649c1e8c5b3fb2e2eea210360f9fb5265930a9c9ccd259635e4246e7d87",
    "pwSalt" : -2847700613490500727,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-03d57ed8122e3fe4d8a37b86d27e4790",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "7677d2ff0c820dc0c3a981a7f491cae4d733be1ff68e0a900eee5e6da2a27e3b",
    "pwSalt" : 5328536688085251204,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ],
    "pwHash" : "29f23e19218b46b17ded2b17760511513ac7409c3c92d6ef20a210de50461abf",
    "pwSalt" : -5770631828510973467,
    "pwLogin" : true
  }, {
    "name" : "idiotek",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "e3152ffdbe705646327d1409d08b8f341cf7fb1249c7ad5bbed527df430d8fec",
    "pwSalt" : -7437667702113534211,
    "pwLogin" : true
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ],
    "pwHash" : "292447af86f6fc93fc3f9de52a8ee162c6aedeedc7e2ccffc73b2b2f29b88357",
    "pwSalt" : 9151422805925883589,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.9.2",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20170330-1814",
    "gitHash" : "822da28bff818f57fc1bfc3eafe3a550300ef1b0",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "roleTypeConfigs" : [ {
        "roleType" : "ACTIVITYMONITOR",
        "items" : [ {
          "name" : "firehose_database_host",
          "value" : "ip-172-31-10-189"
        }, {
          "name" : "firehose_database_name",
          "value" : "amon"
        }, {
          "name" : "firehose_database_password",
          "value" : "Amon4#sebc"
        }, {
          "name" : "firehose_database_user",
          "value" : "amon"
        }, {
          "name" : "rm_io_weight",
          "value" : "1000"
        } ]
      }, {
        "roleType" : "ALERTPUBLISHER",
        "items" : [ {
          "name" : "alert_heapsize",
          "value" : "201326592"
        }, {
          "name" : "rm_io_weight",
          "value" : "1000"
        } ]
      }, {
        "roleType" : "EVENTSERVER",
        "items" : [ {
          "name" : "event_server_heapsize",
          "value" : "1023410176"
        }, {
          "name" : "rm_io_weight",
          "value" : "1000"
        } ]
      }, {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1610612736"
        }, {
          "name" : "rm_io_weight",
          "value" : "1000"
        } ]
      }, {
        "roleType" : "NAVIGATOR",
        "items" : [ {
          "name" : "rm_io_weight",
          "value" : "1000"
        } ]
      }, {
        "roleType" : "NAVIGATORMETASERVER",
        "items" : [ {
          "name" : "rm_io_weight",
          "value" : "1000"
        } ]
      }, {
        "roleType" : "REPORTSMANAGER",
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "ip-172-31-10-189"
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_password",
          "value" : "Rman4#sebc"
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman"
        }, {
          "name" : "headlamp_heapsize",
          "value" : "1023410176"
        }, {
          "name" : "rm_io_weight",
          "value" : "1000"
        } ]
      }, {
        "roleType" : "SERVICEMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1610612736"
        }, {
          "name" : "rm_io_weight",
          "value" : "1000"
        } ]
      } ],
      "items" : [ {
        "name" : "rm_dirty",
        "value" : "true"
      } ]
    },
    "roles" : [ {
      "name" : "mgmt-ACTIVITYMONITOR-03d57ed8122e3fe4d8a37b86d27e4790",
      "type" : "ACTIVITYMONITOR",
      "hostRef" : {
        "hostId" : "i-03d36711045309233"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "57z5ajsm2eq6kfodjoatmlg86"
        } ]
      }
    }, {
      "name" : "mgmt-ALERTPUBLISHER-03d57ed8122e3fe4d8a37b86d27e4790",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "i-03d36711045309233"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "9cx30irgfwwbfwdvnj602n4zp"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-03d57ed8122e3fe4d8a37b86d27e4790",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "i-03d36711045309233"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "eh9xa1c5x13xob9wfhl9dal7q"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-03d57ed8122e3fe4d8a37b86d27e4790",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "i-03d36711045309233"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "cxdqjuzo91sdphbiqekqxu4vm"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-03d57ed8122e3fe4d8a37b86d27e4790",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "i-03d36711045309233"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "eu441o255fg1333mql7gq2epn"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-03d57ed8122e3fe4d8a37b86d27e4790",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "i-03d36711045309233"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "dt2krvgohod5ogvadinfzuwjo"
        } ]
      }
    } ],
    "displayName" : "Cloudera Management Service"
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/26/2012 3:40"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/,http://ip-172-31-8-175/cdh5.9.2/,http://ip-172-31-8-175/spark2/,http://ip-172-31-8-175/gplextras5/,http://ip-172-31-8-175/accumulo-c5/,http://ip-172-31-8-175/cdh5.11.0/"
    } ]
  }
}
```
