# GraphQL @connection

## Intro to Serverless

**What is Serverless Architecture?**

Serverless is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers, and which the cloud provider allocates machine resources on demand, taking care of the servers on behalf of their customers.

## AWS Amplify Kool-Aid

**What is AWS?**

AWS Amplify is a set of tools and services that can be used together or on their own, to help front-end web and mobile developers build scalable full stack applications, powered by AWS.

**Why use AWS amplify?**

1. Amplify facilitates getting started with AWS for web and mobile app development because it is easy to use and flexible. 

2. The Amplify libraries accelerate implementation of functionality like user authentication, data storage, analytics, and predictions, using AWS services for the back-end functionality.


## GraphQL @connection section

* GraphQL is directive enables you to specify relationships between @model types. Currently, this supports one-to-one, one-to-many, and many-to-one relationships

* Definition : directive @connection(keyName: String, fields: [String!]) on FIELD_DEFINITION

* Usage : Relationships between types are specified by annotating fields on an @model object type with the @connection directive.

**************
**Additional resources**

[Intro to Serverless](https://hackernoon.com/what-is-serverless-architecture-what-are-its-pros-and-cons-cc4b804022e9)

[AWS Amplify Kool-Aid](https://aws.amazon.com/amplify/)

[GraphQL @connection section](https://docs.amplify.aws/cli/graphql-transformer/connection/#many-to-many-connections)
**************