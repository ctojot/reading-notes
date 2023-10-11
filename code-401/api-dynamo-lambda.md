# AWS: API, Dynamo and Lambda

## AWS API Gateway Overview

### What is Amazon API Gateway?

Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic.

### Why is Amazon API Gateway an important part of the Serverless ecosystem?

Within the Serverless ecosystem, API Gateway is the piece that ties together Serverless functions and API definitions. Being able to trigger the execution of a Serverless function directly in response to an HTTP request is the key reason why API Gateway is so valuable in Serverless setups: it enables a truly serverless architecture for web applications.

### How does API Gateway integrate with other AWS services?

API Gateway integrates with many other AWS services like AWS Lambda, AWS SNS, AWS IAM, and Cognito Identity Pools. These integrations allow for fully managed authentication and authorization layers, as well as detailed metrics and tracing for API requests.

## AWS API Gateway

### What are the some benefits of using Amazon API Gateway?

- Efficient API development
- Performance at any scale
- Cost savings at scale
- Easy monitoring
- Flexible security controls
- RESTful API options

### What two API types might you choose from?

- RESTful APIs
- WEBSOCKET APIs

## AWS DynamoDB Guide

### What is DynamoDB?

DynamoDB is a hosted NoSQL database offered by AWS.

### Under what circumstances would you recommend DynamoDB over MongoDB?

- DynamoDB has a more hands-off operations model than MongoDB as you don't think to think about instances and scaling up or down
- DynamoDB's connection and security model make it a popular choice for use with serverless compute like AWS Lambda

## AWS DynamoDB

### Explain to a non-technical friend how DynamoDB works.

You can think of a notebook. You can list a bunch of things on it. However, DynamoDB is like a high powered digital notebook that can hold tons of information about the things you are listing and its available at any time.

## Dynamoose

### What is Dynamoose?

Dynamoose is a modeling tool for Amazon's DynamoDB that is heavily inspired by Mongoose.

### What are some key features of Dynamoose?

- Type safety
- High level API
- Easy to use syntax
- DynamoDB Single Table Design Support
- Ability to transform data before saving or retrieving items
- Strict data modeling (validation, required attributes, and more)
- Support for DynamoDB Transactions
- Powerful Conditional/Filtering Support
- Callback & Promise support
- AWS Multi-region support

## Reflection

### What are your learning goals after reading and reviewing the class README?

My learning goal is to get better accustomed to databases with AWS DynamoDB