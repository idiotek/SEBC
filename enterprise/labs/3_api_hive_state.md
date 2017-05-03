* curl statement that stop Hive service 
```
curl -u idiotek:cloudera -XPOST 'http://13.54.14.200:7180/api/v12/clusters/idiotek/services/hive/commands/stop'
{
  "id" : 2117,
  "name" : "Stop",
  "startTime" : "2017-05-03T11:45:14.848Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}
```

* check the status of the previous stop command
```
curl -u idiotek:cloudera 'http://13.54.14.200:7180/api/v12/commands/2117'
{
  "id" : 2117,
  "name" : "Stop",
  "startTime" : "2017-05-03T11:45:14.848Z",
  "endTime" : "2017-05-03T11:45:16.916Z",
  "active" : false,
  "success" : true,
  "resultMessage" : "Successfully stopped service.",
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  },
  "children" : {
    "items" : [ {
      "id" : 2118,
      "name" : "Stop",
      "startTime" : "2017-05-03T11:45:14.857Z",
      "endTime" : "2017-05-03T11:45:16.908Z",
      "active" : false,
      "success" : true,
      "resultMessage" : "Successfully stopped process.",
      "serviceRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive"
      },
      "roleRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive",
        "roleName" : "hive-HIVESERVER2-6f1d0e131507241a3823727fa85c07bb"
      }
    }, {
      "id" : 2119,
      "name" : "Stop",
      "startTime" : "2017-05-03T11:45:14.860Z",
      "endTime" : "2017-05-03T11:45:16.829Z",
      "active" : false,
      "success" : true,
      "resultMessage" : "Successfully stopped process.",
      "serviceRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive"
      },
      "roleRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive",
        "roleName" : "hive-HIVEMETASTORE-03d57ed8122e3fe4d8a37b86d27e4790"
      }
    } ]
  },
  "canRetry" : false
}
```

* curl statement to start Hive service

```
curl -u idiotek:cloudera -XPOST 'http://13.54.14.200:7180/api/v12/clusters/idiotek/services/hive/commands/start'
{
  "id" : 2121,
  "name" : "Start",
  "startTime" : "2017-05-03T11:50:26.898Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}
```

* curl statement to check the current state of Hive service
```
curl -u idiotek:cloudera 'http://13.54.14.200:7180/api/v12/clusters/idiotek/services/hive'
{
  "name" : "hive",
  "type" : "HIVE",
  "clusterRef" : {
    "clusterName" : "cluster"
  },
  "serviceUrl" : "http://ip-172-31-10-189:7180/cmf/serviceRedirect/hive",
  "roleInstancesUrl" : "http://ip-172-31-10-189:7180/cmf/serviceRedirect/hive/instances",
  "serviceState" : "STARTED",
  "healthSummary" : "GOOD",
  "healthChecks" : [ {
    "name" : "HIVE_HIVEMETASTORES_HEALTHY",
    "summary" : "GOOD",
    "suppressed" : false
  }, {
    "name" : "HIVE_HIVESERVER2S_HEALTHY",
    "summary" : "GOOD",
    "suppressed" : false
  } ],
  "configStalenessStatus" : "FRESH",
  "clientConfigStalenessStatus" : "FRESH",
  "maintenanceMode" : false,
  "maintenanceOwners" : [ ],
  "displayName" : "Hive",
  "entityStatus" : "GOOD_HEALTH"
}
```
