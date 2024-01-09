# mongodb

This repository contains interview questions for mongodb.

<a name="TableOfContents"></a><h2>TABLE OF CONTENTS:</h2>
| --------- | ---------------------------------------------------------------- |
| 1 | [MONGODB AND ITS FEATURES](#MDB) |
| 2 | [ALTERNATIVE NOSQL DATABASES TO MONGODB](#ALTERNATIVE) |
| 3 | [WHAT TYPE OF NOSQL DATABASE IS MONGODB?](#TYPE) |
| 4 | [HOW DOES MONGODB STORE DATA?](#STORE) |

## <a name="MDB"></a><h2>MONGODB AND ITS FEATURES</h2>

MongoDb is a NOSQL( Not Only SQL) database that stores large volumes of data of documents. This offers developers the flexibility to work with eveolving data models.

- Relational Databases are mostly rows and columns and in table format and we can link our tables using a foreign key. They follow the ACID properties.

- MongoDB uses documents to store and retrieve documents, which provide scalability and flexibility in terms of quering data and indexing.

- based on JSON like features to store the data.

<br>

## [YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="ALTERNATIVE"></a><h2>ALTERNATIVE NOSQL DATABASES TO MONGODB</h2>

- Apache Cassandra
- Redis
- AMazon DynamoDB
- Neo4j
- Apache HBase

<br>

## [YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="TYPE"></a><h2>WHAT TYPE OF NOSQL DATABASE IS MONGODB?</h2>

- KEY VALUE:

* store values as an index-key and value pairs
* schemaless way
* Cassandra, DynamoDB

- COLUMN BASED:

* stores data in a column format rather than row format.
* row format is used in traditional databases.
* HBASE, CASSANDRA

- DOCUMENT BASED:

* designed to store data in form of documents ; with each document having a unique key
* Couchbase, MongoDB

- GRAPH BASED:

* designed for data that needs to be represented as graphs.
* interconnected data in form of graphs and trees
* Neo4j and BigData

<br>

## [YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="STORE"></a><h2>HOW DOES MONGODB STORE DATA?</h2>

- MongoDB stores data records as documents(specifically BSON/JSON documents) which are gathered together as colletion.
- Documents contain one or more fields and each field contains a valid data type.
- A group of documents is called collection.
- DOCUMENTS -> ROWS, COLLECTION -> TABLES, FIELDS -> COLUMNS

<br>

## [YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---
