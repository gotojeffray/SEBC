~~~~
1. change OS memeory from 12GB to 4GB,
   change OS CPU from 2 to 1;
   
  because no need to reserve so much resource for OS.
 ~~~~~
 ~~~~  
2. change yarn.scheduler.maximum-allocation-mb from 16GB to 8GB. 

a littel risky allocate 16GB for each container? I think 8GB would be safer.

~~~~



