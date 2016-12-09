~~~

[orchard@cdh01 ~]$ kinit  orchard
Password for orchard@GOTOJEFFRAY.SG:
[orchard@cdh01 ~]$ klist
Ticket cache: FILE:/tmp/krb5cc_2800
Default principal: orchard@GOTOJEFFRAY.SG

Valid starting       Expires              Service principal
12/09/2016 02:40:15  12/10/2016 02:40:15  krbtgt/GOTOJEFFRAY.SG@GOTOJEFFRAY.SG
	renew until 12/16/2016 02:40:15
[orchard@cdh01 ~]$
[orchard@cdh01 ~]$
[orchard@cdh01 ~]$ hadoop  jar  /opt/cloudera/parcels/CDH/share/doc/hadoop-0.20-mapreduce/examples/hadoop-examples.jar pi  10  5
Number of Maps  = 10
Samples per Map = 5
Wrote input for Map #0
Wrote input for Map #1
Wrote input for Map #2
Wrote input for Map #3
Wrote input for Map #4
Wrote input for Map #5
Wrote input for Map #6
Wrote input for Map #7
Wrote input for Map #8
Wrote input for Map #9
Starting Job
16/12/09 02:40:35 INFO client.RMProxy: Connecting to ResourceManager at cdh01.gotojeffray.nz/172.31.2.139:8032
16/12/09 02:40:35 INFO hdfs.DFSClient: Created token for orchard: HDFS_DELEGATION_TOKEN owner=orchard@GOTOJEFFRAY.SG, renewer=yarn, realUser=, issueDate=1481251235271, maxDate=1481856035271, sequenceNumber=2, masterKeyId=2 on 172.31.2.139:8020
16/12/09 02:40:35 INFO security.TokenCache: Got dt for hdfs://cdh01.gotojeffray.nz:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.2.139:8020, Ident: (token for orchard: HDFS_DELEGATION_TOKEN owner=orchard@GOTOJEFFRAY.SG, renewer=yarn, realUser=, issueDate=1481251235271, maxDate=1481856035271, sequenceNumber=2, masterKeyId=2)
16/12/09 02:40:35 INFO input.FileInputFormat: Total input paths to process : 10
16/12/09 02:40:35 INFO mapreduce.JobSubmitter: number of splits:10
16/12/09 02:40:35 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1481250898822_0002
16/12/09 02:40:35 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.2.139:8020, Ident: (token for orchard: HDFS_DELEGATION_TOKEN owner=orchard@GOTOJEFFRAY.SG, renewer=yarn, realUser=, issueDate=1481251235271, maxDate=1481856035271, sequenceNumber=2, masterKeyId=2)
16/12/09 02:40:36 INFO impl.YarnClientImpl: Submitted application application_1481250898822_0002
16/12/09 02:40:36 INFO mapreduce.Job: The url to track the job: http://cdh01.gotojeffray.nz:8088/proxy/application_1481250898822_0002/
16/12/09 02:40:36 INFO mapreduce.Job: Running job: job_1481250898822_0002
16/12/09 02:40:44 INFO mapreduce.Job: Job job_1481250898822_0002 running in uber mode : false
16/12/09 02:40:44 INFO mapreduce.Job:  map 0% reduce 0%
16/12/09 02:40:54 INFO mapreduce.Job:  map 20% reduce 0%
16/12/09 02:40:59 INFO mapreduce.Job:  map 30% reduce 0%
16/12/09 02:41:00 INFO mapreduce.Job:  map 100% reduce 0%
16/12/09 02:41:05 INFO mapreduce.Job:  map 100% reduce 100%
16/12/09 02:41:05 INFO mapreduce.Job: Job job_1481250898822_0002 completed successfully
16/12/09 02:41:05 INFO mapreduce.Job: Counters: 49
	File System Counters
		FILE: Number of bytes read=76
		FILE: Number of bytes written=1362345
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=2770
		HDFS: Number of bytes written=215
		HDFS: Number of read operations=43
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=3
	Job Counters
		Launched map tasks=10
		Launched reduce tasks=1
		Data-local map tasks=10
		Total time spent by all maps in occupied slots (ms)=123880
		Total time spent by all reduces in occupied slots (ms)=3229
		Total time spent by all map tasks (ms)=123880
		Total time spent by all reduce tasks (ms)=3229
		Total vcore-seconds taken by all map tasks=123880
		Total vcore-seconds taken by all reduce tasks=3229
		Total megabyte-seconds taken by all map tasks=126853120
		Total megabyte-seconds taken by all reduce tasks=3306496
	Map-Reduce Framework
		Map input records=10
		Map output records=20
		Map output bytes=180
		Map output materialized bytes=337
		Input split bytes=1590
		Combine input records=0
		Combine output records=0
		Reduce input groups=2
		Reduce shuffle bytes=337
		Reduce input records=20
		Reduce output records=0
		Spilled Records=40
		Shuffled Maps =10
		Failed Shuffles=0
		Merged Map outputs=10
		GC time elapsed (ms)=560
		CPU time spent (ms)=6700
		Physical memory (bytes) snapshot=4762316800
		Virtual memory (bytes) snapshot=17372155904
		Total committed heap usage (bytes)=5336203264
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters
		Bytes Read=1180
	File Output Format Counters
		Bytes Written=97
Job Finished in 30.636 seconds
Estimated value of Pi is 3.28000000000000000000

~~~
