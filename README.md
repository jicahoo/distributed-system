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

# Paxos:
* https://blog.openacid.com/algo/paxos/

# 拜占庭将军问题
* https://zhuanlan.zhihu.com/p/33666461
在出现比特币之前，解决分布式系统一致性问题主要是Lamport提出的Paxos算法或其衍生算法。Paxos类算法仅适用于中心化的分布式系统，这样的系统的没有不诚实的节点（不会发送虚假错误消息，但允许出现网络不通或宕机出现的消息延迟）。

中本聪在比特币中创造性的引入了“工作量证明（POW : Proof of Work）”来解决这个问题，有兴趣可进一步阅读工作量证明。

# Paper:

# Cassanrdra
* https://www.ibm.com/developerworks/library/os-apache-cassandra/
* https://www.cs.cornell.edu/projects/ladis2009/papers/lakshman-ladis2009.pdf
* https://www.allthingsdistributed.com/files/amazon-dynamo-sosp2007.pdf

# Distributed DB support ACID transaction.
* CockroachDB
* YugaByte
 * https://blog.yugabyte.com/yes-we-can-distributed-acid-transactions-with-high-performance-a87d17051371
* Fauna 
 * https://blog.fauna.com/acid-transactions-in-a-globally-distributed-database
* Distributed transactions: http://cs.yale.edu/homes/thomson/publications/calvin-sigmod12.pdf

# Key value database:
* LevelDB (not distributed) Google.

# CAP
* CouchDB is AP, Paxos is CP, RDBMS is AC.
![alt text](http://docs.couchdb.org/en/2.1.1/_images/intro-consistency-01.png)
