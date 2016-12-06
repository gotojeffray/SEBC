----
It's really hard to connect to the other cluster since they are in different VPCs.

1) Create VPN connection or VPN Gateway. 
2) WebHDFS


-----
Don't think we have enough time to implement it.

My distcp job was stuck due to can't connect to datanode:50010(eg. 172.3.0.240:50010).

172.3.0.240 is the private IP in the other cluster that my cluster can't resovle it.
