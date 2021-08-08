## **Express**

### ***What’s the difference between PUT and PATCH?***
- `PUT` is a method of modifying resource where the client sends data that updates the entire resource.
- `PATCH` applies a partial update to the resource.
- Using `PUT` request can lead to a number of outcomes.
- `PATCH` is used when you want to apply a partial update to the resource. 
- `PUT` request, the enclosed entity is viewed as the modified version of the resource saved on the original server, and the client is requesting to replace 
- `PATCH`, the enclosed entity boasts a set of instructions that describe how a resource stored on the original server should be partially modified to create a new version.

### ***Provide links to 3 services or tools that allow you to mock an API for development like `json-server`***
1. **Nock**:is an HTTPS library designed to replicate and mock servers and expectations in `Node.js`.
>Link:
    - `https://github.com/nock/nock`
2. **Beeceptor**:is a free online tool for mocking a `REST API` interaction using any HTTP request. 
>Link:
    - `https://beeceptor.com/`
2.  **Stoplight**: is all about the quick creation of mock servers and visualization of the `APIs` that interact with them. 
>Link:
    - `https://stoplight.io/mocking/`

### ***Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?***
- **Swagger  status Codes**:
   - 200 :	Successful request and response.
   - 400:  Bad request
   - 404: Not found
   - 500:  Unexpected error

- **APIDoc.js HTTP status Codes**:
   - 200 :	Successful request and response.
   - 400:  Bad request
   - 404: Not found
   - 500:  Unexpected error

### ***Compare and contrast SOAP and ReST***
1. `SOAP` is a XML-based message protocol, while `REST` is an architectural style
2. `SOAP` uses WSDL for communication between consumer and provider, whereas `REST` just uses XML or JSON to send and receive data
3. `SOAP` invokes services by calling RPC method, `REST` just simply calls services via URL path
4. `SOAP` doesn't return human readable result, whilst `REST` result is readable with is just plain XML or JSON
5. `SOAP` is not just over HTTP, it also uses other protocols such as SMTP, FTP, etc, `REST` is over only HTTP
