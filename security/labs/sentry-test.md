<code><b>[raken@hdp4 ~]$ beeline</b></code><br>
Beeline version 1.1.0-cdh5.9.1 by Apache Hive<br>
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/<br>hdp4.northcentralus.cloudapp.azure.com@RAKENHDP.COM<br>
scan complete in 2ms<br>
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/<br>hdp4.northcentralus.cloudapp.azure.com@RAKENHDP.COM<br>
Connected to: Apache Hive (version 1.1.0-cdh5.9.1)<br>
Driver: Hive JDBC (version 1.1.0-cdh5.9.1)<br>
Transaction isolation: TRANSACTION_REPEATABLE_READ<br>
0: jdbc:hive2://localhost:10000/default> show tables;<br>
INFO  : Compiling command(queryId=hive_20171129200202_b8a8311d-e10a-47d9-85e3-7e5e9093cc1c):
show tables<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129200202_b8a8311d-e10a-47d9-85e3-7e5e9093cc1c); Time taken: 0.679 seconds<br>
INFO  : Executing command(queryId=hive_20171129200202_b8a8311d-e10a-47d9-85e3-7e5e9093cc1c): show tables<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129200202_b8a8311d-e10a-47d9-85e3-7e5e9093cc1c); Time taken: 0.282 seconds<br>
INFO  : OK<br>
+-----------+--+<br>
| tab_name  |<br>
+-----------+--+<br>
+-----------+--+<br>
No rows selected (2.352 seconds)<br>
0: jdbc:hive2://localhost:10000/default> <br>

