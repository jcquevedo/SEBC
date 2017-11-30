<code><b>[raken@hdp4 ~]$ beeline</b></code><br>
Beeline version 1.1.0-cdh5.9.1 by Apache Hive<br>
<code><b>beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/hdp4.northcentralus.cloudapp.azure.com@RAKENHDP.COM</b></code><br>
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


<code><b>[raken@hdp4 ~]$ beeline</b></code><br>
0: jdbc:hive2://localhost:10000/default> CREATE ROLE sentry_admin;<br>
INFO  : Compiling command(queryId=hive_20171129202828_28511b96-4c39-4966-964c-1745fbdc4a7e): CREATE ROLE sentry_admin<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129202828_28511b96-4c39-4966-964c-1745fbdc4a7e); Time taken: 0.069 seconds<br>
INFO  : Executing command(queryId=hive_20171129202828_28511b96-4c39-4966-964c-1745fbdc4a7e): CREATE ROLE sentry_admin<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129202828_28511b96-4c39-4966-964c-1745fbdc4a7e); Time taken: 0.936 seconds<br>
INFO  : OK<br>
No rows affected (1.024 seconds)<br>

<code><b>0: jdbc:hive2://localhost:10000/default> GRANT ALL ON SERVER server1 TO ROLE sentry_admin;</b></code><br>
INFO  : Compiling command(queryId=hive_20171129202929_4548e115-1dc7-44fd-95a6-4042e865d8d6): GRANT ALL ON SERVER server1 TO ROLE sentry_admin<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129202929_4548e115-1dc7-44fd-95a6-4042e865d8d6); Time taken: 0.069 seconds<br>
INFO  : Executing command(queryId=hive_20171129202929_4548e115-1dc7-44fd-95a6-4042e865d8d6): GRANT ALL ON SERVER server1 TO ROLE sentry_admin<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129202929_4548e115-1dc7-44fd-95a6-4042e865d8d6); Time taken: 0.173 seconds<br>
INFO  : OK<br>
No rows affected (0.259 seconds)<br>

<code><b>0: jdbc:hive2://localhost:10000/default> GRANT ROLE sentry_admin TO GROUP jcquevedo;</b></code><br>
INFO  : Compiling command(queryId=hive_20171129203030_8b683e46-4c44-4608-9b1e-8a07cff14570): GRANT ROLE sentry_admin TO GROUP jcquevedo<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129203030_8b683e46-4c44-4608-9b1e-8a07cff14570); Time taken: 0.077 seconds<br>
INFO  : Executing command(queryId=hive_20171129203030_8b683e46-4c44-4608-9b1e-8a07cff14570): GRANT ROLE sentry_admin TO GROUP jcquevedo<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129203030_8b683e46-4c44-4608-9b1e-8a07cff14570); Time taken: 0.125 seconds<br>
INFO  : OK<br>
No rows affected (0.215 seconds)<br>
<code><b>0: jdbc:hive2://localhost:10000/default> show tables;</b></code><br>
INFO  : Compiling command(queryId=hive_20171129203030_0f4195b6-2af3-4e43-bbb5-d4f0a118d1d9): show tables<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129203030_0f4195b6-2af3-4e43-bbb5-d4f0a118d1d9); Time taken: 0.189 seconds<br>
INFO  : Executing command(queryId=hive_20171129203030_0f4195b6-2af3-4e43-bbb5-d4f0a118d1d9): show tables<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129203030_0f4195b6-2af3-4e43-bbb5-d4f0a118d1d9); Time taken: 0.205 seconds<br>
INFO  : OK<br>
+------------+--+<br>
|  tab_name  |<br>
+------------+--+<br>
| customers  |<br>
| sample_07  |<br>
| sample_08  |<br>
| web_logs   |<br>
+------------+--+<br>

4 rows selected (0.452 seconds)<br>
0: jdbc:hive2://localhost:10000/default> <br>

