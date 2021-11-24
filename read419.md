# AWS: Events

## Review, Research, and Discussion 👍

**Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server**

* An API Gateway is “middleware” that makes available backend services to mobile, web and other external clients via a set of protocols and commonly through a set of RESTful application programming interfaces (APIs). An API Gateway makes it much simpler to develop, secure, manage, and scale endpoints by moving most of the required logic from the client, into the gateway.


* Express Gateway is an API Gateway that can sit at the heart of any microservices architecture, regardless of what language or platform you’re using. Express Gateway secures your microservices and exposes them through APIs using Node.js, ExpressJS and Express middleware.

**List the AWS Database offerings and talk about the pros and cons of each**

AWS database services: Amazon RDS, Amazon Aurora, Amazon DynamoDB, Amazon DocumentDB, Amazon ElastiCache, Amazon Neptune, Amazon Timestream, and Amazon Quantum Ledger Database (QLDB)

What’s the difference between a FIFO and a standard queue?

**Standard queues provide at-least-once delivery, which means that each message is delivered at least once. FIFO queues provide exactly-once processing, which means that each message is delivered once and remains available until a consumer processes it and deletes it. Duplicates are not introduced into the queue.**


How can the server be assured a message was properly received?

By Client Response Receiver module is responsible for receiving responses.


--------------------------------------------------------------------------


### Document the following Vocabulary Terms 📑
|||
|-----|-----|
|Serverless API|a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers. A serverless application runs in stateless compute containers that are event-triggered, ephemeral (may last for one invocation), and fully managed by the cloud provider.|
|Triggers|a reminder of a past trauma. This reminder can cause a person to feel overwhelming sadness, anxiety, or panic. It may also cause someone to have flashbacks. A flashback is a vivid, often negative memory that may appear without warning|
|Dynamo vs Mongo|DynamoDB is a key-value store with added support for JSON to provide document-like data structures that better match with objects in application code. ... Compared to MongoDB, DynamoDB has limited support for different data types. For example, it supports only one numeric type and does not support dates.|
|Dynamoose vs Mongoose|is a modeling tool for Amazon's DynamoDB (inspired by Mongoose|

----------------------------------------------

## Preview 📙

1.Which 3 things had you heard about previously and now have better clarity on?

Socket,
events,
WRRC

2.Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

AWS,
k-ary tree,
UDP

3.What are you most excited about trying to implement or see how it works?

AWS & react.js


----------------------------------------------

## Preparation Materials 📚

* Amazon SQS is a reliable, highly-scalable hosted queue for storing messages as they travel between applications or microservices. Amazon SQS moves data between distributed application components and helps you decouple these components.

* Amazon Simple Notification Service (Amazon SNS) is a web service that enables you to build distributed web-enabled applications. Applications can use Amazon SNS to easily push real-time notification messages to interested subscribers over multiple delivery protocols.

***AWS — Difference between SQS and SNS***



* Use Cases
Choose SNS if:

You would like to be able to publish and consume batches of messages.


You would like to allow same message to be processed in multiple ways.
Multiple subscribers are needed.

Choose SQS if:

You need a simple queue with no particular additional requirements.

Decoupling two applications and allowing parallel asynchronous processing.
Only one subscriber is needed. ***[READ MORE](https://medium.com/awesome-cloud/aws-difference-between-sqs-and-sns-61a397bf76c5)***

![SQS VS SNS](https://miro.medium.com/max/875/1*DRrTtdyah9NHwR0VCm6MWA.png)

 #### &copy; Dima Alabsi; 2021