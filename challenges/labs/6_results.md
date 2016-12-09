~~~
[orchard@cdh01 ~]$ kinit orchard
Password for orchard@GOTOJEFFRAY.SG:
[orchard@cdh01 ~]$
[orchard@cdh01 ~]$
[orchard@cdh01 ~]$ beeline
2016-12-09 03:23:01,205 WARN  [main] mapreduce.TableMapReduceUtil: The hbase-prefix-tree module jar containing PrefixTreeCodec is not present.  Continuing without it.
Beeline version 1.1.0-cdh5.9.0 by Apache Hive
beeline>  !connect jdbc:hive2://cdh02.gotojeffray.nz:10000/default;principal=hive/cdh02.gotojeffray.nz@GOTOJEFFRAY.SG
scan complete in 1ms
Connecting to jdbc:hive2://cdh02.gotojeffray.nz:10000/default;principal=hive/cdh02.gotojeffray.nz@GOTOJEFFRAY.SG
Connected to: Apache Hive (version 1.1.0-cdh5.9.0)
Driver: Hive JDBC (version 1.1.0-cdh5.9.0)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://cdh02.gotojeffray.nz:10000/de> show tables;
INFO  : Compiling command(queryId=hive_20161209032323_78950b7b-f63c-45c2-90d0-5d788d046cf9): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20161209032323_78950b7b-f63c-45c2-90d0-5d788d046cf9); Time taken: 0.062 seconds
INFO  : Executing command(queryId=hive_20161209032323_78950b7b-f63c-45c2-90d0-5d788d046cf9): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20161209032323_78950b7b-f63c-45c2-90d0-5d788d046cf9); Time taken: 0.133 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| customers  |
| sample_07  |
| sample_08  |
| web_logs   |
+------------+--+
4 rows selected (0.295 seconds)
~~~


~~~
[raffles@cdh01 ~]$ klist
Ticket cache: FILE:/tmp/krb5cc_2700
Default principal: raffles@GOTOJEFFRAY.SG

Valid starting       Expires              Service principal
12/09/2016 03:28:05  12/10/2016 03:28:05  krbtgt/GOTOJEFFRAY.SG@GOTOJEFFRAY.SG
	renew until 12/16/2016 03:28:05
[raffles@cdh01 ~]$
[raffles@cdh01 ~]$
[raffles@cdh01 ~]$
[raffles@cdh01 ~]$
[raffles@cdh01 ~]$ beeline
2016-12-09 03:28:16,325 WARN  [main] mapreduce.TableMapReduceUtil: The hbase-prefix-tree module jar containing PrefixTreeCodec is not present.  Continuing without it.
Beeline version 1.1.0-cdh5.9.0 by Apache Hive
beeline> !connect jdbc:hive2://cdh02.gotojeffray.nz:10000/default;principal=hive/cdh02.gotojeffray.nz@GOTOJEFFRAY.SG
scan complete in 2ms
Connecting to jdbc:hive2://cdh02.gotojeffray.nz:10000/default;principal=hive/cdh02.gotojeffray.nz@GOTOJEFFRAY.SG
Connected to: Apache Hive (version 1.1.0-cdh5.9.0)
Driver: Hive JDBC (version 1.1.0-cdh5.9.0)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://cdh02.gotojeffray.nz:10000/de> SHOW TABLES;
INFO  : Compiling command(queryId=hive_20161209032828_37f8cbce-4400-4951-a658-6a046bfbef8d): SHOW TABLES
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20161209032828_37f8cbce-4400-4951-a658-6a046bfbef8d); Time taken: 0.061 seconds
INFO  : Executing command(queryId=hive_20161209032828_37f8cbce-4400-4951-a658-6a046bfbef8d): SHOW TABLES
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20161209032828_37f8cbce-4400-4951-a658-6a046bfbef8d); Time taken: 0.156 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| customers  |
| sample_07  |
| sample_08  |
| web_logs   |
+------------+--+
4 rows selected (0.31 seconds)

~~~


