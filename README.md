# 🧠 Real-Time Job Offers Aggregator

This project is a full-stack system that captures, processes, and displays job offers in real-time. It was developed during my internship, and it uses modern technologies such as Kafka, Spring Boot, MySQL, Talend, and a Tailwind-based frontend.

## 📁 Repositories

This project is split into 3 separate repositories:

- 🔌 **Kafka Producer** (Spring Boot) – [View Repository](https://github.com/Zakariae-zemat/JobsProducer)
- 🛠️ **Backend API** (Spring Boot REST + MySQL) – [View Repository](https://github.com/Zakariae-zemat/PFAbackend)
- 🌐 **Frontend Web App** (HTML, Tailwind CSS, JavaScript) – [View Repository](https://github.com/Zakariae-zemat/JobPortal)
---

## 🧰 Technologies Used

- **Apache Kafka** – For real-time data streaming.
- **Talend ETL** – For processing and cleaning job data.
- **Spring Boot** – Backend development (Kafka Producer + REST API).
- **MySQL** – Data storage.
- **HTML, Tailwind CSS, JavaScript** – Frontend user interface.

---

## 📌 Project Overview

The system performs the following flow:

1. **Capture** job data via APIs and send to Kafka.
2. **Process** data using Talend (ETL) and store in MySQL.
3. **Expose** data via a REST API.
4. **Display** jobs in a user-friendly frontend with search and filter.

---

## 📊 Architecture

```plaintext
[API Fetcher] ---> [Kafka Producer] ---> [Kafka Topic] ---> [Talend ETL] ---> [MySQL DB] ---> [REST API] ---> [Frontend UI]
