# Databases 

Data comes in all types of formats – from structured data in relational database management systems (RDBMS) to loosely-typed semi-structured and unstructured data like text documents, emails, videos and audio data which can be stored in NoSQL databases.

This video from Google covers some database options available within Google Cloud across relational (SQL) and non-relational (NoSQL) databases. In particular, it explains which use cases are best suited for each database option (note that there are more open source options available):

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/2TZXSnCTd7E" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<br>

![](../_static/img/Which-Database.jpeg)

## Relational databases

A relational database is a collection of data items with pre-defined relationships between them. These items are organized as a set of tables with columns and rows ([AWS](https://aws.amazon.com/relational-database/?nc1=h_ls)):

- *Tables* are used to hold information about the objects to be represented in the database. 
- Each *column* in a table holds a certain kind of data and a field stores the actual value of an attribute. 
- The *rows* in the table represent a collection of related values of one object or entity. 
- Each row in a table could be marked with a unique identifier called a *primary key*, and rows among multiple tables can be made related using *foreign keys*. 

This data can be accessed in many different ways (e.g. using SQL) without reorganizing the database tables themselves.

What is a Relational Database:

<br>

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/OqjJjpjDRLc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<br>

## NoSQL

No-SQL databases refer to high-performance, non-relational data stores. Instead of joining tables of normalized data, NoSQL stores *unstructured* or *semi-structured data*, often in key-value pairs or JSON documents. NoSQL databases include several different models for accessing and managing data, each suited to specific use cases ([Microsoft, 2021](https://docs.microsoft.com/en-us/dotnet/architecture/cloud-native/relational-vs-nosql-data)): 

<br>

![](../_static/img/types-of-nosql-datastores.png)

Model	| Characteristics | Open Source
--|--|--
Document Store | Data and metadata are stored hierarchically in JSON-based documents inside the database. | MongoDB, CouchDB
Key Value Store |	The simplest of the NoSQL databases, data is represented as a collection of key-value pairs. | Redis
Wide-Column Store |	Related data is stored as a set of nested-key/value pairs within a single column. | HBase, Cassandra
Graph Store |	Data is stored in a graph structure as node, edge, and data properties. | Neo4j


## Hadoop ecosystem

The [Apache Hadoop software](https://hadoop.apache.org/) library is a big data framework that allows for the distributed storing and processing of large data sets.

The Apache Software Foundation provides several open source big data libraries, but here we will mainly focus on the **Hadoop Distributed File System**, which is a distributed file system for storing large data sets (a typical file in HDFS is gigabytes to terabytes in size): 

<br>

![](../_static/img/hadoop.png)

*Picture source: [Du (2018)](https://www.oreilly.com/library/view/apache-hive-essentials/9781788995092/e846ea02-6894-45c9-983a-03875076bb5b.xhtml)*

<br>

HDFS follows the Master-Slave architecture pattern. Two sub-components, namely NameNode and DataNode, are present in master and slave nodes respectively (Tomcy & Pankaj, 2017): 

![](../_static/img/hdfs-master-slave.png)


The DataNode stores the application data and NameNode stores the filesystem metadata. The communication between NameNode and DataNode is through TCP-based protocols and is quite reliable and high-performant.