# DingoDB

[DingoDB](https://github.com/dingodb/dingo) is a distributed real-time multi-modal database. It combines the features of a data lake and a vector database. It can store any type of data (key-value, PDF, audio, video, etc) with data of any size. Using it, you can do analysis on structured and unstructured data in extremely low latency.

 ![](./images/dingo_stack.png)

## Projects about DingoDB

Welcome to visit [DingoDB](https://github.com/dingodb/dingo). The documentation of DingoDB is located on the website: [https://dingodb.readthedocs.io](https://dingodb.readthedocs.io).  The main projects about DingoDB are as follows:

- [DingoDB](https://github.com/dingodb/dingo): A Unified SQL Engine to parse and compute for both structured and unstructured data.
- [Dingo-Store](https://github.com/dingodb/dingo-store): A strongly consistent distributed storage system based on the Raft protocol.
- [Dingo-Deploy](https://github.com/dingodb/dingo-deploy): The deployment project of compute nodes and storage nodes.


## Key Features

### As A Distributed Vector database for Any Data

1. Offering storage for all data types (embeddings, audio, text, videos, images, pdfs, annotations, etc.)
2. query and vector search in low latency 
3. Perform hybrid search including embeddings and structured data such as label or attributes
  
### As A Distributed Relation database

1. Compliant with MySQL-Compatible
   Based on the popular [Apache Calcite](https://calcite.apache.org/) SQL engine, DingoDB can parse, optimize and
   execute standard SQL statements, and is capable to run part of TPC-H and TPC-DS (See [TPC](http://www.tpc.org/))
   queries. DingoDB is also compliant with MySQL Shell and MySQL-JDBC-Driver Client, So you can be seamlessly integrated with web services, BI tools, etc.
2. Support high frequency write operation  
   By using [RAFT](https://raft.github.io/) and log-structured key-value storage [RocksDB](https://rocksdb.org/). You can perform high-frequency INSERT, UPDATE, DELETE and short-QUERY while ensuring strong data consistency. 
3. Support point query and multi-dimensional analysis simultaneously  
   DingoDB can push down the expressioin to store to accelerate 
   query and fast multi-dimensional analysis in low latency.
4. As a distributed storage engine, it provides the ability to store massive amounts of data. At the same time, with the increase in data scale, it can easily perform horizontal scaling operations on clusters.
5. As a distributed storage engine, It is designed based on Raft to provide a multi-replicated management mechanism, which provides extremely high data reliability. It can ensure high data consistency in the event of disk or machine failures, and also provides a fast automatic recovery mechanism.


## Special Thanks

DingoDB is Sponsored by [DataCanvas](https://www.datacanvas.com/), a new platform to do data science and data process in real-time.
