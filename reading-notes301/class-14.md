# [What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

- What is OAuth?
  - OAuth is an authentication protocol that allows you to approve one application interacting with another on your behalf without giving away your password
- Give an example of what using OAuth would look like.
  - one website saying “hey, do you want to log into our website with other website's login?”
- How does OAuth work? What are the steps that it takes to authenticate the user?
  -Step 1 – The User Shows Intent.
  - Step 2 – The Consumer Gets Permission.
  - Step 3 – The User Is Redirected to the Service Provider.
  - Bitly directs Joe to Twitter for authorization
  - Step 4 – The User Gives Permission.
  - Step 5 – The Consumer Obtains an Access Token.
- What is OpenID?
  - OpenID Connect (OIDC) is an open authentication protocol that profiles and extends OAuth 2.0 to add an identity layer.

## [Authorization and Authentication flows](https://auth0.com/docs/flows)

- What is the difference between authorization and authentication?

  - Authorization means granting a user account configured on the computer system the right to make use of a resource (allocating the user privileges on the resource). Authentication protects the validity of the user account by testing that the person accessing that account is who s/he says s/he is.

- What is Authorization Code Flow?
  - used to obtain an access token to authorize API requests
- What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
  - is an OpenId Connect flow specifically designed to authenticate native or mobile application users
- What is Implicit Flow with Form Post?

  - Implicit Flow with Form Post flow uses OIDC to implement web sign-in that is very similar to the way SAML and WS-Federation operates. The web app requests and obtains tokens through the front channel, without the need for secrets or extra backend calls.

- What is Client Credentials Flow?

  - The Client Credentials flow is a server to server flow. There is no user authentication involved in the process. ... This flow is useful for systems that need to perform API operations when no user is present. It can be nightly operations, or other that involve contacting OAuth protected APIs.

- What is Device Authorization Flow?
  - instructs the user to review the authorization request on a secondary device
- What is Resource Owner Password Flow?
  - Resource Owner Password Credentials flow allows exchanging the username and password of a user for an access token and, optionally, a refresh token. The primary difference is that the user's password is accessible to the application
