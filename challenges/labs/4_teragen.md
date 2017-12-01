´´´

[root@host1 CDH5]# HADOOP_USER_NAME=hdfs hdfs dfs -chmod 777 /user/saturn

HADOOP_USER_NAME=saturn time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar teragen 65536000 /user/saturn/tgen

17/12/01 14:23:34 INFO Configuration.deprecation: session.id is deprecated. Instead, use dfs.metrics.session-id
17/12/01 14:23:34 INFO jvm.JvmMetrics: Initializing JVM Metrics with processName=JobTracker, sessionId=
17/12/01 14:23:34 INFO terasort.TeraSort: Generating 65536000 using 1
17/12/01 14:23:34 INFO mapreduce.JobSubmitter: number of splits:1
17/12/01 14:23:34 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_local1424968212_0001
17/12/01 14:23:34 INFO mapreduce.Job: The url to track the job: http://localhost:8080/
17/12/01 14:23:34 INFO mapreduce.Job: Running job: job_local1424968212_0001
17/12/01 14:23:34 INFO mapred.LocalJobRunner: OutputCommitter set in config null
17/12/01 14:23:34 INFO output.FileOutputCommitter: File Output Committer Algorithm version is 1
17/12/01 14:23:34 INFO mapred.LocalJobRunner: OutputCommitter is org.apache.hadoop.mapreduce.lib.output.FileOutputCommitter
17/12/01 14:23:34 INFO mapred.LocalJobRunner: Waiting for map tasks
17/12/01 14:23:34 INFO mapred.LocalJobRunner: Starting task: attempt_local1424968212_0001_m_000000_0
17/12/01 14:23:34 INFO output.FileOutputCommitter: File Output Committer Algorithm version is 1
17/12/01 14:23:34 INFO mapred.Task:  Using ResourceCalculatorProcessTree : [ ]
17/12/01 14:23:34 INFO mapred.MapTask: Processing split: org.apache.hadoop.examples.terasort.TeraGen$RangeInputFormat$RangeInputSplit@407773d4
17/12/01 14:23:35 INFO mapreduce.Job: Job job_local1424968212_0001 running in uber mode : false
17/12/01 14:23:35 INFO mapreduce.Job:  map 0% reduce 0%
17/12/01 14:23:40 INFO mapred.LocalJobRunner: map > map
17/12/01 14:23:41 INFO mapreduce.Job:  map 8% reduce 0%
17/12/01 14:23:43 INFO mapred.LocalJobRunner: map > map
17/12/01 14:23:44 INFO mapreduce.Job:  map 13% reduce 0%
17/12/01 14:23:46 INFO mapred.LocalJobRunner: map > map
17/12/01 14:23:47 INFO mapreduce.Job:  map 17% reduce 0%
17/12/01 14:23:49 INFO mapred.LocalJobRunner: map > map
17/12/01 14:23:50 INFO mapreduce.Job:  map 22% reduce 0%
17/12/01 14:23:52 INFO mapred.LocalJobRunner: map > map
17/12/01 14:23:53 INFO mapreduce.Job:  map 26% reduce 0%
17/12/01 14:23:55 INFO mapred.LocalJobRunner: map > map
17/12/01 14:23:56 INFO mapreduce.Job:  map 30% reduce 0%
17/12/01 14:23:58 INFO mapred.LocalJobRunner: map > map
17/12/01 14:23:59 INFO mapreduce.Job:  map 35% reduce 0%
17/12/01 14:24:01 INFO mapred.LocalJobRunner: map > map
17/12/01 14:24:02 INFO mapreduce.Job:  map 39% reduce 0%
17/12/01 14:24:04 INFO mapred.LocalJobRunner: map > map
17/12/01 14:24:05 INFO mapreduce.Job:  map 44% reduce 0%
17/12/01 14:24:07 INFO mapred.LocalJobRunner: map > map
17/12/01 14:24:08 INFO mapreduce.Job:  map 47% reduce 0%
17/12/01 14:24:10 INFO mapred.LocalJobRunner: map > map
17/12/01 14:24:11 INFO mapreduce.Job:  map 51% reduce 0%
17/12/01 14:24:13 INFO mapred.LocalJobRunner: map > map
17/12/01 14:24:14 INFO mapreduce.Job:  map 54% reduce 0%
17/12/01 14:24:16 INFO mapred.LocalJobRunner: map > map
17/12/01 14:24:17 INFO mapreduce.Job:  map 55% reduce 0%
17/12/01 14:24:19 INFO mapred.LocalJobRunner: map > map
17/12/01 14:24:20 INFO mapreduce.Job:  map 57% reduce 0%
17/12/01 14:24:22 INFO mapred.LocalJobRunner: map > map
17/12/01 14:24:23 INFO mapreduce.Job:  map 59% reduce 0%
17/12/01 14:24:25 INFO mapred.LocalJobRunner: map > map
17/12/01 14:24:26 INFO mapreduce.Job:  map 63% reduce 0%
17/12/01 14:24:28 INFO mapred.LocalJobRunner: map > map
17/12/01 14:24:29 INFO mapreduce.Job:  map 65% reduce 0%
17/12/01 14:24:31 INFO mapred.LocalJobRunner: map > map
17/12/01 14:24:32 INFO mapreduce.Job:  map 67% reduce 0%
17/12/01 14:24:34 INFO mapred.LocalJobRunner: map > map
17/12/01 14:24:35 INFO mapreduce.Job:  map 70% reduce 0%
17/12/01 14:24:37 INFO mapred.LocalJobRunner: map > map
17/12/01 14:24:38 INFO mapreduce.Job:  map 72% reduce 0%
17/12/01 14:24:40 INFO mapred.LocalJobRunner: map > map
17/12/01 14:24:41 INFO mapreduce.Job:  map 74% reduce 0%
17/12/01 14:24:43 INFO mapred.LocalJobRunner: map > map
17/12/01 14:24:44 INFO mapreduce.Job:  map 76% reduce 0%
17/12/01 14:24:46 INFO mapred.LocalJobRunner: map > map
17/12/01 14:24:47 INFO mapreduce.Job:  map 78% reduce 0%
17/12/01 14:24:49 INFO mapred.LocalJobRunner: map > map
17/12/01 14:24:50 INFO mapreduce.Job:  map 81% reduce 0%
17/12/01 14:24:52 INFO mapred.LocalJobRunner: map > map
17/12/01 14:24:53 INFO mapreduce.Job:  map 84% reduce 0%
17/12/01 14:24:55 INFO mapred.LocalJobRunner: map > map
17/12/01 14:24:56 INFO mapreduce.Job:  map 86% reduce 0%
17/12/01 14:24:58 INFO mapred.LocalJobRunner: map > map
17/12/01 14:24:59 INFO mapreduce.Job:  map 88% reduce 0%
17/12/01 14:25:01 INFO mapred.LocalJobRunner: map > map
17/12/01 14:25:02 INFO mapreduce.Job:  map 91% reduce 0%
17/12/01 14:25:04 INFO mapred.LocalJobRunner: map > map
17/12/01 14:25:05 INFO mapreduce.Job:  map 93% reduce 0%
17/12/01 14:25:07 INFO mapred.LocalJobRunner: map > map
17/12/01 14:25:08 INFO mapreduce.Job:  map 95% reduce 0%
17/12/01 14:25:10 INFO mapred.LocalJobRunner: map > map
17/12/01 14:25:11 INFO mapreduce.Job:  map 98% reduce 0%
17/12/01 14:25:13 INFO mapred.LocalJobRunner: map > map
17/12/01 14:25:14 INFO mapred.LocalJobRunner: map > map
17/12/01 14:25:14 INFO mapreduce.Job:  map 99% reduce 0%
17/12/01 14:25:15 INFO mapred.Task: Task:attempt_local1424968212_0001_m_000000_0 is done. And is in the process of committing
17/12/01 14:25:15 INFO mapred.LocalJobRunner: map > map
17/12/01 14:25:15 INFO mapred.Task: Task attempt_local1424968212_0001_m_000000_0 is allowed to commit now
17/12/01 14:25:16 INFO output.FileOutputCommitter: Saved output of task 'attempt_local1424968212_0001_m_000000_0' to hdfs://hosts3.northcentralus.cloudapp.azure.com:8020/user/saturn/tgen/_temporary/0/task_local1424968212_0001_m_000000
17/12/01 14:25:16 INFO mapred.LocalJobRunner: map
17/12/01 14:25:16 INFO mapred.Task: Task 'attempt_local1424968212_0001_m_000000_0' done.
17/12/01 14:25:16 INFO mapred.LocalJobRunner: Finishing task: attempt_local1424968212_0001_m_000000_0
17/12/01 14:25:16 INFO mapred.LocalJobRunner: map task executor complete.
17/12/01 14:25:16 INFO mapreduce.Job:  map 100% reduce 0%
17/12/01 14:25:18 INFO mapreduce.Job: Job job_local1424968212_0001 completed successfully
17/12/01 14:25:18 INFO mapreduce.Job: Counters: 21
	File System Counters
		FILE: Number of bytes read=276333
		FILE: Number of bytes written=566913
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=0
		HDFS: Number of bytes written=6553600000
		HDFS: Number of read operations=4
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=3
	Map-Reduce Framework
		Map input records=65536000
		Map output records=65536000
		Input split bytes=83
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=772
		Total committed heap usage (bytes)=245366784
	org.apache.hadoop.examples.terasort.TeraGen$Counters
		CHECKSUM=140750829423462787
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=6553600000
78.48user 7.68system 1:46.71elapsed 80%CPU (0avgtext+0avgdata 211872maxresident)k
0inputs+3136outputs (0major+99943minor)pagefaults 0swaps


