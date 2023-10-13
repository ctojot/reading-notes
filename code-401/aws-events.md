# AWS: Events

## AWS SQS vs SNS

### What is the difference betweeen SQS and SNS?

SNS is a distributed publish-subscribe service and SQS is distributed queuing service.

### What are some use cases for both SNS and SQS?

- SNS:
  - Be able to publish and consume batches of messages
  - Allow same message to be processed in multiple ways
  - Multiple subscribers are needed

- SQS
  - Need a simple queue with no particular additional requirements
  - Decoupling two applications and allowing parallel asynchronous processing
  - Only one subscriber is needed

## AWS SNS and SQS

### Describe how to use SQS and SNS in a “fanout” pattern

In a fanout pattern SNS is used by publishing messages to a topic and delivering it to many subscribers in different ways. For SQS, SNS can use SQS as one of its subcribers.

### Explain how “push notifications” work, using SNS

Push notifications are the messages that are sent out to subscriber from updates, to order status.

## SQS and SNS Basics

### How might a large scale, distributed application make use of a Queue system like SQS?

With the Queue system of SQS, It allows for load balancing, asynchronous processing, and decoupling between microservices.

## What are your learning goals after reading and reviewing the class README?

SNS and SQS seem a lot like the CAPS Lab we did I'm just hoping its as easy as that was.

## Reference

- ChatGPT
