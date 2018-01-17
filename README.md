**BIG DATA**

Big data is data sets that are so voluminous and complex that traditional data processing application software are inadequate to deal with them. Big data challenges include capturing data, data storage, data analysis, search, sharing, transfer, visualization, querying, updating and information privacy. There are three dimensions to big data known as Volume, Variety and Velocity.

There are 3 types of big data :

    1.Structured - RDBMS  
    2.Semi-structured - XML data  
    3.Unstructured - Word, Pdf, Text, Social media data from Facebook, Twitter, Weather data, Sensor data, etc.  
    
**Characteristics of Big data:**
  
  1.Volume - Amount of data  
  2.Variety - Different forms of data  
  3.Velocity - Analysis of streaming data, speed at which the data is generated  
  4.Veracity - Bias / uncertainity of data  
  5.Valence - Connectiveness of big data in form of graphs  
  6.Value - How big data benefit us and our organization  
  
**Hadoop**

The Apache Hadoop software library is a framework that allows for the distributed processing of large data sets across clusters of computers using simple programming models. It is designed to scale up from single servers to thousands of machines, each offering local computation and storage. Rather than rely on hardware to deliver high-availability, the library itself is designed to detect and handle failures at the application layer, so delivering a highly-available service on top of a cluster of computers, each of which may be prone to failures.

**Hadoop Ecosystem**

![alt text](https://github.com/SaravananJaichandar/Big-Data/blob/master/Hadoopecosystem.jpg)

**HDFS**

A distributed file system that provides high-throughput access to application data.

**Map Reduce**

A YARN-based system for parallel processing of large data sets.

**Hive**

A data warehouse infrastructure that provides data summarization and ad hoc querying.

**Hbase**

A scalable, distributed database that supports structured data storage for large tables. No SQL Database.

**Pig**

A high-level data-flow language and execution framework for parallel computation.

**YARN**

yet Another Resource Negotiator. A framework for job scheduling and cluster resource management.

**Mahout**

 A Scalable machine learning and data mining library.
 
 **Oozie**
 
 A high-performance coordination service for distributed applications.

**Apache Spark**

A fast and general compute engine for Hadoop data. Spark provides a simple and expressive programming model that supports a wide range of applications, including ETL, machine learning, stream processing, and graph computation.

**Sqoop**

Apache Sqoop(TM) is a tool designed for efficiently transferring bulk data between Apache Hadoop and structured datastores such as relational databases.

**Flume**

Flume is a distributed, reliable, and available service for efficiently collecting, aggregating, and moving large amounts of log data. It has a simple and flexible architecture based on streaming data flows. It is robust and fault tolerant with tunable reliability mechanisms and many failover and recovery mechanisms. It uses a simple extensible data model that allows for online analytic application.

**Spark SQL**

Spark SQL is Apache Spark's module for working with structured data.

**Spark MLlib**

MLlib is Apache Spark's scalable machine learning library.

**Spark Streaming**

Spark Streaming is an extension of the core Spark API that enables scalable, high-throughput, fault-tolerant stream processing of live data streams. Data can be ingested from many sources like Kafka, Flume, Kinesis, or TCP sockets, and can be processed using complex algorithms expressed with high-level functions like map, reduce, join and window. Finally, processed data can be pushed out to filesystems, databases, and live dashboards. In fact, you can apply Spark’s machine learning and graph processing algorithms on data streams.

**Spark Graphx**

GraphX is Apache Spark's API for graphs and graph-parallel computation.
