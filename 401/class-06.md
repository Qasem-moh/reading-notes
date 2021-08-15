# Securing Passwords with Bcrypt Hashing Function
* Cryptographic hash algorithms MD5, SHA1, SHA256, SHA512, SHA-3 are general purpose hash functions, designed to calculate a digest of huge amounts of data in as short a time as possible.
* Hashing is the greatest way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.
* The benefit of hashing is that if someone steals the database with hashed passwords, they only make off with the hashes and not the actual plaintext passwords. 
* **Hash Collision attack**: Hash functions have infinite input length and a predefined output length, the possibility of two different inputs that produce the same output hash. **MD5, SHA1, SHA2** are vulnerable to Hash Collision Attack i.e. two input strings of a hash function that produce the same hash result.
*  **PBKDF2** and **BCrypt** algorithms which can make the brute force attacks slower and minimize the impact, both use a technique called Key Stretching.
* **Bcrypt** is an adaptive hash function based on the Blowfish symmetric block cipher cryptographic algorithm and introduces a work factor (also known as security factor)
*  **work factor** which allows you to determine how expensive the hash function will be.
and it's value determines how slow the hash function will be, means different work factor will generate different hash values in different time span, which makes it extremely resistant to brute force attacks. When computers become faster next year we can increase the work factor to balance it out i.e. to make the attack slower.
* This hashing algorithm is implemented in a number programming languages like PHP, Java, Ruby, C#, C etc. If you are a PHP developer, you can simply use the crypt() function with a Blowfish required salt.
* This method of hashing passwords is solid enough for most web applications that stores users' passwords and other sensitive data.


# Basic access authentication
* **basic access authentication** is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request.
* HTTP **Basic authentication** (BA) implementation is the simplest technique for enforcing access controls to web resources because it does not require cookies, session identifiers, or login pages; rather, HTTP Basic authentication uses standard fields in the HTTP header.
* The BA mechanism does not provide confidentiality protection for the transmitted credentials. They are merely encoded with Base64 in transit and not encrypted or hashed in any way. Therefore, basic authentication is typically used in conjunction with HTTPS to provide confidentiality.

* Because the BA field has to be sent in the header of each HTTP request, the web browser needs to cache credentials for a reasonable period of time to avoid constantly prompting the user for their username and password
* HTTP does not provide a method for a web server to instruct the client to "log out" the user====> there are a number of methods to clear cached credentials in certain web browsers:
    1. redirecting the user to a URL on the same domain, using credentials that are intentionally incorrect.but it's inconsistent between various browsers and browser versions
    2. Microsoft Internet Explorer offers a dedicated JavaScript method to clear cached credentials
    ``<script>document.execCommand('ClearAuthenticationCache');</script>``
* To unauthenticated requests, the server should return a response whose header contains a HTTP 401 Unauthorized status and a WWW-Authenticate field.
* WWW-Authenticate field for basic authentication ``WWW-Authenticate: Basic realm="User Visible Realm"``
* server may choose to include the charset parameter from RFC 7617``WWW-Authenticate: Basic realm="User Visible Realm", charset="UTF-8"``
* **charset="UTF-8"** This parameter indicates that the server expects the client to use UTF-8 for encoding username and password (see below).

**The Authorization header field is constructed as follows:**

1. The username and password are combined with a single colon (:). This means that the username itself cannot contain a colon.
2. The resulting string is encoded into an octet sequence. The character set to use for this encoding is by default unspecified, as long as it is compatible with US-ASCII, but the server may suggest use of UTF-8 by sending the charset parameter.
3. The resulting string is encoded using a variant of Base64 (+/ and with padding).
4. The authorization method and a space (e.g. "Basic ") is then prepended to the encoded string.
``Aladdin:open sesame, or Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==``

# OWASP auth cheatsheet

* **Authentication** is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed **by** submitting a username or ID and one or more items of private information that only a given user should know.

* **Session Management** is a process by which a server maintains the state of an entity interacting with it
* Sessions are maintained on the server by a session identifier which can be passed back and forward between the client and server when transmitting and receiving requests.
*  Sessions should be unique per user and very difficult to predict.

## Use of authentication protocols that require no password¶

1. **Open Authorization (OAuth ¶)** is a protocol that allows an application to authenticate against a server as a user, without requiring passwords or any third party server that acts as an identity provider
2. **OpenId ¶** is an HTTP-based protocol that uses identity providers to validate that a user is whom he says he is. It is a very simple protocol which allows a service provider initiated way for single sign-on (SSO).
3. **SAML¶** Security Assertion Markup Language (SAML)
4. **FIDO¶**
    * The Fast Identity Online (FIDO)  has created two protocols to facilitate online authentication: the Universal Authentication Framework (UAF) protocol and the Universal Second Factor (U2F) protocol.
    * While **UAF** focuses on passwordless authentication, **U2F** allows the addition of a second factor to existing password-based authentication.


# bcrypt docs
* **node.bcrypt.js** A library to help you hash passwords.
*  bcrypt module uses **node-gyp** to build and install, you'll need a stable version of node to use bcrypt.
## Install via NPM
``npm install bcrypt``
## Usage

``async (recommended)``

``const bcrypt = require('bcrypt');``

``const saltRounds = 10;``

``const myPlaintextPassword = 's0/\/\P4$$w0rD';``

``const someOtherPlaintextPassword = 'not_bacon';``



**To hash a password:**
*Technique 1 (generate a salt and hash on separate function calls):*

``bcrypt.genSalt(saltRounds, function(err, salt) {``

  ``  bcrypt.hash(myPlaintextPassword, salt, function(err, hash) {``
  
``    // Store hash in your password DB.``

``});``

``});``


*Technique 2 (auto-gen a salt and hash):*

``bcrypt.hash(myPlaintextPassword, saltRounds, function(err, hash) {``

  ``  // Store hash in your password DB.``

``});``

**To check a password:**
*// Load hash from your password DB.*
``bcrypt.compare(myPlaintextPassword, hash, function(err, result) {``

``    // result == true``

``});``

``bcrypt.compare(someOtherPlaintextPassword, hash, function(err, result) {``

``    // result == false``

``});``


# Q:
1. Explain what a “Singleton” is (in Computer Science terms)
- Is a software design pattern that restricts the instantiation of a class to one "single" instance. 

2. Explain how the Singleton pattern can be used with Node modules, specifically with classes
- IT'S restricts the instantiation of a class to one "single" instance ;useful when exactly one object is needed to coordinate actions across the system. 

3. If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?
- write middlewear function 
- importe this middlewear Either globally ``app.use(middleware)`` or locally ``app.get('/',middleware,CB).``


* **Middleware** is functions that have access to the request object (req), the response object (Links to an external site.) (res)
* A **REST** API (also known as RESTful API) is an application programming interface (API or web API) that conforms to the constraints of REST architectural style and allows for interaction with RESTful web services. REST stands for representational state transfer
* **Mock testing** is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules
* **Dynamic loading** is a mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, 
- allows a computer program to start up in the absence of these libraries, to discover available libraries, and to potentially gain additional functionality
* **singleton pattern**is a software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system. 