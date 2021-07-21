# Reading 8 - APIs

## RESTful web API Design
[All notes were taken from here](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)

- What does **REST** stand for?
  - Representational State Transfer
- REST APIs are designed around a <ins>*resource*</ins>.
- What is an identifer of a resource? Give an example.
  - URI = Uniform Resource Identifier.
  ```
  https://adventure-works.com/orders/1
  ```
- What are the most common HTTP verbs?
  - `GET`, `POST`, `PUT`, `PATCH`, and `DELETE`.
- What should the URIs be based on?
  - They should be based on **nouns**.
- Give an example of a good URI.
  ```
  https://adventure-works.com/orders // Good

  https://adventure-works.com/create-order // Avoid
  ```
- What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
  - An API sending a large number of small resources is described as "chatty".
  - It is mostly bad because it imposes a load on the server.
  - But sending a large resource could increase latency and bandwith costs.
- What status code does a successful GET request return?
  - 200 (OK)
- What status code does an unsuccessful GET request return?
  - 404 (Not Found)
- What status code does a successful POST request return?
  - 200 or 201 (Created)
- What status code does a successful DELETE request return?
  - 204

[Back to HOME](../README.md)