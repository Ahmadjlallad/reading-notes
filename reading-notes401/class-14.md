## Review, Research, and Discussion

- What’s the difference between a FIFO and a standard queue?
  - FIFO: First in, first out
    - Standard queue: First in, first out, but not necessarily in the order you put it in
- How can the server be assured a message was properly received?
  - using message queue
- What classic design pattern is best represented by event driven programming?
  - Observer pattern
- How do you test an event driven system?

  - using a mock framework

| Term       | Definition                                                                                                                                                                                                                                                                                                        |
| ---------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| FIFO Queue | A FIFO queue is a queue that operates on a first-in, first-out (FIFO) principle. This means that the request (like a customer in a store or a print job sent to a printer) is processed in the order in which it arrives.                                                                                         |
| Pub/Sub    | Publish/subscribe messaging Publish/subscribe messaging, or pub/sub messaging, is a form of asynchronous service-to-service communication used in serverless and microservice architectures. In a pub/sub model, any message published to a topic is immediately received by all of the subscribers to the topics |

## [aws sns and sqs](https://www.youtube.com/watch?v=mXk0MNjlO7A)

Amazon Simple Queue Service (SQS) and Amazon SNS are both messaging services within AWS, which provide different benefits for developers. Amazon SNS allows applications to send time-critical messages to multiple subscribers through a “push” mechanism, eliminating the need to periodically check or “poll” for updates.
Amazon SQS is a message queue service used by distributed applications to exchange messages through a polling model, and can be used to decouple sending and receiving components. Amazon SQS provides flexibility for distributed components of applications to send and receive messages without requiring each component to be concurrently available.
