~~~
[raffles@cdh01 cloudera-scm-agent]$ time hadoop  jar  /opt/cloudera/parcels/CDH/share/doc/hadoop-0.20-mapreduce/examples/hadoop-examples.jar teragen  -D dfs.block.size=67108864 5120000  /user/raffles/tgen512m
16/12/09 02:08:26 INFO client.RMProxy: Connecting to ResourceManager at cdh01.gotojeffray.nz/172.31.2.139:8032
16/12/09 02:08:26 INFO terasort.TeraSort: Generating 5120000 using 2
16/12/09 02:08:26 INFO mapreduce.JobSubmitter: number of splits:2
16/12/09 02:08:26 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
16/12/09 02:08:27 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1481248463579_0001
16/12/09 02:08:27 INFO impl.YarnClientImpl: Submitted application application_1481248463579_0001
16/12/09 02:08:27 INFO mapreduce.Job: The url to track the job: http://cdh01.gotojeffray.nz:8088/proxy/application_1481248463579_0001/
16/12/09 02:08:27 INFO mapreduce.Job: Running job: job_1481248463579_0001
16/12/09 02:08:33 INFO mapreduce.Job: Job job_1481248463579_0001 running in uber mode : false
16/12/09 02:08:33 INFO mapreduce.Job:  map 0% reduce 0%
16/12/09 02:08:45 INFO mapreduce.Job:  map 100% reduce 0%
16/12/09 02:08:46 INFO mapreduce.Job: Job job_1481248463579_0001 completed successfully
16/12/09 02:08:47 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=244766
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=167
		HDFS: Number of bytes written=512000000
		HDFS: Number of read operations=8
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=4
	Job Counters
		Launched map tasks=2
		Other local map tasks=2
		Total time spent by all maps in occupied slots (ms)=19928
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=19928
		Total vcore-seconds taken by all map tasks=19928
		Total megabyte-seconds taken by all map tasks=20406272
	Map-Reduce Framework
		Map input records=5120000
		Map output records=5120000
		Input split bytes=167
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=234
		CPU time spent (ms)=15170
		Physical memory (bytes) snapshot=747040768
		Virtual memory (bytes) snapshot=3128975360
		Total committed heap usage (bytes)=869269504
	org.apache.hadoop.examples.terasort.TeraGen$Counters
		CHECKSUM=10993942703914404
	File Input Format Counters
		Bytes Read=0
	File Output Format Counters
		Bytes Written=512000000

~~~

~~~
real	0m23.446s
user	0m5.688s
sys	0m0.215s

~~~

~~~
[raffles@cdh01 cloudera-scm-agent]$ hdfs dfs -ls /user/raffles/tgen512m
Found 3 items
-rw-r--r--   3 raffles raffles          0 2016-12-09 02:08 /user/raffles/tgen512m/_SUCCESS
-rw-r--r--   3 raffles raffles  256000000 2016-12-09 02:08 /user/raffles/tgen512m/part-m-00000
-rw-r--r--   3 raffles raffles  256000000 2016-12-09 02:08 /user/raffles/tgen512m/part-m-00001
~~~

~~~
[raffles@cdh01 cloudera-scm-agent]$ hadoop fsck   /user/raffles/tgen512m -blocks
DEPRECATED: Use of this script to execute hdfs command is deprecated.
Instead use the hdfs command for it.

Connecting to namenode via http://cdh01.gotojeffray.nz:50070
FSCK started by raffles (auth:SIMPLE) from /172.31.2.139 for path /user/raffles/tgen512m at Fri Dec 09 02:14:06 UTC 2016
...Status: HEALTHY
 Total size:	512000000 B
 Total dirs:	1
 Total files:	3
 Total symlinks:		0
 Total blocks (validated):	8 (avg. block size 64000000 B)
 Minimally replicated blocks:	8 (100.0 %)
 Over-replicated blocks:	0 (0.0 %)
 Under-replicated blocks:	0 (0.0 %)
 Mis-replicated blocks:		0 (0.0 %)
 Default replication factor:	3
 Average block replication:	3.0
 Corrupt blocks:		0
 Missing replicas:		0 (0.0 %)
 Number of data-nodes:		4
 Number of racks:		1
FSCK ended at Fri Dec 09 02:14:06 UTC 2016 in 2 milliseconds


The filesystem under path '/user/raffles/tgen512m' is HEALTHY

~~~
