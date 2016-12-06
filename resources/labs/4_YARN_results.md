
-----
Slowest:

Teragen 10GB:
real	3m44.037s

Terasort 10GB:
real	16m7.260s

yarn.nodemanager.resource.cpu-vcores=1
yarn.nodemanager.resource.memory-mb=2048
mapreduce.job.maps=8 
mapreduce.job.reduces=8 
mapreduce.map.memory.mb=2048

-----


---
fastest:
~~~~
Teragen 10GB:
real	2m27.986s
~~~~

~~~~
Terasort 10GB:
real	3m28.710s
~~~

~~~
yarn.nodemanager.resource.cpu-vcores=3
yarn.nodemanager.resource.memory-mb=12GB
mapreduce.job.maps=8
mapreduce.job.reduces=8
mapreduce.map.memory.mb=2048
~~~
----
