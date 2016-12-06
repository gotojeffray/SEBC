~~~~~

hadoop  jar  /opt/cloudera/parcels/CDH/share/doc/hadoop-0.20-mapreduce/examples/hadoop-examples.jar teragen  -D dfs.block.size=33554432 100000000  /user/gotojeffray/input/

real	3m3.099s
user	0m5.770s
sys	0m0.257s


~~~~~



~~~~
time  hadoop  jar  /opt/cloudera/parcels/CDH/share/doc/hadoop-0.20-mapreduce/examples/hadoop-examples.jar terasort  /user/gotojeffray/input/  /user/gotojeffray/output

real	7m8.602s
user	0m9.170s
sys	0m0.389s
~~~~
