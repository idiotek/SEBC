* Create a 10 GB file using teragen
* Set the mappers to 4
* Limit the block size to 32 MB
* Output to /user/idiotek directory
* Use the time command to report the job's duration
```
time hadoop jar hadoop-examples.jar teragen -D dfs.blocksize=33554432 -D mapreduce.job.maps=4 100000000 /user/idiotek/terasort-input
17/05/02 20:31:53 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-2-85/172.31.2.85:8032
17/05/02 20:31:53 INFO terasort.TeraSort: Generating 100000000 using 4
17/05/02 20:31:53 INFO mapreduce.JobSubmitter: number of splits:4
17/05/02 20:31:54 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1493709758444_0005
17/05/02 20:31:54 INFO impl.YarnClientImpl: Submitted application application_1493709758444_0005
17/05/02 20:31:54 INFO mapreduce.Job: The url to track the job: http://ip-172-31-2-85:8088/proxy/application_1493709758444_0005/
17/05/02 20:31:54 INFO mapreduce.Job: Running job: job_1493709758444_0005
17/05/02 20:32:00 INFO mapreduce.Job: Job job_1493709758444_0005 running in uber mode : false
17/05/02 20:32:00 INFO mapreduce.Job:  map 0% reduce 0%
17/05/02 20:32:12 INFO mapreduce.Job:  map 11% reduce 0%
17/05/02 20:32:15 INFO mapreduce.Job:  map 15% reduce 0%
17/05/02 20:32:18 INFO mapreduce.Job:  map 16% reduce 0%
17/05/02 20:32:19 INFO mapreduce.Job:  map 19% reduce 0%
17/05/02 20:32:22 INFO mapreduce.Job:  map 22% reduce 0%
17/05/02 20:32:24 INFO mapreduce.Job:  map 23% reduce 0%
17/05/02 20:32:25 INFO mapreduce.Job:  map 24% reduce 0%
17/05/02 20:32:27 INFO mapreduce.Job:  map 25% reduce 0%
17/05/02 20:32:28 INFO mapreduce.Job:  map 27% reduce 0%
17/05/02 20:32:31 INFO mapreduce.Job:  map 28% reduce 0%
17/05/02 20:32:33 INFO mapreduce.Job:  map 29% reduce 0%
17/05/02 20:32:34 INFO mapreduce.Job:  map 31% reduce 0%
17/05/02 20:32:36 INFO mapreduce.Job:  map 32% reduce 0%
17/05/02 20:32:37 INFO mapreduce.Job:  map 33% reduce 0%
17/05/02 20:32:39 INFO mapreduce.Job:  map 34% reduce 0%
17/05/02 20:32:40 INFO mapreduce.Job:  map 35% reduce 0%
17/05/02 20:32:42 INFO mapreduce.Job:  map 37% reduce 0%
17/05/02 20:32:43 INFO mapreduce.Job:  map 38% reduce 0%
17/05/02 20:32:45 INFO mapreduce.Job:  map 39% reduce 0%
17/05/02 20:32:46 INFO mapreduce.Job:  map 40% reduce 0%
17/05/02 20:32:48 INFO mapreduce.Job:  map 42% reduce 0%
17/05/02 20:32:49 INFO mapreduce.Job:  map 43% reduce 0%
17/05/02 20:32:51 INFO mapreduce.Job:  map 44% reduce 0%
17/05/02 20:32:52 INFO mapreduce.Job:  map 45% reduce 0%
17/05/02 20:32:54 INFO mapreduce.Job:  map 47% reduce 0%
17/05/02 20:32:55 INFO mapreduce.Job:  map 48% reduce 0%
17/05/02 20:32:57 INFO mapreduce.Job:  map 49% reduce 0%
17/05/02 20:32:58 INFO mapreduce.Job:  map 50% reduce 0%
17/05/02 20:33:00 INFO mapreduce.Job:  map 51% reduce 0%
17/05/02 20:33:01 INFO mapreduce.Job:  map 52% reduce 0%
17/05/02 20:33:03 INFO mapreduce.Job:  map 53% reduce 0%
17/05/02 20:33:06 INFO mapreduce.Job:  map 55% reduce 0%
17/05/02 20:33:09 INFO mapreduce.Job:  map 58% reduce 0%
17/05/02 20:33:12 INFO mapreduce.Job:  map 61% reduce 0%
17/05/02 20:33:15 INFO mapreduce.Job:  map 64% reduce 0%
17/05/02 20:33:18 INFO mapreduce.Job:  map 67% reduce 0%
17/05/02 20:33:22 INFO mapreduce.Job:  map 69% reduce 0%
17/05/02 20:33:25 INFO mapreduce.Job:  map 71% reduce 0%
17/05/02 20:33:28 INFO mapreduce.Job:  map 73% reduce 0%
17/05/02 20:33:29 INFO mapreduce.Job:  map 74% reduce 0%
17/05/02 20:33:31 INFO mapreduce.Job:  map 75% reduce 0%
17/05/02 20:33:40 INFO mapreduce.Job:  map 79% reduce 0%
17/05/02 20:33:43 INFO mapreduce.Job:  map 81% reduce 0%
17/05/02 20:33:46 INFO mapreduce.Job:  map 83% reduce 0%
17/05/02 20:33:49 INFO mapreduce.Job:  map 85% reduce 0%
17/05/02 20:33:52 INFO mapreduce.Job:  map 86% reduce 0%
17/05/02 20:33:55 INFO mapreduce.Job:  map 88% reduce 0%
17/05/02 20:33:58 INFO mapreduce.Job:  map 90% reduce 0%
17/05/02 20:34:01 INFO mapreduce.Job:  map 91% reduce 0%
17/05/02 20:34:04 INFO mapreduce.Job:  map 93% reduce 0%
17/05/02 20:34:07 INFO mapreduce.Job:  map 95% reduce 0%
17/05/02 20:34:10 INFO mapreduce.Job:  map 97% reduce 0%
17/05/02 20:34:13 INFO mapreduce.Job:  map 99% reduce 0%
17/05/02 20:34:15 INFO mapreduce.Job:  map 100% reduce 0%
17/05/02 20:34:17 INFO mapreduce.Job: Job job_1493709758444_0005 completed successfully
17/05/02 20:34:17 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=499280
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=344
		HDFS: Number of bytes written=10000000000
		HDFS: Number of read operations=16
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=8
	Job Counters 
		Launched map tasks=4
		Other local map tasks=4
		Total time spent by all maps in occupied slots (ms)=308622
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=308622
		Total vcore-seconds taken by all map tasks=308622
		Total megabyte-seconds taken by all map tasks=316028928
	Map-Reduce Framework
		Map input records=100000000
		Map output records=100000000
		Input split bytes=344
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=1195
		CPU time spent (ms)=146740
		Physical memory (bytes) snapshot=822636544
		Virtual memory (bytes) snapshot=6267510784
		Total committed heap usage (bytes)=868220928
	org.apache.hadoop.examples.terasort.TeraGen$Counters
		CHECKSUM=214760662691937609
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=10000000000

real	2m27.112s
user	0m5.743s
sys	0m0.769s
```

