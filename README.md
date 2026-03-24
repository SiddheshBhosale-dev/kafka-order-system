# Kafka Order-Delivery System

## Overview
This project demonstrates an event-driven architecture using Apache Kafka with two services:
- Order Service (Producer)
- Delivery Service (Consumer)

## Architecture
Order Service → Kafka Topic → Delivery Service

## Tech Stack
- Java
- Spring Boot
- Apache Kafka (3.5.0)
- Zookeeper

## Flow
1. User places order via API
2. Order service publishes message to Kafka
3. Delivery service consumes message
4. Order is processed asynchronously

##  Key Learnings
- Kafka Producer & Consumer
- Event-driven architecture
- Asynchronous communication between services

##  How to Run
1. Start Zookeeper
2. Start Kafka server
3. Run order-service
4. Run delivery-service
5. Hit API endpoint
