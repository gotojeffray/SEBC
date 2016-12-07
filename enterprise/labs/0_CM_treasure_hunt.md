----
What is ubertask optimization?
###
By default a job that has less than 10 mappers only and one reducer, and the input size is less than the size of one HDFS block is said to be Ubertask. Application Master could run ubertask in its own container instead of allocating new container for saving time. 
###
---
Where in CM is the Kerberos Security Realm value displayed?
###
Settings -> Kerberos
###
----
Which CDH service(s) host a property for enabling Kerberos authentication?
###
Security
###
----
How do you upgrade the CM agents?
###
* 1.Update the yum.repos.d file for new version of cloudera agent.
* 2.yum update
* 3.stop the agent
* 4.yum upgrade cloudera-manager-agent.x86_64
* 5.start the agent
###

----
Give the tsquery statement used to chart Hue's CPU utilization?
###
SELECT cpu_system_rate + cpu_user_rate WHERE entityName = "hue-HUE_SERVER-f2373c0f7b73eec64dbc188eb4e7d42b" AND category = ROLE
###
----
Name all the roles that make up the Hive service
* Hive Metastore
* Hive Server2
* Gateway
* WebHcat(optional)


----
What steps must be completed before integrating Cloudera Manager with Kerberos?
###
* set up a working KDC
* Congfigure the renew tickets allowed in KDC.
* Create a super previleage account for cloudera manager
* install JCE for AES-256 encrytion
###
----
