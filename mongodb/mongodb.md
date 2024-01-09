# mongodb

This repository contains interview questions for mongodb.

<a name="TableOfContents"></a><h2>TABLE OF CONTENTS:</h2>

| Serial No | Topic Name                                                                                                                       |
| --------- | -------------------------------------------------------------------------------------------------------------------------------- |
| 1         | [MONGODB AND ITS FEATURES](#mdb)                                                                                                 |
| 2         | [ALTERNATIVE NOSQL DATABASES TO MONGODB](#alternative)                                                                           |
| 3         | [WHAT TYPE OF NOSQL DATABASE IS MONGODB?](#type)                                                                                 |
| 4         | [HOW DOES MONGODB STORE DATA?](#store)                                                                                           |
| 5         | [MONGODB IS A SCHEMALESS DATABASE. IF YES < HOW DO WE CREATE SCHEMAS IN MONGODB?](#schemas)                                      |
| 6         | [HOW IS MONGODB DIFFERENT FROM SQL AND BETTER THAN MYSQL?](#sql)                                                                 |
| 7         | [DIFFERENT DATA MODELS IN MONGODB](#datamodels)                                                                                  |
| 8         | [HOW DOES INDEXING WORK IN MONGODB?](#indexing)                                                                                  |
| 9         | [WHAT IS MONGODB REPLICATION AND SHARDING? ](#replication)                                                                       |
| 10        | [HORIZONTAL AND VERTICAL SCALING](#scaling)                                                                                      |
| 11        | [WHAT ARE REPLICA SETS? EXPLAIN PRIMARY AND SECONDARY REPLICA SETS?](#replica)                                                   |
| 12        | [USE OF CAPPED COLLECTION](#capped)                                                                                              |
| 13        | [HOW CAN YOU STORE IMAGES,VIDEOS & OTHER LARGE FILES(> 16mb?](#large)                                                            |
| 14        | [AGGREGATION IN MONGODB](#aggregation)                                                                                           |
| 15        | [\_id FIELD IN MONGODB?](#id)                                                                                                    |
| 16        | [MAP REDUCE PROCESS IN MONGODB](#mapreduce)                                                                                      |
| 17        | [WHAT ARE SOME UTILITIES FOR BACKUP AND RESTORING IN MONGODB](#backup)                                                           |
| 18        | [HOW DOES MONGODB ENSURE HIGH AVAILABILITY OF DATA?](#availability)                                                              |
| 19        | [ROLE OF PROFILER IN MONGODB](#profiler)                                                                                         |
| 20        | [CAN WE USE REGULAR EXPRESSIONS IN MONGODB?](#regex)                                                                             |
| 21        | [DIFFERENCE BETWEEN $all AND $in OPERATOR](#diff)                                                                                |
| 22        | [BOTH WRITES AND READS BECOME FASTER WHEN YOU ADD MORE SLAVES TO REPLICA SET. IS THIS STATEMENT TRUE OR FALSE? EXPLAIN](#slaves) |
| 23        | [MONGODB EQUIVALENT OF JOIN CLAUSE & ITS LIMITATIONS](#equi)                                                                     |
| 24        | [ADVANTAGES OF MONGODB](#adv)                                                                                                    |
| 25        | [APPLICATIONS OF MONGODB](#application)                                                                                          |
| 26        | [WHEN SHOULD WE EMBED ONE DOCUMENT WITH ANOTHER?](#embed)                                                                        |
| 27        | [DIFFERENT DATA MODELS IN MONGODB](#datamodels)                                                                                  |
| 28        | [DIFFERENT DATA MODELS IN MONGODB](#datamodels)                                                                                  |
| 29        | [DIFFERENT DATA MODELS IN MONGODB](#datamodels)                                                                                  |
| 30        | [DIFFERENT DATA MODELS IN MONGODB](#datamodels)                                                                                  |
| 31        | [ DIFFERENCE BETWEEN `update` AND `FindOneAndUpdate` ](#update)                                                                  |
| 32        | [DIFFERENCE BETWEEN `drop` AND `remove`](#drop)                                                                                  |

## <a name="mdb"></a><h2>1. MONGODB AND ITS FEATURES</h2>

MongoDb is a NOSQL( Not Only SQL) database that stores large volumes of data of documents. This offers developers the flexibility to work with eveolving data models.

- Relational Databases are mostly rows and columns and in table format and we can link our tables using a foreign key. They follow the ACID properties.

- MongoDB uses documents to store and retrieve documents, which provide scalability and flexibility in terms of quering data and indexing.

- based on JSON like features to store the data.

<br>

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="alternative"></a><h2>2. ALTERNATIVE NOSQL DATABASES TO MONGODB</h2>

- Apache Cassandra
- Redis
- AMazon DynamoDB
- Neo4j
- Apache HBase

<br>

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="type"></a><h2>3. WHAT TYPE OF NOSQL DATABASE IS MONGODB?</h2>

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

## <a name="store"></a><h2>4. HOW DOES MONGODB STORE DATA?</h2>

- MongoDB stores data records as documents(specifically BSON/JSON documents) which are gathered together as colletion.
- Documents contain one or more fields and each field contains a valid data type.
- A group of documents is called collection.
- DOCUMENTS -> ROWS, COLLECTION -> TABLES, FIELDS -> COLUMNS

<br>

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="schemas"></a><h2>5. MONGODB IS A SCHEMALESS DATABASE. IF YES < HOW DO WE CREATE SCHEMAS IN MONGODB?</h2>

- The schema of a database describes the structure of the data to be stored.
- In relational databases, schema defined by the tables, fields and relationship between them. EG SQL
- In documented oreiented databases like mongodb , data is stored in key value pairs, given that MongoDB is schema free - which means it has dynamically typed data.
- Whenever we create a document to create a schema, it will automatically generate for us.
- Whenever the document is added the database automatically creates the collectiom

<br>

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="sql"></a><h2>6. HOW IS MONGODB DIFFERENT FROM SQL AND BETTER THAN MYSQL?</h2>

![image](https://github.com/Sushmita-Ghosh/interview_practice/assets/82622059/343ffeb2-5c7f-48bc-8cb7-bfe243fc8d97)

- Atomic Operations - ACID PROPERTIES
- No TRANSACTION- SUPPORTS CAP THEROM

<br>

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="datamodels"></a><h2>7. DIFFERENT DATA MODELS IN MONGODB</h2>

Data Models are of two types

- EMBEDDED DATA MODEL: Embedded documents capture relationships between data by storing related data in a single document structure.
- REFERENCE DATA MODEL: Reference model store the elationships between data by including links or references from one document to another.

<br>

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="datamodels"></a><h2>7. DIFFERENT DATA MODELS IN MONGODB</h2>

Data Models are of two types

- EMBEDDED DATA MODEL: Embedded documents capture relationships between data by storing related data in a single document structure.
- REFERENCE DATA MODEL: Reference model store the elationships between data by including links or references from one document to another.

<br>

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="indexing"></a><h2>| 8. HOW DOES INDEXING WORK IN MONGODB?</h2>

Indexes provide users with an efficient way of quering data.

- Avoid Collection Scan: In absence of indexing in mongodb we have run through every collection which is a collection scan.

- Effective Indexing Strategy: MongoDB allows indexing on one or multiple fields across collections. We need a good indexing strategy to quickly acces the data we need.

- Search Efficiently: Indexing is a necessary operation in
  MongoDB, which will bring search efficiency in various execution of statements.

<br>

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="replication"></a><h2>| 9. WHAT IS MONGODB REPLICATION AND SHARDING?</h2>

- **Replication:** Involves duplicating data across multiple MongoDB servers for high availability and data redundancy.

  - Data redundancy and High Availaility
  - Multiple Copies Across Servers - gets corrupted by any meand or lost we can get from replicas
  - Data Recovery and Backup Options - Data can be retrieved on hardware failures

- **Sharding:** Distributes data across multiple databases or servers, enhancing throughput and scalability.
  <br>

  - Eg : Database with 2 million users - having capacity of 2 million records. Now we can divide this data into 2 mc which each have 1 million user capacity.

  - We can add more capacity to a single server such as adding more memory and processing units or adding more ram on the single server.

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="scaling"></a><h2>| 10. HORIZONTAL AND VERTICAL SCALING</h2>

- **VERTICAL SCALING:** refers to adding more resources (CPU/RAM/DISK) to ur server(database or application server is still remains one) as on demand

- **HORIZONTAL SCALING:** involves adding more processing units or physical machines to your server or database. MongoDb handles horizontal scaling through sharding.

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="embed"></a><h2>26. WHEN SHOULD WE EMBED ONE DOCUMENT WITH ANOTHER?</h2>

We should consider embedded documents(subdocuments) for:
![image](https://github.com/Sushmita-Ghosh/interview_practice/assets/82622059/981b4105-a25a-44d1-a43d-b5d126150bee)

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="replica"></a><h2>11. WHAT ARE REPLICA SETS? EXPLAIN PRIMARY AND SECONDARY REPLICA SETS?</h2>

We should consider embedded documents(subdocuments) for:

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="capped"></a><h2>12.USE OF CAPPED COLLECTION</h2>

We should consider embedded documents(subdocuments) for:

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="large"></a><h2>13.HOW CAN YOU STORE IMAGES,VIDEOS & OTHER LARGE FILES(> 16mb?</h2>

We should consider embedded documents(subdocuments) for:

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="aggregation"></a><h2>14.AGGREGATION IN MONGODB</h2>

We should consider embedded documents(subdocuments) for:

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="id"></a><h2>15.\_id FIELD IN MONGODB?</h2>

We should consider embedded documents(subdocuments) for:

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="mapreduce"></a><h2>16.MAP REDUCE PROCESS IN MONGODB</h2>

We should consider embedded documents(subdocuments) for:

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="backup"></a><h2>17.WHAT ARE SOME UTILITIES FOR BACKUP AND RESTORING IN MONGODB</h2>

We should consider embedded documents(subdocuments) for:

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="availability"></a><h2>18. HOW DOES MONGODB ENSURE HIGH AVAILABILITY OF DATA?</h2>

We should consider embedded documents(subdocuments) for:

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="profiler"></a><h2>19. ROLE OF PROFILER IN MONGODB</h2>

We should consider embedded documents(subdocuments) for:

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="regex"></a><h2>20. CAN WE USE REGULAR EXPRESSIONS IN MONGODB?</h2>

We should consider embedded documents(subdocuments) for:

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="diff"></a><h2>21. DIFFERENCE BETWEEN $all AND $in OPERATOR</h2>

We should consider embedded documents(subdocuments) for:

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="slaves"></a><h2>22. BOTH WRITES AND READS BECOME FASTER WHEN YOU ADD MORE SLAVES TO REPLICA SET. IS THIS STATEMENT TRUE OR FALSE? EXPLAIN</h2>

We should consider embedded documents(subdocuments) for:

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="equi"></a><h2>23. MONGODB EQUIVALENT OF JOIN CLAUSE & ITS LIMITATIONS</h2>

We should consider embedded documents(subdocuments) for:

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="adv"></a><h2>24. ADVANTAGES OF MONGODB</h2>

MongoDB stands out due to its:

- Open-source nature
- User-friendly syntax
- High flexibility for diverse data types
- Advanced security features
- Efficient indexing for rapid data retrieval
- Dynamic schema design adaptable to evolving data requirements

---

## <a name="application"></a><h2>25. APPLICATIONS OF MONGODB</h2>

MongoDB's versatility finds applications in:

- IoT data storage
- Mobile applications for real-time analysis
- Catalog, content, and product management
- Large-scale databases like India's Aadhar card system

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="capped"></a><h2>26. USE OF CAPPED COLLECTION</h2>

We should consider embedded documents(subdocuments) for:

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="capped"></a><h2>27. USE OF CAPPED COLLECTION</h2>

We should consider embedded documents(subdocuments) for:

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="capped"></a><h2>28. USE OF CAPPED COLLECTION</h2>

We should consider embedded documents(subdocuments) for:

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="capped"></a><h2>29. USE OF CAPPED COLLECTION</h2>

We should consider embedded documents(subdocuments) for:

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="capped"></a><h2>30. USE OF CAPPED COLLECTION</h2>

We should consider embedded documents(subdocuments) for:

[YT](https://www.youtube.com/watch?v=EKEpVhi-29Q)

---

## <a name="update"></a><h2>31. DIFFERENCE BETWEEN `update` AND `FindOneAndUpdate` </h2>

![image](https://github.com/Sushmita-Ghosh/interview_practice/assets/82622059/d3464961-615d-41c6-9681-d23c1661fe04)


- update - more than one documents matching the condition
- findOneAndUpdate - only one document - if not matched origin document is returned

[YT](https://www.youtube.com/watch?v=fxUCxEQY7sM&list=PLp50dWW_m40X_GTW0CXYlkojMT74i2O1i&index=1)

---
