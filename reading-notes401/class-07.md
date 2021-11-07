# class 07 - reading notes

## Review, Research, and Discussion

1. Write the following steps in the correct order:

   - Ask the client if they want to sign in via a third party
   - Make a request to a third-party API endpoint
   - Redirect to a third party authentication endpoint
   - Register your application to get a client_id and client_secret
   - Receive authorization code
   - Receive access token
   - Make a request to the access token endpoint

2. What can you do with an authorization code?

   - You can use it to get an access token

3. What can you do with an access token?
   - You can use it to make requests to an API
4. What’s a benefit of using OAuth instead of your own basic authentication?

- You can use OAuth to authenticate with multiple services

---

## Document the following Vocabulary Terms

| Term                    | Definition                                                                                                                                                                                                                                     |
| ----------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Client ID               | public identifier for apps. Even though it's public, it's best that it isn't guessable by third parties, so many implementations use something like a 32-character                                                                             |
| Client Secret           | secret known only to your application and the authorization server.                                                                                                                                                                            |
| Authentication Endpoint | security mechanism designed to ensure that only authorized devices can connect to a given network                                                                                                                                              |
| Access Token Endpoint   | The token endpoint is where apps make a request to get an access token for a user. This section describes how to verify token requests and how to return the appropriate response and errors.                                                  |
| API Endpoint            | the code that allows two software programs to communicate with each other                                                                                                                                                                      |
| Authorization Code      | temporary code that the client will exchange for an access token. The code itself is obtained from the authorization server where the user gets a chance to see what the information the client is requesting, and approve or deny the request |
| Access Token            | Information about the user, permissions, groups, and timeframes is embedded within one token that passes from a server to a user's device.                                                                                                     |

---

## Preparation Materials

- [JWTs Explained](https://jwt.io/introduction/)

  - JSON Web Token (JWT) self-contained way for securely transmitting information between parties as a JSON object.
    JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.
  - When should you use JSON Web Tokens?

    - Authorization This is the most common scenario for using JWT. Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token. Single Sign On is a feature that widely uses JWT nowadays, because of its small overhead and its ability to be easily used across different domains.

    - Information Exchange: JSON Web Tokens are a good way of securely transmitting information between parties

  - What is the JSON Web Token structure? spread by .

    - Header === xxx

    - Then, this JSON is Base64Url encoded to form the first part of the JWT.

    - Payload === yyyyy

    - Signature === zzzzzz
      The signature is used to verify the message wasn't changed along the way, and, in the case of tokens signed with a private key, it can also verify that the sender of the JWT is who it says it is.

    - To create the signature part you have to take the encoded header, the encoded payload, a secret, the algorithm specified in the header, and sign that.

    Therefore, a JWT typically looks like the following.
    xxxxx.yyyyy.zzzzz

```javascript
header: {
"alg": "HS256",
"typ": "JWT"
}
payload:  {

"sub": "1234567890",
"name": "John Doe",
"admin": true
}
HMACSHA256(
base64UrlEncode(header) + "." +
base64UrlEncode(payload),
secret)
```

- Are JWTs Secure?
  Token (JWT, pronounced “jot”) is a compact and url-safe way of passing a JSON message between two parties. It's a standard, defined in RFC 7519. tokens are usually signed or even encrypted
