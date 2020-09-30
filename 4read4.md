## Why would a developer choose to make data models?
Models allow devs to easily normalize data!
Data models allow devs to clearly define the scope of the the project, as well as clarifying the purpose of the application.  Data models also allow clearer documentation and can help prevent data errors.

## What purpose do CRUD operations serve?
CRUD operations are the 4 basic data manipulations of a relational database.  It stands for Create Read Update Delete.

## What kind of database is Postgres? What kind of database is MongoDB?
Postgres is a relational database, MongoDB is a document-oriented or NoSQL database, that uses optional schemas and is not relational.  

## What is Mongoose and why do we need it?
[Mongo Basics](https://www.freecodecamp.org/news/introduction-to-mongoose-for-mongodb-d2a7aa593c57/#:~:text=Mongoose%20is%20an%20Object%20Data,of%20those%20objects%20in%20MongoDB)
Mongoose is an Object Data Modeling (ODM) library for MongoDB and Node.js. It manages relationships between data, provides schema validation, and is used to translate between objects in code and the representation of those objects in MongoDB.

Using Mongoose, a user can define the schema for the documents in a particular collection. It provides a lot of convenience in the creation and management of data in MongoDB. On the downside, learning mongoose can take some time, and has some limitations in handling schemas that are quite complex.


## Describe how NoSQL Databases scale horizontally
NoSQL DBs can scale on many small distributed machines since it is able to scale horizontally, whereas a relational database must be stored on a single server on a single machine.

## Give one strong argument for and against NoSQL Databases
noSQL databases are much easier to scale than SQL dbs, but these benefits come at the cost of relaxing ACID principles: instead of keeping all four parameters consistent throughout every transaction, NoSQL uses the principle of eventual consistency. This means that if there are no new updates for a particular data item for a certain period of time, eventually all accesses to it will return the last updated value. That’s why such systems are usually described as providing BASE guarantees (Basically Available, Soft state, Eventual consistency) — as opposed to ACID.

While this approach greatly increases access time and scalability, it may lead to data loss – the severity of the problem depends on database server support and the quality of application code. In some cases, this issue might be very serious.

(https://bitnine.net/blog-computing/sql-vs-nosql-comparative-advantages-and-disadvantages/)


## Name 3 cloud based NoSQL Databases
Apache Cassandra, MongoDB,

# Terminologies

## Collections
‘Collections’ in Mongo are equivalent to tables in relational databases. They can hold multiple JSON documents.

## Documents
‘Documents’ are equivalent to records or rows of data in SQL. While a SQL row can reference data in other tables, Mongo documents usually combine that in a document.

## Fields
‘Fields’ or attributes are similar to columns in a SQL table.

## Schema
While Mongo is schema-less, SQL defines a schema via the table definition. A Mongoose ‘schema’ is a document data structure (or shape of the document) that is enforced via the application layer.

## Models
‘Models’ are higher-order constructors that take a schema and create an instance of a document equivalent to records in a relational database.

- database - any organized collection of data
- data model - A data model is an abstract model that organizes elements of data and standardizes how they relate to one another and to the properties of real-world entities. For instance, a data model may specify that the data element representing a car be composed of a number of other elements which, in turn, represent the color and size of the car and define its owner.
- CRUD - Create Read Update Delete
- schema - schemas define the 'shape' of the data in a database.  In a relational database the schema is enforced by default, whereas in a nonrelational database schemas must be artificially enforced.
- sanitize - refers to normalization of data before inputting into a database
- Structured Query Language (SQL) is a domain-specific language used in programming and designed for managing data held in a relational database management system (RDBMS), or for stream processing in a relational data stream management system (RDSMS). It is particularly useful in handling structured data, i.e. data incorporating relations among entities and variables.
- Non SQL (NoSQL) - A NoSQL (originally referring to "non-SQL" or "non-relational")[1] database provides a mechanism for storage and retrieval of data that is modeled in means other than the tabular relations used in relational databases. 
- MongoDB - MongoDB is a cross-platform document-oriented database program. Classified as a NoSQL database program, MongoDB uses JSON-like documents with optional schemas.
- Mongoose - Mongoose is an Object Data Modeling (ODM) library for MongoDB and Node.js. It manages relationships between data, provides schema validation, and is used to translate between objects in code and the representation of those objects in MongoDB.
- record
- document
- Object Relation Mapping (ORM) - Object-relational mapping (ORM, O/RM, and O/R mapping tool) in computer science is a programming technique for converting data between incompatible type systems using object-oriented programming languages. This creates, in effect, a "virtual object database" that can be used from within the programming language.

[what is a rest api?](https://www.youtube.com/watch?v=Q-BpqyOT3a8)
[http basics](https://code.tutsplus.com/tutorials/http-the-protocol-every-web-developer-must-know-part-1--net-31177)
[what is REST?](https://restfulapi.net/)

How to insert cursor at beginning of every line:

Press CTRL + A to select all of the text.
Press SHIFT + ALT + I to insert multiple cursors at the end of each line.
Press Home twice to jump to the start of every line.