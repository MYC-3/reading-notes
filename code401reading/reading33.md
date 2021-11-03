# GraphQL
[Notes were taken from this site](https://docs.amplify.aws/cli/graphql-transformer/directives/#connection)

- Amplify-provided directives:
  - `@model`: Defines top level object types in your API that are backed by Amazon DynamoDB
  - `@key`: Configures custom index structures for @model types
  - `@auth`: Defines authorization rules for your @model types and fields
  - `@connection`: Defines 1:1, 1:M, and N:M relationships between @model types
  - `@function`: Configures a Lambda function resolvers for a field
  - `@http`: Configures an HTTP resolver for a field
  - `@predictions`: Queries an orchestration of AI/ML services such as Amazon Rekognition, Amazon Translate, and/or Amazon Polly
  - `@searchable`: Makes your data searchable by streaming it to Amazon OpenSearch
  - `@versioned`: Defines the versioning and conflict resolution strategy for an @model type
- AWS AppSync-provided directives:
  - `@aws_api_key`
  - `@aws_iam`
  - `@aws_oidc`
  - `@aws_cognito_user_pools`
  - `@aws_auth`
  - `@aws_subscribe`
- 3rd party directives:
  - `@algolia`: Add serverless search to your Amplify API with Algolia
  - `@ttl`: Enable DynamoDB's time-to-live feature to auto-delete old entries in your AWS Amplify API
  - `@firehose`: Add a simple interceptor to all of your Amplify API mutations and queries
  - `@retain`: Enable the "Retain" deletion policy for your Amplify-generated DynamoDB tables

[Back to HOME](../README.md)