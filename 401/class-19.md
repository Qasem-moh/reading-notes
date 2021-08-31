# AWS: Events
## To build Modern Apps over AWS we need :
1. comput : ``Lambda``
2. Database : ``Dynamo DB``
3. Masseging : it's seinding between software componant not people 

## Massaging 
- format ``json`` have key and value paires
- massaging concipt : 
    1. Queue (SQS)
    2. Pub/Sub (SNS)
    3. Streams

- Queue  is buffer between processor and consumer and process msg in FIFO consipt :
    1. send msg to buffer 
    2. store msf in queue until consumer recived it and asknoldg that he recived 
    3. remove msg from queue 

- Pub/Sub concipt: every msg will publish with it's topic while send seperate topice to each subscriber 


* SQS and SNS are important components for scalable, large scale, distributed, cloud-based application
* SNS (Simple Notification Service)
* SQS (Simple Queue Service)

# Difference between SQS and SNS

## SNS (Simple Notification Service)

* **SNS** (Simple Notification Service)
* **SNS is a distributed publish-subscribe system. Messages are pushed to subscribers as and when they are sent by publishers to SNS.**
*  fast
* flexible
* fully managed push notification service that lets you send individual messages or to bulk messages to large numbers of recipients.
*  makes it simple and cost effective to send push notifications to mobile device users
* A distributed publish-subscribe system ,Messages are pushed to subscribers as and when they are sent by publishers to SNS ,SNS supports several end points such as email, sms, http end point and SQS.**you want unknown number and type of subscribers to receive messages, you need SNS.**
 * You can use SNS to send SMS messages to mobile device users in the US or to email recipients worldwide.



## SQS
**SQS** is distributed queuing service.
* Messages are not pushed to receivers. Receivers have to poll SQS to receive messages
* Messages can’t be received by multiple receivers at the same time
*  Any one receiver can receive a message, process and delete it
* Other receivers do not receive the same message later.
* is mainly used to decouple applications or integrate applications.
* Messages can be stored in SQS for short duration of time (max 14 days).
* Messages can be stored in SQS for short duration of time (max 14 days).


# Q 
1. 
- Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server

# Terms
- **Serverless API** Creates a collection of Amazon API Gateway resources and methods that can be invoked through HTTPS endpoints.
- **triggering** event is a tangible or intangible barrier or occurrence which, once breached or met, causes another event to occur

- **Dynamo vs Mongo**
* DynamoDB is a fully managed AWS service ,supports limited data types and smaller item sizes; supports more data types and has fewer size restrictions‏

* MongoDB uses tables, items and attributes ,can be self installed or fully managed with MongoDB Atlas.  uses JSON-like documents.

* **Dynamoose vs Mongoose**  Dynamoose is a modeling tool for Amazon's DynamoDB (inspired by Mongoose). Dynamoose is Sponsored by Dynobase. Dynobase helps you accelerate your ...

