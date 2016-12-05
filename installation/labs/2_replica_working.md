~~~~~~~
172.31.3.200  ip-172-31-3-200.ap-southeast-1.compute.internal  --  primary 
172.31.12.88 ip-172-31-12-88.ap-southeast-1.compute.internal   --  replication


I'm using postgresql server.

-bash-4.2$ psql
psql (9.2.15)
Type "help" for help.

postgres=# select * from pg_stat_replication;
  pid  | usesysid | usename | application_name | client_addr  | client_hostname | client_port |         backend_start         |   state   | sent_location | write_location | flush_location | replay_locatio
n | sync_priority | sync_state
-------+----------+---------+------------------+--------------+-----------------+-------------+-------------------------------+-----------+---------------+----------------+----------------+---------------
--+---------------+------------
 13425 |    17713 | replica | walreceiver      | 172.31.12.88 |                 |       46770 | 2016-12-05 07:51:20.712064+00 | streaming | 0/7894918     | 0/7894918      | 0/7894918      | 0/7894918
  |             0 | async
(1 row)

~~~~~~~
