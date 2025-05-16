# Advprog Tutorial 9 - Subscriber
## Priscilla Natanael Surjanto - 2306152153

### Understanding publisher and message broker.

#### 1. How much data your publisher program will send to the message broker in one run?

In one run, the publisher sends 5 data/messages to the message broker.

#### 2. The url of: `amqp://guest:guest@localhost:5672` is the same as in the subscriber program, what does it mean?

It means that they are both connected to the same RabbitMQ server in local. This allows them to exchange messages through RabbitMQ by publishing and consuming messages from queues in the same broker.

### Running RabbitMQ as message broker
![image](https://github.com/user-attachments/assets/5659410d-470e-4a65-bc09-e1b83af10974)

### Sending and processing event
The publisher and subscriber are connected to the same RabbitMQ server. So, whenever the publisher sends data, the subscriber will receive them.
![Screenshot (251)](https://github.com/user-attachments/assets/f516214c-249e-49a7-93fd-34b308040c46)
![Screenshot (250)](https://github.com/user-attachments/assets/3508b256-a5f3-44e9-ab48-b34c1c29f38f)

### Monitoring chart based on publisher
When we run the publisher, more messages are being published to the broker. The spike indicates a sudden surge in the rate at which messages are being published to the broker by the publisher and subsequently delivered to the subscribers.
![image](https://github.com/user-attachments/assets/2f9a9bd8-d28c-4cdf-88e0-0de2a46a4b29)

