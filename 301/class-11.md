# Class 10

## Significance

There are fundamental differences between the two types of databases in common use; knowing about them is important to using them.

## Things I want to know more about

I'd like to learn PostgreSQL as well as MongoDB.

## Questions:

[nosql vs sql](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

1. Differences Between SQL & NoSQL:

SQL |   NoSQL
---
tabled based | key-value pairs
---
pre-defined schema | dynamic schema
---
vertically scalable | horizontally scalable
---
atomicity, consistency, isolation, durability | consistency, availability, partition tolarance
---
transactional | not as good for "transactional"

2. What kind of data is a good for an SQL database?

transactional
    
    Real World Example: Banking, where a high level of data integrity is required

3. What kind of data is a good fit for a NoSQL database?

heirarchical

    Real World Example: "big data" where emphasis is on speed, scaling, and dynamicity 

4. Which type of database is best for heirarchical data storage?

NoSQL

5. Which type of database is best for scalability?

NoSql can be scaled more easily accross servers, big data

[nosql vs sql](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y) Video

1. What does SQL stand for?

Structured Query Language

2. What is a relational database?

A database with tables with fields that have defined relationships with fields in other tables. 

3. Which type of structure does a relational database work with?

Tables

4. What is a 'schema'?

The structure of the database records, such as the exact fields that *every* record in a table has.

5. What is a NoSQL database?

A NoSQL database doesn't have tables or relationships. Instead, it has collections of key-value pairs (document objects).

6. How does it work?

The collection of documents associates identifying keys with values of varying schema.

8. Which is more flexible - SQL or MongoDB, and why?

NoSQL databases can hold varying types of data without adherence to a strict schema, meaning they can handle new types of entries without restructuring the database.

9. What is the disadvantage of a NoSQL database?

Relations and strict schema can ensure data integrity and allow for complex queries, which NoSQL lacks.