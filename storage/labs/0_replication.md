[hdfs@ip-172-31-3-200 root]$ hdfs fsck /tmp/chiehwoei/teragen-500MB -files -blocks
Connecting to namenode via http://ip-172-31-3-200.ap-southeast-1.compute.internal:50070
FSCK started by hdfs (auth:SIMPLE) from /172.31.3.200 for path /tmp/chiehwoei/teragen-500MB at Tue Dec 06 03:38:39 UTC 2016
/tmp/chiehwoei/teragen-500MB <dir>
/tmp/chiehwoei/teragen-500MB/_SUCCESS 0 bytes, 0 block(s):  OK

/tmp/chiehwoei/teragen-500MB/part-m-00000 250000000 bytes, 2 block(s):  OK
0. BP-549446534-172.31.3.200-1480928869644:blk_1073746162_5338 len=134217728 Live_repl=3
1. BP-549446534-172.31.3.200-1480928869644:blk_1073746163_5339 len=115782272 Live_repl=3

/tmp/chiehwoei/teragen-500MB/part-m-00001 250000000 bytes, 2 block(s):  OK
0. BP-549446534-172.31.3.200-1480928869644:blk_1073746164_5340 len=134217728 Live_repl=3
1. BP-549446534-172.31.3.200-1480928869644:blk_1073746165_5341 len=115782272 Live_repl=3

Status: HEALTHY
 Total size:	500000000 B
 Total dirs:	1
 Total files:	3
 Total symlinks:		0
 Total blocks (validated):	4 (avg. block size 125000000 B)
 Minimally replicated blocks:	4 (100.0 %)
 Over-replicated blocks:	0 (0.0 %)
 Under-replicated blocks:	0 (0.0 %)
 Mis-replicated blocks:		0 (0.0 %)
 Default replication factor:	3
 Average block replication:	3.0
 Corrupt blocks:		0
 Missing replicas:		0 (0.0 %)
 Number of data-nodes:		3
 Number of racks:		1
FSCK ended at Tue Dec 06 03:38:39 UTC 2016 in 1 milliseconds


The filesystem under path '/tmp/chiehwoei/teragen-500MB' is HEALTHY
