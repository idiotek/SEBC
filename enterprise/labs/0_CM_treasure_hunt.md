* What is ubertask optimization?
```
When enabled, this YARN Performance setting runs "sufficiently small" jobs sequentially within a single JVM. "Small" is defined by the mapreduce.job.ubertask.maxmaps, mapreduce.job.ubertask.maxreduces, and mapreduce.job.ubertask.maxbytes settings.
```

* Where in CM is the Kerberos Security Realm value displayed?
```
Under Administration -> Settings -> Kerberos Category -> Kerberos Security Realm
```

* Which CDH service(s) host a property for enabling Kerberos authentication?
```
ZooKeeper - ZooKeeper -> Configuration -> Main Category -> Enable Kerberos Authentication
```
[All of them do]


* How do you upgrade the CM agents?
```
More details - https://www.cloudera.com/documentation/enterprise/5-9-x/topics/cm_ag_ug_cm5.html#concept_gs4_bsg_xw

* Stop all CDH services, then Cloudera Manager Server and Cloudera Manager database
* Stop the Cloudera Manager Agent on the Cloudera Manager host
* Download the latest cloudera-manager.repo file for your distribution
* For RHEL/CentOS, copy the cloudera-manager.repo file to /etc/yum.repos.d/
* sudo yum clean all
* sudo yum upgrade cloudera-manager-server cloudera-manager-daemons cloudera-manager-agent
* sudo service cloudera-scm-server start
* sudo service cloudera-scm-agent start
* Login to Cloudera Manager console and follow on-screen instructions to update other hosts' Cloudera Manager agent and JDK (optional)
```

* Give the tsquery statement used to chart Hue's CPU utilization?
```
select cpu_system_rate + cpu_user_rate where category=ROLE and serviceName=Hue
```

* Name all the roles that make up the Hive service
```
* Hive Metastore Server
* WebHCat Server
* HiveServer2
* Hive Gateway
```

* What steps must be completed before integrating Cloudera Manager with Kerberos?
```
Assuming the cluster is hosted on RHEL/CentOS 6:
* working KDC and realm
* secured communication between Cloudera Manager server and all agents
* installed openldap-clients on the Cloudera Manager host
* installed krb5-workstation and krb5-libs packages on all hosts
```
