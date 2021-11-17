



# Event Driven Architecture

## Review, Research, and Discussion 💬

* What’s the difference between a FIFO and a standard queue?

  * Standard queues provide at-least-once delivery, which means that each message is delivered at least once. FIFO queues provide exactly-once processing, which means that each message is delivered once and remains available until a consumer processes it and deletes it

* How can the server be assured a message was properly received?

    * because of the process of the Message queue architecture

* What classic design pattern is best represented by event driven programming?
 
   * An event-driven architecture enables applications to act on these events as they occur. This is in contrast to traditional architectures, which largely dealt with data as batches of information to be inserted and updated at some defined interval, and responded to user-initiated requests rather than new information.

* How do you test an event driven system?

    * There are multiple levels of tests you will typically write for your system. In the most canonical case, you will write unit tests, service tests, and end-to-end tests. In each of these cases, your System Under Test (SUT, what is actually being tested) comprises a different part of your application
---------------------------

## Document the following Vocabulary Terms 📕

|Term||
|---|---|
|FIFO Queue|n FIFO queues, messages are ordered based on message group ID. If multiple hosts (or different threads on the same host) send messages with the same message group ID to a FIFO queue, Amazon SQS stores the messages in the order in which they arrive for processing|
|Pub/Sub|Publish/subscribe messaging, or pub/sub messaging, is a form of asynchronous service-to-service communication used in serverless and microservices architectures. In a pub/sub model, any message published to a topic is immediately received by all of the subscribers to the topic|






![FIFO Queue](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTyrXA6bQcffpHrUZJs3JwdepB9WfPLkUxozA&usqp=CAU)


![pop/sub](https://cloud.google.com/pubsub/images/pub_sub_flow.svg)

-------------------------------

## Preview 📓

1.Which 3 things had you heard about previously and now have better clarity on?

ROUTES,
ENDPOINT ,
SOCKET

2.Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

queue Message
TCP,
UDP
3.What are you most excited about trying to implement or see how it works?

SOCKET.IO with real chatting

----------------------------------

## Preparation Materials 📚

**AWS SNS and SQS**

* AWS SNS is a publisher subscriber network, where subscribers can subscribe to topics and will receive messages whenever a publisher publishes to that topic. AWS SQS is a queue service, which stores messages in a queue.



* When you subscribe an Amazon SQS queue to an Amazon SNS topic, you can publish a message to the topic and Amazon SNS sends an Amazon SQS message to the subscribed queue. The Amazon SQS message contains the subject and message that were published to the topic along with metadata about the message in a JSON document.

* Amazon SNS enables you to send messages or notifications directly to users with SMS text messages to over 200 countries, mobile push on Apple, Android, and other platforms or email (SMTP).


![AWS SNS and SQS](https://miro.medium.com/max/1004/1*mdUPKzrfJFuXa4d43KhKUQ.png)



 #### &copy; Dima Alabsi; 2021