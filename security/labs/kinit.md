~~~
[root@ip-172-31-3-200 ~]# kinit  gotojeffray@CLOUDERA.LOCAL
Password for gotojeffray@CLOUDERA.LOCAL:
[root@ip-172-31-3-200 ~]# hadoop dfs  -ls /user/gotojeffray
DEPRECATED: Use of this script to execute hdfs command is deprecated.
Instead use the hdfs command for it.

Found 5 items
drwx------   - gotojeffray gotojeffray          0 2016-12-07 08:22 /user/gotojeffray/.staging
drwxrwxrwx   - gotojeffray gotojeffray          0 2016-12-07 08:21 /user/gotojeffray/2015_11_18
drwxrwxrwx   - gotojeffray gotojeffray          0 2016-12-07 08:21 /user/gotojeffray/2015_11_19
drwxrwxrwx   - gotojeffray gotojeffray          0 2016-12-07 08:21 /user/gotojeffray/2015_11_20
drwxrwxrwx   - gotojeffray gotojeffray          0 2016-12-07 08:21 /user/gotojeffray/2015_11_21
[root@ip-172-31-3-200 ~]# klist
Ticket cache: FILE:/tmp/krb5cc_0
Default principal: gotojeffray@CLOUDERA.LOCAL

Valid starting       Expires              Service principal
12/07/2016 23:17:06  12/08/2016 23:17:06  krbtgt/CLOUDERA.LOCAL@CLOUDERA.LOCAL
	renew until 12/14/2016 23:17:06
  ~~~
