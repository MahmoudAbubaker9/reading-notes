# Serverless and Amplify

## Intro to Serverless

**What is Serverless Architecture?**

Serverless is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers, and which the cloud provider allocates machine resources on demand, taking care of the servers on behalf of their customers.

**some of the currently available cloud services:**

1. AWS Lambda
2. Google Cloud Functions
3. Azure Functions
4. IBM OpenWhisk
5. Alibaba Function Compute
6. Iron Functions
7. Auth0 Webtask
8. Oracle Fn Project
9. Kubeless


1. **Traditional:** applications have run on servers which you had to patch, update, and continuously look after late nights and early mornings due to all the unimaginable errors that broke your production.

2. **Serveless:** users are no longer need to worry about the underlying servers.beacuse they are not managed by users anymore and with management out of the picture the responsibility falls on the Cloud vendors.

## AWS Amplify Kool-Aid:

**What is AWS?**

AWS Amplify is a set of tools and services that can be used together or on their own, to help front-end web and mobile developers build scalable full stack applications, powered by AWS.

**Why use AWS amplify?**

1. Amplify facilitates getting started with AWS for web and mobile app development because it is easy to use and flexible. 

2. The Amplify libraries accelerate implementation of functionality like user authentication, data storage, analytics, and predictions, using AWS services for the back-end functionality.

## GraphQL Intro

It is tool helps on create backends for your web and mobile applications on AWS.

**Create a GraphQL API**

1. amplify init

2. amplify add api

```
Select GraphQL
When asked if you have a schema, say No
Select one of the default samples; you can change this later
Choose to edit the schema and it will open the new schema.graphql in your editor
```

3. amplify push

**************
**Additional resources**

[Intro to Serverless](https://hackernoon.com/what-is-serverless-architecture-what-are-its-pros-and-cons-cc4b804022e9)

[AWS Amplify Kool-Aid](https://aws.amazon.com/amplify/)

[GraphQL Intro](https://docs.amplify.aws/cli/graphql-transformer/overview/)
**************