<code><b>0: jdbc:hive2://localhost:10000/default> CREATE ROLE reads;</b></code><br>
INFO  : Compiling command(queryId=hive_20171129203434_c0893927-934e-4eca-8c42-97b9bb0c725d): CREATE ROLE reads<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129203434_c0893927-934e-4eca-8c42-97b9bb0c725d); Time taken: 0.085 seconds<br>
INFO  : Executing command(queryId=hive_20171129203434_c0893927-934e-4eca-8c42-97b9bb0c725d): CREATE ROLE reads<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129203434_c0893927-934e-4eca-8c42-97b9bb0c725d); Time taken: 0.155 seconds<br>
INFO  : OK<br>
No rows affected (0.255 seconds)<br>
<code><b>0: jdbc:hive2://localhost:10000/default> CREATE ROLE writes;</b></code><br>
INFO  : Compiling command(queryId=hive_20171129203434_5d140428-43d0-419f-b691-6a26c9f72dd7): CREATE ROLE writes<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129203434_5d140428-43d0-419f-b691-6a26c9f72dd7); Time taken: 0.067 seconds<br>
INFO  : Executing command(queryId=hive_20171129203434_5d140428-43d0-419f-b691-6a26c9f72dd7): CREATE ROLE writes<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129203434_5d140428-43d0-419f-b691-6a26c9f72dd7); Time taken: 0.086 seconds<br>
INFO  : OK<br>
No rows affected (0.17 seconds)<br>
<code><b>0: jdbc:hive2://localhost:10000/default> GRANT SELECT ON DATABASE default TO ROLE reads;</b></code><br>
INFO  : Compiling command(queryId=hive_20171129203535_c6659437-d13d-4134-9c41-c2b28caa8689): GRANT SELECT ON DATABASE default TO ROLE reads<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129203535_c6659437-d13d-4134-9c41-c2b28caa8689); Time taken: 0.065 seconds<br>
INFO  : Executing command(queryId=hive_20171129203535_c6659437-d13d-4134-9c41-c2b28caa8689): GRANT SELECT ON DATABASE default TO ROLE reads<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129203535_c6659437-d13d-4134-9c41-c2b28caa8689); Time taken: 0.166 seconds<br>
INFO  : OK<br>
No rows affected (0.246 seconds)<br>
<code><b>0: jdbc:hive2://localhost:10000/default> GRANT ROLE reads TO GROUP selector;</b></code><br>
INFO  : Compiling command(queryId=hive_20171129203535_9ea28c28-827d-4cd7-9983-87f0e033918b): GRANT ROLE reads TO GROUP selector<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129203535_9ea28c28-827d-4cd7-9983-87f0e033918b); Time taken: 0.065 seconds<br>
INFO  : Executing command(queryId=hive_20171129203535_9ea28c28-827d-4cd7-9983-87f0e033918b): GRANT ROLE reads TO GROUP selector<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129203535_9ea28c28-827d-4cd7-9983-87f0e033918b); Time taken: 0.174 seconds<br>
INFO  : OK<br>
No rows affected (0.251 seconds)<br>

<code><b>0: jdbc:hive2://localhost:10000/default> REVOKE ALL ON DATABASE default FROM ROLE writes;</b></code><br>
INFO  : Compiling command(queryId=hive_20171129203636_18faeee4-894e-4e93-b7f4-f21d37f96da3): REVOKE ALL ON DATABASE default FROM ROLE writes<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129203636_18faeee4-894e-4e93-b7f4-f21d37f96da3); Time taken: 0.06 seconds<br>
INFO  : Executing command(queryId=hive_20171129203636_18faeee4-894e-4e93-b7f4-f21d37f96da3): REVOKE ALL ON DATABASE default FROM ROLE writes<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129203636_18faeee4-894e-4e93-b7f4-f21d37f96da3); Time taken: 0.218 seconds<br>
INFO  : OK<br>
No rows affected (0.294 seconds)<br>

<code><b>0: jdbc:hive2://localhost:10000/default> GRANT SELECT ON default.sample_07 TO ROLE writes;</b></code><br>
INFO  : Compiling command(queryId=hive_20171129203636_70c14661-d4af-4d4f-8d83-268e83bde5db): GRANT SELECT ON default.sample_07 TO ROLE writes<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129203636_70c14661-d4af-4d4f-8d83-268e83bde5db); Time taken: 0.058 seconds<br>
INFO  : Executing command(queryId=hive_20171129203636_70c14661-d4af-4d4f-8d83-268e83bde5db): GRANT SELECT ON default.sample_07 TO ROLE writes<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129203636_70c14661-d4af-4d4f-8d83-268e83bde5db); Time taken: 0.063 seconds<br>
INFO  : OK<br>
No rows affected (0.136 seconds)<br>

<code><b>0: jdbc:hive2://localhost:10000/default> GRANT ROLE writes TO GROUP inserters;</b></code><br>
INFO  : Compiling command(queryId=hive_20171129203636_5c2cfa43-27bf-47ab-be7c-2079c245cbc3): GRANT ROLE writes TO GROUP inserters<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129203636_5c2cfa43-27bf-47ab-be7c-2079c245cbc3); Time taken: 0.061 seconds<br>
INFO  : Executing command(queryId=hive_20171129203636_5c2cfa43-27bf-47ab-be7c-2079c245cbc3): GRANT ROLE writes TO GROUP inserters<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129203636_5c2cfa43-27bf-47ab-be7c-2079c245cbc3); Time taken: 0.066 seconds<br>
INFO  : OK<br>
No rows affected (0.141 seconds)<br>
0: jdbc:hive2://localhost:10000/default> <br>

