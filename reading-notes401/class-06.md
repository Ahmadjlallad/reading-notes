# class 6

## Review, Research, and Discussion

### In your reading notes page for this class, provide answers to the following prompts. Cite any external sources

- Explain what a “Singleton” is (in Computer Science terms): singleton pattern is a software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system.

- Explain how the Singleton pattern can be used with Node modules, specifically with classes
  using the `module.exports` syntax, to create a singleton class.
- If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?
  implanting as a function run in the middle of the stack.

---

### Document the following Vocabulary Terms

| Term                        | Definition                                                                                                                |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| Router Middleware           | It is a piece of code that comes in the middle of request and response                                                    |
| Dynamic Module Loading      | Dynamic loading is a mechanism by which a computer program can, at run time, load a library (or other binary) into memory |
| Singleton Pattern           | a single database object shared by different parts of the program                                                         |
| CRUD -> REST Method Matches | create, read, update and delete.                                                                                          |
| Mock Testing                | creating a fake version of an external or internal service that can stand in for the real one,                            |

---

### Preview

Skim the following materials in preparation for the upcoming lecture. Note the following as you browse the material, and be prepared to participate in discussions during lecture

- Which 3 things had you heard about previously and now have better clarity on?

  1. BIG O SPACE
  2. Big O Time
  3. Big O Complexity

- Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  - Null
- What are you most excited about trying to implement or see how it works? Auth, JWT

### Preparation Materials

[Securing Passwords](https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html)

#### summary:

- Cryptographic hash algorithms MD5, SHA1, SHA256, SHA512, SHA-3 are general purpose hash functions, designed to calculate a digest of huge amounts of data in as short a time as possible. Hashing is the greatest way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.

- PROBLEMS WITH CRYPTOGRAPHIC HASH ALGORITHMS:

  - Brute Force attack

    - so instead of reversing the hash of the password, an attacker can simply keep trying different inputs until he does not find the right now that generates the same hash value, called brute force attack.

  - Hash Collision attack

    - there is inevitably going to be the possibility of two different inputs that produce the same output hash.

  - BCrypt

    - Bcrypt is an adaptive hash function based on the Blowfish symmetric block cipher cryptographic algorithm and introduces a work factor (also known as security factor), which allows you to determine how expensive the hash function will be to compute.

[Basic Auth](https://en.wikipedia.org/wiki/Basic_access_authentication)

#### summary:

- to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic <credentials>, where credentials is the Base64 encoding of ID and password joined by a single colon

  - is the simplest technique for enforcing access controls to web resources because it does not require cookies, session identifiers, or login pages; rather, HTTP Basic authentication uses standard fields in the HTTP header.

[OWASP auth Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html)

#### summary:

- Authentication is the process of verifying the identity of a user.
- Session Management is the process of maintaining a session between the client and the server.

- Authentication General Guidelines:
  - User IDs
    1. case-insensitive
    2. must be unique
  - Implement Proper Password Strength Controls
    1. Password Length
    - must be at least 8 characters long
    1. usage of all characters
    - must contain at least one upper case letter
    - must contain at least one lower case letter
    - must contain at least one number
    - must contain at least one special character
  - Password Recovery Mechanism
  - Compare Password Hashes Using Safe Functions
    1.  set a maximum number of inputs
    2.  Explicitly sets the type of both variable
    3.  Returns in constant time
  - Change Password Feature
  - Transmit Passwords Only Over TLS or Other Strong Transport
    - The login page and all subsequent authenticated pages must be exclusively accessed over TLS or other strong transport.

[bycrypt](https://www.npmjs.com/package/bcrypt)
[repo usage section](https://github.com/kelektiv/node.bcrypt.js#usage)