* Run the terasort command on this file
* Use the time command to report the job's duration
* Output to /user/idiotek directory
```
time hadoop jar hadoop-examples.jar terasort /user/idiotek/terasort-input /user/idiotek/terasort-output
17/05/02 20:36:14 INFO terasort.TeraSort: starting
17/05/02 20:36:16 INFO input.FileInputFormat: Total input paths to process : 4
Spent 276ms computing base-splits.
Spent 7ms computing TeraScheduler splits.
Computing input splits took 283ms
Sampling 10 splits of 300
Making 8 from 100000 sampled records
Computing parititions took 932ms
Spent 1218ms computing partitions.
17/05/02 20:36:17 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-2-85/172.31.2.85:8032
17/05/02 20:36:18 INFO mapreduce.JobSubmitter: number of splits:300
17/05/02 20:36:18 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1493709758444_0006
17/05/02 20:36:18 INFO impl.YarnClientImpl: Submitted application application_1493709758444_0006
17/05/02 20:36:18 INFO mapreduce.Job: The url to track the job: http://ip-172-31-2-85:8088/proxy/application_1493709758444_0006/
17/05/02 20:36:18 INFO mapreduce.Job: Running job: job_1493709758444_0006
17/05/02 20:36:24 INFO mapreduce.Job: Job job_1493709758444_0006 running in uber mode : false
17/05/02 20:36:24 INFO mapreduce.Job:  map 0% reduce 0%
17/05/02 20:36:32 INFO mapreduce.Job:  map 1% reduce 0%
17/05/02 20:36:38 INFO mapreduce.Job:  map 2% reduce 0%
17/05/02 20:36:44 INFO mapreduce.Job:  map 3% reduce 0%
17/05/02 20:36:50 INFO mapreduce.Job:  map 4% reduce 0%
17/05/02 20:36:57 INFO mapreduce.Job:  map 5% reduce 0%
17/05/02 20:37:03 INFO mapreduce.Job:  map 6% reduce 0%
17/05/02 20:37:09 INFO mapreduce.Job:  map 7% reduce 0%
17/05/02 20:37:16 INFO mapreduce.Job:  map 8% reduce 0%
17/05/02 20:37:23 INFO mapreduce.Job:  map 9% reduce 0%
17/05/02 20:37:29 INFO mapreduce.Job:  map 10% reduce 0%
17/05/02 20:37:35 INFO mapreduce.Job:  map 11% reduce 0%
17/05/02 20:37:41 INFO mapreduce.Job:  map 12% reduce 0%
17/05/02 20:37:47 INFO mapreduce.Job:  map 13% reduce 0%
17/05/02 20:37:54 INFO mapreduce.Job:  map 14% reduce 0%
17/05/02 20:38:00 INFO mapreduce.Job:  map 15% reduce 0%
17/05/02 20:38:06 INFO mapreduce.Job:  map 16% reduce 0%
17/05/02 20:38:12 INFO mapreduce.Job:  map 17% reduce 0%
17/05/02 20:38:19 INFO mapreduce.Job:  map 18% reduce 0%
17/05/02 20:38:25 INFO mapreduce.Job:  map 19% reduce 0%
17/05/02 20:38:31 INFO mapreduce.Job:  map 20% reduce 0%
17/05/02 20:38:38 INFO mapreduce.Job:  map 21% reduce 0%
17/05/02 20:38:44 INFO mapreduce.Job:  map 22% reduce 0%
17/05/02 20:38:51 INFO mapreduce.Job:  map 23% reduce 0%
17/05/02 20:38:57 INFO mapreduce.Job:  map 24% reduce 0%
17/05/02 20:39:03 INFO mapreduce.Job:  map 25% reduce 0%
17/05/02 20:39:10 INFO mapreduce.Job:  map 26% reduce 0%
17/05/02 20:39:16 INFO mapreduce.Job:  map 27% reduce 0%
17/05/02 20:39:22 INFO mapreduce.Job:  map 28% reduce 0%
17/05/02 20:39:28 INFO mapreduce.Job:  map 29% reduce 0%
17/05/02 20:39:34 INFO mapreduce.Job:  map 30% reduce 0%
17/05/02 20:39:40 INFO mapreduce.Job:  map 31% reduce 0%
17/05/02 20:39:46 INFO mapreduce.Job:  map 32% reduce 0%
17/05/02 20:39:52 INFO mapreduce.Job:  map 33% reduce 0%
17/05/02 20:39:58 INFO mapreduce.Job:  map 34% reduce 0%
17/05/02 20:40:04 INFO mapreduce.Job:  map 35% reduce 0%
17/05/02 20:40:11 INFO mapreduce.Job:  map 36% reduce 0%
17/05/02 20:40:17 INFO mapreduce.Job:  map 37% reduce 0%
17/05/02 20:40:23 INFO mapreduce.Job:  map 38% reduce 0%
17/05/02 20:40:29 INFO mapreduce.Job:  map 39% reduce 0%
17/05/02 20:40:35 INFO mapreduce.Job:  map 40% reduce 0%
17/05/02 20:40:41 INFO mapreduce.Job:  map 41% reduce 0%
17/05/02 20:40:47 INFO mapreduce.Job:  map 42% reduce 0%
17/05/02 20:40:53 INFO mapreduce.Job:  map 43% reduce 0%
17/05/02 20:40:59 INFO mapreduce.Job:  map 44% reduce 0%
17/05/02 20:41:06 INFO mapreduce.Job:  map 45% reduce 0%
17/05/02 20:41:13 INFO mapreduce.Job:  map 46% reduce 0%
17/05/02 20:41:20 INFO mapreduce.Job:  map 47% reduce 0%
17/05/02 20:41:26 INFO mapreduce.Job:  map 48% reduce 0%
17/05/02 20:41:32 INFO mapreduce.Job:  map 49% reduce 0%
17/05/02 20:41:39 INFO mapreduce.Job:  map 50% reduce 0%
17/05/02 20:41:45 INFO mapreduce.Job:  map 51% reduce 0%
17/05/02 20:41:51 INFO mapreduce.Job:  map 52% reduce 0%
17/05/02 20:41:57 INFO mapreduce.Job:  map 53% reduce 0%
17/05/02 20:42:03 INFO mapreduce.Job:  map 54% reduce 0%
17/05/02 20:42:09 INFO mapreduce.Job:  map 55% reduce 0%
17/05/02 20:42:16 INFO mapreduce.Job:  map 56% reduce 0%
17/05/02 20:42:22 INFO mapreduce.Job:  map 57% reduce 0%
17/05/02 20:42:29 INFO mapreduce.Job:  map 58% reduce 0%
17/05/02 20:42:35 INFO mapreduce.Job:  map 59% reduce 0%
17/05/02 20:42:41 INFO mapreduce.Job:  map 60% reduce 0%
17/05/02 20:42:47 INFO mapreduce.Job:  map 61% reduce 0%
17/05/02 20:42:52 INFO mapreduce.Job:  map 62% reduce 0%
17/05/02 20:42:59 INFO mapreduce.Job:  map 63% reduce 0%
17/05/02 20:43:05 INFO mapreduce.Job:  map 64% reduce 0%
17/05/02 20:43:10 INFO mapreduce.Job:  map 65% reduce 0%
17/05/02 20:43:17 INFO mapreduce.Job:  map 66% reduce 0%
17/05/02 20:43:23 INFO mapreduce.Job:  map 67% reduce 0%
17/05/02 20:43:29 INFO mapreduce.Job:  map 68% reduce 0%
17/05/02 20:43:36 INFO mapreduce.Job:  map 69% reduce 0%
17/05/02 20:43:41 INFO mapreduce.Job:  map 70% reduce 0%
17/05/02 20:43:48 INFO mapreduce.Job:  map 71% reduce 0%
17/05/02 20:43:55 INFO mapreduce.Job:  map 72% reduce 0%
17/05/02 20:44:01 INFO mapreduce.Job:  map 73% reduce 0%
17/05/02 20:44:08 INFO mapreduce.Job:  map 74% reduce 0%
17/05/02 20:44:14 INFO mapreduce.Job:  map 75% reduce 0%
17/05/02 20:44:20 INFO mapreduce.Job:  map 76% reduce 0%
17/05/02 20:44:26 INFO mapreduce.Job:  map 77% reduce 0%
17/05/02 20:44:32 INFO mapreduce.Job:  map 78% reduce 0%
17/05/02 20:44:39 INFO mapreduce.Job:  map 79% reduce 0%
17/05/02 20:44:45 INFO mapreduce.Job:  map 80% reduce 0%
17/05/02 20:44:51 INFO mapreduce.Job:  map 81% reduce 0%
17/05/02 20:44:56 INFO mapreduce.Job:  map 82% reduce 0%
17/05/02 20:45:03 INFO mapreduce.Job:  map 82% reduce 3%
17/05/02 20:45:05 INFO mapreduce.Job:  map 83% reduce 3%
17/05/02 20:45:15 INFO mapreduce.Job:  map 84% reduce 3%
17/05/02 20:45:18 INFO mapreduce.Job:  map 84% reduce 4%
17/05/02 20:45:24 INFO mapreduce.Job:  map 85% reduce 4%
17/05/02 20:45:32 INFO mapreduce.Job:  map 86% reduce 4%
17/05/02 20:45:44 INFO mapreduce.Job:  map 87% reduce 4%
17/05/02 20:45:50 INFO mapreduce.Job:  map 88% reduce 4%
17/05/02 20:46:03 INFO mapreduce.Job:  map 89% reduce 4%
17/05/02 20:46:10 INFO mapreduce.Job:  map 90% reduce 4%
17/05/02 20:46:21 INFO mapreduce.Job:  map 91% reduce 4%
17/05/02 20:46:30 INFO mapreduce.Job:  map 92% reduce 4%
17/05/02 20:46:39 INFO mapreduce.Job:  map 93% reduce 4%
17/05/02 20:46:50 INFO mapreduce.Job:  map 94% reduce 4%
17/05/02 20:46:57 INFO mapreduce.Job:  map 95% reduce 4%
17/05/02 20:47:09 INFO mapreduce.Job:  map 96% reduce 4%
17/05/02 20:47:17 INFO mapreduce.Job:  map 97% reduce 4%
17/05/02 20:47:29 INFO mapreduce.Job:  map 98% reduce 4%
17/05/02 20:47:36 INFO mapreduce.Job:  map 99% reduce 4%
17/05/02 20:47:47 INFO mapreduce.Job:  map 100% reduce 4%
17/05/02 20:47:50 INFO mapreduce.Job:  map 100% reduce 8%
17/05/02 20:47:53 INFO mapreduce.Job:  map 100% reduce 9%
17/05/02 20:47:56 INFO mapreduce.Job:  map 100% reduce 10%
17/05/02 20:47:57 INFO mapreduce.Job:  map 100% reduce 13%
17/05/02 20:47:58 INFO mapreduce.Job:  map 100% reduce 16%
17/05/02 20:47:59 INFO mapreduce.Job:  map 100% reduce 17%
17/05/02 20:48:00 INFO mapreduce.Job:  map 100% reduce 18%
17/05/02 20:48:01 INFO mapreduce.Job:  map 100% reduce 19%
17/05/02 20:48:02 INFO mapreduce.Job:  map 100% reduce 20%
17/05/02 20:48:03 INFO mapreduce.Job:  map 100% reduce 21%
17/05/02 20:48:04 INFO mapreduce.Job:  map 100% reduce 24%
17/05/02 20:48:06 INFO mapreduce.Job:  map 100% reduce 27%
17/05/02 20:48:07 INFO mapreduce.Job:  map 100% reduce 30%
17/05/02 20:48:09 INFO mapreduce.Job:  map 100% reduce 31%
17/05/02 20:48:10 INFO mapreduce.Job:  map 100% reduce 32%
17/05/02 20:48:12 INFO mapreduce.Job:  map 100% reduce 33%
17/05/02 20:48:13 INFO mapreduce.Job:  map 100% reduce 34%
17/05/02 20:48:14 INFO mapreduce.Job:  map 100% reduce 37%
17/05/02 20:48:16 INFO mapreduce.Job:  map 100% reduce 38%
17/05/02 20:48:17 INFO mapreduce.Job:  map 100% reduce 39%
17/05/02 20:48:18 INFO mapreduce.Job:  map 100% reduce 40%
17/05/02 20:48:19 INFO mapreduce.Job:  map 100% reduce 41%
17/05/02 20:48:21 INFO mapreduce.Job:  map 100% reduce 42%
17/05/02 20:48:22 INFO mapreduce.Job:  map 100% reduce 46%
17/05/02 20:48:25 INFO mapreduce.Job:  map 100% reduce 47%
17/05/02 20:48:28 INFO mapreduce.Job:  map 100% reduce 48%
17/05/02 20:48:30 INFO mapreduce.Job:  map 100% reduce 51%
17/05/02 20:48:31 INFO mapreduce.Job:  map 100% reduce 54%
17/05/02 20:48:33 INFO mapreduce.Job:  map 100% reduce 56%
17/05/02 20:48:34 INFO mapreduce.Job:  map 100% reduce 58%
17/05/02 20:48:36 INFO mapreduce.Job:  map 100% reduce 59%
17/05/02 20:48:37 INFO mapreduce.Job:  map 100% reduce 60%
17/05/02 20:48:39 INFO mapreduce.Job:  map 100% reduce 64%
17/05/02 20:48:40 INFO mapreduce.Job:  map 100% reduce 67%
17/05/02 20:48:42 INFO mapreduce.Job:  map 100% reduce 68%
17/05/02 20:48:44 INFO mapreduce.Job:  map 100% reduce 69%
17/05/02 20:48:45 INFO mapreduce.Job:  map 100% reduce 70%
17/05/02 20:48:47 INFO mapreduce.Job:  map 100% reduce 73%
17/05/02 20:48:48 INFO mapreduce.Job:  map 100% reduce 74%
17/05/02 20:48:50 INFO mapreduce.Job:  map 100% reduce 76%
17/05/02 20:48:51 INFO mapreduce.Job:  map 100% reduce 77%
17/05/02 20:48:53 INFO mapreduce.Job:  map 100% reduce 79%
17/05/02 20:48:54 INFO mapreduce.Job:  map 100% reduce 80%
17/05/02 20:48:56 INFO mapreduce.Job:  map 100% reduce 84%
17/05/02 20:48:59 INFO mapreduce.Job:  map 100% reduce 85%
17/05/02 20:49:02 INFO mapreduce.Job:  map 100% reduce 86%
17/05/02 20:49:05 INFO mapreduce.Job:  map 100% reduce 89%
17/05/02 20:49:08 INFO mapreduce.Job:  map 100% reduce 91%
17/05/02 20:49:11 INFO mapreduce.Job:  map 100% reduce 93%
17/05/02 20:49:14 INFO mapreduce.Job:  map 100% reduce 96%
17/05/02 20:49:18 INFO mapreduce.Job:  map 100% reduce 97%
17/05/02 20:49:21 INFO mapreduce.Job:  map 100% reduce 98%
17/05/02 20:49:24 INFO mapreduce.Job:  map 100% reduce 99%
17/05/02 20:49:27 INFO mapreduce.Job:  map 100% reduce 100%
17/05/02 20:49:28 INFO mapreduce.Job: Job job_1493709758444_0006 completed successfully
17/05/02 20:49:28 INFO mapreduce.Job: Counters: 50
	File System Counters
		FILE: Number of bytes read=4478682130
		FILE: Number of bytes written=8892808477
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=10000037500
		HDFS: Number of bytes written=10000000000
		HDFS: Number of read operations=924
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=16
	Job Counters 
		Launched map tasks=300
		Launched reduce tasks=8
		Data-local map tasks=298
		Rack-local map tasks=2
		Total time spent by all maps in occupied slots (ms)=1604325
		Total time spent by all reduces in occupied slots (ms)=415949
		Total time spent by all map tasks (ms)=1604325
		Total time spent by all reduce tasks (ms)=415949
		Total vcore-seconds taken by all map tasks=1604325
		Total vcore-seconds taken by all reduce tasks=415949
		Total megabyte-seconds taken by all map tasks=1642828800
		Total megabyte-seconds taken by all reduce tasks=425931776
	Map-Reduce Framework
		Map input records=100000000
		Map output records=100000000
		Map output bytes=10200000000
		Map output materialized bytes=4375223545
		Input split bytes=37500
		Combine input records=0
		Combine output records=0
		Reduce input groups=100000000
		Reduce shuffle bytes=4375223545
		Reduce input records=100000000
		Reduce output records=100000000
		Spilled Records=200000000
		Shuffled Maps =2400
		Failed Shuffles=0
		Merged Map outputs=2400
		GC time elapsed (ms)=20485
		CPU time spent (ms)=1203340
		Physical memory (bytes) snapshot=144010641408
		Virtual memory (bytes) snapshot=483377561600
		Total committed heap usage (bytes)=175228583936
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters 
		Bytes Read=10000000000
	File Output Format Counters 
		Bytes Written=10000000000
17/05/02 20:49:28 INFO terasort.TeraSort: done

real	13m14.812s
user	0m10.518s
sys	0m1.197s
```
