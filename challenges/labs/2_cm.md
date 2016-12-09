~~~

[root@cdh01 ~]# ls /etc/yum.repos.d
CentOS-Base.repo       CentOS-Vault.repo
CentOS-CR.repo         cloudera-manager.repo
CentOS-Debuginfo.repo  epel.repo
CentOS-fasttrack.repo  epel-testing.repo
CentOS-Media.repo      mysql-community.repo
CentOS-Sources.repo    mysql-community-source.repo
~~~

~~~
[root@cdh01 ~]# /usr/share/cmf/schema/scm_prepare_database.sh mysql -h cdh02.gotojeffray.nz -uroot -proot  --scm-host  cdh01.gotojeffray.nz  scm scm scm
JAVA_HOME=/usr/java/jdk1.7.0_67-cloudera
Verifying that we can write to /etc/cloudera-scm-server
Creating SCM configuration file in /etc/cloudera-scm-server
Executing:  /usr/java/jdk1.7.0_67-cloudera/bin/java -cp /usr/share/java/mysql-connector-java.jar:/usr/share/java/oracle-connector-java.jar:/usr/share/cmf/schema/../lib/* com.cloudera.enterprise.dbutil.DbCommandExecutor /etc/cloudera-scm-server/db.properties com.cloudera.cmf.db.
[                          main] DbCommandExecutor              INFO  Successfully connected to database.
All done, your SCM database is configured correctly!

~~~
