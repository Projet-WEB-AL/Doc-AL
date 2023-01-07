# Doc-AL

## Project architecture

```mermade
flowchart
adminer -- manages the database --> MySQL
MySQL --> BACK
BACK --> FRONT
BACK -- Send data for email--> RabbitMQ
RabbitMQ-->Quarkus
Quarkus-- Send email -->mailDev
```

## Problems during the project 

1. Connection problem between the backend and the database [Solved] -> Big waste of project time
2. Connection problem between the backend and the frontend [Solved] (need to use chromium on linux ???!) -> waste of project time
3. Problem sending data to the rabbitmq queue [actual]