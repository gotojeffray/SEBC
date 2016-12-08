```
Connecting to jdbc:hive2://ip-172-31-11-106.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-11-106.ap-southeast-1.compute.internal@CLOUDERA.LOCAL
Enter username for jdbc:hive2://ip-172-31-11-106.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-11-106.ap-southeast-1.compute.internal@CLOUDERA.LOCAL: gotojeffray
Enter password for jdbc:hive2://ip-172-31-11-106.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-11-106.ap-southeast-1.compute.internal@CLOUDERA.LOCAL: ********
Connected to: Apache Hive (version 1.1.0-cdh5.8.3)
Driver: Hive JDBC (version 1.1.0-cdh5.8.3)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://ip-172-31-11-106.ap-southeast> show tables;
INFO  : Compiling command(queryId=hive_20161208031414_84143eb0-9767-4a7c-bff4-3f33e86c717f): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20161208031414_84143eb0-9767-4a7c-bff4-3f33e86c717f); Time taken: 0.81 seconds
INFO  : Executing command(queryId=hive_20161208031414_84143eb0-9767-4a7c-bff4-3f33e86c717f): show tables
INFO  : Starting task [Stage-0:DDL] in
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20161208031414_84143eb0-9767-4a7c-bff4-3f33e86c717f); Time taken: 0.281 seconds
INFO  : OK
+-----------+--+
| tab_name  |
+-----------+--+
+-----------+--+
No rows selected (2.416 seconds)
0: jdbc:hive2://ip-172-31-11-106.ap-southeast>
```


```
0: jdbc:hive2://ip-172-31-11-106.ap-southeast> SHOW TABLES;
INFO  : Compiling command(queryId=hive_20161208031616_a57e823b-b1c9-4d48-8422-cdadc3d527d0): SHOW TABLES
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20161208031616_a57e823b-b1c9-4d48-8422-cdadc3d527d0); Time taken: 0.063 seconds
INFO  : Executing command(queryId=hive_20161208031616_a57e823b-b1c9-4d48-8422-cdadc3d527d0): SHOW TABLES
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20161208031616_a57e823b-b1c9-4d48-8422-cdadc3d527d0); Time taken: 0.124 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| customers  |
| sample_07  |
| sample_08  |
| web_logs   |
+------------+--+
4 rows selected (0.238 seconds)
0: jdbc:hive2://ip-172-31-11-106.ap-southeast>
```
