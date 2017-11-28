<b>We create user jcquevedo in all nodes:</b><br>

<code>[raken@hdp1 ~]$ sudo useradd jcquevedo<br>
<br>[raken@hdp1 ~]$ sudo passwd jcquevedo<br></code><br>
Changing password for user jcquevedo.
New password: 
Retype new password: 
passwd: all authentication tokens updated successfully.
<br>[raken@hdp1 ~]$ 

<code><br><b>[raken@hdp1 ~]$ HADOOP_USER_NAME=hdfs hadoop fs -mkdir /user/jcquevedo<br>
<br>[raken@hdp1 ~]$ hadoop fs -ls /user</b></code><br>
Found 5 items<br>
drwxrwxrwx   - mapred hadoop              0 2017-11-27 21:15 /user/history<br>
drwxrwxr-t   - hive   hive                0 2017-11-27 21:16 /user/hive<br>
drwxrwxr-x   - hue    hue                 0 2017-11-27 21:17 /user/hue<br>
drwxr-xr-x   - hdfs   supergroup          0 2017-11-28 11:10 /user/jcquevedo<br>
drwxrwxr-x   - oozie  oozie               0 2017-11-27 21:17 /user/oozie<br>
[raken@hdp1 ~]$ HADOOP_USER_NAME=hdfs hadoop fs -chown -R jcquevedo:supergroup /user/jcquevedo
[raken@hdp1 ~]$ hadoop fs -ls /user
Found 5 items<br>
drwxrwxrwx   - mapred    hadoop              0 2017-11-27 21:15 /user/history<br>
drwxrwxr-t   - hive      hive                0 2017-11-27 21:16 /user/hive<br>
drwxrwxr-x   - hue       hue                 0 2017-11-27 21:17 /user/hue<br>
drwxr-xr-x   - jcquevedo supergroup          0 2017-11-28 11:10 /user/jcquevedo<br>
drwxrwxr-x   - oozie     oozie               0 2017-11-27 21:17 /user/oozie<br>
<br><br>

