~~~

Report the latest available version of the API
Report the database server in use by CM

#I didn't find any api for above.

~~~
~~~
Report the database server in use by CM
 curl  -u gotojeffray:cloudera  http://localhost:7180/api/v2/cm/version/
{
  "version" : "5.9.0",
  "buildUser" : "jenkins",
  "buildTimestamp" : "20161006-1801",
  "gitHash" : "898a5e032c080e18833dfc58180761f6ef2ea351",
  "snapshot" : false
~~~
~~~
List all CM users
[root@ip-172-31-3-200 data]# curl  -u gotojeffray:cloudera  http://localhost:7180/api/v12/users/
{
  "items" : [ {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ]
  }, {
    "name" : "gotojeffray",
    "roles" : [ "ROLE_ADMIN" ]
  } ]
  ~~~
