# Mongoose

        Mongoose is an Object Data Modeling (ODM) library for MongoDB
        and Node.js. It manages relationships between data, provides
        schema validation, and is used to translate between objects
        in code and the representation of those objects in MongoDB.



![Mongoose](https://cdn-media-1.freecodecamp.org/images/0*b5piDNW1dqlkJWKe.)


_MongoDB is a schema-less **NoSQL** document database. It means you can store JSON documents in it, and the structure of these documents can
vary as it is not enforced like SQL databases. This is one of the 
advantages of using NoSQL as it speeds up application development and reduces the complexity of deployments._

### Below is an example of how data is stored in Mongo vs. SQL Database:



![example](https://cdn-media-1.freecodecamp.org/images/0*rcotALFe2LeebN_y.)


**SQL**

![sql](https://cdn-media-1.freecodecamp.org/images/0*QOKLctlRwxs5uKVo.)



## Terminologies

**Collections**

        ‘Collections’ in Mongo are equivalent to tables in relational
         databases. They can hold multiple JSON documents.

**Documents**

        ‘Documents’ are equivalent to records or rows of data in SQL.
         While a SQL row can reference data in other tables, Mongo 
         documents usually combine that in a document.

**Fields**
        ‘Fields’ or attributes are similar to columns in a SQL table.

**Schema**

        While Mongo is schema-less, SQL defines a schema via the
        table definition. A Mongoose ‘schema’ is a document data
        structure (or shape of the document) that is enforced via
        the application layer.

**Models**

        ‘Models’ are higher-order constructors that take a schema and 
        create an instance of a document equivalent to records in a 
        relational database.



# Mongo and Mongoose

1- What kind of data is a good fit for an SQL database?

        data that is highly structured and associations among the
        program entities are clearly defined.

2- Give a real world example.

        if you are developing a point of employees system where you
        need to store ID Employees and position and salary and
        departments.

3- What kind of data is a good fit a NoSQL database?

        key-value stores, wide column stores, graph databases, and
        document databases,

4- Give a real world example.

        JSON files

5- Which type of database is best for hierarchical data storage?

        N0-SQL

6- Which type of database is best for scalability?

        SQL
