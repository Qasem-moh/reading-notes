## [Socket.io Emit Cheatsheet](https://socket.io/get-started/chat/)
# Room
* **Room**: A room is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of clients ,**server-only** concept (i.e. the client does not have access to the list of rooms it has joined
* You can call join to subscribe the socket to a given channel, And then simply use **to** or **in** (they are the same) when broadcasting or emitting
* You can emit to several rooms at the same time

## Room events
* create-room (argument: room)
* delete-room (argument: room)
* join-room (argument: room, id)
* leave-room (argument: room, id)

 **code sample**
 ``io.of("/").adapter.on("create-room", (room) => {``

 `` console.log(`room ${room} was created`);``
``});``

``io.of("/").adapter.on("join-room", (room, id) => {``

  ``console.log(`socket ${id} has joined room ${room}`);``
``});``

## Server-side
``io.on("connection", (socket) => {``

``// basic emit``
``socket.emit(/* ... */);``

``// to all clients in the current namespace except the sender``

``socket.broadcast.emit(/* ... */);``

``// to all clients in room1 except the sender``

``socket.to("room1").emit(/* ... */);``

``// to all clients in room1 and/or room2 except the sender``

``socket.to("room1").to("room2").emit(/* ... */);``

``// to all clients in room1``

``io.in("room1").emit(/* ... */);``

``// to all clients in namespace "myNamespace"``

``io.of("myNamespace").emit(/* ... */);``

``// to all clients in room1 in namespace "myNamespace"``

``io.of("myNamespace").to("room1").emit(/* ... */);``

``// to individual socketid (private message)``

``io.to(socketId).emit(/* ... */);``

``// to all clients on this node (when using multiple nodes)``

``io.local.emit(/* ... */);``

``// to all connected clients``

``io.emit(/* ... */);``

``// WARNING: `socket.to(socket.id).emit()` will NOT work, as it will send to everyone in the room``

``// named `socket.id` but the sender. Please use the classic `socket.emit()` instead.``

``// with acknowledgement``

``socket.emit("question", (answer) => {``

````// ...``
``});``

``// without compression``

``socket.compress(false).emit(/* ... */);``

``// a message that might be dropped if the low-level transport is not writable``

``socket.volatile.emit(/* ... */);``

``});``

## Client Side 
``// basic emit``

``socket.emit(/* ... */);``

``// with acknowledgement``

``socket.emit("question", (answer) => {``
``// ...``
``});``

``// without compression``

``socket.compress(false).emit(/* ... */);``

``// a message that might be dropped if the low-level transport is not writable``

``socket.volatile.emit(/* ... */);``


## Reserved events
On each side, the following events are reserved and should not be used as event names by your application:

* connect
* connect_error
* disconnect
* disconnecting
* newListener
* removeListener

## Disconnection
- You can fetch the rooms the Socket was in by listening to the disconnecting event:

``io.on('connection', socket => {``

``socket.on('disconnecting', () => {``

````console.log(socket.rooms); // the Set contains at least the socket ID``
``});``

``socket.on('disconnect', () => {``

````// socket.rooms.size === 0``
``});``
``});``

# Q 
1. What does it mean that web sockets are bidirectional? Why is this useful?
- WebSockets are bidirectional — they allow 'full-duplex communication'. This means that, once the initial handshake has taken place and the connection is established, the client and server can both communicate with each other freely. (And at the 

2. Does socket.io use HTTP? Why?
- the initial connection setup it done over HTTP. Also, a socket.io server will attach to an HTTP server so it can serve its own client code through /socket.io/socket.io.js 

3. What happens when a client emits an event?
- The event emitted from client side to server then it implement.
- In your frontend code you should have something that looks similar to

``<script src="/socket.io/socket.io.js"></script>``   

``<script>``

  ``var socket = io();``

``</script>``

4. What happens when a server emits an event?
- event emitted as many as server


5. What happens if a client “misses” an event?
- can't lestining to emmiting 

# Terms 
**Socket** :
* a channel to linked 2-end point with each other .
**Web Socket** :
* communications teqnoligy protocol between a client and a server.
**Socket.io** :
* JavaScript library for realtime web applications.
**Client** :
* a computer that connects to the network.
**Server** :
* who receive and process the requests from the client.
**OSI Model** :
* Open Systems Interconnection Model is a conceptual framework used to make a connection happen accurately.
**TCP Model** :
* It stands for Transmission Control Protocol/Internet Protocol. The TCP/IP model is a concise version of the OSI model.
**TCP** :
Transmission Control Protocol.
**UDP** :
User Datagram Protocol.