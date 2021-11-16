


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

* Socket.io is a robust server client->server event handler, and is really great at that. However to handle some events within the app itself
What happens if a client “misses” an event?

*  something your application needs to handle by storing the state that is necessary to restore a returning client. Presumably your clients have a way to identify with your application, either with a token or some other identification. When the server starts one of these file copies, it can assign an id to the operation, and store that id in a database, associated with the client that requested it. If the client goes away and then returns, you can find if there are any ongoing file copies for it, and that way sync the client back to the way it was before it closed the browser.

* How can we mitigate this?

  by  attaching methods to each listener...

---------------------------

## Document the following Vocabulary Terms 📕

|Term||
|---|---|
|Socket|one endpoint of a two-way communication link between two programs running on the network. A socket is bound to a port number so that the TCP layer can identify the application that data is destined to be sent to. ... Every TCP connection can be uniquely identified by its two endpoints|
|Web Socket|WebSocket is a communications protocol for a persistent, bi-directional, full duplex TCP connection from a user's web browser to a server. ... The communication can be initiated at either end, which makes event-driven web programming possible. In contrast, standard HTTP allows only users to request new data|
|Socket.io| a library that enables real-time, bidirectional and event-based communication between the browser and the server. It consists of: a Node.js server: Source | API & Javascript client library for the browser (which can be also run from Node.js)
|Client| computer in a network that uses the services provided by a server|
|Server| a piece of computer hardware or software (computer program) that provides functionality for other programs or devices,|
|OSI Model| (Open Systems Interconnection Model) is a conceptual framework used to describe the functions of a networking system. The OSI model characterizes computing functions into a universal set of rules and requirements in order to support interoperability between different products and software|
|TCP Model|TCP/IP stands for Transmission Control Protocol/Internet Protocol. TCP/IP is a set of standardized rules that allow computers to communicate on a network such as the internet|
|TCP|Transmission Control Protocol (TCP) is a standard that defines how to establish and maintain a network conversation by which applications can exchange data.|
|UDP|User datagram protocol (UDP) operates on top of the Internet Protocol (IP) to transmit datagrams over a network. UDP does not require the source and destination to establish a three-way handshake before transmission takes place. Additionally, there is no need for an end-to-end connection|
|Packets|the unit of data routed between an origin and a destination on the internet or other packet-switched network -- or networks that ship data around in small packets|


-------------------------------

## Preview

1.Which 3 things had you heard about previously and now have better clarity on?

ROUTES,
ENDPOINT ,
FRAMEWORKS

2.Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

SOCKET,
TCP,
UDP
3.What are you most excited about trying to implement or see how it works?

SOCKET.IO

----------------------------------

## Preparation Materials


**Socket.io Chat Example**

* Express initializes app to be a function handler that you can supply to an HTTP server (as seen in line 4).
We define a route handler / that gets called when we hit our website home.
We make the http server listen on port 3000. :
"const express = require('express');

const app = express();

const http = require('http');

const server = http.createServer(app);

app.get('/', (req, res) => {

  res.send('< h1 >Hello world< /h1>');
});

server.listen(3000, () => {

  console.log('listening on *:3000');
});  "


***Rooms and Namespaces***

**Both namespaces and rooms are created on the server side
Multiple namespaces and multiple rooms share the same (WebSocket) connection**

* The server will transmit messages over the wire only to those clients that connected to / joined a nsp / room, i.e. it's not just client-side filtering

#### The differences:

* namespaces are connected to by the client using io.connect(urlAndNsp) (the client will be added to that namespace only if it already exists on the server)

* rooms can be joined only on the server side (although creating an API on the server side to enable clients to join is straightforward)

* namespaces can be authorization protected
authorization is not available with rooms, but custom authorization could be added to the aforementioned, easy-to-create API on the server, in case one is bent on using rooms

* rooms are part of a namespace (defaulting to the 'global' namespace)

* namespaces are always rooted in the global scope**







 #### &copy; Dima Alabsi; 2021
