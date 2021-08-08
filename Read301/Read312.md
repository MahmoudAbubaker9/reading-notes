# Mongo and Mongoose 

## 1. Fill in the chart below with five differences between SQL and NoSQL databases:

 	 
| SQL  |   NoSQL                                          |
|-------|--------------------------------------------------|
|SQL databases are table based databases  |NoSQL databases are document based|
|SQL databases have predefined schema|databases have dynamic schema for unstructured data|
|SQL databases are vertically scalable|NoSQL databases are horizontally scalable|
|SQL databases are not best fit for hierarchical data storage|NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data|
|SQL databases are vertically scalable. You can manage increasing load by increasing the CPU, RAM, SSD, etc, on a single server. On the other hand|NoSQL databases are horizontally scalable. You can just add few more servers easily in your NoSQL database infrastructure to handle the large traffic.|
 	 
 	 
## 2. What kind of data is a good fit for an SQL database?

SQL databases are good fit for the complex query intensive environment

## 3. What kind of data is a good fit a NoSQL database?

NoSQL databases are not good fit for complex queries. On a high-level

## 4. Which type of database is best for hierarchical data storage?

NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data. NoSQL database are highly preferred for large data set (i.e for big data). Hbase is an example for this purpose.

## 5. Which type of database is best for scalability?

NoSQL databases

# sql vs nosql

## 1. What does SQL stand for?

Structured Query Language

## 2. What is a realational database?

is a type of database that stores and provides access to data points that are related to one another

## 3. What type of structure does a relational database work with?

1. one-to-one
2. one-to-many
3. many-to-many


## 4. What is a ‘schema’?

is the organization or structure for a database, 


## 5. What is a NoSQL database?

 database provides a mechanism for storage and retrieval of data that is modeled in means other than the tabular relations used in relational databases


## 6. How does it work?

One way of understanding the appeal of NoSQL databases from a design perspective is to look at how the data models of a SQL and a NoSQL database might look in an oversimplified example using address data.




## 7. What is inside of a Mongo database?

MongoDB stores data records as documents (specifically BSON documents) which are gathered together in collections. A database stores one or more collections of documents.



## 8. Which is more flexible - SQL or MongoDB? and why.

MongoDB offers faster query processing but with an increased load and system requirements. Without knowing the purpose of use, it is not possible to classify SQL Databases or NoSQL Databases like MongoDB as better or worse than the other. 

SQL is better 

## 9. What is the disadvantage of a NoSQL database?

1. NoSQL databases don’t have the reliability functions which Relational Databases have (basically don’t support ACID).

2. NoSQL are very new compared to Relational Databases, which means that are far less stable and may have a lot less functionalities

3. NoSQL is not compatible (at all) with SQL