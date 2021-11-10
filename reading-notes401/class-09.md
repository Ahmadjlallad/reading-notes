# Review, Research, and Discussion

- What header(s) are used in authentication and authorization
  - The Authorization and Proxy-Authorization request headers contain the credentials to authenticate a user agent with a (proxy) server. Here, the <type> is needed again followed by the credentials, which can be encoded or encrypted depending on which authentication scheme is used
- What is safe to put into a JWT

  - The general opinion is that they're good for being used as ID Tokens or Access Tokens and that they're secure - as the tokens are usually signed or even encrypted. ... A JSON Web Token (JWT, pronounced “jot”) is a compact and url-safe way of passing a JSON message between two parties. It's a standard, defined in RFC 7519.

- How are JWTs validated
  - Check signature. The last segment of a JWT is the signature, which is used to verify that the token was signed by the sender and not altered in any way. The Signature is created using the Header and Payload segments, a signing algorithm, and a secret or public key (depending on the chosen signing algorithm).

## Document the following Vocabulary Terms

| Term       | Definition                                                                                                                                                       |
| ---------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| RBAC       | Role-based access control (RBAC) is a method of restricting network access based on the roles of individual users within an enterprise.                          |
| User Roles | User Roles are permission sets that control access to areas and features within the Professional Archive Platform. Each User account requires a Role assignment. |
|            |
| JWT Token  | JSON Web Token (JWT) is a JSON encoded representation of a claim(s) that can be transferred between two parties.                                                 |

- Which 3 things had you heard about previously and now have better clarity on?

  - JWT
  - RBAC
  - User Roles

- Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  -authentication
  -authorization
  -JWT

- What are you most excited about trying to implement or see how it works?
  - JWT
