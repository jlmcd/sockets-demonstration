# `Socket.io` Example

This repository contains examples for basic socket functionality using socket.io.

## How to use this repo

1. Fork and clone it!
2. Run `npm install`
3. `npm start`
4. Experiment. Send messages in the global room, and try to follow the flow of data from frontend to backend, and then back to frontend.
5. Once you understand the flow of data in the global socket, try adding "rooms" and again follow the flow of data through each message type.

## Notes

* The Global Room will send a socket message to every connected socket.

* When you join a room, messages will be sent to everyone who has joined that room's socket.

    * To send a message to only a room, append `.to(<roomname>)` on socket or io, depending on the message type.

* **Emit (socket.emit) -** will send a message to only the user.

* **Broadcast (socket.broadcast.emit) -** will send a message to everyone *except* the user.

* **Blast (io.sockets.emit) -** will send a message to every user connected to the socket.
