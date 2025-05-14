## How much data will your publisher program send to the message broker in one run? ##

In one execution, the publisher program sends five messages to the message broker. 
Each message is a UserCreatedEventMessage containing two string fields: user_id and user_name.

## The URL "amqp://guest:guest@localhost:5672" is the same as in the subscriber program. What does it mean? ##

The URL used in both the publisher and subscriber programs is the connection string to the RabbitMQ message broker. 
The first guest is the username, and the second guest is the password for authentication. 
localhost indicates that the broker is running on the same machine as the program, and 5672 is the default port used by the AMQP protocol.

## RabbitMQ Dashboard ##
![RabbitMQ Dashboard](images/image1.png)

## Consoles After Running Both Publisher and Subcriber ##
![RabbitMQ Dashboard](images/image2.png)

## Chart Activity After Running Publisher Multiple Times ##
![RabbitMQ Dashboard](images/image3.png)

The spikes in the chart show that the publisher is sending messages to the RabbitMQ server.
Every spike represents the message being sent overtime. 