# - What does REST stand for?

- REST is an architectural style for building distributed systems based on hypermedia
- REST APIs are designed around a designed to take advantage of existing protocols.
- What is an identifier of a resource? Give an example.
  - An identifier is a unique identifier for a resource, used by many cache implementations as the key to cached data, The JSON is a representation of the resource
- What are the most common HTTP verbs?

```json
[
  {
    "id": 6,
    "name": "John"
  },
  {
    "id": 7,
    "name": "Jane"
  }
]
```

- What should the URIs be based on?
  - resource that is a thing (noun) instead of referring to an action (verb) because nouns have properties which verbs do not have
    Give an example of a good URI. “/customers/{customerId}/accounts”
- What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
  - web APIs that expose a large number of small resources, and are not well structured try to avoid "chatty" web APIs
- What status code does a successful GET request return?
  - code 200 (OK).
- What status code does an unsuccessful GET request return?
  - code 404 (Not Found).
- What status code does a successful POST request return?
  - code 201 (Created).
- What status code does a successful DELETE request return?

  - code 204 (No Content).

## RegEx

- How would you match your name using RegEx? /[a|A-z]/g
