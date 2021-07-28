# Mongo and Mongoose

## NoSQL and SQL
[Questions were answered based on info from here](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

1. Fill in the chart below with five differences between SQL and NoSQL databases:

SQL                  |  NoSQL
---------------------|-----------------
Relational Databases | non-relational
Table based | document based, key-value, graph, wide-column stores
Predefined schema | dyanmic schema
vertically scalabe | horizontally scalable
Uses Structured Query Language | Collection of documents (somtimes called UnQL for Unstructured Query Language)

2. What kind of data is a good fit for an SQL database?
  - Complex query intensive environment
  - Heirarchical data storage
3. Give a real world example.
  - Transactions
4. What kind of data is a good fit a NoSQL database?
  - Large data sets
5. Give a real world example.
  - Hbase, anything that can be stored in key-value pairs.
6. Which type of database is best for hierarchical data storage?
  - NoSQL
7. Which type of database is best for scalability?
> In most typical situations, SQL databases are vertically scalable. You can manage increasing load by increasing the CPU, RAM, SSD, etc, on a single server. On the other hand, NoSQL databases are horizontally scalable. You can just add few more servers easily in your NoSQL database infrastructure to handle the large traffic.

[Following questions were answered based on this video](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)

1. What does SQL stand for?
  - Structured Query Language
2. What is a realational database?
  - Collection of data that works in a predetermined way.
3. What type of structure does a relational database work with?
  - Table
4. What is a ‘schema’?
  - Determines which data is allowed into the table.
  - Data must conform to a defind layout/organization.
5. What is a NoSQL database?
  - MongoDB
6. How does it work?
  - Instead of Tables, noSQL has `collections`.
  - Inside the collections you have `documents`.
  - Documents do not have to follow the same schema.
7. What is inside of a Mongo database?
  - A `Collection` of `documents` that contain relevant data.
8. Which is more flexible - SQL or MongoDB? and why.
  - MongoDB because data does not have to conform to the same schema and therefore you can store more data.
  - No relations, or very few relations. 
9. What is the disadvantage of a NoSQL database?
  - Duplicate data. Data needs to be updated in all documents with that data.

[Back to HOME](../README.md)