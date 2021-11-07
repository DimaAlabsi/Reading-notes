#  Authentication

## Review, Research, and Discussion 👍

1.Explain what a “Singleton” is (in Computer Science terms)


* A singleton is a class that allows only a single instance of itself to be created and gives access to that created instance. It contains static variables that can accommodate unique and private instances of itself. It is used in scenarios when a user wants to restrict instantiation of a class to only one object.

2.Explain how the Singleton pattern can be used with Node modules, specifically with classes

* We need singleton when we want to make sure there is only one object instantiated. Therefore, instead of creating a new object we need to ensure the constructor was called only once and then we reuse the instance.
We can achieve this by refactoring our class to have:
hidden (private)constructor
public getInstance method that returns instance of the class

3.If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?

* Middleware is software which is in the middle of an operating system and the applications working on it. It permits communication and data management for distributed applications by operating as a hidden translation layer. The term is considered vague since it is used to link two separate applications together.

--------------------------------

## Document the following Vocabulary Terms 🖥️
|||
|-|-----|
|Router Middleware|The term is composed of 2 words router and middleware. Middleware. It is a piece of code that comes in the middle of request and response . It kind of hijacks your request so that you can do anything that you want with your request or response eg: Modify the data or call the next middleware|
|Dynamic Module Loading|mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory|
|Singleton Pattern|a software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system. The term comes from the mathematical concept of a singleton|
|CRUD -> REST Method Matches|a cycle meant for maintaining permanent records in a database setting. CRUD principles are mapped to REST commands to comply with the goals of RESTful architecture|
|Mock Testing|is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules. In mock testing, the dependencies are replaced with objects that simulate the behaviour of the real ones. |

-----------------------------

## Preview 📖

Which 3 things had you heard about previously and now have better clarity on?
* CRUD methods  
* Sql & nosql
* REST
Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

* middleware
* Linked Lists
* Test Driven Development (TDD)
What are you most excited about trying to implement or see how it works?

* Singleton pattern



-----------------------------

## Preparation Materials 📚

#### Securing Passwords

* Passwords : It is the most vital secret of every activity we do over the internet and also a final check to get into any of your user account.
 * Hashing is the greatest way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.

   * The benefit of hashing is that if someone steals the database with hashed passwords, they only make off with the hashes and not the actual plaintext passwords.
   * PROBLEMS WITH CRYPTOGRAPHIC HASH ALGORITHM :  
       *  Hash Collision attack 
       * Brute Force attack

 **This method of hashing passwords is solid enough for most web applications that stores users' passwords and other sensitive data.**

  #### Basic Auth

  *  basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request

  * HTTP Basic authentication (BA) implementation is the simplest technique for enforcing access controls to web resources because it does not require cookies, session identifiers, or login pages; rather, HTTP Basic authentication uses standard fields in the HTTP header.


#### OWASP auth cheatsheet

"* Authentication is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.

* Session Management is a process by which a server maintains the state of an entity interacting with it. This is required for a server to remember how to react to subsequent requests throughout a transaction. Sessions are maintained on the server by a session identifier which can be passed back and forward between the client and server when transmitting and receiving requests. Sessions should be unique per user and computationally very difficult to predict. The Session Management Cheat Sheet contains further guidance on the best practices in this area.

* ***Password Managers¶***

* Password managers are programs, browser plugins or web services that automate management of large number of different credentials. Most password managers have functionality to allow users to easily use them on websites, either by pasting the passwords into the login form, or by simulating the user typing them in.

* Web applications should at least not make password managers job more difficult than necessary by observing the following recommendations:

* Use standard HTML forms for username and password input with appropriate type attributes.
* Avoid plugin-based login pages (such as Flash or Silverlight).
* Implement a reasonable maximum password length, such as 64 characters, as discussed in the Password Storage Cheat Sheet.
* Allow any printable characters to be used in passwords.
* Allow users to paste into the username and password fields.
* Allow users to navigate between the username and password field with a single press of the Tab key.


" **[READ MORE-cheatsheetseries](https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html)**

#### bcrypt docs

* node.bcrypt.js : A library to help you hash passwords

* Dependencies
  * NodeJS
  * node-gyp

* Credits

  * blowfish.cc - OpenBSD
  * bcrypt.cc - OpenBSD
  * bcrypt::gen_salt - gen_salt inclusion to bcrypt
   * bcrypt_node.cc - me      ***[...MORE INFORMATION ](https://www.npmjs.com/package/bcrypt)***


 #### &copy; Dima Alabsi; 2021
