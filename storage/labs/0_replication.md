* Choose a partner in class
<code>NithK45</code>

* Name a source directory after your GitHub handle
<code>/user/idiotek/0_replication_source_idiotek</code>

* Name a target directory after your partner's GitHub handle
<code>/user/idiotek/0_replication_target_NithK45</code>

* Use teragen to create a 500 MB file
```
hadoop jar hadoop-examples.jar teragen -D mapreduce.job.maps=1 5242880 /user/idiotek/0_replication_source_idiotek
17/05/03 12:18:40 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-2-85/172.31.2.85:8032
17/05/03 12:18:40 INFO terasort.TeraSort: Generating 5242880 using 1
17/05/03 12:18:41 INFO mapreduce.JobSubmitter: number of splits:1
17/05/03 12:18:41 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1493776969938_0002
17/05/03 12:18:41 INFO impl.YarnClientImpl: Submitted application application_1493776969938_0002
17/05/03 12:18:41 INFO mapreduce.Job: The url to track the job: http://ip-172-31-2-85:8088/proxy/application_1493776969938_0002/
17/05/03 12:18:41 INFO mapreduce.Job: Running job: job_1493776969938_0002
17/05/03 12:18:48 INFO mapreduce.Job: Job job_1493776969938_0002 running in uber mode : false
17/05/03 12:18:48 INFO mapreduce.Job:  map 0% reduce 0%
17/05/03 12:19:01 INFO mapreduce.Job:  map 72% reduce 0%
17/05/03 12:19:02 INFO mapreduce.Job:  map 100% reduce 0%
17/05/03 12:19:03 INFO mapreduce.Job: Job job_1493776969938_0002 completed successfully
17/05/03 12:19:03 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=124829
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=82
		HDFS: Number of bytes written=524288000
		HDFS: Number of read operations=4
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=2
	Job Counters 
		Launched map tasks=1
		Other local map tasks=1
		Total time spent by all maps in occupied slots (ms)=11818
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=11818
		Total vcore-seconds taken by all map tasks=11818
		Total megabyte-seconds taken by all map tasks=12101632
	Map-Reduce Framework
		Map input records=5242880
		Map output records=5242880
		Input split bytes=82
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=82
		CPU time spent (ms)=11170
		Physical memory (bytes) snapshot=368259072
		Virtual memory (bytes) snapshot=1567928320
		Total committed heap usage (bytes)=400556032
	org.apache.hadoop.examples.terasort.TeraGen$Counters
		CHECKSUM=11257830824958050
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=524288000
```

* Copy your partner's file to your target directory, one use distcp (NithK45), one use BDR (idiotek)
```
Please refer to 0_replication_config.png for HDFS Replication configuration
```

* Browse the results
```
Unable to complete transfer as map reduce job is stuck at 58%
Please refer to 0_replicaton_stderr.log for log details
```
