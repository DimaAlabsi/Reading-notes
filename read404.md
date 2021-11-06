# Data Modeling

**Name 3 advantages to Test Driven Development**

1. Better program design and higher code quality

2. Detailed project documentation


3. TDD reduces the time required for project development


---------------

**In what case would you need to use beforeEach() or afterEach() in a test suite?**

 which 1. removes the explicit calls from the tests themselves, and 2. invites inexperienced users to share state between tests.

 --------------------------

 **What is one downside of Test Driven Development?**

 * No silver bullet: Tests help to find bugs, but they can't find bugs that you introduce in the test code and in implementation code. If you haven't understood the problem you need to solve, writing tests most probably doesn't help.
It seems slower at the beginning: If you start TDD, you will get the feeling that you need a longer duration of time for easy implementations. You need to think about the interfaces, write the test code, and run the tests before you can finally start writing the code.

-------------

**What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?**

* ES6 class constructors : This can be said to be a syntax base for constructor functions and instantiate objects using a new operator

* 	ES5 function constructors : 
This can be said to be a syntax base for constructor functions and instantiate objects using a new operator.	This also uses a new operator for object creation but focuses on how the objects are being instantiated.

---------------------

Why REST ?

* REST aims to make caching easier. Since the server is stateless and each request can be processed individually, GET requests should usually return the same response regardless of previous ones and the session. This makes the GET requests easily cacheable and browsers usually treat them as such.
----------------------

|TERM||
|----|------|
|functional programming|a programming paradigm where programs are constructed by applying and composing functions. It is a declarative programming paradigm in which function definitions are trees of expressions that map values to other values, rather than a sequence of imperative statements which update the running state of the program.|
|object-oriented programming (OOP)|is a computer programming model that organizes software design around data, or objects, rather than functions and logic. An object can be defined as a data field that has unique attributes and behavior.|
|class| blueprint for creating objects. A class encapsulates data and functions that manipulate data. |
|super|keyword is used to access and call functions on an object's parent.|
|this| the value of this is determined by how a function is called (runtime binding). It can't be set by assignment during execution, and it may be different each time the function is called. |
|Test Driven Development (TDD)| software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing the software against all test cases. This is as opposed to software being developed first and test cases created later.|
|Jest| software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing the software against all test cases. This is as opposed to software being developed first and test cases created later.|
|Continuous Integration (CI)|the practice of automating the integration of code changes from multiple contributors into a single software project. It’s a primary DevOps best practice, allowing developers to frequently merge code changes into a central repository where builds and tests then run. Automated tools are used to assert the new code’s correctness before integration.|
|REST|an application programming interface (API or web API) that conforms to the constraints of REST architectural style and allows for interaction with RESTful web services. REST stands for representational state transfer and was created by computer scientist Roy Fielding.|
|Data Model| abstract model that organizes elements of data and standardizes how they relate to one another and to the properties of real-world entities. ... The term data model can refer to two distinct but closely related concepts.
|

Which 3 things had you heard about previously and now have better clarity on?

DB ever
pg admin
sqlite3

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
postregs
testing by jest
react.js

What are you most excited about trying to implement or see how it works?
react.js

--------------------------

### Preparation Materials :

### sql vs nosql


**What is NoSQL?**

* NoSQL is a non-relational DMS, that does not require a fixed schema, avoids joins, and is easy to scale. NoSQL database is used for distributed data stores with humongous data storage needs. NoSQL is used for Big data and real-time web apps. For example companies like Twitter, Facebook, Google that collect terabytes of user data every single day.

* NoSQL database stands for “Not Only SQL” or “Not SQL.” Though a better term would NoREL NoSQL caught on. Carl Strozz introduced the NoSQL concept in 1998.

* Traditional RDBMS uses SQL syntax to store and retrieve data for further insights. Instead, a NoSQL database system encompasses a wide range of database technologies that can store structured, semi-structured, unstructured and polymorphic data.


**What is SQL?**

* Structured Query language (SQL) pronounced as “S-Q-L” or sometimes as “See-Quel” is the standard language for dealing with Relational Databases. A relational database defines relationships in the form of tables.

* SQL programming can be effectively used to insert, search, update, delete database records.

* That doesn’t mean SQL cannot do things beyond that. It can do a lot of things including, but not limited to, optimizing and maintenance of databases.

* Relational databases like MySQL Database, Oracle, Ms SQL Server, Sybase, etc. use SQL.


[Read MORE about sql vs nosql](https://youtu.be/FR4QIeZaPeM)

* Sequelize is a promise-based Node.js ORM tool for Postgres, MySQL, MariaDB, SQLite and Microsoft SQL Server. It features solid transaction support, relations, eager and lazy loading, read replication and more. [Visit sequelize website & Know More](https://sequelize.org/master/)


***Differences between **sql** and **nosql***** 👍

|Sql|Nosql|
|------|--------|
|SQL databases are vertically scalable|NoSQL databases are horizontally scalable|
|SQL databases are primarily called as Relational Databases (RDBMS)|NoSQL database are primarily called as non-relational or distributed database.|
|SQL databases are table based databases|NoSQL databases are document based|
|SQL databases uses SQL ( structured query language ) for defining and manipulating the data, which is very powerful|In NoSQL database, queries are focused on collection of documents.|


 #### &copy; Dima Alabsi; 2021

