# mongodb

This repository contains interview questions for mongodb.

<a name="TableOfContents"></a><h2>TABLE OF CONTENTS:</h2>

| Serial No | Topic Name                                                                                  |
| --------- | ------------------------------------------------------------------------------------------- |
| 1         | [MONGODB AND ITS FEATURES](#mdb)                                                            |
| 2         | [ALTERNATIVE NOSQL DATABASES TO MONGODB](#alternative)                                      |
| 3         | [WHAT TYPE OF NOSQL DATABASE IS MONGODB?](#type)                                            |
| 4         | [HOW DOES MONGODB STORE DATA?](#store)                                                      |
| 5         | [MONGODB IS A SCHEMALESS DATABASE. IF YES < HOW DO WE CREATE SCHEMAS IN MONGODB?](#schemas) |
| 6         | [HOW IS MONGODB DIFFERENT FROM SQL AND BETTER THAN MYSQL?](#sql)                            |

## <a name="mdb"></a><h2>MONGODB AND ITS FEATURES</h2>

MongoDb is a NOSQL( Not Only SQL) database that stores large volumes of data of documents. This offers developers the flexibility to work with eveolving data models.

- Relational Databases are mostly rows and columns and in table format and we can link our tables using a foreign key. They follow the ACID properties.

- MongoDB uses documents to store and retrieve documents, which provide scalability and flexibility in terms of quering data and indexing.

- based on JSON like features to store the data.

<br>

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="alternative"></a><h2>ALTERNATIVE NOSQL DATABASES TO MONGODB</h2>

- Apache Cassandra
- Redis
- AMazon DynamoDB
- Neo4j
- Apache HBase

<br>

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="type"></a><h2>WHAT TYPE OF NOSQL DATABASE IS MONGODB?</h2>

- KEY VALUE:

  - store values as an index-key and value pairs
  - schemaless way
  - Cassandra, DynamoDB

- COLUMN BASED:

  - stores data in a column format rather than row format.
  - row format is used in traditional databases.
  - HBASE, CASSANDRA

- DOCUMENT BASED:

  - designed to store data in form of documents ; with each document having a unique key
  - Couchbase, MongoDB

- GRAPH BASED:

  - designed for data that needs to be represented as graphs.
  - interconnected data in form of graphs and trees
  - Neo4j and BigData

<br>

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="store"></a><h2>HOW DOES MONGODB STORE DATA?</h2>

- MongoDB stores data records as documents(specifically BSON/JSON documents) which are gathered together as colletion.
- Documents contain one or more fields and each field contains a valid data type.
- A group of documents is called collection.
- DOCUMENTS -> ROWS, COLLECTION -> TABLES, FIELDS -> COLUMNS

<br>

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="schemas"></a><h2>MONGODB IS A SCHEMALESS DATABASE. IF YES < HOW DO WE CREATE SCHEMAS IN MONGODB?</h2>

- The schema of a database describes the structure of the data to be stored.
- In relational databases, schema defined by the tables, fields and relationship between them. EG SQL
- In documented oreiented databases like mongodb , data is stored in key value pairs, given that MongoDB is schema free - which means it has dynamically typed data.
- Whenever we create a document to create a schema, it will automatically generate for us.
- Whenever the document is added the database automatically creates the collectiom

<br>

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="sql"></a><h2>HOW IS MONGODB DIFFERENT FROM SQL AND BETTER THAN MYSQL?</h2>

![image](https://github.com/Sushmita-Ghosh/interview_practice/assets/82622059/343ffeb2-5c7f-48bc-8cb7-bfe243fc8d97)

<br>

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---