<code><b>[raken@hdp4 ~]$ kinit george</b></code><br>
Password for george@RAKENHDP.COM: <br>
<code><b>[[raken@hdp4 ~]$ klist</b></code><br>
Ticket cache: FILE:/tmp/krb5cc_1000<br>
Default principal: george@RAKENHDP.COM<br>

Valid starting     Expires            Service principal<br>
11/29/17 20:44:50  11/30/17 20:44:50  krbtgt/RAKENHDP.COM@RAKENHDP.COM<br>
	renew until 12/06/17 20:44:50<br>
<code><b>[raken@hdp4 ~]$ beeline</b></code><br>
Beeline version 1.1.0-cdh5.9.1 by Apache Hive<br>
<code><b>beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/hdp4.northcentralus.cloudapp.azure.com@RAKENHDP.COM</b></code><br>
scan complete in 3ms<br>
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/hdp4.northcentralus.cloudapp.azure.com@RAKENHDP.COM<br>
Connected to: Apache Hive (version 1.1.0-cdh5.9.1)<br>
Driver: Hive JDBC (version 1.1.0-cdh5.9.1)<br>
Transaction isolation: TRANSACTION_REPEATABLE_READ<br>
<code><b>0: jdbc:hive2://localhost:10000/default> show tables;</b></code><br>
INFO  : Compiling command(queryId=hive_20171129204747_977e022d-328c-4492-8f54-dcf7959c3b1b): show tables<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129204747_977e022d-328c-4492-8f54-dcf7959c3b1b); Time taken: 0.081 seconds<br>
INFO  : Executing command(queryId=hive_20171129204747_977e022d-328c-4492-8f54-dcf7959c3b1b): show tables<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129204747_977e022d-328c-4492-8f54-dcf7959c3b1b); Time taken: 0.186 seconds<br>
INFO  : OK<br>
+------------+--+<br>
|  tab_name  |<br>
+------------+--+<br>
| customers  |<br>
| sample_07  |<br>
| sample_08  |<br>
| web_logs   |<br>
+------------+--+<br>
4 rows selected (0.392 seconds)<br>
0: jdbc:hive2://localhost:10000/default> <br>


<code><b>[raken@hdp4 ~]$ kinit ferdinand</b></code><br>
Password for ferdinand@RAKENHDP.COM: <br>
<code><b>[raken@hdp4 ~]$ klist</b></code><br>
Ticket cache: FILE:/tmp/krb5cc_1000<br>
Default principal: ferdinand@RAKENHDP.COM<br>

Valid starting     Expires            Service principal<br>
11/29/17 20:48:53  11/30/17 20:48:53  krbtgt/RAKENHDP.COM@RAKENHDP.COM<br>
	renew until 12/06/17 20:48:53<br>
<code><b>[raken@hdp4 ~]$ beeline</b></code><br>
Beeline version 1.1.0-cdh5.9.1 by Apache Hive<br>
<code><b>beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/hdp4.northcentralus.cloudapp.azure.com@RAKENHDP.COM</b></code><br>
scan complete in 2ms<br>
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/hdp4.northcentralus.cloudapp.azure.com@RAKENHDP.COM<br>
Connected to: Apache Hive (version 1.1.0-cdh5.9.1)<br>
Driver: Hive JDBC (version 1.1.0-cdh5.9.1)<br>
Transaction isolation: TRANSACTION_REPEATABLE_READ<br>
<code><b>0: jdbc:hive2://localhost:10000/default> show tables;</b></code><br>
INFO  : Compiling command(queryId=hive_20171129204949_e533e6ab-276f-4daa-82de-10827c49a9b1): show tables<br>
INFO  : Semantic Analysis Completed<br>
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)<br>
INFO  : Completed compiling command(queryId=hive_20171129204949_e533e6ab-276f-4daa-82de-10827c49a9b1); Time taken: 0.072 seconds<br>
INFO  : Executing command(queryId=hive_20171129204949_e533e6ab-276f-4daa-82de-10827c49a9b1): show tables<br>
INFO  : Starting task [Stage-0:DDL] in serial mode<br>
INFO  : Completed executing command(queryId=hive_20171129204949_e533e6ab-276f-4daa-82de-10827c49a9b1); Time taken: 0.187 seconds<br>
INFO  : OK<br>
+------------+--+<br>
|  tab_name  |<br>
+------------+--+<br>
| sample_07  |<br>
+------------+--+<br>
1 row selected (0.388 seconds)<br>
0: jdbc:hive2://localhost:10000/default> <br>





