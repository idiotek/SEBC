* The hostname of your db server node
```
# hostname
ip-172-31-28-115
```

* The command and output for display your database server's version
```
# mysql -V
mysql  Ver 14.14 Distrib 5.6.36, for Linux (x86_64) using  EditLine wrapper
```

* The command and output for listing your created databases
```
# mysql -u root -p -e 'show databases;'
Enter password: 
+--------------------+
| Database           |
+--------------------+
| information_schema |
| hive               |
| hue                |
| mysql              |
| oozie              |
| performance_schema |
| rman               |
| scm                |
| sentry             |
+--------------------+
```
