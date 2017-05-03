* Report the latest available version of the API
```
curl -u idiotek:cloudera -XGET 'http://13.54.14.200:7180/api/version'
v16
```

* Report the CM version
```
curl -u idiotek:cloudera 'http://13.54.14.200:7180/api/v16/cm/version'
{
  "version" : "5.11.0",
  "buildUser" : "jenkins",
  "buildTimestamp" : "20170412-1249",
  "gitHash" : "70cb1442626406432a6e7af5bdf206a384ca3f98",
  "snapshot" : false
}
```

* List all CM users
```
curl -u idiotek:cloudera 'http://13.54.14.200:7180/api/v16/users'
{
  "items" : [ {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ]
  }, {
    "name" : "idiotek",
    "roles" : [ "ROLE_ADMIN" ]
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ]
  } ]
}
```

* Report the database server in use by CM
```
curl -u idiotek:cloudera -XGET 'http://13.54.14.200:7180/api/v16/cm/scmDbInfo'
{
  "scmDbType" : "MYSQL",
  "embeddedDbUsed" : false
}
```
