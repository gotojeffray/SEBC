~~~
{
  "timestamp" : "2016-12-07T03:06:05.536Z",
  "clusters" : [ {
    "name" : "cluster",
    "displayName" : "gotojeffray",
    "version" : "CDH5",
    "fullVersion" : "5.8.3",
    "services" : [ {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "items" : [ ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-2080bdf39ad661ad2eeb435d02b45b98",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "4cf8f637-04c4-48de-bbfa-12faeb6f3379"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5tzs7pryxdur06jl0sf13lzct"
          }, {
            "name" : "serverId",
            "value" : "3"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "zookeeper-SERVER-BASE"
        }
      }, {
        "name" : "zookeeper-SERVER-2882409f66e1c9c5a02b2541d83f9583",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "f21abc82-ebf5-45ee-ba35-1a0d9a6603bc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "9xpkok2lz0lcwy0dbw65y8mw2"
          }, {
            "name" : "serverId",
            "value" : "1"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "zookeeper-SERVER-BASE"
        }
      }, {
        "name" : "zookeeper-SERVER-a3ae9015797700bf4903b8d0a1f4dba5",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "382b1c6c-67bf-4067-b8bb-fdedfa8d192e"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "9b76opxkl2bn52dr35u8zj7o2"
          }, {
            "name" : "serverId",
            "value" : "2"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "zookeeper-SERVER-BASE"
        }
      } ],
      "displayName" : "ZooKeeper",
      "roleConfigGroups" : [ {
        "name" : "zookeeper-SERVER-BASE",
        "displayName" : "Server Default Group",
        "roleType" : "SERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "zookeeper"
        },
        "config" : {
          "items" : [ {
            "name" : "heap_dump_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "log_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":5368709120,\"critical\":5368709120}"
          }, {
            "name" : "zookeeper_server_data_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":5368709120,\"critical\":5368709120}"
          }, {
            "name" : "zookeeper_server_data_log_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":5368709120,\"critical\":5368709120}"
          }, {
            "name" : "zookeeper_server_java_heapsize",
            "value" : "763363328"
          } ]
        }
      } ]
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
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
          "name" : "yarn_service_cgroups",
          "value" : "false"
        }, {
          "name" : "yarn_service_lce_always",
          "value" : "false"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "i7X7LQovedylCG6NJnum2f0jTktmrb"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-GATEWAY-2080bdf39ad661ad2eeb435d02b45b98",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "4cf8f637-04c4-48de-bbfa-12faeb6f3379"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-GATEWAY-BASE"
        }
      }, {
        "name" : "yarn-GATEWAY-2882409f66e1c9c5a02b2541d83f9583",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "f21abc82-ebf5-45ee-ba35-1a0d9a6603bc"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-GATEWAY-BASE"
        }
      }, {
        "name" : "yarn-GATEWAY-5537dfd2b2c1891a3e5860ca2ae70ea9",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "557450b1-d1dd-41d9-9649-89f010bd1147"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-GATEWAY-BASE"
        }
      }, {
        "name" : "yarn-GATEWAY-a3ae9015797700bf4903b8d0a1f4dba5",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "382b1c6c-67bf-4067-b8bb-fdedfa8d192e"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-GATEWAY-BASE"
        }
      }, {
        "name" : "yarn-GATEWAY-f2373c0f7b73eec64dbc188eb4e7d42b",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "d7b8d6e4-d3ab-49ab-80ca-e0c006b45134"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-GATEWAY-BASE"
        }
      }, {
        "name" : "yarn-JOBHISTORY-2080bdf39ad661ad2eeb435d02b45b98",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "4cf8f637-04c4-48de-bbfa-12faeb6f3379"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1lgppbs2wsby083wumejbfk8h"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-JOBHISTORY-BASE"
        }
      }, {
        "name" : "yarn-NODEMANAGER-2882409f66e1c9c5a02b2541d83f9583",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "f21abc82-ebf5-45ee-ba35-1a0d9a6603bc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "esxn73apql2tmmd83oukqkaju"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-1"
        }
      }, {
        "name" : "yarn-NODEMANAGER-5537dfd2b2c1891a3e5860ca2ae70ea9",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "557450b1-d1dd-41d9-9649-89f010bd1147"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "eufyaryl8yoq7rqw02hlkz1di"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-BASE"
        }
      }, {
        "name" : "yarn-NODEMANAGER-f2373c0f7b73eec64dbc188eb4e7d42b",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "d7b8d6e4-d3ab-49ab-80ca-e0c006b45134"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "g7z6kpks6yfbvh339hroyr6n"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-BASE"
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-2080bdf39ad661ad2eeb435d02b45b98",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "4cf8f637-04c4-48de-bbfa-12faeb6f3379"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "50"
          }, {
            "name" : "role_jceks_password",
            "value" : "6fff5fctqu6plrgrbqgwf26og"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-RESOURCEMANAGER-BASE"
        }
      } ],
      "displayName" : "YARN (MR2 Included)",
      "roleConfigGroups" : [ {
        "name" : "yarn-GATEWAY-BASE",
        "displayName" : "Gateway Default Group",
        "roleType" : "GATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "mapred_reduce_tasks",
            "value" : "4"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "1"
          } ]
        }
      }, {
        "name" : "yarn-JOBHISTORY-BASE",
        "displayName" : "JobHistory Server Default Group",
        "roleType" : "JOBHISTORY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "heap_dump_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "log_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-1",
        "displayName" : "NodeManager Group 1",
        "roleType" : "NODEMANAGER",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "heap_dump_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "log_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "nodemanager_local_data_directories_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "nodemanager_log_directories_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "nodemanager_recovery_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
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
            "value" : "12288"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-BASE",
        "displayName" : "NodeManager Default Group",
        "roleType" : "NODEMANAGER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "heap_dump_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "log_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "nodemanager_local_data_directories_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "nodemanager_log_directories_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "nodemanager_recovery_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "rm_cpu_shares",
            "value" : "1800"
          }, {
            "name" : "rm_io_weight",
            "value" : "900"
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
            "value" : "12288"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-BASE",
        "displayName" : "ResourceManager Default Group",
        "roleType" : "RESOURCEMANAGER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "heap_dump_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "log_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "4939"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "3"
          } ]
        }
      } ]
    }, {
      "name" : "oozie",
      "type" : "OOZIE",
      "config" : {
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
        "name" : "oozie-OOZIE_SERVER-f2373c0f7b73eec64dbc188eb4e7d42b",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "d7b8d6e4-d3ab-49ab-80ca-e0c006b45134"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8eow422tf5sbmh6l4gupybu38"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "oozie-OOZIE_SERVER-BASE"
        }
      } ],
      "displayName" : "Oozie",
      "roleConfigGroups" : [ {
        "name" : "oozie-OOZIE_SERVER-BASE",
        "displayName" : "Oozie Server Default Group",
        "roleType" : "OOZIE_SERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "oozie"
        },
        "config" : {
          "items" : [ {
            "name" : "log_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":5368709120,\"critical\":5368709120}"
          }, {
            "name" : "oozie_database_host",
            "value" : "ip-172-31-3-200.ap-southeast-1.compute.internal"
          }, {
            "name" : "oozie_database_password",
            "value" : "oozie"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie"
          }, {
            "name" : "oozie_java_heapsize",
            "value" : "52428800"
          } ]
        }
      } ]
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "items" : [ {
          "name" : "database_host",
          "value" : "ip-172-31-3-200.ap-southeast-1.compute.internal"
        }, {
          "name" : "database_password",
          "value" : "hue"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-NAMENODE-a3ae9015797700bf4903b8d0a1f4dba5"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-f2373c0f7b73eec64dbc188eb4e7d42b",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "d7b8d6e4-d3ab-49ab-80ca-e0c006b45134"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2b6sj9djub5pn88e8b3uoir9"
          }, {
            "name" : "secret_key",
            "value" : "ete64S58xWOWa15rDsLUcaTXlDljpr"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hue-HUE_SERVER-BASE"
        }
      } ],
      "displayName" : "Hue",
      "roleConfigGroups" : [ {
        "name" : "hue-HUE_LOAD_BALANCER-BASE",
        "displayName" : "Load Balancer Default Group",
        "roleType" : "HUE_LOAD_BALANCER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hue"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hue-HUE_SERVER-BASE",
        "displayName" : "Hue Server Default Group",
        "roleType" : "HUE_SERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hue"
        },
        "config" : {
          "items" : [ {
            "name" : "log_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":5368709120,\"critical\":5368709120}"
          } ]
        }
      }, {
        "name" : "hue-KT_RENEWER-BASE",
        "displayName" : "Kerberos Ticket Renewer Default Group",
        "roleType" : "KT_RENEWER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hue"
        },
        "config" : {
          "items" : [ ]
        }
      } ]
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "items" : [ {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "zA8j0fxDmnJFmMZbtoe0sjVeuZmuLH"
        }, {
          "name" : "dfs_ha_fencing_methods",
          "value" : "shell(true)"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "ekosKQXhRySNKO5JZui0dhFhoV7Ep2"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "sLXdltEToZLihGnnpCNHXfBfIqlxi0"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "10"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-a3ae9015797700bf4903b8d0a1f4dba5",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "382b1c6c-67bf-4067-b8bb-fdedfa8d192e"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-BALANCER-BASE"
        }
      }, {
        "name" : "hdfs-DATANODE-2882409f66e1c9c5a02b2541d83f9583",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "f21abc82-ebf5-45ee-ba35-1a0d9a6603bc"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bvmrmqjvsrfmc9tmkfyuo4v48"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-1"
        }
      }, {
        "name" : "hdfs-DATANODE-5537dfd2b2c1891a3e5860ca2ae70ea9",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "557450b1-d1dd-41d9-9649-89f010bd1147"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "afijyuqnkmtgqgqy4jjyhrm6d"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-BASE"
        }
      }, {
        "name" : "hdfs-DATANODE-f2373c0f7b73eec64dbc188eb4e7d42b",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "d7b8d6e4-d3ab-49ab-80ca-e0c006b45134"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ez9w2r6vijt2ooh7166d7fgeh"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-BASE"
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-2080bdf39ad661ad2eeb435d02b45b98",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "4cf8f637-04c4-48de-bbfa-12faeb6f3379"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "89aqjoyn4qnpyenlt978dy8jw"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-FAILOVERCONTROLLER-BASE"
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-a3ae9015797700bf4903b8d0a1f4dba5",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "382b1c6c-67bf-4067-b8bb-fdedfa8d192e"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5g5mc47jd2sayx9hy4cccpiy1"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-FAILOVERCONTROLLER-BASE"
        }
      }, {
        "name" : "hdfs-HTTPFS-5537dfd2b2c1891a3e5860ca2ae70ea9",
        "type" : "HTTPFS",
        "hostRef" : {
          "hostId" : "557450b1-d1dd-41d9-9649-89f010bd1147"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8aqiajozthhzcdkdv0haspf5w"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-HTTPFS-BASE"
        }
      }, {
        "name" : "hdfs-JOURNALNODE-2080bdf39ad661ad2eeb435d02b45b98",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "4cf8f637-04c4-48de-bbfa-12faeb6f3379"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ednac7hun1e3r8q8wxyxz6ed4"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-JOURNALNODE-BASE"
        }
      }, {
        "name" : "hdfs-JOURNALNODE-a3ae9015797700bf4903b8d0a1f4dba5",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "382b1c6c-67bf-4067-b8bb-fdedfa8d192e"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "cozlnx068d1g44n8mr3dyxui2"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-JOURNALNODE-BASE"
        }
      }, {
        "name" : "hdfs-JOURNALNODE-f2373c0f7b73eec64dbc188eb4e7d42b",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "d7b8d6e4-d3ab-49ab-80ca-e0c006b45134"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bggoyqkk1gsrx9hwspggpnlen"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-JOURNALNODE-BASE"
        }
      }, {
        "name" : "hdfs-NAMENODE-2080bdf39ad661ad2eeb435d02b45b98",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "4cf8f637-04c4-48de-bbfa-12faeb6f3379"
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
            "value" : "115"
          }, {
            "name" : "role_jceks_password",
            "value" : "68b4fgwonxs4ted7kitnuanhr"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-NAMENODE-BASE"
        }
      }, {
        "name" : "hdfs-NAMENODE-a3ae9015797700bf4903b8d0a1f4dba5",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "382b1c6c-67bf-4067-b8bb-fdedfa8d192e"
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
            "value" : "52"
          }, {
            "name" : "role_jceks_password",
            "value" : "cgw6igsbmm69e76oey86opt1x"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-NAMENODE-BASE"
        }
      } ],
      "displayName" : "HDFS",
      "roleConfigGroups" : [ {
        "name" : "hdfs-BALANCER-BASE",
        "displayName" : "Balancer Default Group",
        "roleType" : "BALANCER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "balancer_java_heapsize",
            "value" : "763363328"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-1",
        "displayName" : "DataNode Group 1",
        "roleType" : "DATANODE",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "datanode_data_directories_free_space_absolute_thresholds",
            "value" : "{\"warning\":5368709120,\"critical\":5368709120}"
          }, {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn,/dfs/dn2"
          }, {
            "name" : "dfs_datanode_available_space_balanced_threshold",
            "value" : "6442450944"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "1716285030"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "4294967296"
          }, {
            "name" : "heap_dump_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "log_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-BASE",
        "displayName" : "DataNode Default Group",
        "roleType" : "DATANODE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "datanode_data_directories_free_space_absolute_thresholds",
            "value" : "{\"warning\":5368709120,\"critical\":5368709120}"
          }, {
            "name" : "datanode_java_heapsize",
            "value" : "1073741824"
          }, {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn,/dfs/dn2"
          }, {
            "name" : "dfs_datanode_available_space_balanced_threshold",
            "value" : "6442450944"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "1716285030"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "4294967296"
          }, {
            "name" : "heap_dump_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "log_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":5368709120,\"critical\":5368709120}"
          }, {
            "name" : "rm_cpu_shares",
            "value" : "200"
          }, {
            "name" : "rm_io_weight",
            "value" : "100"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-BASE",
        "displayName" : "Failover Controller Default Group",
        "roleType" : "FAILOVERCONTROLLER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "heap_dump_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "log_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":5368709120,\"critical\":5368709120}"
          } ]
        }
      }, {
        "name" : "hdfs-GATEWAY-BASE",
        "displayName" : "Gateway Default Group",
        "roleType" : "GATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }
      }, {
        "name" : "hdfs-HTTPFS-BASE",
        "displayName" : "HttpFS Default Group",
        "roleType" : "HTTPFS",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "heap_dump_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "log_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-BASE",
        "displayName" : "JournalNode Default Group",
        "roleType" : "JOURNALNODE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_journalnode_edits_dir",
            "value" : "/dfs/jn"
          }, {
            "name" : "heap_dump_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "journalnode_edits_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":5368709120,\"critical\":5368709120}"
          }, {
            "name" : "log_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":5368709120,\"critical\":5368709120}"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-BASE",
        "displayName" : "NameNode Default Group",
        "roleType" : "NAMENODE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/dfs/nn"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          }, {
            "name" : "heap_dump_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "log_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":5368709120,\"critical\":5368709120}"
          }, {
            "name" : "namenode_data_directories_free_space_absolute_thresholds",
            "value" : "{\"warning\":5368709120,\"critical\":5368709120}"
          } ]
        }
      }, {
        "name" : "hdfs-NFSGATEWAY-BASE",
        "displayName" : "NFS Gateway Default Group",
        "roleType" : "NFSGATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "heap_dump_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "log_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "nfsgateway_dump_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          } ]
        }
      }, {
        "name" : "hdfs-SECONDARYNAMENODE-BASE",
        "displayName" : "SecondaryNameNode Default Group",
        "roleType" : "SECONDARYNAMENODE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/dfs/snn"
          }, {
            "name" : "heap_dump_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "log_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          }, {
            "name" : "secondarynamenode_checkpoint_directories_free_space_absolute_thresholds",
            "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
          } ]
        }
      } ],
      "replicationSchedules" : [ ],
      "snapshotPolicies" : [ ]
    }, {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "ip-172-31-3-200.ap-southeast-1.compute.internal"
        }, {
          "name" : "hive_metastore_database_password",
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
        "name" : "hive-GATEWAY-2080bdf39ad661ad2eeb435d02b45b98",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "4cf8f637-04c4-48de-bbfa-12faeb6f3379"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-2882409f66e1c9c5a02b2541d83f9583",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "f21abc82-ebf5-45ee-ba35-1a0d9a6603bc"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-5537dfd2b2c1891a3e5860ca2ae70ea9",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "557450b1-d1dd-41d9-9649-89f010bd1147"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-a3ae9015797700bf4903b8d0a1f4dba5",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "382b1c6c-67bf-4067-b8bb-fdedfa8d192e"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-f2373c0f7b73eec64dbc188eb4e7d42b",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "d7b8d6e4-d3ab-49ab-80ca-e0c006b45134"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-HIVEMETASTORE-f2373c0f7b73eec64dbc188eb4e7d42b",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "d7b8d6e4-d3ab-49ab-80ca-e0c006b45134"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6mwxvq56jo4t4k30igv1mj6ui"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-HIVEMETASTORE-BASE"
        }
      }, {
        "name" : "hive-HIVESERVER2-f2373c0f7b73eec64dbc188eb4e7d42b",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "d7b8d6e4-d3ab-49ab-80ca-e0c006b45134"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "12ygeekmuqdxv5vkglrq7kvlj"
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-HIVESERVER2-BASE"
        }
      } ],
      "displayName" : "Hive",
      "roleConfigGroups" : [ {
        "name" : "hive-GATEWAY-BASE",
        "displayName" : "Gateway Default Group",
        "roleType" : "GATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hive"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-BASE",
        "displayName" : "Hive Metastore Server Default Group",
        "roleType" : "HIVEMETASTORE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hive"
        },
        "config" : {
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "52428800"
          }, {
            "name" : "log_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":5368709120,\"critical\":5368709120}"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-BASE",
        "displayName" : "HiveServer2 Default Group",
        "roleType" : "HIVESERVER2",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hive"
        },
        "config" : {
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "52428800"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "3433247539"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "577"
          }, {
            "name" : "log_directory_free_space_absolute_thresholds",
            "value" : "{\"warning\":5368709120,\"critical\":5368709120}"
          } ]
        }
      }, {
        "name" : "hive-WEBHCAT-BASE",
        "displayName" : "WebHCat Server Default Group",
        "roleType" : "WEBHCAT",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hive"
        },
        "config" : {
          "items" : [ ]
        }
      } ],
      "replicationSchedules" : [ ]
    } ],
    "parcels" : [ {
      "product" : "CDH",
      "version" : "5.8.3-1.cdh5.8.3.p0.2",
      "stage" : "DISTRIBUTED",
      "clusterRef" : {
        "clusterName" : "cluster"
      }
    }, {
      "product" : "CDH",
      "version" : "5.8.3-1.cdh5.8.3.p0.2",
      "stage" : "ACTIVATED",
      "clusterRef" : {
        "clusterName" : "cluster"
      }
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "d7b8d6e4-d3ab-49ab-80ca-e0c006b45134",
    "ipAddress" : "172.31.11.106",
    "hostname" : "ip-172-31-11-106.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ {
        "name" : "memory_overcommit_threshold",
        "value" : "1"
      } ]
    }
  }, {
    "hostId" : "4cf8f637-04c4-48de-bbfa-12faeb6f3379",
    "ipAddress" : "172.31.12.88",
    "hostname" : "ip-172-31-12-88.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "382b1c6c-67bf-4067-b8bb-fdedfa8d192e",
    "ipAddress" : "172.31.3.200",
    "hostname" : "ip-172-31-3-200.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "f21abc82-ebf5-45ee-ba35-1a0d9a6603bc",
    "ipAddress" : "172.31.3.45",
    "hostname" : "ip-172-31-3-45.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "557450b1-d1dd-41d9-9649-89f010bd1147",
    "ipAddress" : "172.31.6.86",
    "hostname" : "ip-172-31-6-86.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__0bc0e175-109b-4bbf-bbcd-9d77ab8bd108",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "a8f2b00e887f9a6632bd06a16d01274365867f54e70f7fb3ecd2c690274f3219",
    "pwSalt" : -4227564573272292716,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-a3ae9015797700bf4903b8d0a1f4dba5",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "d641578cf531abde050d2f1ec2a30cc3b3df17bb13397452faad06d60648500e",
    "pwSalt" : -3720116617830909245,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-f2373c0f7b73eec64dbc188eb4e7d42b",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "7db81ed8ba2313cea11b93ad2725d95e9511edb2fa1067259b4bad7305090fb8",
    "pwSalt" : -2705787151694324794,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-a3ae9015797700bf4903b8d0a1f4dba5",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "cd21b965687e647cb6c2b6d00bf587638caabdf568dd22fba6435162c8b28caa",
    "pwSalt" : 3514634331458081336,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-f2373c0f7b73eec64dbc188eb4e7d42b",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "9f32f3bfe50144b4cc0ddb82c3c44a9956d91093230ee756d7d441b6455e6697",
    "pwSalt" : -6017448194954105189,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-a3ae9015797700bf4903b8d0a1f4dba5",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "c1469f66605362caf2b367a54a1a45537ef9e9e679b4606b4c1c6a8714a75cec",
    "pwSalt" : -8004500971663559145,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-f2373c0f7b73eec64dbc188eb4e7d42b",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "914c56ac7021c178ae5b41f63339c339d9b5078c78b64496c7b51c44e74e2e95",
    "pwSalt" : 1376390685426153090,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-a3ae9015797700bf4903b8d0a1f4dba5",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "4fb5ae235999c526b561a3f894cae50590b19658339d967a4faee460882b0540",
    "pwSalt" : 7325148892243484749,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-f2373c0f7b73eec64dbc188eb4e7d42b",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "99ff1d1cec5481fcc2d16166763ef821d6d55cb1fa2d8b6dc67b3e2ac11f735f",
    "pwSalt" : -1381909337570047142,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ],
    "pwHash" : "5ef80baf180be1a2235d489199da9b80c1e5b3df6452ff6e31ee2dd6b58f26d9",
    "pwSalt" : 4644890279105451542,
    "pwLogin" : true
  }, {
    "name" : "gotojeffray",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "22ae0b9e53755313f7344eac81503e2aa47e34bfa299f4f006c94e646f469c87",
    "pwSalt" : -3150269670934810552,
    "pwLogin" : true
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ],
    "pwHash" : "55a1b785d9243c6886f4b7a89fab84a76ab7e26698dd01e7305615c0cd0055ee",
    "pwSalt" : -4912735947048958037,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.8.2",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20160916-1419",
    "gitHash" : "d23c620f3a3bbd85d8511d6ebba49beaaab14b75",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ALERTPUBLISHER-f2373c0f7b73eec64dbc188eb4e7d42b",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "d7b8d6e4-d3ab-49ab-80ca-e0c006b45134"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "d4h7hurcf56061b8y8drl10qw"
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-ALERTPUBLISHER-BASE"
      }
    }, {
      "name" : "mgmt-EVENTSERVER-f2373c0f7b73eec64dbc188eb4e7d42b",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "d7b8d6e4-d3ab-49ab-80ca-e0c006b45134"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "976bkl0ophj2zoukdtgtt1282"
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-EVENTSERVER-BASE"
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-f2373c0f7b73eec64dbc188eb4e7d42b",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "d7b8d6e4-d3ab-49ab-80ca-e0c006b45134"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "9wecfa4cann99xapola1kq9jb"
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-HOSTMONITOR-BASE"
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-f2373c0f7b73eec64dbc188eb4e7d42b",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "d7b8d6e4-d3ab-49ab-80ca-e0c006b45134"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "4luz33kugbwwr9xxxop2ufnom"
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-REPORTSMANAGER-BASE"
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-f2373c0f7b73eec64dbc188eb4e7d42b",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "d7b8d6e4-d3ab-49ab-80ca-e0c006b45134"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "9z2zooa68qgv6rl5c0xgj3lf9"
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-SERVICEMONITOR-BASE"
      }
    } ],
    "displayName" : "Cloudera Management Service",
    "roleConfigGroups" : [ {
      "name" : "mgmt-ACTIVITYMONITOR-BASE",
      "displayName" : "Activity Monitor Default Group",
      "roleType" : "ACTIVITYMONITOR",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "heap_dump_directory_free_space_absolute_thresholds",
          "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
        }, {
          "name" : "log_directory_free_space_absolute_thresholds",
          "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
        } ]
      }
    }, {
      "name" : "mgmt-ALERTPUBLISHER-BASE",
      "displayName" : "Alert Publisher Default Group",
      "roleType" : "ALERTPUBLISHER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "heap_dump_directory_free_space_absolute_thresholds",
          "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
        }, {
          "name" : "log_directory_free_space_absolute_thresholds",
          "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-BASE",
      "displayName" : "Event Server Default Group",
      "roleType" : "EVENTSERVER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "event_server_heapsize",
          "value" : "52428800"
        }, {
          "name" : "eventserver_index_directory_free_space_absolute_thresholds",
          "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
        }, {
          "name" : "heap_dump_directory_free_space_absolute_thresholds",
          "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
        }, {
          "name" : "log_directory_free_space_absolute_thresholds",
          "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-BASE",
      "displayName" : "Host Monitor Default Group",
      "roleType" : "HOSTMONITOR",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "268435456"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "805306368"
        }, {
          "name" : "firehose_storage_directory_free_space_absolute_thresholds",
          "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
        }, {
          "name" : "heap_dump_directory_free_space_absolute_thresholds",
          "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
        }, {
          "name" : "log_directory_free_space_absolute_thresholds",
          "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
        } ]
      }
    }, {
      "name" : "mgmt-NAVIGATOR-BASE",
      "displayName" : "Navigator Audit Server Default Group",
      "roleType" : "NAVIGATOR",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "heap_dump_directory_free_space_absolute_thresholds",
          "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
        }, {
          "name" : "log_directory_free_space_absolute_thresholds",
          "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
        } ]
      }
    }, {
      "name" : "mgmt-NAVIGATORMETASERVER-BASE",
      "displayName" : "Navigator Metadata Server Default Group",
      "roleType" : "NAVIGATORMETASERVER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "heap_dump_directory_free_space_absolute_thresholds",
          "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
        }, {
          "name" : "log_directory_free_space_absolute_thresholds",
          "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
        }, {
          "name" : "navigatormetaserver_audit_event_log_directory_free_space_absolute_thresholds",
          "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
        }, {
          "name" : "navigatormetaserver_data_directory_free_space_absolute_thresholds",
          "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-BASE",
      "displayName" : "Reports Manager Default Group",
      "roleType" : "REPORTSMANAGER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "ip-172-31-3-200.ap-southeast-1.compute.internal"
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_password",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman"
        }, {
          "name" : "headlamp_heapsize",
          "value" : "268435456"
        }, {
          "name" : "heap_dump_directory_free_space_absolute_thresholds",
          "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
        }, {
          "name" : "log_directory_free_space_absolute_thresholds",
          "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
        }, {
          "name" : "reportsmanager_scratch_directory_free_space_absolute_thresholds",
          "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-BASE",
      "displayName" : "Service Monitor Default Group",
      "roleType" : "SERVICEMONITOR",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "268435456"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "805306368"
        }, {
          "name" : "firehose_storage_directory_free_space_absolute_thresholds",
          "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
        }, {
          "name" : "heap_dump_directory_free_space_absolute_thresholds",
          "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
        }, {
          "name" : "log_directory_free_space_absolute_thresholds",
          "value" : "{\"warning\":6442450944,\"critical\":5368709120}"
        } ]
      }
    } ]
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/22/2012 6:30"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,http://archive.cloudera.com/beta/spark2/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/,http://ec2-52-221-239-59.ap-southeast-1.compute.amazonaws.com/parcel/"
    } ]
  },
  "allHostsConfig" : {
    "items" : [ {
      "name" : "host_agent_parcel_directory_free_space_absolute_thresholds",
      "value" : "{\"warning\":5368709120,\"critical\":5368709120}"
    }, {
      "name" : "host_clock_offset_thresholds",
      "value" : "{\"warning\":5000,\"critical\":10000}"
    }, {
      "name" : "rm_enabled",
      "value" : "true"
    } ]
  },
  "peers" : [ {
    "name" : "chiehwoei",
    "type" : "REPLICATION",
    "url" : "http://54.254.130.16:7180",
    "username" : "__cloudera_internal_user__6eb79bb9-f979-4b18-9965-9b3bf8fc858c",
    "password" : "13933343-92fb-4cf2-82b9-da08a688ceeb7261e5a7-3d79-4fbd-86ed-b7f6232c0f58",
    "clouderaManagerCreatedUser" : true
  } ],
  "hostTemplates" : {
    "items" : [ ]
  }
}
~~~
