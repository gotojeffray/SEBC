~~~
[root@ip-172-31-3-200 ~]# curl -X POST -u gotojeffray:cloudera 'htp://localhost:7180/api/v12/clusters/gotojeffray/services/hive/commands/stop'
{
  "id" : 1433,
  "name" : "Stop",
  "startTime" : "2016-12-07T03:15:11.478Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}
~~~~
~~~~
[root@ip-172-31-3-200 ~]# curl -X POST -u gotojeffray:cloudera 'htp://localhost:7180/api/v12/clusters/gotojeffray/services/hive/commands/start'
{
  "id" : 1436,
  "name" : "Start",
  "startTime" : "2016-12-07T03:15:29.544Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}
~~~~
