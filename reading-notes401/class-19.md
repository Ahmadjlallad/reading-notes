# Readings: AWS: Events

- Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server

  - Amazon API Gateway and Express Gateway both have their strengths and weaknesses. Amazon API Gateway has a compelling case for massively scalable API gateways at a competitive price point. With Express Gateway, you are responsible for hosting and running your own API Gateway, which may be more or less expensive depending on your experience and the load on your API Gateway. In particular, you may need to manage the number of Express Gateway servers you’re running and configure a load balancer in front of your gateway servers if your API has sufficient load, which may be cumbersome and expensive.

- List the AWS Database offerings and talk about the pros and cons of each

  - Relational Database. Relational databases store data with predefined schemas and relationships
  - Amazon Aurora
  - Amazon Relational Database Service (RDS)
  - Amazon Redshift.
  - Key-value Database.
  - Amazon DynamoDB.
  - In-memory Database.
  - Amazon MemoryDB for Redis.

- What’s the difference between a FIFO and a standard queue?
  - FIFO: First in, first out. - Standard queue: First in, first out.
- How can the server be assured a message was properly received?
  - The server can be assured a message was properly received by checking the message’s receipt handle.

|         Term          |                                                                                                                                                                                                                                                                        |
| :-------------------: | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|    Serverless API     |                                                                Serverless is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers.                                                                |
|       Triggers        |                                       A trigger generally causes a program routine to be executed. (2) In a database management system (DBMS), a trigger is an SQL procedure that is executed when a record is added or deleted.                                       |
|    Dynamo vs Mongo    | Both these databases support multi-document transactions, but with key differences: MongoDB supports read and writes to the same documents and fields in a single database transaction. DynamoDB lacks support for multiple operations within a single transaction.Jul |
| Dynamoose vs Mongoose |                                                    Dynamoose is obviously inspired by mongoose and is a good choice if you have a well-defined schema and/or want to be abstracted away from the DynamoDB details.                                                     |

[SQS and SNS Basics](https://www.youtube.com/watch?v=UesxWuZMZqI)
[AWS SQS vs SNS](https://medium.com/awesome-cloud/aws-difference-between-sqs-and-sns-61a397bf76c5)

Use Cases

- Choose SNS if:

  - You would like to be able to publish and consume batches of messages.
  - You would like to allow same message to be processed in multiple ways.
  - Multiple subscribers are needed.

- Choose SQS if:
  - You need a simple queue with no particular additional requirements.
  - Decoupling two applications and allowing parallel asynchronous processing.
  - Only one subscriber is needed.
