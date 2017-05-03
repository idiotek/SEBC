* Create a precious directory in HDFS
<code>sudo -u idiotek hdfs dfs -mkdir /user/idiotek/precious</code>

* Copy the ZIP course file into it
<code>sudo -u idiotek hdfs dfs -put /home/idiotek/SEBC.zip /user/idiotek/precious/</code>

* Enable snapshots for precious
<code>sudo -u hdfs hdfs dfsadmin -allowSnapshot /user/idiotek/precious</code>

* Create a snapshot called sebc-hdfs-test
<code>sudo -u idiotek hdfs dfs -createSnapshot /user/idiotek/precious sebc-hdfs-test</code>

* Delete the directory
```
sudo -u idiotek hdfs dfs -rm -f -r -skipTrash /user/idiotek/precious
rm: The directory /user/idiotek/precious cannot be deleted since /user/idiotek/precious is snapshottable and already has snapshots
```
* Delete the ZIP file
```
sudo -u idiotek hdfs dfs -rm -f -skipTrash /user/idiotek/precious/SEBC.zip
Deleted /user/idiotek/precious/SEBC.zip
```
* Restore the deleted file
<code>sudo -u idiotek hdfs dfs -cp /user/idiotek/precious/.snapshot/sebc-hdfs-test/SEBC.zip /user/idiotek/precious/</code>
