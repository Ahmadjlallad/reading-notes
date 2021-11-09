# Class 8 Reading Notes

## Review, Research, and Discussion

- When is Basic Authorization used vs. Bearer Authorization?
  - Basic Authorization is used when the client is not trusted.
  - Bearer Authorization is used when the client is trusted.
- What does the JSON Web Token package do?
  - The JSON Web Token package is used to create and verify tokens.
- What considerations should we make when creating and storing a SECRET?
  - The SECRET should be stored in a secure location.
  - The SECRET should be stored in a file that is not accessible to the public.

## Document the following Vocabulary Terms

| Term           | Definition                                                                                                                                                                                                                                                                                                              |
| -------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| encryption     | Encryption is a means of securing digital data using one or more mathematical techniques, along with a password or "key" used to decrypt the information. The encryption process translates information using an algorithm that makes the original information unreadable.                                              |
| token          | It enables users to verify their identity to websites, which then generates a unique encrypted authentication token.                                                                                                                                                                                                    |
| bearer         | Bearer Tokens are the predominant type of access token used with OAuth 2.0. A Bearer Token is an opaque string, not intended to have any meaning to clients using it. Some servers will issue tokens that are a short string of hexadecimal characters, while others may use structured tokens such as JSON Web Tokens. |
| secret         | a symmetric key that is known by both the sender and the receiver.                                                                                                                                                                                                                                                      |
| JSON Web Token | is a means of representing claims to be transferred between two parties. The claims in a JWT are encoded as a JSON object that is digitally signed using JSON Web Signature (JWS) and/or encrypted using JSON Web Encryption (JWE).                                                                                     |

## 3 Preview

- Which 3 things had you heard about previously and now have better clarity on?
  - I have heard about the JSON Web Token package.
  - I have heard about the Bearer Token.
  - I have heard about the Basic Authorization.
- Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  - I am hoping to learn more about the JSON Web Token package.
  - I am hoping to learn more about the Bearer Token.
  - I am hoping to learn more about the Basic Authorization.
- What are you most excited about trying to implement or see how it works?
  - I am excited to see how the JSON Web Token package works.

## Preparation Materials

[RBAC tutorial](https://www.youtube.com/watch?v=C4NP8Eon3cA)
[5 steps to RBAC](https://www.csoonline.com/article/3060780/5-steps-to-simple-role-based-access-control.html)
[wiki - RBAC](https://en.wikipedia.org/wiki/Role-based_access_control)

### RBAC is the idea of assigning system access to users based on their role in an organization. It's important to remember that not every employee needs a starring role.

- user can be assigned to a role in a system (e.g. admin, user, guest)
- role can be assigned to a user in a system (e.g. admin, user, guest)
- user can be assigned to multiple roles in a system (e.g. admin, user, guest)
- role can be assigned to multiple users in a system (e.g. admin, user, guest)

#### simplified five-step approach to getting it implemented:

- Inventory your systems
- divide your system into a accessible and unaccessible areas
  - Examples would include an email system, customer database, contact management system, major folders on a file server, etc.
- Analyze your workforce and create roles
  - divide your workforce into roles
    - Avoid the temptation to have too many roles defined. Keep them as simple and stratified as possible
    - Example basic user role, which includes the access any employee would need
- Assign people to roles
  - figure out which role(s) each employee belongs in, and set their access accordingly.
- Audit
  - Periodically review your roles, the employees assigned to them, and the access permitted for each. If you discover, for example, that a role has unnecessary access to a particular system, change the role and adjust the access level for all employees in that role.
