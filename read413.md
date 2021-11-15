


# Message Queues

## Review, Research, and Discussion 💬

What does it mean that web sockets are bidirectional? Why is this useful?

* BIDIRECTIONAL. Whereas HTTP relies on a client request to receive a response from the server for every exchange,
WebSockets allow for full-duplex bidirectional communication. This enables the server to send real-time updates
asynchronously, without requiring the client to submit a request each time. In the context of networked AV and control
systems, this allows devices to send and receive continuous streams of data to and from any point on the network.

Does socket.io use HTTP? Why?

* Websocket is created when you make upgrade from http to websocket, so it kind of does need http. socket.io isn't a pure Websocket server/implementation, it depends on HTTP for its initial connection setup..

What happens when a client emits an event?

* Socket.emit allows you to emit custom events on the server and client. socket.send sends messages which are received with the 'message' event..

What happens when a server emits an event?
What happens if a client “misses” an event?
How can we mitigate this?

---------------------------

## Document the following Vocabulary Terms 📕

|Term||
|---|---|
|Socket||
|Web Socket||
|Socket.io||
|Client||
|Server||
|OSI Model||
|TCP Model||
|TCP||
|UDP||
|Packets||



## Preview

1.Which 3 things had you heard about previously and now have better clarity on?
2.Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
3.What are you most excited about trying to implement or see how it works?

----------------------------------

## Preparation Materials


Socket.io Chat Example
Rooms and Namespaces
Socket.io Emit Cheatsheet







 #### &copy; Dima Alabsi; 2021
