# DingoDB

[DingoDB](https://github.com/dingodb/dingo) is a distributed multi-modal vector database. It combines the features of a data lake and a vector database, allowing for the storage of any type of data (key-value, PDF, audio, video, etc.) regardless of its size. Utilizing DingoDB, you can construct your own **Vector Ocean** (the next-generation data architecture following data warehouse and data lake, as introduced by [DataCanvas](https://www.datacanvas.com/)). This enables the analysis of both structured and unstructured data through a singular SQL with exceptionally low latency in real time.

 ![](./images/dingo_stack.png)

## Projects about DingoDB

Welcome to visit [DingoDB](https://github.com/dingodb/dingo). The documentation of DingoDB is located on the website: [https://dingodb.readthedocs.io](https://dingodb.readthedocs.io).  The main projects about DingoDB are as follows:

- [DingoDB](https://github.com/dingodb/dingo): A Unified SQL Engine to parse and compute for both structured and unstructured data.
- [Dingo-Store](https://github.com/dingodb/dingo-store): A strongly consistent distributed storage system based on the Raft protocol.
- [Dingo-Deploy](https://github.com/dingodb/dingo-deploy): The deployment project of compute nodes and storage nodes.


## Key Features

### As a Distributed Vector Database for Any Data

1. Provides comprehensive data storage solutions, accommodating a wide range of data types including but not limited to embeddings, audio files, text, videos, images, PDFs, and annotations.
2. Facilitates efficient querying and vector searching with minimal latency using a singular SQL approach.
3. Employs a hybrid search mechanism that caters to both structured and unstructured data, supporting operations like metadata querying and vector querying.
4. Possesses the ability to dynamically ingest data and construct corresponding indexes in real time, promoting operational efficiency.
  
### As a Distributed Relation database

1. MySQL Compatibility
   Built upon the acclaimed [Apache Calcite](https://calcite.apache.org/) SQL engine, DingoDB is capable of parsing, optimizing, and executing standard SQL statements, and can handle parts of TPC-H and TPC-DS(See [TPC](http://www.tpc.org/)) queries. Compliant with MySQL Shell and MySQL-JDBC-Driver Client, it offers seamless integration with web services, BI tools, and more.
2. Supports High Frequency Write Operations:
   With the use of [RAFT](https://raft.github.io/) and the log-structured key-value storage [RocksDB](https://rocksdb.org/)., DingoDB can handle high-frequency INSERT, UPDATE, DELETE, and short-QUERY operations while maintaining strong data consistency.
3. Facilitates Point Queries and Multi-dimensional Analysis Simultaneously:
   DingoDB can push down expressions to accelerate queries and quickly carry out multi-dimensional analysis with low latency.
4. Distributed Storage Capabilities
   As a distributed storage engine, DingoDB has the capacity to store vast amounts of data. It allows for easy horizontal scaling operations on clusters as data scale increases.
5. High Data Reliability and Recovery:
   Designed based on Raft, DingoDB provides a multi-replicated management mechanism, ensuring extraordinarily high data reliability. It can maintain high data consistency even in the event of disk or machine failures and offers a swift automatic recovery mechanism.

## Documentation

The documentation of DingoDB is located on the website: [https://dingodb.readthedocs.io](https://dingodb.readthedocs.io)
or in the `docs/` directory of the source code.

## Special Thanks

DingoDB is Sponsored by [DataCanvas](https://www.datacanvas.com/), a new platform to do data science and data process in real-time.
