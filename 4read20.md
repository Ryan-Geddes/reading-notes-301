# Readings: Message Queues

[Stackoverflow - what are websockets and why use them](https://stackoverflow.com/questions/44898882/why-to-use-websocket-and-what-is-the-advantage-of-using-it)

[how do websockets work?](https://sookocheff.com/post/networking/how-do-websockets-work/#:~:text=WebSocket%20uses%20HTTP%20as%20the,the%20use%20of%20long%2Dpolling.)
## What does it mean that web sockets are bidirectional? Why is this useful?

[Who needs websockets?](https://blog.logrocket.com/beyond-rest-using-websockets-for-two-way-communication-in-your-react-app-884eff6655f5/)

Sockets allow you to send data back and forth from server to client and vice cersa without requiring a TCP connection w/ a 3 way handshake to be established for every piece of data sent.

Data can be sent from server to client at any time, without the client even requesting it. This is often called server-push and is very valuable for applications where the client needs to know fairly quickly when something happens on the server (like a new chat messages has been received or a new price has been udpated). **A client cannot be pushed data over http. The client would have to regularly poll by making an http request every few seconds in order to get timely new data.** Client polling is not efficient.

Data can be sent either way very efficiently. Because the connection is already established and a webSocket data frame is very efficiently organized, one can send data a lot more efficiently that via an HTTP request that necessarily contains headers, cookies, etc...

The idea of WebSockets was borne out of the limitations of HTTP-based technology. With HTTP, a client requests a resource, and the server responds with the requested data. HTTP is a strictly unidirectional protocol — any data sent from the server to the client must be first requested by the client. Long-polling has traditionally acted as a workaround for this limitation. With long-polling, a client makes an HTTP request with a long timeout period, and the server uses that long timeout to push data to the client. Long-polling works, but comes with a drawback — resources on the server are tied up throughout the length of the long-poll, even when no data is available to send.

## Does socket.io use HTTP? Why?

Socket.io is a library that uses the WebSocket API.  

WebSockets allow for sending message-based data, similar to UDP, but with the reliability of TCP. WebSocket uses HTTP as the initial transport mechanism, but keeps the TCP connection alive after the HTTP response is received so that it can be used for sending messages between client and server. WebSockets allow us to build “real-time” applications without the use of long-polling.


## What happens when a client emits an event?
An object is sent out, for use, on the EventsEmitter global object. It can have several key value pairs, and be custom.

## What happens when a server emits an event?
The client needs to have a listener listening for that event so it can be triggered. socket.on('some event', function(do something here))

## What happens if a client “misses” an event?

If a client 'misses' an event, it is lost forever, ejected directly into the void.

## How can we mitigate this?
Always have a handler, or store events in an event queue to resend to the client at a future time.

## Vocabulary Terms

- **Web Socket** - The WebSocket API is an advanced technology that makes it possible to open a two-way interactive communication session between the user's browser and a server. With this API, you can send messages to a server and receive event-driven responses without having to poll the server for a reply.
- **Socket.io** -  Socket.io is a library that uses the WebSocket API.  
- **Client** - def: Servers provide data and information to clients, a client is a user of a server.
Resource: techterms.com
- **Server** - def: Severs serve up data, web applications and content so users, clients, can access them.
Resource: techterms.com
- **Full Duplex** - Full duplex means that data can be sent either way on the connection at any time.




Preparation Materials
Socket.io Chat Example
Rooms and Namespaces
Socket.io Emit Cheatsheet