~~~~
1. change OS memeory from 12GB to 4GB,
   change OS CPU from 2 to 1;
   
  because no need to reserve so much resource for OS.
 ~~~~~
 ~~~~  
2. change yarn.scheduler.maximum-allocation-mb from 16GB to 8GB. 

a littel risky allocate 16GB for each container? I think 8GB would be safer.

~~~~
----
What criteria affects workload factor? What does a value of 1, 2, or 4 signify?

workload factor means the concurrency. The lager number you have signify that the more containers will be lauched when you submmit a job.

----
