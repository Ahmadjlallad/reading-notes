## Review, Research, and Discussion

- Why is access control important?
  - to prevent unauthorized access to data
- Describe an application that would need access control.
  - a web application that would need to protect sensitive data
- What is a role used for?
  - to define a set of permissions
- Why is role based access control more scalable than discretionary or mandatory access control?
  - because it is more flexible

## Document the following Vocabulary Terms

| Term                      | Definition                                                                                                |
| ------------------------- | --------------------------------------------------------------------------------------------------------- |
| Authorization             | Authorization is the process of giving someone permission to do or have something.                        |
| Role Based Access Control | Role-based access control (RBAC) restricts network access based on a person's role within an organization |
| Capabilities              | the quality or state of being capable                                                                     |

## Preview

Preparation Materials
[Event Driven Programming](https://www.digitalocean.com/community/tutorials/nodejs-event-driven-programming)

- Event-Driven Programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.
- example: a web application that has a user interface and a backend.
- usage

1. create a new instance of the EventEmitter class

```js
const EventEmitter = require("events").EventEmitter;
const myEventEmitter = new EventEmitter();
```

2. create a new instance of the EventEmitter class and add a listener to it on the "userJoined" event

```js
const EventEmitter = require("events").EventEmitter;
const chatRoomEvents = new EventEmitter();

function userJoined(username) {
  // Assuming we already have a function to alert all users.
  alertAllUsers("User " + username + " has joined the chat.");
}

// Run the userJoined function when a 'userJoined' event is triggered.
chatRoomEvents.on("userJoined", userJoined);
```

3. emit the "userJoined" event when a user joins the chat

```js
function login(username) {
  chatRoomEvents.emit("userJoined", username);
}
```

- remove the listener
  - the reason performance reasons (the event is no longer needed) or to avoid memory leaks (if an event listener references an object that is no longer needed, it won’t be able to be garbage-collected. This can lead to a build up of unnecessary objects).
- Object Oriented Programming + Event-Driven Programming
  use the EventEmitter class to create an object that can emit events and listen for events.
  to make use on events to run it like middleware if some object requires it.
  [Node docs: events](https://nodejs.org/api/events.html)
