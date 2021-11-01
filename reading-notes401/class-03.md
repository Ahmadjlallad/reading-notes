# reading class 3 Express REST API

- Name 3 real world use cases where you’d want to change the request with custom middleware
  - bad request
  - authentication
  - filtering
- True or false: The route handler is middleware?
  - True
- In what ways can a middleware function end the process and send data to the browser?
  - send data to the browser with res.send()
- At what point in the request lifecycle can you “inject” middleware?
  - in the request handler
- What can cause express to error with “Request headers sent twice, cannot start a second response”
  - res.send() is called twice

---

## Document the following Vocabulary Terms

| Term                    | a                                                                                                                                                                                                             |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| MiddlewareMiddleware    | is a type of computer software that provides services to software applications beyond those available from the operating system                                                                               |
| Request Object          | The req object is an enhanced version of Node's own request object and supports all built-in fields and methods                                                                                               |
| Response Object         | The res object represents the HTTP response that an Express app sends when it gets an HTTP request.                                                                                                           |
| Application Middleware  | Middleware is software that lies between an operating system and the applications running on it.                                                                                                              |
| Routing Middleware      | Express is a routing and middleware web framework that has minimal functionality of its own                                                                                                                   |
| Test Driven Development | software development practice that focuses on creating unit test cases before developing the actual code. It is an iterative approach that combines programming, the creation of unit tests, and refactoring. |
| Behavioral Testing      | Behavioural Testing is a testing of the external behaviour of the program, also known as black box testing. It is usually a functional testing.                                                               |
|                         |

## Preview

- Which 3 things had you heard about previously and now have better clarity on?

  1. ES6 Classes

  2. Using Express Routing

  3. Express Routing

- Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  1. ES6 Classes
  2. Using Express Routing
  3. Express Routing
- What are you most excited about trying to implement or see how it works?
  ES6 Classes
