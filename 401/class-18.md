# AWS: API, Dynamo and Lambda

## Amazon API Gateway
* is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale.
* APIs act as the "front door" for applications to access data, business logic, or functionality from your backend services.
* Using API Gateway, you can create RESTful APIs and WebSocket APIs that enable real-time two-way communication applications. API Gateway supports containerized and serverless workloads, as well as web applications.

### How does API Gateway work?
* API Gateway sits between the backend services of your API and your API’s users, handling the HTTP requests to your API endpoints and routing them to the correct backends.
* API Gateway integrates with many other AWS services like AWS **Lambda**, **AWS SNS**, **AWS IAM**, and Cognito Identity Pools. These integrations allow for fully managed authentication and authorization layers, as well as detailed metrics and tracing for API requests.


## DynamoDB
* **DynamoDB** is a hosted NoSQL database offered by Amazon Web Services (AWS).
* **Amazon DynamoDB** is a key-value and document database that delivers single-digit millisecond performance at any scale.
* It's a fully managed, multi-region, multi-active, durable database with built-in security, backup and restore, and in-memory caching for internet-scale applications. 

* **use cases**:

1. Applications with large amounts of data and strict latency requirements. As your amount of data scales, JOINs and advanced SQL operations can slow down your queries. With DynamoDB, your queries have predictable latency up to any size, including over 100 TBs!

2. Serverless applications using AWS Lambda. AWS Lambda provides auto-scaling, stateless, ephemeral compute in response to event triggers. DynamoDB is accessible via an HTTP API and performs authentication & authorization via IAM roles, making it a perfect fit for building Serverless applications.

3. Data sets with simple, known access patterns. If you're generating recommendations and serving them to users, DynamoDB's simple key-value access patterns make it a fast, reliable choice.

## Dynamoose
* is a modeling tool for Amazon's DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familar.

## Lambda
* is a compute service that lets you run code without provisioning or managing servers.
# Terms
* **CDN** Content Delivery Network
* **Cloud Storage** It is  storage model Over internet where data is stored on multiple virtual servers, rather than being hosted on a specific server.
* A **serverless function** is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies.

# Q 
1. What are serverless functions?
- A serverless function is a programmatic function written by a software developer for a single purpose. It's then hosted and maintained on infrastructure by cloud computing companies.

2. If you were to create a system that emulated Lambda functions, how would you do it?
- Lambda runs your function only when needed and scales automatically
- You can invoke your Lambda functions using the Lambda API, or Lambda can run your functions in response to events from other AWS services.

3. Describe how a CDN works
- is a highly-distributed platform of servers that helps minimize delays in loading web page content by reducing the physical distance between the server and the user(distance that the request has to travel)
- To combat this, CDNs store a cached version of your website content in multiple geographical locations around the world, which are known as “points of presence” (PoPs). These PoPs will contain their own caching servers and will be responsible for delivering that content in the user’s location.