# Express



* The difference between PUT and PATCH


|||
|-----|-----|
| PUT|                                        PATCH  |
|PUT is a method of modifying resource where the client sends data that updates the entire resource .|PATCH is a method of modifying resources where the client sends partial data that is to be updated without modifying the entire data.|
|In a PUT request, the enclosed entity is considered to be a modified version of the resource stored on the origin server, and the client is requesting that the stored version be replaced|With PATCH, however, the enclosed entity contains a set of instructions describing how a resource currently residing on the origin server should be modified to produce a new version.|
|HTTP PUT is said to be idempotent, So if you send retry a request multiple times, that should be equivalent to a single request modification| HTTP PATCH is basically said to be non-idempotent. So if you retry the request N times, you will end up having N resources with N different URIs created on the server.|
|It has High Bandwidth |Since Only data that need to be modified if send in the request body as a payload , It has Low Bandwidth |


### services or tools that allow you to “mock” an API for development like json-server 


* A mock server uses fake responses to imitate the response of a real server. By mocking the response of your under-development backend, for example, your frontend team can independently develop and test other components. 

* Mocking services in API design and testing tools 
   
     * Mockable.io 

     * Mocky.io 

     * Stoplight 

     *   Postman 


#### REST API vs. SOAP

* REST (Representational State Transfer) is an architectural style with loose guidelines, and either one can be used to develop data-retrieval APIs for a system.

 * SOAP (Simple Object Access Protocol) is a standardized protocol with pre-defined rules.

 ![REST API vs. SOAP](https://blogs.sap.com/wp-content/uploads/2015/03/6_674409.png)

 #### API status and error codes

![API status and error codes](https://s3.us-west-1.wasabisys.com/idbwmedia.com/images/api/nonref_statuscodes.svg)


[READ MORE about API status and error codes](https://idratherbewriting.com/learnapidoc/docapis_doc_status_codes.html)


|||
|-------|----|
|WRRC| web request response cycle|
|Routing|Routing defines the way in which the client requests are handled by the application endpoints.|
|Express|a minimal and flexible Node.js web application framework that provides a robust set of features to develop web and mobile applications|
|Web Server|a computer that runs websites. It's a computer program that distributes web pages as they are requisitioned. The basic objective of the web server is to store, process and deliver web pages to the users. This intercommunication is done using Hypertext Transfer Protocol (HTTP)|
|TDD|“Test-driven development” refers to a style of programming in which three activities are tightly interwoven: coding, testing (in the form of writing unit tests) and design (in the form of refactoring).|
|CI/CD|tools can help a team automate their development, deployment, and testing.|
|npm|npm is the world's largest software registry. Open source developers from every continent use npm to share and borrow packages, and many organizations use npm to manage private development as well.|


  #### &copy; Dima Alabsi; 2021 
