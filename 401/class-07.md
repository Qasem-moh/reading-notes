# JWT (JSON Web Token)
* JSON Web Token (JWT) is an open standard (RFC 7519)
* that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. 
* This information can be verified and trusted because it is digitally signed.
* JWT can send via URL, POST request, HTTP Header
*  JWTs can be encrypted to also provide secrecy between parties

## When should you use JSON Web Tokens?
1. **Authorization**:  allowing the user to access routes, services, and resources that are permitted with that token.
2. **Information Exchange** :  JSON Web Tokens are a good way of securely transmitting information between parties.you can be sure the senders are who they say they are

## What is the JSON Web Token structure?
* In its compact form, JSON Web Tokens consist of three parts separated by dots (.), which are: **Header** / **Payload** / **Signature**
* looks like the following.```xxxxx.yyyyy.zzzzz```

1. **Header**
The header typically consists of two parts: the type of the token, which is JWT, and the signing algorithm being used, such as HMAC SHA256 or RSA.
2. **Payload**
The second part of the token is the payload, which contains the claims. Claims are statements about an entity (typically, the user) and additional data. There are three types of claims: registered, public, and private claims.
3. **Signature**
To create the signature part you have to take the encoded header, the encoded payload, a secret, the algorithm specified in the header, and sign that.

## If you can decode JWT, how are they secure?
* JWTs can be either signed, encrypted or both. If a token is signed, but not encrypted, everyone can read its contents, but when you don't know the private key, you can't change it. Otherwise, the receiver will notice that the signature won't match anymore.٢٢‏/٠٢‏/٢٠١٧



# Q
1. Write the following steps in the correct order:

* Register your application to get a client_id and client_secret
* Ask the client if they want to sign in via a third party
* Make a request to a third-party API endpoint
* Make a request to the access token endpoint
* Receive access token
* Redirect to a third party authentication endpoint
* Receive authorization code

2. What can you do with an authorization code?

 An authorization code is an alphanumeric password that authorizes its user to purchase, sell or transfer items, or to enter information into a security-protected space

3. What can you do with an access token?

Access tokens are the thing that applications use to make API requests on behalf of a user. The access token represents the authorization of a specific application to access specific parts of a user's data. Access tokens must be kept confidential in transit and in storage.


4. What’s a benefit of using OAuth instead of your own basic authentication?

OAuth is a delegated authorization framework for REST/APIs. It enables apps to obtain limited access (scopes) to a user's data without giving away a user's password. It decouples authentication from authorization and supports multiple use cases addressing different device capabilities.

## Terms 
* **Client ID** Aunique identification number used when sending data to a specific client.
* **Client Secret** A client secret is a secret known only to your application and the authorization server. It protects your resources by only granting tokens to authorized requestors.
* **Authentication Endpoint** Use the authentication endpoint to specify an endpoint that is called to obtain an access token which can then be used in the subsequent password update .
* **Access Token Endpoint** is used by a client to obtain an ID token, access token, and refresh token.
* **API Endpoint** an endpoint can include a URL of a server or service. Each endpoint is the location from which APIs can access the resources they need to carry out their function.
* **Authorization Code** is an alphanumeric password that authorizes its user to purchase, sell or transfer items, or to enter information into a security-protected space
* **Access tokens** are used in token-based authentication to allow an application to access an API.
