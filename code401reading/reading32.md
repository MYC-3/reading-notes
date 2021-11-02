# Serverless and Amplify
[Notes taken from this site](https://hackernoon.com/what-is-serverless-architecture-what-are-its-pros-and-cons-cc4b804022e9)

- > Serverless applications are event-driven cloud-based systems where application development rely solely on a combination of third-party services, client-side logic and cloud-hosted remote procedure calls
- Cloud Providers:
  - AWS Lambda
  - Azure Functions
  - Google Cloud Functions
  - IBM OpenWhisk
  - Auth0 WebTask
- Traditional Vs. Serverless:
![Serveless Diagram](https://hackernoon.com/hn-images/1*x_v5NRC3TTMt1MaYl1gMUg.jpeg
)
- Pros and cons of serverless architecture:
  - Pricing - Reduces cost by not having to upkeep servers 24x7.
  - Networking - Serveless functions can only be accessed by as private APIs. You must setup an API gateway.
  - 3rd pary dependencies - The winner here is based on the context. For simple applications with few dependencies, Serverless is the winner; for anything more complex, Traditional Architecture is the winner.
  - Environments - Setting up different environments for Serverless is as easy as setting up a single environment.
  - Timeout - functions that are too long or too complex can make it impossible to complete before you get timed out in a serverless architecture.

## AWS Amplify
[Notes taken from this site](https://aws.amazon.com/amplify/)

![AWS Amplif](https://d1.awsstatic.com/AWS%20Amplify/Features/product-page-diagram_Amplify_How-it-works_Develop%402x%20(1).86135eef1e1961cf5cc41fba8c1a5fc46bf38cf2.png)

## GraphQL
- >The GraphQL Transform provides a simple to use abstraction that helps you quickly create backends for your web and mobile applications on AWS

- Create a GraphQL API:
  1. `amplify init`
  2. `amplify add api`
      - Select GraphQL
      - When asked if you have a schema, say No
      - Select one of the default samples; you can change this later
      - Choose to edit the schema and it will open the new schema.graphql in your editor
  3. `amplify push`

[Back to HOME](../README.md)