[root@host1 CDH5]# hdfs dfs -ls /user/saturn/tgen
Found 2 items
-rw-r--r--   3 saturn supergroup          0 2017-12-01 14:25 /user/saturn/tgen/_SUCCESS
-rw-r--r--   3 saturn supergroup 6553600000 2017-12-01 14:25 /user/saturn/tgen/part-m-00000


[root@host1 CDH5]# hadoop fsck -blocks /user/saturn
DEPRECATED: Use of this script to execute hdfs command is deprecated.
Instead use the hdfs command for it.

Connecting to namenode via http://hosts3.northcentralus.cloudapp.azure.com:50070
FSCK started by root (auth:SIMPLE) from /10.0.0.9 for path /user/saturn at Fri Dec 01 14:26:38 EST 2017
..Status: HEALTHY
 Total size:	6553600000 B
 Total dirs:	2
 Total files:	2
 Total symlinks:		0
 Total blocks (validated):	49 (avg. block size 133746938 B)
 Minimally replicated blocks:	49 (100.0 %)
 Over-replicated blocks:	0 (0.0 %)
 Under-replicated blocks:	0 (0.0 %)
 Mis-replicated blocks:		0 (0.0 %)
 Default replication factor:	3
 Average block replication:	3.0
 Corrupt blocks:		0
 Missing replicas:		0 (0.0 %)
 Number of data-nodes:		3
 Number of racks:		1
FSCK ended at Fri Dec 01 14:26:38 EST 2017 in 3 milliseconds


The filesystem under path '/user/saturn' is HEALTHY
[root@host1 CDH5]# 

´´´
