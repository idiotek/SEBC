* The full teragen command and job output
```
[cate@ip-172-31-23-151 ~]$ time hadoop jar /opt/cloudera/parcels/CDH/jars/hadoop-examples.jar teragen -D dfs.block.size=16777216 -D mapreduce.map.memory.mb=512 65536000 /user/cate/tgen
17/05/05 01:10:35 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-19-216/172.31.19.216:8032
17/05/05 01:10:36 INFO terasort.TeraGen: Generating 65536000 using 2
17/05/05 01:10:36 INFO mapreduce.JobSubmitter: number of splits:2
17/05/05 01:10:36 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/05/05 01:10:36 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1493945454085_0001
17/05/05 01:10:37 INFO impl.YarnClientImpl: Submitted application application_1493945454085_0001
17/05/05 01:10:37 INFO mapreduce.Job: The url to track the job: http://ip-172-31-19-216:8088/proxy/application_1493945454085_0001/
17/05/05 01:10:37 INFO mapreduce.Job: Running job: job_1493945454085_0001
17/05/05 01:10:44 INFO mapreduce.Job: Job job_1493945454085_0001 running in uber mode : false
17/05/05 01:10:44 INFO mapreduce.Job:  map 0% reduce 0%
17/05/05 01:11:03 INFO mapreduce.Job:  map 27% reduce 0%
17/05/05 01:11:09 INFO mapreduce.Job:  map 33% reduce 0%
17/05/05 01:11:15 INFO mapreduce.Job:  map 38% reduce 0%
17/05/05 01:11:22 INFO mapreduce.Job:  map 45% reduce 0%
17/05/05 01:11:28 INFO mapreduce.Job:  map 57% reduce 0%
17/05/05 01:11:34 INFO mapreduce.Job:  map 63% reduce 0%
17/05/05 01:11:40 INFO mapreduce.Job:  map 68% reduce 0%
17/05/05 01:11:46 INFO mapreduce.Job:  map 75% reduce 0%
17/05/05 01:11:52 INFO mapreduce.Job:  map 85% reduce 0%
17/05/05 01:11:58 INFO mapreduce.Job:  map 93% reduce 0%
17/05/05 01:12:04 INFO mapreduce.Job:  map 95% reduce 0%
17/05/05 01:12:08 INFO mapreduce.Job:  map 100% reduce 0%
17/05/05 01:12:08 INFO mapreduce.Job: Job job_1493945454085_0001 completed successfully
17/05/05 01:12:08 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=248924
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=170
		HDFS: Number of bytes written=6553600000
		HDFS: Number of read operations=8
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=4
	Job Counters 
		Launched map tasks=2
		Other local map tasks=2
		Total time spent by all maps in occupied slots (ms)=161989
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=161989
		Total vcore-seconds taken by all map tasks=161989
		Total megabyte-seconds taken by all map tasks=165876736
	Map-Reduce Framework
		Map input records=65536000
		Map output records=65536000
		Input split bytes=170
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=1008
		CPU time spent (ms)=94130
		Physical memory (bytes) snapshot=330674176
		Virtual memory (bytes) snapshot=2229833728
		Total committed heap usage (bytes)=421527552
	org.apache.hadoop.examples.terasort.TeraGen$Counters
		CHECKSUM=140750829423462787
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=6553600000
```

* The result of the time command
```
real	1m35.642s
user	0m5.962s
sys	0m0.756s
```

* The command and output of hdfs dfs -ls /user/cate/tgen
```
[cate@ip-172-31-23-151 ~]$ hdfs dfs -ls /user/cate/tgen
Found 3 items
-rw-r--r--   3 cate aussies          0 2017-05-05 01:12 /user/cate/tgen/_SUCCESS
-rw-r--r--   3 cate aussies 3276800000 2017-05-05 01:12 /user/cate/tgen/part-m-00000
-rw-r--r--   3 cate aussies 3276800000 2017-05-05 01:12 /user/cate/tgen/part-m-00001
```
