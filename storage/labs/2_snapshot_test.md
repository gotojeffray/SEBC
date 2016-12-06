~~~
1. [gotojeffray@ip-172-31-3-200 ~]$hadoop dfs  -mkdir  /user/gotojeffray/precious

   [gotojeffray@ip-172-31-3-200 ~]$hadoop dfs -put SEBC-master.zip /user/gotojeffray/precious

~~~

~~~
2.create snapshot
[hdfs@ip-172-31-3-200 ~]$ hdfs dfsadmin -allowSnapshot /user/gotojeffray/precious
Allowing snaphot on /user/gotojeffray/precious succeeded

[gotojeffray@ip-172-31-3-200 ~]$ hdfs dfs -createSnapshot /user/gotojeffray/precious    sebc-hdfs-test
Created snapshot /user/gotojeffray/precious/.snapshot/sebc-hdfs-test

~~~
~~~
3. delete file
[gotojeffray@ip-172-31-3-200 ~]$ hadoop dfs  -rmr /user/gotojeffray/precious/SEBC-master.zip

16/12/06 06:28:35 INFO fs.TrashPolicyDefault: Moved: 'hdfs://nameservice1/user/gotojeffray/precious/SEBC-master.zip' to trash at: hdfs://nameservice1/user/gotojeffray/.Trash/Current/user/gotojeffray/precious/SEBC-master.zip

[gotojeffray@ip-172-31-3-200 ~]$ hadoop dfs  -rmr /user/gotojeffray/precious
rmr: Failed to move to trash: hdfs://nameservice1/user/gotojeffray/precious: The directory /user/gotojeffray/precious cannot be deleted since /user/gotojeffray/precious is snapshottable and already has snapshots
~~~~
~~~
4. recover file
[gotojeffray@ip-172-31-3-200 ~]$ hadoop dfs  -cp  /user/gotojeffray/precious/.snapshot/sebc-hdfs-test/SEBC-master.zip   /user/gotojeffray/precious/

[gotojeffray@ip-172-31-3-200 ~]$ hadoop dfs -ls /user/gotojeffray/precious/

Found 1 items
-rw-r--r--   3 gotojeffray gotojeffray        401 2016-12-06 06:35 /user/gotojeffray/precious/SEBC-master.zip
~~~~
