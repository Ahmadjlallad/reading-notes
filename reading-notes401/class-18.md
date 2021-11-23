# Readings: AWS: API, DynamoDB

## Review, Research, and Discussion

- What are serverless functions?
  - What is the use of serverless function?
    A serverless function is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies. These companies take care of code maintenance and execution so that developers can deploy new code faster and easier.
- If you were to create a system that emulated Lambda functions, how would you do it?
- Open the Functions page on the Lambda console.
  Choose Create function.
- Under Basic information, do the following: For Function name, enter my-function . For Runtime, confirm that Node. js 14. x is selected. Note that Lambda provides runtimes for Python, Ruby, and Node. js.

- Describe how a CDN works
  - A CDN is a network of servers that distributes content from an “origin” server throughout the world by caching content close to where each end user is accessing the internet via a web-enabled device.

# Document the following Vocabulary Terms

| Term                 | asd                                                                                                                                                                   |
| -------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Serverless Functions | A serverless function is a programmatic function written by a software developer for a single purpose.                                                                |
| Cloud Storage        | Object storage for companies of all sizes. Secure, durable, and with low latency. Store any amount of data. Retrieve it as often as you'd like.                       |
|                      |
| CDN                  | A content delivery network (CDN) is a group of geographically distributed servers that speed up the delivery of web content by bringing it closer to where users are. |

## Preparation Materials

- [AWS API Gateway Overview](https://www.serverless.com/guides/amazon-api-gateway)

  - In this guide, we’ll walk you through all the details of API Gateway. We’ll show you how it can be used with the Serverless Framework and give you a list of resources should you want to learn even more.
  - Within the Serverless ecosystem, API Gateway is the piece that ties together Serverless functions and API definitions. Being able to trigger the execution of a Serverless function directly in response to an HTTP request is the key reason why API Gateway is so valuable in Serverless setups: it enables a truly serverless architecture for web applications. When using API Gateway together with other AWS services, it’s possible to build a fully functional customer-facing web application without maintaining a single server yourself.

- [AWS API Gateway](https://aws.amazon.com/api-gateway/)
  - amazon docs
- [AWS DynamoDB Guide](https://www.dynamodbguide.com/what-is-dynamo-db/)
- [Dynamoose](https://dynamoosejs.com/getting_started/Introduction/)
  - Dynamoose is a modeling tool for Amazon's DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familar.
