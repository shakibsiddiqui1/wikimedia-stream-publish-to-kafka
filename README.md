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
