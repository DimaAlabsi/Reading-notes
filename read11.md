# Mongo and Mongoose



### nosql vs sql
| nosql    | sql |
| ----------- | ----------- |
|NoSQL database are primarily called as non-relational or distributed database.|SQL databases are primarily called as Relational Databases (RDBMS);|
| NoSQL databases are document based, key-value pairs, graph databases or wide-column stores|SQL databases are table based databases|
|NoSQL databases have dynamic schema for unstructured data.|SQL databases have predefined schema|
|NoSQL databases are horizontally scalable|SQL databases are vertically scalable |
|In NoSQL database, queries are focused on collection of documents. Sometimes it is also called as UnQL (Unstructured Query Language). |SQL databases uses SQL ( structured query language ) for defining and manipulating the data, which is very powerful|

------------------------------------
![sql vs nosql](https://i.ytimg.com/vi/QwevGzVu_zk/maxresdefault.jpg)

+ **SQL databases are good fit for the complex query intensive environment whereas NoSQL databases are not good fit for complex queries. On a high-level, NoSQL don’t have standard interfaces to perform complex queries, and the queries themselves in NoSQL are not as powerful as SQL query language.**


+ ***SQL databases are not best fit for hierarchical data storage. But, NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data. NoSQL database are highly preferred for large data set (i.e for big data). Hbase is an example for this purpose.***



+ **In most typical situations, SQL databases are vertically scalable. You can manage increasing load by increasing the CPU, RAM, SSD, etc, on a single server. On the other hand, NoSQL databases are horizontally scalable. You can just add few more servers easily in your NoSQL database infrastructure to handle the large traffic.**

![sql vs nosql](https://www.clariontech.com/hs-fs/hubfs/SQL-NOSQL.png?width=813&name=SQL-NOSQL.png)


---------------------------------

+ SQL stands for Structured Query Language
+ SQL lets you access and manipulate databases
+ SQL became a standard of the American National Standards Institute (ANSI) in 1986, and of the International Organization for Standardization (ISO) in 1987..

+ relational database is a type of database that stores and provides access to data points that are related to one another.

+ ***relational model means that the logical data structures—the data tables, views, and indexes—are separate from the physical storage structures. This separation means that database administrators can manage physical data storage without affecting access to that data as a logical structure***



+ schema, or scheme, is an abstract concept proposed by J. Piaget to refer to our, well, abstract concepts. Schemas (or schemata) are units of understanding that can be hierarchically categorized as well as webbed into complex relationships with one another.

+ A NoSQL (originally referring to "non-SQL" or "non-relational")[1] database provides a mechanism for storage and retrieval of data that is modeled in means other than the tabular relations used in relational databases

+ ***MongoDB is a document-oriented NoSQL database used for high volume data storage. Instead of using tables and rows as in the traditional relational databases, MongoDB makes use of collections and documents. Documents consist of key-value pairs which are the basic unit of data in MongoDB. Collections contain sets of documents and function which is the equivalent of relational database tables. MongoDB is a database which came into light around the mid-2000s.***


+ The core differences between these two database systems are significant. Choosing which one to use is really a question of approach rather than purely a technical decision.


+ MySQL is a mature relational database system, offering a familiar database environment for experienced IT professionals.

![SQL or MongoDB?](https://blog.sqlauthority.com/wp-content/uploads/2020/05/MappingRelationalSQL-scaled.jpg)


+ MongoDB is a well-established, non-relational database system offering improved flexibility and horizontal scalability, but at the cost of some safety features of relational databases, such as referential integrity.




+ MongoDB vs MySQL Flexibility
This is an easy one, and a hands down win for MongoDB. The schemaless design of MongoDB documents makes it extremely easy to build and enhance applications over time, without needing to run complex and expensive schema migration processes as you would with a relational database.

* With MongoDB, there are more dynamic options for updating the schema of a collection, such as creating new fields based on an aggregation pipeline or updating nested array fields. This benefit is particularly important as databases grow in size. In contrast, larger MySQL databases are slower to migrate schemas and stored procedures that can be dependent on the updated schemas. MongoDB’s flexible design makes this much less of a concern.

* databases don't have the reliability functions which Relational Databases have (basically don't support ACID). ...
In order to support ACID developers will have to implement their own code, making their systems more complex. ...
NoSQL is not compatible (at all) with SQL.

![SQL or MongoDB?](https://www.researchgate.net/profile/Smaqil-Burney/publication/340622952/figure/fig4/AS:880217438564360@1586871599608/SQL-vs-MongoDB-terms.png)



 #### &copy; Dima Alabsi; 2021 
