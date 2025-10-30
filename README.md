# 📡 Real-Time Wikimedia Stream Publisher & Consumer using Apache Kafka and Spring Boot

## 🧩 Overview
This project demonstrates a **real-time data streaming pipeline** built with **Apache Kafka** and **Spring Boot**.  
It consumes live change events from the **Wikimedia public stream API**, publishes them to a Kafka topic, and consumes the same data for further processing or storage.  

This setup replicates a real-world **event-driven microservice architecture** commonly used in large-scale systems for data processing, monitoring, and analytics.

---

## 🚀 Features
- 🔁 Real-time streaming from **Wikimedia Recent Changes API**
- ⚙️ Kafka **Producer** implemented using `Spring Kafka`
- 📨 Kafka **Consumer** service for message processing
- 🌐 Reactive streaming with **Spring WebClient**
- 💾 Configurable **Kafka topics** and consumer groups
- 🧠 Modular and scalable architecture

---

## 🧱 Architecture Diagram
    Wikimedia Stream (public API)
                │
                ▼
       [Spring Boot Producer]
                │
                ▼
          Apache Kafka Topic
                │
                ▼
       [Spring Boot Consumer]
                │
                ▼
             Storage


---

## 🧰 Tech Stack
| Component | Technology |
|------------|-------------|
| **Language** | Java 21 |
| **Framework** | Spring Boot 3.x |
| **Messaging** | Apache Kafka |
| **HTTP Client** | Spring WebClient |
| **Build Tool** | Maven |
| **Logging** | SLF4J + Logback |

---

## ⚙️ How It Works
1. The **Producer** connects to Wikimedia’s public “Recent Changes” stream via WebClient.  
2. It continuously listens to live updates and publishes messages to a Kafka topic (e.g., `wikimedia_stream`).  
3. The **Consumer** listens to this topic and processes each event — you can extend it to save data in a database, trigger events, or perform analytics.

---

## 🧑‍💻 Setup & Run Instructions

### ✅ You should have Kafka installed in your machine.
## 1️⃣ Start Kafka Broker
.\bin\windows\kafka-server-start.bat .\config\kraft\server.properties

## 3️⃣ Run the Producer
## 4️⃣ Run the Consumer
## 5️⃣ Hit API from Postman : localhost:8081/api/v1/wikimedia

## 💡 Key Learnings

- Integrating **Spring Boot** with **Apache Kafka**  
- Consuming **live real-time streams** using **Spring WebClient**  
- Designing **event-driven microservices**  

---

## 👨‍💻 Author

**Shakib Siddiqui**  
💼 Passionate Java Backend Developer | Spring Boot | Microservices | Kafka  
📧 [https://www.linkedin.com/in/shakib-siddiqui-5861a81b4/]

---

⭐ *If you like this project, don’t forget to give it a star on GitHub!*


