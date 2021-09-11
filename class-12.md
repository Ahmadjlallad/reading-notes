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
