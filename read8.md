 # APIs

***An API, or application programming interface, is a set of rules that define how applications or devices can connect to and communicate with each other. A REST API is an API that conforms to the design principles of the REST, or representational state transfer architectural style. For this reason, REST APIs are sometimes referred to RESTful APIs.***


**REST design principles** :

* Layered system architecture. 

* Cacheability

* Statelessness.

* Client-server decoupling.

* Uniform interface

![rest](https://martinfowler.com/articles/images/richardsonMaturityModel/overview.png)

**REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client.**

**A resource has an identifier, which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:HTTP**


**REST APIs built on HTTP, the uniform interface includes using standard HTTP verbs to perform operations on resources. The most common operations are GET, POST, PUT, PATCH, and DELETE.**

" ***A Uniform Resource Identifier (URI) is a unique sequence of characters that identifies a logical or physical resource used by web technologies. URIs may be used to identify anything, including real-world objects, such as people and places, concepts, or information resources such as web pages and books. Some URIs provide a means of locating and retrieving information resources on a network (either on the Internet or on another private network, such as a computer filesystem or an Intranet); these are Uniform Resource Locators (URLs). A URL provides the location of the resource. A URI identifies the resource by name at the specified location or URL. Other URIs provide only a unique name, without a means of locating or retrieving the resource or information about it, these are Uniform Resource Names (URNs). The web technologies that use URIs are not limited to web browsers. URIs are used to identify anything described using the Resource Description Framework (RDF), for example, concepts that are part of an ontology defined using the Web Ontology Language (OWL), and people who are described using the Friend of a Friend vocabulary would each have an individual URI.*** " [Read MORE!](https://en.wikipedia.org/wiki/Uniform_Resource_Identifier)



"
+ **Adopt a consistent naming convention in URIs. In general, it helps to use plural nouns for URIs that reference collections. It's a good practice to organize URIs for collections and items into a hierarchy. For example, /customers is the path to the customers collection, and /customers/5 is the path to the customer with ID equal to 5. This approach helps to keep the web API intuitive. Also, many web API frameworks can route requests based on parameterized URI paths, so you could define a route for the path /customers/{id}.** 

+ ***nother factor is that all web requests impose a load on the web server. The more requests, the bigger the load. Therefore, try to avoid "chatty" web APIs that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires. Instead, you might want to denormalize the data and combine related information into bigger resources that can be retrieved with a single request. However, you need to balance this approach against the overhead of fetching data that the client doesn't need. Retrieving large objects can increase the latency of a request and incur additional bandwidth costs. For more information about these performance antipatterns*** 


+ The HTTP protocol defines a number of methods that assign semantic meaning to a request. The common HTTP methods used by most RESTful web APIs are:

    + GET retrieves a representation of the resource at the specified URI. The body of the response message contains the details of the requested resource.



     +  POST creates a new resource at the specified URI. The body of the request message provides the details of the new resource. Note that POST can also be used to trigger operations that don't actually create resources.


     +  PUT either creates or replaces the resource at the specified URI. The body of the request message specifies the resource to be created or updated.




     + DELETE removes the resource at the specified URI." [Read More..](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)




---------------------


  + If a **PUT** method creates a new resource, it returns HTTP status code 201 (Created)..

  + If a **POST** method creates a new resource, it returns HTTP status code 201 (Created)..

  + A successful **GET** method typically returns HTTP status code 200 (OK)..

  + If the **delete** operation is successful, the web server should respond with HTTP status code 204 (No Content),











    #### &copy; Dima Alabsi; 2021 
