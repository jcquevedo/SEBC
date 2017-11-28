<code><b>[raken@hdp1 ~]$ HADOOP_USER_NAME=jcquevedo hadoop fs -mkdir /user/jcquevedo/precious</b></code><br>
<code><b>[raken@hdp1 ~]$ hadoop fs -ls /user/jcquevedo</b></code><br>
Found 4 items<br>
drwx------   - jcquevedo supergroup          0 2017-11-28 11:47 /user/jcquevedo/.staging<br>
drwxr-xr-x   - jcquevedo supergroup          0 2017-11-28 12:19 /user/jcquevedo/precious<br>
drwxr-xr-x   - jcquevedo supergroup          0 2017-11-28 11:34 /user/jcquevedo/<br>teragen-10gb-test-3<br>
drwxr-xr-x   - jcquevedo supergroup          0 2017-11-28 11:47 /user/jcquevedo/<br>terasortjcquevedo<br>
[raken@hdp1 ~]$ <br>


<code><b>[raken@hdp1 ~]$ HADOOP_USER_NAME=jcquevedo hadoop fs -put SEBC-master.zip /user/jcquevedo/precious/</b></code><br>
<code><b>[raken@hdp1 ~]$ hadoop fs -ls /user/jcquevedo/precious</b></code><br>
Found 1 items<br>
-rw-r--r--   3 jcquevedo supergroup     474833 2017-11-28 12:31 /user/jcquevedo/precious/<br>SEBC-master.zip<br>
[raken@hdp1 ~]$ 


<code><b>[raken@hdp1 ~]$ HADOOP_USER_NAME=jcquevedo hadoop fs -rm /user/jcquevedo/precious/</b></code><br>
rm: `/user/jcquevedo/precious': Is a directory<br>

<code><b>[raken@hdp1 ~]$ HADOOP_USER_NAME=jcquevedo hadoop fs -rm -R /user/jcquevedo/precious/</b></code><br>
rm: Failed to move to trash: hdfs://hdp1.northcentralus.cloudapp.azure.com:8020/user/jcquevedo/precious: The directory /user/jcquevedo/precious cannot be deleted since /user/jcquevedo/precious is snapshottable and already has snapshots<br>

<code><b>[raken@hdp1 ~]$ HADOOP_USER_NAME=jcquevedo hadoop fs -rm /user/jcquevedo/precious/SEBC-master.zip</b></code><br>
17/11/28 12:50:47 INFO fs.TrashPolicyDefault: Moved: 'hdfs://hdp1.northcentralus.cloudapp.azure.com:8020/user/jcquevedo/precious/SEBC-master.zip' to trash at: hdfs://hdp1.northcentralus.cloudapp.azure.com:8020/user/jcquevedo/.Trash/Current/user/jcquevedo/precious/SEBC-master.zip<br>
[raken@hdp1 ~]$ 


