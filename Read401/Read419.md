# Spring and Sockets

### Real time messaging with websockets

The WebSocket protocol is one of the ways to make The application handle real-time messages.

#### Using WebSocket to build an interactive web application:

1. first strp in Gradle, you will need to add this dependencies to work:

```
implementation 'org.webjars:webjars-locator-core'
implementation 'org.webjars:sockjs-client:1.0.2'
implementation 'org.webjars:stomp-websocket:2.3.3'
implementation 'org.webjars:bootstrap:3.3.7'
implementation 'org.webjars:jquery:3.1.1-1'
```
2. Create a Resource Representation Class

The service will accept messages that contain a name in a STOMP message in JSON object and to model JSON file contact you need to create name property and a corresponding getName() method.

3. Create a Message-handling Controller

Implement a controller that will handle user requests. It will broadcast received message to all users subscribed to a given topic.

4. Configure Spring for STOMP messaging

* in this step you need to create WebSocketConfig by @Configuration to indicate that it is a Spring configuration class.

*Also annotated with @EnableWebSocketMessageBroker to enables WebSocket message handling, backed by a message broker.

5. Create a Browser Client

With the server side the client can  send and receive messages to the server side.

* imports the SockJS and STOMP in HTML file will be used to communicate with our server through STOMP over websocket



* This guide walks you through the process of creating a “Hello, world” application that sends messages back and forth between a browser and a server. 

[Resource](https://spring.io/guides/gs/messaging-stomp-websocket/)





