# Hadoop ecosystem

The [Apache Hadoop software](https://hadoop.apache.org/) library is a big data framework that allows for the distributed storing and processing of large data sets.

The Apache Software Foundation provides several open source big data libraries, but here we will mainly focus on the **Hadoop Distributed File System**, which is a distributed file system for storing large data sets (a typical file in HDFS is gigabytes to terabytes in size): 

<br>

![](../_static/img/hadoop.png)

*Picture source: [Du (2018)](https://www.oreilly.com/library/view/apache-hive-essentials/9781788995092/e846ea02-6894-45c9-983a-03875076bb5b.xhtml)*

<br>

HDFS follows the Master-Slave architecture pattern. Two sub-components, namely NameNode and DataNode, are present in master and slave nodes respectively (Tomcy & Pankaj, 2017): 

![](../_static/img/hdfs-master-slave.png)


The DataNode stores the application data and NameNode stores the filesystem metadata. The communication between NameNode and DataNode is through TCP-based protocols and is quite reliable and high-performant.