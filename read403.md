#  Express REST API

### Review, Research, and Discussion

 * Is the route handler a middleware?

**They are not middleware functions by definition. If such function is used on routing methods then they are only handler functions. We use such a handler function which is not a middleware when it is the only one callback function**

----------------------

* In what ways can a middleware function end the process and send data to the browser ?

***You can send a response and not call next() at all. That finishes the request and stops further routing. 2) You can do just plain next() which advances to the next route in the chain. 3) You can call next('route') to bypass all the rest of the routes in this router and continue routing in other routers***

--------------------------

* At what point in the request lifecycle can you “inject” middleware? 

***the request object can be injected into middleware by passing the Request parameter into the constructor like so:
from masonite.request import Requestclass SomeMiddleware:    def __init__(self, request: Request):***        ***self.request = request***    ...

* this will inject the Request class into the constructor when that middleware is executed

--------------------


* Name 3 real world use cases where you’d want to change the request with custom middleware

    * login and logout

     * Data Integration.

    * Message Oriented Middleware.

    --------------------------



    * What can cause express to error with “Request headers sent twice, cannot start a second response” ?

      ***means that you're already in the Body or Finished state, but some function tried to set a header or statusCode. When you see this error, try to look for anything that tries to send a header after some of the body has already been written. For example, look for callbacks that are accidentally called twice, or any error that happens after the body is sent.***

       -----------------------------------

      ### Document the following Vocabulary Terms

|Term||
|-------|---------|
|Middleware|software that enables one or more kinds of communication or connectivity between two or more applications or application components in a distributed network.|
Request Object|the main entry point for an application to issue a request to the Library - all operations on a URL must use a Request object.|
|Response Object| instance of a javax.servlet.http.HttpServletResponse object. Just as the server creates the request object, it also creates an object to represent the response to the client.|
|Application Middleware| database middleware, application server middleware, message-oriented middleware, web middleware and transaction-processing monitors.|
|Routing Middleware|the way in which the client requests are handled by the application endpoints|
|Test Driven Development|software development practice that focuses on creating unit test cases before developing the actual code|
|Behavioral Testing|testing of the external behaviour of the program, also known as black box testing|



"* Middleware functions are functions that have access to the request object (req), the response object (res), and the next function in the application’s request-response cycle. The next function is a function in the Express router which, when invoked, executes the middleware succeeding the current middleware.

Middleware functions can perform the following tasks:

* Execute any code.
* Make changes to the request and the response objects.
* End the request-response cycle.
* Call the next middleware in the stack." [READ MORE](https://expressjs.com/en/guide/writing-middleware.html)


----------------------------


### Middleware

As generic terms, middleware is code that examines an incoming request and prepares it for further processing by other handlers or short circuits the processing (like when it discovered the user is not authenticated yet). Some examples:

* Session Management. Parse cookies, look for session cookie, lookup session state for that cookie and add session info to the request so that other handlers down the line have ready access to the session object without any additional work on their part. In express, this would be express.session().

* Authentication. Check if the user is trying to access a portion of the site that requires authentication. If so, check if their authentication credentials are good. If not, send an error response and prevent further processing. If so, allow further processing.

* Parsing of Cookies. Parse incoming cookies into an easy-to-use data structure a request handler can have easy access to cookie data without each having to parse them on their own. This type of middleware is built into Express and happens automatically.

* Parsing and Reading of POST/PUT bodies. If the incoming request is a POST or PUT, the body of the request may contain data that is needed for processing the request and needs to be read from the incoming stream. Middleware can centralize this task reading the body, then parsing it according to the data type and putting the result into a known request parameter (in Express this would be req.body). Express has some ready-to-use middleware for this type of body parsing with express.json() or express.urlencoded(). A middleware library like multer is for handling file uploads.

* Serve static files (HTML, CSS, JS, etc...). For some groups of URLs, all the server needs to do is to serve a static file (no custom content added to the file). This is common for CSS files, JS files and even some HTML files. Express provides middleware for this which is called express.static().



--------------------------

## Preview

Which 3 things had you heard about previously and now have better clarity on?

  WRRC
  diffrerence between framework and library
  app.use method

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?


CI / IDD

What are you most excited about trying to implement or see how it works?

   Start work with REACT deeply..

   ---------------------------------------

   ## Preparation Materials

* Classes

***Classes are a template for creating objects. They encapsulate data with code to work on that data. Classes in JS are built on prototypes but also have some syntax and semantics that are not shared with ES5 class-like semantics.***

*  To declare a class, you use the class keyword with the name of the class.
.
* Hoisting
    * An important difference between function declarations and class declarations is that function declarations are hoisted and class declarations are not. You first need to declare your class and then access it, 

* Routing refers to how an application’s endpoints (URIs) respond to client requests
 to handle GET requests and app.post to handle POST requests. For a full list, see app.METHOD. You can also use app.all() to handle all HTTP methods and app.use() to specify middleware as the callback function route method is derived from one of the HTTP methods, and is attached to an instance of the express class.

* There is a special routing method, app.all(), used to load middleware functions at a path for all HTTP request methods. For example, the following handler is executed for requests to the route “/secret” whether using GET, POST, PUT, DELETE, or any other HTTP request method supported in the http module.

* Response methods

   * The methods on the response object (res) in the following table can send a response to the client, and terminate the request-response cycle. If none of these methods are called from a route handler, the client request will be left hanging.


   * app.route()

     * You can create chainable route handlers for a route path by using app.route(). Because the path is specified at a single location, creating modular routes is helpful, as is reducing redundancy and typos

  * express.Router

    * Use the express.Router class to create modular, mountable route handlers. A Router instance is a complete middleware and routing system; for this reason, it is often referred to as a “mini-app”.


 * Use express.Router() multiple times to define groups of routesApply the express.Router() to a section of our site using app.use()Use route middleware to process requestsUse route middleware to validate parameters using .param()Use app.route() as a shortcut to the Router to define multiple requests on a route

* **Route Handler**

  * As a generic term, a route handler is code that is looking for a request to a specific incoming URL such as /login and often a specific HTTP verb such as POST and has specific code for handling that precise URL and verb. Some examples:

  * Serve a specific web page. Handle a browser request for a specific web page.

  * Handle a specific form post. For example, when the user logs into the site, a login for is submitted to the server. This would be handled by a request handler in Express such as app.post("/login", ...).

  * Respond to a specific API request. Suppose you had an API for a book selling web-site. You might provide in that API the ability to get info on a book by its ISBN number. So, you design an api that supports a query for a particular book such as /api/book/list/0143105426 where 0143105426 is the ISBN number for the book (a universal book identifier). In that case, you'd create a request handler in Express for a URL that looks like that: app.get('/api/book/list/:isbn', ...). The request handler in Express could then programmatically examine req.parms.isbn to get the request isbn number, look it up in the database and return the desired info on the book.

So, those are somewhat generic descriptions of middleware vs. request handlers in any web server system in any language. " **quoted from [stackoverflow](https://stackoverflow.com/questions/58925276/what-is-the-difference-between-a-route-handler-and-middleware-function-in-expres)**

"
"Express 4.0 comes with the new Router. Router is like a mini express application. It doesn't bring in views or settings, but provides us with the routing APIs like .use, .get, .param, and route."  [READ MORE](https://scotch.io/tutorials/learn-to-use-the-new-router-in-expressjs-4)

 #### &copy; Dima Alabsi; 2021