<code><b>[raken@hdp1 ~]$ HADOOP_USER_NAME=jcquevedo time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar teragen 100000000 /user/jcquevedo/teragen-10gb-test-3</b><br></code><br>
17/11/28 11:32:38 INFO client.RMProxy: Connecting to ResourceManager at hdp2.northcentralus.cloudapp.azure.com/10.0.0.6:8032<br>
17/11/28 11:32:38 INFO terasort.TeraSort: Generating 100000000 using 2
17/11/28 11:32:38 INFO mapreduce.JobSubmitter: number of splits:2<br>
17/11/28 11:32:39 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1511835348102_0001<br>
17/11/28 11:32:39 INFO impl.YarnClientImpl: Submitted application application_1511835348102_0001<br>
17/11/28 11:32:39 INFO mapreduce.Job: The url to track the job: http://hdp2.northcentralus.cloudapp.azure.com:8088/proxy/application_1511835348102_0001</br>
17/11/28 11:32:39 INFO mapreduce.Job: Running job: job_1511835348102_0001<br>
17/11/28 11:32:46 INFO mapreduce.Job: Job job_1511835348102_0001 running in uber mode : false<br>
17/11/28 11:32:46 INFO mapreduce.Job:  map 0% reduce 0%<br>
17/11/28 11:32:57 INFO mapreduce.Job:  map 8% reduce 0%<br>
17/11/28 11:33:00 INFO mapreduce.Job:  map 13% reduce 0%<br>
17/11/28 11:33:03 INFO mapreduce.Job:  map 18% reduce 0%<br>
17/11/28 11:33:07 INFO mapreduce.Job:  map 23% reduce 0%<br>
17/11/28 11:33:10 INFO mapreduce.Job:  map 28% reduce 0%<br>
17/11/28 11:33:13 INFO mapreduce.Job:  map 32% reduce 0%<br>
17/11/28 11:33:16 INFO mapreduce.Job:  map 37% reduce 0%<br>
17/11/28 11:33:19 INFO mapreduce.Job:  map 41% reduce 0%<br>
17/11/28 11:33:22 INFO mapreduce.Job:  map 45% reduce 0%<br>
17/11/28 11:33:25 INFO mapreduce.Job:  map 49% reduce 0%<br>
17/11/28 11:33:28 INFO mapreduce.Job:  map 52% reduce 0%<br>
17/11/28 11:33:32 INFO mapreduce.Job:  map 57% reduce 0%<br>
17/11/28 11:33:35 INFO mapreduce.Job:  map 60% reduce 0%<br>
17/11/28 11:33:38 INFO mapreduce.Job:  map 64% reduce 0%<br>
17/11/28 11:33:41 INFO mapreduce.Job:  map 68% reduce 0%<br>
17/11/28 11:33:44 INFO mapreduce.Job:  map 70% reduce 0%<br>
17/11/28 11:33:47 INFO mapreduce.Job:  map 72% reduce 0%<br>
17/11/28 11:33:50 INFO mapreduce.Job:  map 73% reduce 0%<br>
17/11/28 11:33:53 INFO mapreduce.Job:  map 74% reduce 0%<br>
17/11/28 11:33:56 INFO mapreduce.Job:  map 75% reduce 0%<br>
17/11/28 11:33:59 INFO mapreduce.Job:  map 76% reduce 0%<br>
17/11/28 11:34:02 INFO mapreduce.Job:  map 77% reduce 0%<br>
17/11/28 11:34:05 INFO mapreduce.Job:  map 79% reduce 0%<br>
17/11/28 11:34:08 INFO mapreduce.Job:  map 80% reduce 0%<br>
17/11/28 11:34:11 INFO mapreduce.Job:  map 82% reduce 0%<br>
17/11/28 11:34:14 INFO mapreduce.Job:  map 83% reduce 0%<br>
17/11/28 11:34:17 INFO mapreduce.Job:  map 85% reduce 0%<br>
17/11/28 11:34:20 INFO mapreduce.Job:  map 86% reduce 0%<br>
17/11/28 11:34:24 INFO mapreduce.Job:  map 87% reduce 0%<br>
17/11/28 11:34:27 INFO mapreduce.Job:  map 89% reduce 0%<br>
17/11/28 11:34:30 INFO mapreduce.Job:  map 90% reduce 0%<br>
17/11/28 11:34:33 INFO mapreduce.Job:  map 92% reduce 0%<br>
17/11/28 11:34:36 INFO mapreduce.Job:  map 94% reduce 0%<br>
17/11/28 11:34:39 INFO mapreduce.Job:  map 95% reduce 0%<br>
17/11/28 11:34:42 INFO mapreduce.Job:  map 96% reduce 0%<br>
17/11/28 11:34:45 INFO mapreduce.Job:  map 97% reduce 0%<br>
17/11/28 11:34:48 INFO mapreduce.Job:  map 99% reduce 0%<br>
17/11/28 11:34:51 INFO mapreduce.Job:  map 100% reduce 0%<br>
17/11/28 11:34:51 INFO mapreduce.Job: Job job_1511835348102_0001 completed successfully<br>
17/11/28 11:34:51 INFO mapreduce.Job: Counters: 31<br>
	File System Counters<br>
		FILE: Number of bytes read=0<br>
		FILE: Number of bytes written=245822<br>
		FILE: Number of read operations=0<br>
		FILE: Number of large read operations=0<br>
		FILE: Number of write operations=0<br>
		HDFS: Number of bytes read=170<br>
		HDFS: Number of bytes written=10000000000<br>
		HDFS: Number of read operations=8<br>
		HDFS: Number of large read operations=0<br>
		HDFS: Number of write operations=4<br>
	Job Counters <br>
		Launched map tasks=2<br>
		Other local map tasks=2<br>
		Total time spent by all maps in occupied slots (ms)=245247<br>
		Total time spent by all reduces in occupied slots (ms)=0<br>
		Total time spent by all map tasks (ms)=245247<br>
		Total vcore-seconds taken by all map tasks=245247<br>
		Total megabyte-seconds taken by all map tasks=251132928<br>
	Map-Reduce Framework<br>
		Map input records=100000000<br>
		Map output records=100000000<br>
		Input split bytes=170<br>
		Spilled Records=0<br>
		Failed Shuffles=0<br>
		Merged Map outputs=0<br>
		GC time elapsed (ms)=1553<br>
		CPU time spent (ms)=154050<br>
		Physical memory (bytes) snapshot=355647488<br>
		Virtual memory (bytes) snapshot=3176267776<br>
		Total committed heap usage (bytes)=801112064<br>
	org.apache.hadoop.examples.terasort.TeraGen$Counters<br>
		CHECKSUM=214760662691937609<br>
	File Input Format Counters <br>
		Bytes Read=0<br>
	File Output Format Counters <br>
		Bytes Written=10000000000<br>
