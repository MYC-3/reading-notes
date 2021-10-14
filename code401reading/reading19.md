# Spring and Sockets

## Real time web messaging with sockets
[Notes taken from this site](https://spring.io/guides/gs/messaging-stomp-websocket/)

- WebSocket is a thin, lightweight layer above TCP.
- STOMP is a subprotocol operating on top of the lower-level WebSocket.
- The following is summary of the steps to create a basic web messaging app (Visit the site for more detailed instructions):
1. Spring Initilizr - Pick the Websocket dependency
2. Add the following dependencies:
```Java
implementation 'org.webjars:webjars-locator-core'
implementation 'org.webjars:sockjs-client:1.0.2'
implementation 'org.webjars:stomp-websocket:2.3.3'
implementation 'org.webjars:bootstrap:3.3.7'
implementation 'org.webjars:jquery:3.1.1-1'
```
3. Create a Resource Representation Class
4. Create a Message-handling controller
5. Configure Spring for STOMP messaging
5. Create a browser client
6. Make the application executable
7. Test the service

[Back to HOME](../README.md)