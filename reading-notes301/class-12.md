# [Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

In your own words, describe what each group of status code represents:

- 100’s = inform the client that we still working on the request and the server is not ready to respond yet.
- 200’s = success, the request was processed successfully.
- 300’s = The resource location changed and the server is redirecting the client to the new location.
- 400’s = The request was not processed successfully, trigger error exceptions on the server.
- 500’s = The server encountered an unexpected condition that prevented it from fulfilling the request.
- What is a status code 202? Accepted
  – The request has been accepted for processing, but the processing has not been completed.
- What is a status code 308? Permanent Redirect
  – The requested resource has been assigned a new permanent URI and any future references to this resource should use one of the returned URIs.
- What code would you use if an update didn’t return data to a client?
  - 204
- What code would you use if a resource used to exist but no longer does?
  - 410
- What is the ‘Forbidden’ status code?
  - 403

## [Build A REST API With Node.js, Express, & MongoDB - Quick](https://www.youtube.com/watch?v=fgTGADljAeg)

- Why do we need to pull our MongoDB database string out of our server and put it into our .env?
  - We need to do this because we are using Heroku, which will automatically deploy our app to a new server. Heroku will automatically deploy our app to a new server, and we need to be able to access our database on that new server.
- What is middleware?
  - Middleware is a function that runs before the route handler.
- What does app.use(express.json()) do?
  - app.use(express.json()) is a middleware function that parses incoming requests with JSON payloads.
- What does the /:id mean in a route?
  - The :id means that the route will accept a parameter called id.
- What is the difference between PUT and PATCH?
  - PUT is used to update an existing resource. PATCH is used to update a portion of an existing resource.
- How do you make a defalut value in a schema?
  - You can use the default keyword in the schema.
- What does a 500 error status code mean?
  - The server encountered an unexpected condition that prevented it from fulfilling the request.
- What is the difference between a status 200 and a status 201?
  - The status 200 means that the request was successful. The status 201 means that the request was successful and a new resource was created.