5.00user 0.31system 2:15.59elapsed 3%CPU (0avgtext+0avgdata 248040maxresident)k
0inputs+2032outputs (0major+67816minor)pagefaults 0swaps<br>
<br>
<code><b>[raken@hdp1 ~]$ hadoop fs -ls /user/jcquevedo</b></code><br>
Found 2 items
drwx------   - jcquevedo supergroup          0 2017-11-28 11:34 /user/jcquevedo/.staging<br>
drwxr-xr-x   - jcquevedo supergroup          0 2017-11-28 11:34 /user/jcquevedo/teragen-10gb-test-3<br>

<br><br><br>

<code><b>[raken@hdp1 ~]$ HADOOP_USER_NAME=jcquevedo time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar terasort /user/jcquevedo/teragen-10gb-test-3 /user/jcquevedo/terasortjcquevedo</b></code><br>
17/11/28 11:44:43 INFO terasort.TeraSort: starting<br>
17/11/28 11:44:44 INFO input.FileInputFormat: Total input paths to process : 2<br>
Spent 165ms computing base-splits.<br>
Spent 3ms computing TeraScheduler splits.<br>
Computing input splits took 168ms<br>
Sampling 10 splits of 76<br>
Making 12 from 100000 sampled records<br>
Computing parititions took 602ms<br>
Spent 773ms computing partitions.<br>
17/11/28 11:44:45 INFO client.RMProxy: Connecting to ResourceManager at hdp2.northcentralus.cloudapp.azure.com/10.0.0.6:8032<br>
17/11/28 11:44:46 INFO mapreduce.JobSubmitter: number of splits:76<br>
17/11/28 11:44:46 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1511835348102_0002<br>
17/11/28 11:44:46 INFO impl.YarnClientImpl: Submitted application application_1511835348102_0002<br>
17/11/28 11:44:46 INFO mapreduce.Job: The url to track the job: http://hdp2.northcentralus.cloudapp.azure.com:8088/proxy/application_1511835348102_0002/<br>
17/11/28 11:44:46 INFO mapreduce.Job: Running job: job_1511835348102_0002<br>
17/11/28 11:44:52 INFO mapreduce.Job: Job job_1511835348102_0002 running in uber mode : false<br>
17/11/28 11:44:52 INFO mapreduce.Job:  map 0% reduce 0%<br>
17/11/28 11:45:06 INFO mapreduce.Job:  map 1% reduce 0%<br>
17/11/28 11:45:07 INFO mapreduce.Job:  map 5% reduce 0%<br>
17/11/28 11:45:08 INFO mapreduce.Job:  map 10% reduce 0%<br>
17/11/28 11:45:09 INFO mapreduce.Job:  map 18% reduce 0%<br>
17/11/28 11:45:10 INFO mapreduce.Job:  map 22% reduce 0%<br>
17/11/28 11:45:11 INFO mapreduce.Job:  map 23% reduce 0%<br>
17/11/28 11:45:12 INFO mapreduce.Job:  map 25% reduce 0%<br>
17/11/28 11:45:13 INFO mapreduce.Job:  map 30% reduce 0%<br>
17/11/28 11:45:23 INFO mapreduce.Job:  map 34% reduce 0%<br>
17/11/28 11:45:25 INFO mapreduce.Job:  map 36% reduce 0%<br>
17/11/28 11:45:26 INFO mapreduce.Job:  map 40% reduce 0%<br>
17/11/28 11:45:27 INFO mapreduce.Job:  map 42% reduce 0%<br>
17/11/28 11:45:28 INFO mapreduce.Job:  map 46% reduce 0%<br>
17/11/28 11:45:29 INFO mapreduce.Job:  map 54% reduce 0%<br>
17/11/28 11:45:31 INFO mapreduce.Job:  map 55% reduce 0%<br>
17/11/28 11:45:32 INFO mapreduce.Job:  map 58% reduce 0%<br>
17/11/28 11:45:33 INFO mapreduce.Job:  map 61% reduce 0%<br>
17/11/28 11:45:40 INFO mapreduce.Job:  map 62% reduce 0%<br>
17/11/28 11:45:41 INFO mapreduce.Job:  map 64% reduce 0%<br>
17/11/28 11:45:43 INFO mapreduce.Job:  map 67% reduce 0%<br>
17/11/28 11:45:44 INFO mapreduce.Job:  map 68% reduce 0%<br>
17/11/28 11:45:46 INFO mapreduce.Job:  map 72% reduce 0%<br>
17/11/28 11:45:47 INFO mapreduce.Job:  map 74% reduce 0%<br>
17/11/28 11:45:48 INFO mapreduce.Job:  map 79% reduce 0%<br>
17/11/28 11:45:49 INFO mapreduce.Job:  map 84% reduce 0%<br>
17/11/28 11:45:51 INFO mapreduce.Job:  map 87% reduce 0%<br>
17/11/28 11:45:52 INFO mapreduce.Job:  map 91% reduce 0%<br>
17/11/28 11:45:56 INFO mapreduce.Job:  map 93% reduce 0%<br>
17/11/28 11:45:57 INFO mapreduce.Job:  map 95% reduce 0%<br>
17/11/28 11:45:58 INFO mapreduce.Job:  map 96% reduce 0%<br>
17/11/28 11:45:59 INFO mapreduce.Job:  map 98% reduce 0%<br>
17/11/28 11:46:00 INFO mapreduce.Job:  map 99% reduce 0%<br>
17/11/28 11:46:01 INFO mapreduce.Job:  map 100% reduce 0%<br>
17/11/28 11:46:05 INFO mapreduce.Job:  map 100% reduce 8%<br>
17/11/28 11:46:07 INFO mapreduce.Job:  map 100% reduce 17%<br>
17/11/28 11:46:08 INFO mapreduce.Job:  map 100% reduce 25%<br>
17/11/28 11:46:11 INFO mapreduce.Job:  map 100% reduce 30%<br>
17/11/28 11:46:13 INFO mapreduce.Job:  map 100% reduce 34%<br>
17/11/28 11:46:14 INFO mapreduce.Job:  map 100% reduce 43%<br>
17/11/28 11:46:15 INFO mapreduce.Job:  map 100% reduce 44%<br>
17/11/28 11:46:17 INFO mapreduce.Job:  map 100% reduce 47%<br>
17/11/28 11:46:18 INFO mapreduce.Job:  map 100% reduce 51%<br>
17/11/28 11:46:20 INFO mapreduce.Job:  map 100% reduce 71%<br>
17/11/28 11:46:21 INFO mapreduce.Job:  map 100% reduce 72%<br>
17/11/28 11:46:23 INFO mapreduce.Job:  map 100% reduce 75%<br>
17/11/28 11:46:24 INFO mapreduce.Job:  map 100% reduce 77%<br>
17/11/28 11:46:26 INFO mapreduce.Job:  map 100% reduce 80%<br>
17/11/28 11:46:27 INFO mapreduce.Job:  map 100% reduce 81%<br>
17/11/28 11:46:29 INFO mapreduce.Job:  map 100% reduce 85%<br>
17/11/28 11:46:32 INFO mapreduce.Job:  map 100% reduce 88%<br>
17/11/28 11:46:35 INFO mapreduce.Job:  map 100% reduce 89%<br>
17/11/28 11:46:39 INFO mapreduce.Job:  map 100% reduce 90%<br>
17/11/28 11:46:42 INFO mapreduce.Job:  map 100% reduce 91%<br>
17/11/28 11:46:44 INFO mapreduce.Job:  map 100% reduce 92%<br>
17/11/28 11:46:56 INFO mapreduce.Job:  map 100% reduce 93%<br>
17/11/28 11:47:02 INFO mapreduce.Job:  map 100% reduce 94%<br>
17/11/28 11:47:11 INFO mapreduce.Job:  map 100% reduce 95%<br>
17/11/28 11:47:17 INFO mapreduce.Job:  map 100% reduce 96%<br>
17/11/28 11:47:23 INFO mapreduce.Job:  map 100% reduce 97%<br>
17/11/28 11:47:29 INFO mapreduce.Job:  map 100% reduce 98%<br>
17/11/28 11:47:35 INFO mapreduce.Job:  map 100% reduce 99%<br>
17/11/28 11:47:41 INFO mapreduce.Job:  map 100% reduce 100%<br>
17/11/28 11:47:44 INFO mapreduce.Job: Job job_1511835348102_0002 completed successfully<br>
17/11/28 11:47:44 INFO mapreduce.Job: Counters: 49<br>
	File System Counters<br>
		FILE: Number of bytes read=4442516576<br>
		FILE: Number of bytes written=8824331622<br>
		FILE: Number of read operations=0<br>
		FILE: Number of large read operations=0<br>
		FILE: Number of write operations=0<br>
		HDFS: Number of bytes read=10000012388<br>
		HDFS: Number of bytes written=10000000000<br>
		HDFS: Number of read operations=264<br>
		HDFS: Number of large read operations=0<br>
		HDFS: Number of write operations=24<br>
	Job Counters <br>
		Launched map tasks=76<br>
		Launched reduce tasks=12<br>
		Data-local map tasks=76<br>
		Total time spent by all maps in occupied slots (ms)=1292589<br>
		Total time spent by all reduces in occupied slots (ms)=982434<br>
		Total time spent by all map tasks (ms)=1292589<br>
		Total time spent by all reduce tasks (ms)=982434<br>
		Total vcore-seconds taken by all map tasks=1292589<br>
		Total vcore-seconds taken by all reduce tasks=982434<br>
		Total megabyte-seconds taken by all map tasks=1323611136<br>
		Total megabyte-seconds taken by all reduce tasks=1006012416<br>
	Map-Reduce Framework<br>
		Map input records=100000000<br>
		Map output records=100000000<br>
		Map output bytes=10200000000<br>
		Map output materialized bytes=4370860826<br>
		Input split bytes=12388<br>
		Combine input records=0<br>
		Combine output records=0<br>
		Reduce input groups=100000000<br>
		Reduce shuffle bytes=4370860826<br>
		Reduce input records=100000000<br>
		Reduce output records=100000000<br>
		Spilled Records=200000000<br>
		Shuffled Maps =912<br>
		Failed Shuffles=0<br>
		Merged Map outputs=912<br>
		GC time elapsed (ms)=31997<br>
		CPU time spent (ms)=1129740<br>
		Physical memory (bytes) snapshot=54048014336<br>
		Virtual memory (bytes) snapshot=140457549824<br>
		Total committed heap usage (bytes)=55225352192<br>
	Shuffle Errors<br>
		BAD_ID=0<br>
		CONNECTION=0<br>
		IO_ERROR=0<br>
		WRONG_LENGTH=0<br>
		WRONG_MAP=0<br>
		WRONG_REDUCE=0<br>
	File Input Format Counters <br>
		Bytes Read=10000000000<br>
	File Output Format Counters <br>
		Bytes Written=10000000000<br>
17/11/28 11:47:44 INFO terasort.TeraSort: done<br>
7.31user 0.42system 3:01.80elapsed 4%CPU (0avgtext+0avgdata 248080maxresident)k
0inputs+2136outputs (0major+67234minor)pagefaults 0swaps<br>
<br>
<code><b>[raken@hdp1 ~]$ hadoop fs -ls /user/jcquevedo</b></code><br>
Found 3 items
drwx------   - jcquevedo supergroup          0 2017-11-28 11:47 /user/jcquevedo/.staging<br>
drwxr-xr-x   - jcquevedo supergroup          0 2017-11-28 11:34 /user/jcquevedo/teragen-10gb-test-3<br>
drwxr-xr-x   - jcquevedo supergroup          0 2017-11-28 11:47 /user/jcquevedo/terasortjcquevedo<br>
[raken@hdp1 ~]$ 







<br>