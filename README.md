# microservices-nestjs
Implementation of non-HTTP microservices in NestJs

## microservice-app
The microservice app is using the TCP protocol to send messages, with the  `@EventPattern()` decorator we are creating a event handler, that will receive the message.

To start the app:
```bash
$ npm run start
```

## microservice-client
The microservice client will send messages to the microservice app

To start the app:
```bash
$ npm run start
```

To send a message perform a GET request to the endpoint:
```
curl --request GET \
  --url http://localhost:3001/ \
```

The output in the console should be like this:
![terminal-example](images/terminal.png)