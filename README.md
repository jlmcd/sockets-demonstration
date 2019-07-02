# <div style="display: inline">Socket.io</div> Example

This repository contains examples for basic socket functionality using socket.io.

## Notes

* The Global Room will send a socket message to every connected socket.

* When you join a room, messages will be sent to everyone who has joined that room's socket.

    * To send a message to only a room, append `.to(roomname)` on socket or io, depending on the message type.

* **Emit (socket.emit) -** will send a message to only the user.

* **Broadcast (socket.broadcast.emit) -** will send a message to everyone *except* the user.

* **Blast (io.sockets.emit) -** will send a message to every user connected to the socket.
