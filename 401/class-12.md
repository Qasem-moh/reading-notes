# TCP
* stands for transmission control protocol.
* TCP is a reliable and connection-oriented transport protocol
  With TCP, data can be delivered successfully and accurately. 
* Many applications, such as web,  email, and FTP, use TCP. Before TCP transmits data, it will use **three-way handshake** to establish a connection:

1. Host X begins the connection by sending the TCP SYN packet to its host destination. The packets contain a random sequence number (For example, 4321) that indicates the beginning of the sequence numbers for data that the Host X should transmit.

2. After that, the Server will receive the packet, and it responds with its sequence number. It's response also includes the acknowledgment number, that is Host X's sequence number incremented with 1 (Here, it is 4322).

3. Host X responds to the Server by sending the acknowledgment number that is mostly server's sequence number that is incremented by 1.

* After the data transmission process is over, TCP automatically terminates the connection between two separate endpoints.


# OSI Model
* open system intecration model 

![check](https://media.geeksforgeeks.org/wp-content/uploads/computer-network-osi-model-layers.png)

## The 7 Layers of the OSI Model
1. **physical Layer**
The lowest layer of the OSI Model is concerned with electrically or optically transmitting raw unstructured data bits across the network from the physical layer of the sending device to the physical layer of the receiving device. It can include specifications such as voltages, pin layout, cabling, and radio frequencies. At the physical layer, one might find “physical” resources such as network hubs, cabling, repeaters, network adapters or modems.

2. **Data Link Layer**
At the data link layer, directly connected nodes are used to perform node-to-node data transfer where data is packaged into frames. **The data link layer also corrects errors that may have occurred at the physical layer.**
The data link layer encompasses two sub-layers of its own. The first, media access control (MAC), provides flow control and multiplexing for device transmissions over a network. The second, the logical link control (LLC), provides flow and error control over the physical medium as well as identifies line protocols.


3. **Network Layer**
The network layer is responsible for receiving frames from the data link layer, and delivering them to their intended destinations among based on the addresses contained inside the frame. **The network layer finds the destination by using logical addresses, such as IP (internet protocol).** At this layer, routers are a crucial component used to quite literally route information where it needs to go between networks.

4. **Transport Layer**
The transport layer manages the delivery and error checking of data packets. **It regulates the size, sequencing, and ultimately the transfer of data between systems and hosts**. **One of the most common examples of the transport layer is TCP or the Transmission Control Protocol**.

5. **Session Layer**
The session layer controls the conversations between different computers.**A session or connection between machines is set up, managed, and termined at layer 5**. Session layer services also include authentication and reconnections.

6. **Presentation Layer**
The presentation layer **formats or translates data for the application layer based on the syntax or semantics that the application accepts**. Because of this, it at times also called the syntax layer. This layer can also handle the encryption and decryption required by the application layer.

7. **Application Layer**
At this layer, **both the end user and the application layer interact directly with the software application. This layer sees network services provided to end-user applications such as a web browser** or Office 365. The **application layer identifies communication partners, resource availability, and synchronizes communication**.
**HTTP protocol and websoket protocole are located at layer 7**

# Soket
*  socket is an endpoint of a communication between two programs running on a network. it's used to create a connection between a client program and a server program.and  Sockets API is available in the Node. js 


## Difference Between WebSocket and Socket.io
### **WebSocket** is the communication Protocol that provides bidirectional communication between the Client and the Server over a TCP connection;
- WebSocket remains open all the time, so they allow real-time data transfer. When clients trigger the request to the server, it does not close the connection on receiving the response; it rather persists and waits for the Client or server to terminate the request.

### Socket.IO is a library that enables real-time and full-duplex communication between the Client and the Web servers. 
* It **uses the WebSocket protocol to provide the interface**. Generally, it is divided into two parts; both WebSocket vs Socket.io are event-driven libraries.

* **Client-Side:** it is the library that runs inside the browser
* **Server Side:** It is the library for Node.js






## Differences between WebSocket and socket.io
* **Socket.io** It provides the Connection over TCP, while Socket.io is a library to abstract the WebSocket connections.
* **WebSocket** doesn’t have fallback options, while **Socket.io** supports fallback.
* **WebSocket** is the technology, while **Socket.io** is a library for WebSockets


# Terms 
*  **database** is a collection of information that is organized so that it can be easily accessed, managed and updated
* The **.subscribe()** function is similar to the Promise.then(), .catch() and .finally() methods in jQuery, but instead of dealing with promises it deals with Observables
* **Emit/Raise/Trigger** TP EMIT or fire events
* a **call stack** is a stack data structure that stores information , it's follow LIFO approch 
* **event queue** is a repository where events from an application are held prior to being processed by a receiving program or system
* **Event Loop**  design pattern that waits for and dispatches events or messages in a program
* **Event-driven programming** is a programming paradigm in which the flow of program execution is determined by events 
* **Event handlers**, scripts that are automatically executed when an event occurs.
* **Listener** waits for an event to occur
* **Observer pattern** is used when there is one-to-many relationship between objects such as if one object is modified, its depenedent objects are to be notified automatically.

# Q
1. What is the benefit of transforming data into packets?

- Packets are intended to transfer data reliably and efficiently. Instead of transferring a large file as a single block of data, sending smaller packets helps ensure each section is transmitted successfully.
UDP is often refereed to as a connectionless protocol. Why is this?


2. Can a socket server application have multiple socket connections?

Yes.

3. Can a socket connection application be connected to multiple socket servers?

Yes

4. Can an application be both a socket server and a socket connection?

No.