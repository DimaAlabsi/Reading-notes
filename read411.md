# Event Driven Applications

## Review, Research, and Discussion

1. Why is access control important ?

* Access controls limit access to information and information processing systems. When implemented effectively, they mitigate the risk of information being accessed without the appropriate authorisation, unlawfully and the risk of a data breach.

2. Describe an application that would need access control.

* Access control (or authorization) is the application of constraints on who (or what) can perform attempted actions or access resources that they have requested. ... Access control determines whether the user is allowed to carry out the action that they are attempting to perform.

3. What is a role used for ?

* A role is a collection of privileges that can be granted to one or more users or other roles. Roles help you grant and manage sets of privileges for various categories of users, rather than grant those privileges to each user individually. For example, several users might require administrative privileges.

4. Why is role based access control more scalable than discretionary or mandatory access control ?

* For most business applications, RBAC is superior to ACL in terms of security and administrative overhead. ACL is better suited for implementing security at the individual user level and for low-level data, while RBAC better serves a company-wide security system with an overseeing administrator.

-------------------------

## Document the following Vocabulary Terms

 
|Term||
|---|---|
|Authorization| the process of giving someone permission to do or have something. ... Thus, authorization is sometimes seen as both the preliminary setting up of permissions by a system administrator and the actual checking of the permission values that have been set up when a user is getting access|
|Role Based Access Control|Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network|
|Capabilities|Capability The mayor has demonstrated his capability to handle municipal problems. 2 : a feature or faculty capable of development : potentiality This vacant urban district has great capabilities|


--------------------------

## Preview

* Which 3 things had you heard about previously and now have better clarity on?
Authentiacted
Payload
Deployment
bearer

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
QUEUE & STACK
JWT
Testing


What are you most excited about trying to implement or see how it works?

React


-----------------

## Preparation Materials

### Event Driven Programming

***Event-Driven Programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision*** .

* Event-Driven Programming makes use of the following concepts:

|||
|-----|----|
|An Event Handler is a callback function that will be called when an event is triggered.||
|A Main Loop listens for event triggers and calls the associated event handler for that event.|


* The Object Oriented approach promotes the idea that all behavior of an individual unit (or object) be handled from code within that unit. Using this approach, applications are built with many different units that all speak to and interact with each other.

" Much of the Node.js core API is built around an idiomatic asynchronous event-driven architecture in which certain kinds of objects (called "emitters") emit named events that cause Function objects ("listeners") to be called.

For instance: a net.Server object emits an event each time a peer connects to it; a fs.ReadStream emits an event when the file is opened; a stream emits an event whenever data is available to be read.

All objects that emit events are instances of the EventEmitter class. These objects expose an eventEmitter.on() function that allows one or more functions to be attached to named events emitted by the object. Typically, event names are camel-cased strings but any valid JavaScript property key can be used.

When the EventEmitter object emits an event, all of the functions attached to that specific event are called synchronously. Any values returned by the called listeners are ignored and discarded."

[TO KNOW MORE ABOUT Node docs: events](https://nodejs.org/api/events.html)

#### Node docs: events










 #### &copy; Dima Alabsi; 2021
