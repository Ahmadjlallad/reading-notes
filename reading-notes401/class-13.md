## Review, Research, and Discussion

- What does it mean that web sockets are bidirectional? Why is this useful?
  - bidirectional because it allows you to send and receive data from the same computer
- Does socket.io use HTTP? Why?

  - socket.io isn't a pure Websocket server/implementation, it depends on HTTP for its initial connection setup.

- What happens when a client emits an event?
  - the server receives the event
- What happens when a server emits an event?
  - the client receives the event
- What happens if a client “misses” an event?
  - the server receives the event
- How can we mitigate this?

  - we can use a “heartbeat” to keep the connection alive

## Document the following Vocabulary Terms

|    Term    |                                                                                                      def                                                                                                       |
| :--------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|   Socket   |                                                     socket is one endpoint of a two-way communication link between two programs running on the network. A                                                      |
| Web Socket |                                   WebSocket is a communications protocol for a persistent, bi-directional, full duplex TCP connection from a user's web browser to a server                                    |
| Socket.io  | IO is a JavaScript library for realtime web applications. It enables realtime, bi-directional communication between web clients and servers. It has two parts: a client-side library that runs in the browser, |
|   Client   |                                                         person or organization using the services of a lawyer or other professional person or company                                                          |
|   Server   |                                                    A server is a computer or system that provides resources, data, services, or programs to other computers                                                    |
| OSI Model  |                                                                 a conceptual framework used to describe the functions of a networking system.                                                                  |
| TCP Model  |                                                                   TCP/IP Reference Model is a four-layered suite of communication protocols.                                                                   |
|    TCP     |                          Transmission Control Protocol (TCP) is a standard that defines how to establish and maintain a network conversation by which applications can exchange data.                          |
|    UDP     |                User Decagram Protocol (UDP) is a communications protocol that is primarily used to establish low-latency and loss-tolerating connections between applications on the internet.                 |
|  Packets   |                A packet is the unit of data routed between an origin and a destination on the internet or other packet-switched network -- or networks that ship data around in small packets.                 |

## Preparation Materials

- connect a express with socket.io

```javascript
const express = require("express");
const app = express();
const http = require("http");
const server = http.createServer(app);
const { Server } = require("socket.io");
const io = new Server(server);

server.listen(3000, () => {
  console.log("listening on *:3000");
});
```

- connect a express server with socket.io server and client and render a html from express and
  make a socket.io client
