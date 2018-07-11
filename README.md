# distributed-system
As title. Distributed cache(redis), database, hash table, file system. block storage (vsan, ceph), computing(spark, mapreduce,....). The monitor and manage of distributed system -- kubernets,YARN. The debug tools (log track) of distributed system.  Message queue, Search engine, distributed basics algorithm(paxos, raft,...). distbuted AI system, framewor for distributed system (Akka, Vertx), Network Lib: ZeroMQ, netty for fast/efficient communication between nodes. Ngnix.

# CAP on real products
## HDFS is CP?
* Why C?
  * 写的时候，因为写第二，三份副本的时候是异步的，读取副本的时候，可能会看到老的数据？
* Why P
  * 副本尽量放在不同的子网和机架，所以，网络分割的时候，虽然某些数据可能不能访问，但也能保证提供一定的服务，不会使得整个HDFS倒掉。
# Web sites
* https://www.allthingsdistributed.com/

# Paper:
* https://www.allthingsdistributed.com/files/amazon-dynamo-sosp2007.pdf

# Cassanrdra
* https://www.ibm.com/developerworks/library/os-apache-cassandra/
