# AWS: API, Dynamo and Lambda

## Review, Research, and Discussion 👍

**What are serverless functions?**
serverless function is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.

**If you were to create a system that emulated Lambda functions, how would you do it?**

You create a Node.js Lambda function using the Lambda console. Lambda automatically creates default code for the function.

To create a Lambda function with the console

Open the Functions page of the Lambda console.

Choose Create function.

Under Basic information, do the following:

For Function name, enter my-function.

For Runtime, confirm that Node.js 14.x is selected. Note that Lambda provides runtimes for .NET (PowerShell, C#), Go, Java, Node.js, Python, and Ruby.

Choose Create function.

Lambda creates a Node.js function and an execution role that grants the function permission to upload logs. The Lambda function assumes the execution role when you invoke your function, and uses the execution role to create credentials for the AWS SDK and to read data from event sources.

**Describe how a CDN works**

 CDN is a network of servers that distributes content from an “origin” server throughout the world by caching content close to where each end user is accessing the internet via a web-enabled device. The content they request is first stored on the origin server and is then replicated and stored elsewhere as needed.

--------------------------------------------------------------------------


### Document the following Vocabulary Terms 📑
|||
|-----|-----|
|Serverless Functions|is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.|
|Cloud Storage|a cloud computing model that stores data on the Internet through a cloud computing provider who manages and operates data storage as a service. ... This gives you agility, global scale and durability, with “anytime, anywhere” data access|
|CDN| group of geographically distributed servers that speed up the delivery of web content by bringing it closer to where users are. Data centers across the globe use caching, a process that temporarily stores copies of files, so that you can access internet content from a web-enabled device or browser more quickly through a server near you. CDNs cache content like web pages, images, and video in proxy servers near to your physical location. This allows you to do things like watch a movie, download software, check your bank balance, post on social media, or make purchases, without having to wait for content to load.|
----------------------------------------------

## Preview 📙

1.Which 3 things had you heard about previously and now have better clarity on?

Socket,
events,
WRRC

2.Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

AWS,
Tree data structure,
UDP

3.What are you most excited about trying to implement or see how it works?

AWS & react.js


----------------------------------------------

## Preparation Materials 📚

**API Gateway work**

* Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale. APIs act as the "front door" for applications to access data, business logic, or functionality from your backend services. Using API Gateway, you can create RESTful APIs and WebSocket APIs that enable real-time two-way communication applications. API Gateway supports containerized and serverless workloads, as well as web applications.

* API Gateway sits between the backend services of your API and your API’s users, handling the HTTP requests to your API endpoints and routing them to the correct backends. It provides a set of tools that help you manage your API definitions and the mappings between endpoints and their respective backend services. It can also generate API references from your definitions and make them available to your users as API documentation.

![api gateawy](https://d1.awsstatic.com/serverless/New-API-GW-Diagram.c9fc9835d2a9aa00ef90d0ddc4c6402a2536de0d.png)


 ***DynamoDB is a hosted NoSQL database offered by Amazon Web Services (AWS)***. It offers:

reliable performance even as it scales;
a managed experience, so you won't be SSH-ing into servers to upgrade the crypto libraries;
a small, simple API allowing for simple key-value access as well as more advanced query patterns.


* DynamoDB is a particularly good fit for the following use cases:

   * Data sets with simple, known access patterns.
   * Serverless applications using AWS Lambda
   * Applications with large amounts of data and strict latency requirements. **[TO KNOW MORE ](https://aws.amazon.com/dynamodb/)**


**Dynamoose is a modeling tool for Amazon's DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familar.** [MORE ABOUT DYNAMOOSE](https://dynamoosejs.com/getting_started/Introduction/)


 #### &copy; Dima Alabsi; 2021