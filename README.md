# Docker Compose PHP & MariaDB Stack

## 📌 Overview

This project demonstrates a simple **multi-container application deployment** using **Docker Compose**.  
It includes a **PHP application running on Apache** and a **MariaDB database**, each running in separate containers and managed together.

The project focuses on basic **Docker and DevOps concepts** such as containerization, service orchestration, persistent storage using volumes, and environment-based configuration.  
It represents a typical setup used in real-world applications where the web and database services run independently but communicate through Docker networking.

---

## 🏗️ Architecture
The application follows a simple two-tier architecture:

- **Web Tier**
  - PHP application running on Apache
  - Exposed via host port `8083`

- **Database Tier**
  - MariaDB database
  - Uses persistent storage for data durability

---

## 🛠️ Technologies Used
- Docker
- Docker Compose (v2)
- PHP
- Apache
- MariaDB
- Linux

---

---

## ⚙️ Prerequisites
Make sure the following tools are installed on your system:

```bash
docker --version
docker compose version
```
## 🚀 How to Run the Project

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/<your-username>/docker-compose-php-mariadb-stack.git
cd docker-compose-php-mariadb-stack
```
### 2️⃣ Start the Application
```bash
docker compose up -d
```
### 3️⃣ Verify Running Containers
```bash
docker ps
```
### You should see two running containers:
- php_host
- mysql_host
### 4️⃣ Access the Application
- If running locally:
```bash
curl localhost:8083
```
- If running on a remote server:
```bash
curl <server-ip>:8083
```
### 5️⃣ Stop the Application
```bash
docker compose down
```
### ⭐ Key Features
- Multi-container orchestration using Docker Compose
- Persistent storage using Docker volumes
- Service-to-service communication via Docker networking
- Port mapping to expose services
- Environment-based configuration
- Production-like containerized deployment workflow
