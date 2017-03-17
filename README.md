# RabbitMQ Golang Example

This example will demonstrate how to use RabbitMQ as a simple queue for sending and consuming json structured message in golang.

Make sure you have RabbitMQ server running locally or in cloud before running the example.

You can also run RabbitMQ server on docker container using below command.

`docker run -d --hostname rabbit-cluster --name go-rabbit -p 8080:15672 -p 5672:5672 rabbitmq:3-management`

Before you run the code samples, make sure your local Go workspace has a copy of the **amqp** dependency:

`go get github.com/streadway/amqp`

Once docker is running, you can use the following command to send a message via RabbitMQ:

`go run send.go`

and to receive a message:

`go run receive.go`