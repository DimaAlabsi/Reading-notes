 #  Socket.io 

 ## Review, Research, and Discussion 💬

1.What is the benefit of transforming data into packets?

* Data packets are able to find the destination without the use of a dedicated channel. Reduces lost data packets because packet switching allows for resending of packets. More cost-effective since there is no need for a dedicated channel for voice or data traffic

2.UDP is often refereed to as a connectionless protocol. Why is this?

* UDP is a connectionless protocol. No connection needs to be established between the source and destination before you transmit data. UDP does not have a mechanism to make sure that the payload is not corrupted. As a result, the application must take care of data integrity all by itsel

3.Can a socket server application have multiple socket connections?

* Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to.

4.Can a socket connection application be connected to multiple socket servers ?
 
A connected socket is assigned to a new (dedicated) port, so it means that the number of concurrent connections is limited by the number of ports, unless multiple sockets can share the same port

5.Can an application be both a socket server and a socket connection ?

Yes, you definitely can.

one thing to notice that client host will be a localhost as both lie on the same machine and you are just creating two different socket with help of two different threads for sending and listening. (server being the listener, and client being the sender).

---------------------------

## Document the following Vocabulary Terms 📕

|Term||
|---|---|
|Observer Pattern|software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods|
|Listener|registered with the object that generates the event. When the event occurs, the object iterates through all listeners registered with it informing them of the event. Have a look at the AWT/Swing event model in Java for example|
|Event Handler|event handler has the name of the event, preceded by "on." For example, the event handler for the Focus event is onFocus. Many objects also have methods that emulate events. For example, button has a click method that emulates the button being clicked|
|Event Driven Programming|When you perform an action on a graphical component you generate an event. In event-driven programming the program responds to events. The program responds to events that the user generates in interacting with GUI components. The order of events is controlled by the user|
|Event Loop|a programming construct or design pattern that waits for and dispatches events or messages in a program. ... The event loop is also sometimes referred to as the message dispatcher, message loop, message pump, or run loop|
|Event Queue|Repository where events from an application are held prior to being processed by a receiving program or system. Event queues are often used in the context of an enterprise messaging system|
|Call Stack|a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc|
|Emit/Raise/Trigger|A trigger generally causes a program routine to be executed. (2) In a database management system (DBMS), a trigger is an SQL procedure that is executed when a record is added or deleted. It is used to maintain referential integrity in the database. A trigger may |
|Subscribe|to sign one's name to a document. 2a : to give consent or approval to something written by signing unwilling to subscribe to the agreement. b : to set one's name to a paper in token of promise to give something (such as a sum of money) also : to give something in accordance |
|database|n organized collection of structured information, or data, typically stored electronically in a computer system.|


## Preview

1.Which 3 things had you heard about previously and now have better clarity on?
Authentiacation
   Payload
 Signature  
 
2.Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
events at node.js
JWT
Testing
3.What are you most excited about trying to implement or see how it works?
continue what we have learned and see the result of those concepts in the front-end with REACT.

----------------------------------

## Preparation Materials


* "**WebSocket** : is a computer communications protocol, providing full-duplex communication channels over a single TCP connection. The WebSocket protocol was standardized by the IETF as RFC 6455 in 2011, and the WebSocket API in Web IDL is being standardized by the W3C.

    * **WebSocket is distinct from HTTP. Both protocols are located at layer 7 in the OSI model and depend on TCP at layer 4. Although they are different, RFC 6455 states that WebSocket "is designed to work over HTTP ports 443 and 80 as well as to support HTTP proxies and intermediaries," thus making it compatible with HTTP. To achieve compatibility, the WebSocket handshake uses the HTTP Upgrade header[1] to change from the HTTP protocol to the WebSocket protocol.**" [READ MORE ABOUT **WebSocket**](https://en.wikipedia.org/wiki/WebSocket)


* ***Socket.IO is a JavaScript library for real-time web applications. It enables real-time, bi-directional communication between web clients and servers. It has two parts − a client-side library that runs in the browser, and a server-side library for node.js. Both components have an identical API.***



* **Real-time Applications**
     * A  real-time application (RTA) is an application that functions within a period that the user senses as immediate or current.

     * Some examples of real-time applications are −

          * Instant messengers − Chat apps like Whatsapp, Facebook Messenger, etc. You need not refresh your app/website to receive new messages.

        * Push Notifications − When someone tags you in a picture on Facebook, you receive a notification instantly.

        * Collaboration Applications − Apps like google docs, which allow multiple people to update same documents simultaneously and apply changes to all people's instances.

       * Online Gaming − Games like Counter Strike, Call of Duty, etc., are also some examples of real-time applications.



        #### &copy; Dima Alabsi; 2021
