# CRUD


### HTTP Status Codes

* 100 - 199 : These are informational status codes

* 200 - 299Permalink : These are the success codes. 

* 300 - 399Permalink : These are redirection codes

* 400 - 499Permalink : These are the client error codes

* 500 - 599Permalink : These are the server error codes

![ HTTP Status Codes](https://softcrony.com/blog/wp-content/uploads/2020/07/http-code.png)

----------- 

### Status Codes

* 200 OK - It’s the basic status code to tell the client everything went good

* 201 Created - The most fitting for Create operations.

* 202 Accepted - Often used for asynchronous processing.

* 303 See Other - Like the 202 code but using a Location header field in response to informing the client about the location ..

* 403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.


    * It’s better to reduce traffic and simply tell the client the deletion is complete and return no response body (as the resource has been deleted).
     * If the deletion is asynchronous and takes some time, which is the case in distributed systems, it can be appropriate to return this code with some information or URL to tell the client when it will be deleted.



#### middleware :

**Middleware is software that enables one or more kinds of communication or connectivity between two or more applications or application components in a distributed network. By making it easier to connect applications that weren't designed to connect with one another - and providing functionality to connect them in intelligent ways - middleware streamlines application development and speeds time to market.**

![middleware](https://www.researchgate.net/profile/Livio-Pompianu/publication/303222728/figure/fig1/AS:423293980286978@1477932558682/A-diagram-of-the-middleware-architecture_Q640.jpg)



***express. json() is a method inbuilt in express to recognize the incoming Request Object as a JSON Object. This method is called as a middleware in your application using the code: app. use(express.***


* ***Route parameters are named URL segments that are used to capture the values specified at their position in the URL. The captured values are populated in the req.params object, with the name of the route parameter specified in the path as their respective keys.***

 |PUT|PATCH|
|--------|--------|
|PUT is a method of modifying resource where the client sends data that updates the entire resource .|PATCH is a method of modifying resources where the client sends partial data that is to be updated without modifying the entire data.|
|In a PUT request, the enclosed entity is considered to be a modified version of the resource stored on the origin server, and the client is requesting that the stored version be replaced|With PATCH, however, the enclosed entity contains a set of instructions describing how a resource currently residing on the origin server should be modified to produce a new version.|
|It has High Bandwidth |Since Only data that need to be modified if send in the request body as a payload , It has Low Bandwidth |

* Declaring Defaults in Your Schema

   * Your schemas can define default values for certain paths. If you create a new document without that path set, the default will kick in.


**The HyperText Transfer Protocol (HTTP) 500 Internal Server Error server error response code indicates that the server encountered an unexpected condition that prevented it from fulfilling the request.**

***201-Created***
A 201 status code indicates that a request was successful and as a result, a resource has been created (for example a new page).***

***200 - OK***
The 200 status code is by far the most common returned. It means, simply, that the request was received and understood and is being processed.***


####  &copy; Dima Alabsi; 2021 
