## Review, Research, and Discussion

- What is the benefit of transforming data into packets?
  - enable new innovations, services, and business opportunities, they are also the most cost-effective, efficient, and scalable networks for content delivery
- UDP is often refereed to as a connectionless protocol. Why is this?
  - No connection needs to be established between the source and destination before you transmit data
- Can a socket server application have multiple socket connections?
  - yes it can
- Can a socket connection application be connected to multiple socket servers?
  - yes it can
- Can an application be both a socket server and a socket connection?
  - yes it can

## Document the following Vocabulary Terms

| Term                     |                                                                                                                                                 |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| Observer Pattern         | which an object, named the subject, maintains a list of its dependents, called observers                                                        |
| Listener                 | A listener is a function that is invoked when a particular event occurs, typically with an event object containing information about the event. |
| Event Handler            | a piece of code that will execute to respond to that event.                                                                                     |
| Event Driven Programming | which the flow of the program is determined by events                                                                                           |
| Event Loop               | what allows Node. js to perform non-blocking I/O operations — despite the fact that JavaScript is single-threaded                               |
| Event Queue              | a repository where events from an application are held prior to being processed by a receiving program or system.                               |
| Call Stack               | A call stack is a series of program counter addresses representing instructions from within the program.                                        |
| Emit/Raise/Trigger       | start a new event                                                                                                                               |
| Subscribe                | a messaging pattern where senders of messages, called publishers,                                                                               |
| database                 | database is an organized collection of structured information, or data, typically stored electronically in a computer system.                   |

[socket.io_overview](https://www.tutorialspoint.com/socket.io/socket.io_overview.htm)

## Socket.IO

- is a JavaScript library for real-time web applications. It enables real-time, bi-directional communication between web clients and servers. It has two parts − a client-side library that runs in the browser, and a server-side library for node.js. Both components have an identical API.

- Socket.IO is quite popular, it is used by Microsoft Office, Yammer, Zendesk, Trello,. and numerous other organizations to build robust real-time systems.

- Key features of Socket.IO
  - It helps in broadcasting to multiple sockets at a time and handles the connection transparently.
  - It works on all platform, server or device, ensuring equality, reliability, and speed.
  - It automatically upgrades the requirement to WebSocket if needed.
  - It is a custom real-time transport protocol implementation on top of other protocols.
  - It requires both libraries to be used Client side as well as a server-side library.
  - IO works on work-based events. there are some reserved events that can be accessed using the Socket on the server side like Connect, message, Disconnect, Ping and Reconnect.
  - There are some Client based reserved events like Connect, connect- error, connect-timeout and Reconnect etc.

## WebSocket

- Key features of WebSocket

  - WebSocket helps in real-time communication between the Client and the webserver.
  - This protocol helps in transforming to cross-platform in a real-time world between the server and the client.
  - This also enables the business worldwide for a real-time web application to enhance and increase the feasibility.
  - The major advantage it stands over an HTTP connection that it provides full-duplex communication.

- Why do we need WebSocket?

  - It provides full-duplex communication, which helps in persisting the connection established between the Client and the Web Server.
  - It also lives up to the standards and provides the accuracy and efficiency stream events to and from with negligible latency.
  - WebSocket removes the overhead and reduce complexity.
  - It makes real-time communication effortless and efficient.
