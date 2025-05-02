Here’s a rewritten version of the README that keeps all the original content and structure but uses refreshed wording and formatting:

---

# 🍞 Dockerized Bakery Management System

## 📚 Project Overview

This repository features a fully containerized Bakery Management System, orchestrated using Docker Compose. The system comprises:

- **PostgreSQL** for persistent data storage  
- **Flask API** for backend services  
- **React.js** frontend for user interaction  
- **Redis** for caching product data  
- **RabbitMQ** as the message broker  
- **Worker service** for asynchronous order processing  

All components run in isolated containers for streamlined deployment and development.

---

## 🏛️ System Architecture

![System Architecture](https://github.com/user-attachments/assets/d4a2c60d-812a-4069-bb1f-a6182e0b912d)

---

## ⚙️ Setup Instructions

### 1. Clone the repository

```bash
git clone <repository-link>
cd bakery-system
```

### 2. Create a `.env` file

Make sure to define necessary environment variables in a `.env` file at the root of the project.

### 3. Build and run the services

```bash
docker-compose up --build
```

---

## 🔗 Accessing the System

- **Frontend:** [http://localhost:3000](http://localhost:3000)  
- **Backend API:** [http://localhost:5000/api/products](http://localhost:5050/api/products)  
- **RabbitMQ Dashboard:** [http://localhost:15672](http://localhost:15672)  

![RabbitMQ UI](https://github.com/user-attachments/assets/a522b956-abac-48d2-95c2-0bc625368f48)

---

## 🔋 Technologies Used

| Layer       | Technology                                 |
|-------------|---------------------------------------------|
| Backend     | Flask, `psycopg2` (PostgreSQL), `pika` (RabbitMQ), `redis-py` |
| Frontend    | React.js                                   |
| Database    | PostgreSQL                                 |
| Caching     | Redis                                       |
| Messaging   | RabbitMQ                                   |
| Containers  | Docker, Docker Compose                      |

---

## 📜 Key Design Decisions

- **Modular Architecture:** Each service is containerized, promoting separation of concerns and easy scalability.
- **Redis Caching:** Improves product retrieval speed and reduces load on the PostgreSQL database.
- **Async Order Processing:** Combines RabbitMQ and a background worker for efficient, non-blocking order handling.
- **Health Checks:** Each container includes health checks to monitor uptime and reliability.

---

## 🧹 Clean-Up

To shut down and remove all running containers, use:

```bash
docker-compose down
```

---

Let me know if you'd like to convert this into a printable PDF or Markdown file.
