# 🚀 Kafka Order-Delivery System (Event-Driven Microservices)

## 📌 Overview

This project demonstrates a real-world **event-driven microservices architecture** using Apache Kafka.

It simulates how platforms like food delivery systems process orders asynchronously using messaging queues.

---

## 🏗️ Architecture

Order Service → Kafka Topic → Delivery Service

* **Order Service** → Produces order events
* **Kafka Broker** → Handles message queue
* **Delivery Service** → Consumes and processes events

---

## ⚙️ Tech Stack

* Java 8+
* Spring Boot
* Apache Kafka (3.5.0)
* Zookeeper
* Maven

---

## 🔄 Workflow

1. User places an order via REST API
2. Order Service publishes event to Kafka topic
3. Kafka stores and distributes the event
4. Delivery Service consumes the event
5. Order is processed asynchronously

---

## ✨ Features

* Asynchronous communication between services
* Loose coupling using Kafka
* Scalable microservices architecture
* Real-time event processing

---

## 🧠 Key Concepts Learned

* Kafka Producer & Consumer
* Event-driven architecture
* Microservices communication
* Message brokers & topics

---

## ▶️ How to Run

### Step 1: Start Zookeeper

```bash
zookeeper-server-start.bat config/zookeeper.properties
```

### Step 2: Start Kafka

```bash
kafka-server-start.bat config/server.properties
```

### Step 3: Run Services

```bash
cd order-service
mvn spring-boot:run

cd delivery-service
mvn spring-boot:run
```

### Step 4: Hit API

```
POST /order
```

---

## 📌 Future Improvements

* Retry mechanism (failed events)
* Dead Letter Queue (DLQ)
* Logging & monitoring
* Docker support
* AWS deployment

---

## 👨‍💻 Author

**Siddhesh Bhosale**
