~~~
[raffles@cdh01 cloudera-scm-agent]$ klist
Ticket cache: FILE:/tmp/krb5cc_2700
Default principal: raffles@GOTOJEFFRAY.SG

Valid starting       Expires              Service principal
12/09/2016 02:37:14  12/10/2016 02:37:14  krbtgt/GOTOJEFFRAY.SG@GOTOJEFFRAY.SG
	renew until 12/16/2016 02:37:14
[raffles@cdh01 cloudera-scm-agent]$
[raffles@cdh01 cloudera-scm-agent]$ time hadoop  jar  /opt/cloudera/parcels/CDH/share/doc/hadoop-0.20-mapreduce/examples/hadoop-examples.jar terasort   /user/raffles/tgen512m  /user/raffles/tsort512m
16/12/09 02:37:49 INFO terasort.TeraSort: starting
16/12/09 02:37:50 INFO hdfs.DFSClient: Created token for raffles: HDFS_DELEGATION_TOKEN owner=raffles@GOTOJEFFRAY.SG, renewer=yarn, realUser=, issueDate=1481251070844, maxDate=1481855870844, sequenceNumber=1, masterKeyId=2 on 172.31.2.139:8020
16/12/09 02:37:50 INFO security.TokenCache: Got dt for hdfs://cdh01.gotojeffray.nz:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.2.139:8020, Ident: (token for raffles: HDFS_DELEGATION_TOKEN owner=raffles@GOTOJEFFRAY.SG, renewer=yarn, realUser=, issueDate=1481251070844, maxDate=1481855870844, sequenceNumber=1, masterKeyId=2)
16/12/09 02:37:50 INFO input.FileInputFormat: Total input paths to process : 2
Spent 263ms computing base-splits.
Spent 2ms computing TeraScheduler splits.
Computing input splits took 266ms
Sampling 8 splits of 8
Making 8 from 100000 sampled records
Computing parititions took 787ms
Spent 1055ms computing partitions.
16/12/09 02:37:51 INFO client.RMProxy: Connecting to ResourceManager at cdh01.gotojeffray.nz/172.31.2.139:8032
16/12/09 02:37:52 INFO mapreduce.JobSubmitter: number of splits:8
16/12/09 02:37:52 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1481250898822_0001
16/12/09 02:37:52 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.2.139:8020, Ident: (token for raffles: HDFS_DELEGATION_TOKEN owner=raffles@GOTOJEFFRAY.SG, renewer=yarn, realUser=, issueDate=1481251070844, maxDate=1481855870844, sequenceNumber=1, masterKeyId=2)
16/12/09 02:37:53 INFO impl.YarnClientImpl: Submitted application application_1481250898822_0001
16/12/09 02:37:53 INFO mapreduce.Job: The url to track the job: http://cdh01.gotojeffray.nz:8088/proxy/application_1481250898822_0001/
16/12/09 02:37:53 INFO mapreduce.Job: Running job: job_1481250898822_0001
16/12/09 02:38:02 INFO mapreduce.Job: Job job_1481250898822_0001 running in uber mode : false
16/12/09 02:38:02 INFO mapreduce.Job:  map 0% reduce 0%
16/12/09 02:38:12 INFO mapreduce.Job:  map 25% reduce 0%
16/12/09 02:38:13 INFO mapreduce.Job:  map 38% reduce 0%
16/12/09 02:38:16 INFO mapreduce.Job:  map 63% reduce 0%
16/12/09 02:38:19 INFO mapreduce.Job:  map 88% reduce 0%
16/12/09 02:38:20 INFO mapreduce.Job:  map 100% reduce 0%
16/12/09 02:38:28 INFO mapreduce.Job:  map 100% reduce 13%
16/12/09 02:38:29 INFO mapreduce.Job:  map 100% reduce 63%
16/12/09 02:38:32 INFO mapreduce.Job:  map 100% reduce 88%
16/12/09 02:38:33 INFO mapreduce.Job:  map 100% reduce 100%
16/12/09 02:38:33 INFO mapreduce.Job: Job job_1481250898822_0001 completed successfully
16/12/09 02:38:34 INFO mapreduce.Job: Counters: 50
	File System Counters
		FILE: Number of bytes read=225174489
		FILE: Number of bytes written=449828824
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=512001056
		HDFS: Number of bytes written=512000000
		HDFS: Number of read operations=48
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=16
	Job Counters
		Launched map tasks=8
		Launched reduce tasks=8
		Data-local map tasks=7
		Rack-local map tasks=1
		Total time spent by all maps in occupied slots (ms)=91389
		Total time spent by all reduces in occupied slots (ms)=67165
		Total time spent by all map tasks (ms)=91389
		Total time spent by all reduce tasks (ms)=67165
		Total vcore-seconds taken by all map tasks=91389
		Total vcore-seconds taken by all reduce tasks=67165
		Total megabyte-seconds taken by all map tasks=93582336
		Total megabyte-seconds taken by all reduce tasks=68776960
	Map-Reduce Framework
		Map input records=5120000
		Map output records=5120000
		Map output bytes=522240000
		Map output materialized bytes=222661263
		Input split bytes=1056
		Combine input records=0
		Combine output records=0
		Reduce input groups=5120000
		Reduce shuffle bytes=222661263
		Reduce input records=5120000
		Reduce output records=5120000
		Spilled Records=10240000
		Shuffled Maps =64
		Failed Shuffles=0
		Merged Map outputs=64
		GC time elapsed (ms)=1485
		CPU time spent (ms)=74790
		Physical memory (bytes) snapshot=6636806144
		Virtual memory (bytes) snapshot=25372581888
		Total committed heap usage (bytes)=7847542784
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters
		Bytes Read=512000000
	File Output Format Counters
		Bytes Written=512000000
16/12/09 02:38:34 INFO terasort.TeraSort: done

real	0m45.606s
user	0m7.587s
sys	0m0.267s
~~~
