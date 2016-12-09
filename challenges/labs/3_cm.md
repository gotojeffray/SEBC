~~~
[hdfs@cdh01 cloudera-scm-agent]$ hdfs dfs -ls /user
Found 6 items
drwxrwxrwx   - mapred  hadoop           0 2016-12-09 01:54 /user/history
drwxrwxr-t   - hive    hive             0 2016-12-09 01:55 /user/hive
drwxrwxr-x   - hue     hue              0 2016-12-09 01:55 /user/hue
drwxrwxr-x   - oozie   oozie            0 2016-12-09 01:55 /user/oozie
drwxr-xr-x   - orchard orchard          0 2016-12-09 01:58 /user/orchard
drwxr-xr-x   - raffles raffles          0 2016-12-09 01:57 /user/raffles
~~~
~~~
[hdfs@cdh01 cloudera-scm-agent]$ curl  -u admin:admin  http://cdh01.gotojeffray.nz:7180/api/v14/hosts
{
  "items" : [ {
    "hostId" : "c5bf96f8-dca4-463f-8c9d-f56555b334c6",
    "ipAddress" : "172.31.2.139",
    "hostname" : "cdh01.gotojeffray.nz",
    "rackId" : "/default",
    "hostUrl" : "http://cdh01.gotojeffray.nz:7180/cmf/hostRedirect/c5bf96f8-dca4-463f-8c9d-f56555b334c6",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "4f124acb-64ad-43f9-978a-ff7ac7e3c10f",
    "ipAddress" : "172.31.2.140",
    "hostname" : "cdh02.gotojeffray.nz",
    "rackId" : "/default",
    "hostUrl" : "http://cdh01.gotojeffray.nz:7180/cmf/hostRedirect/4f124acb-64ad-43f9-978a-ff7ac7e3c10f",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "5ae2e233-8ea4-47c4-9140-8f0019fc86c5",
    "ipAddress" : "172.31.2.141",
    "hostname" : "cdh03.gotojeffray.nz",
    "rackId" : "/default",
    "hostUrl" : "http://cdh01.gotojeffray.nz:7180/cmf/hostRedirect/5ae2e233-8ea4-47c4-9140-8f0019fc86c5",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "d64c9629-10fe-4362-8129-74cc65a6ca65",
    "ipAddress" : "172.31.2.142",
    "hostname" : "cdh04.gotojeffray.nz",
    "rackId" : "/default",
    "hostUrl" : "http://cdh01.gotojeffray.nz:7180/cmf/hostRedirect/d64c9629-10fe-4362-8129-74cc65a6ca65",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  }, {
    "hostId" : "0ef863f2-7618-4431-87fc-e8ac97947f3c",
    "ipAddress" : "172.31.2.143",
    "hostname" : "cdh05.gotojeffray.nz",
    "rackId" : "/default",
    "hostUrl" : "http://cdh01.gotojeffray.nz:7180/cmf/hostRedirect/0ef863f2-7618-4431-87fc-e8ac97947f3c",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15332438016
  } ]
~~~
