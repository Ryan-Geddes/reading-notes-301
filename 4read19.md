# Socket.io


## What is the benefit of transforming data into packets?
(https://techterms.com/definition/packet#:~:text=Packets%20are%20intended%20to%20transfer,packet%20needs%20to%20be%20resent)
"Packets are intended to transfer data reliably and efficiently. Instead of transferring a large file as a single block of data, sending smaller packets helps ensure each section is transmitted successfully. If a packet is not received or is "dropped," only the dropped packet needs to be resent. Additionally, if a data transfer encounters network congestion due to multiple simultaneous transfers, the remaining packets can be rerouted through a less congested path."
## UDP is often refereed to as a connectionless protocol. Why is this? 
(https://en.wikibooks.org/wiki/Communication_Networks/TCP_and_UDP_Protocols/UDP#:~:text=Unlike%20TCP%2C%20UDP%20doesn't,are%20often%20called%20%22Datagrams%22.&text=DNS%20servers%20send%20and%20receive%20DNS%20requests%20using%20UDP)
UDP does not extablish a connection before sending data, unlike TCP.

## Can a socket server application have multiple socket connections?

On the server side, yes, there can be multiple connections as long as they are associated with different client-side IP/Port pairs.

## Can a socket connection application be connected to multiple socket servers?

No, all client side connections are associated with one single listening port.


## Can an application be both a socket server and a socket connection?

Ben Hill Today at 1:33 PM
the question in the reading “can an application be both a socket server and a socket connection?” From what i can find on the googles, the answer is no, right? You want your client side connection listening on a single port, but server side you can have multiple connections and whatever.
the question says can, so the reason i’m bringing it here is because i’m sure there is a way to do it, so technically the answer is yes, but don’t do it. right?

John Cokos:code-fellows:  4 hours ago
You’re spot on. You can do it, but the idea is to have everything be separate mini apps.
:the_horns:
1


Ben Hill  4 hours ago
that’s what i thought! thanks John!

## What is the difference between a port and a socket?
[what is the difference between port and socket?](https://stackoverflow.com/questions/152457/what-is-the-difference-between-a-port-and-a-socket) 

A TCP socket is an endpoint instance defined by an IP address and a port in the context of either a particular TCP connection or the listening state.

A port is a virtualisation identifier defining a service endpoint (as distinct from a service instance endpoint aka session identifier).

A TCP socket is not a connection, it is the endpoint of a specific connection.

There can be concurrent connections to a service endpoint, because a connection is identified by both its local and remote endpoints, allowing traffic to be routed to a specific service instance.

There can only be one listener socket for a given address/port combination.


# Document the following Vocabulary Terms
## Term
- **OSI Model** - The Open Systems Interconnection model for understanding the 7 layers of abstraction that make up online communication.  The OSI provides a standard for different computer systems to be able to communicate with each other.
- **TCP Model** - From wiki: The Internet protocol suite provides end-to-end data communication specifying how data should be packetized, addressed, transmitted, routed, and received. This functionality is organized into four abstraction layers, which classify all related protocols according to the scope of networking involved. From lowest to highest, the layers are the link layer, containing communication methods for data that remains within a single network segment; the internet layer, providing internetworking between independent networks; the transport layer, handling host-to-host communication; and the application layer, providing process-to-process data exchange for applications.
- **TCP** - Stands for Transmission Control Protocol.  TCP establishs a connection between sender and receiver and permits lossless sending of data packets.
- **UDP** - Stands for User Datagram Protocol.  Allows lossy sending, like for livestreaming.  Does not establish a connection before sending packets, just sends regardless if packets are dropped.
- **Packets** - A packet is a small amount of data sent over a network, such as a LAN or the Internet. Similar to a real-life package, each packet includes a source and destination as well as the content (or data) being transferred. When the packets reach their destination, they are reassembled into a single file or other contiguous block of data.
- **Socket** - A TCP socket is an endpoint instance defined by an IP address and a port in the context of either a particular TCP connection or the listening state.

Ben Hill's notes on this subject are phenomenal:

https://benhill-401-advanced-javascript.github.io/reading-notes/401-js/class-19.html

How to insert cursor at beginning of every line:

Press CTRL + A to select all of the text.
Press SHIFT + ALT + I to insert multiple cursors at the end of each line.
Press Home twice to jump to the start of every line.

