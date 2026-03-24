# 🛒 Emart App — Full Stack Microservices Project

A full-stack e-commerce application built with microservices architecture, containerized using Docker and deployed on AWS EC2.

---

## 🚀 Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | Angular (Client) |
| Backend API | Node.js |
| Java API | Spring Boot (Java 8) |
| Database | MongoDB, MySQL |
| Web Server | Nginx (Reverse Proxy) |
| Containerization | Docker, Docker Compose |
| Cloud | AWS EC2 (Ubuntu) |

---

## 🏗️ Architecture

The app consists of multiple services managed via Docker Compose:

- **Nginx** — reverse proxy routing traffic to the correct service
- **Client** — Angular frontend
- **API (Node.js)** — handles product and user operations
- **Webapi (Spring Boot)** — Java-based REST API for book/order management
- **MongoDB** — database for Node.js API
- **MySQL** — database for Java API

---

## ⚙️ What I Did

- ✅ Deployed the full application using Docker and Docker Compose
- ✅ Fixed a critical `openjdk:8` deprecation issue — migrated to `eclipse-temurin:8` which is the official supported replacement
- ✅ Set up and configured the application on an AWS EC2 instance (Ubuntu)
- ✅ Configured `docker-compose.yaml` to orchestrate all microservices

---

## 🛠️ How to Run

### Prerequisites
- Docker
- Docker Compose

### Steps

```bash
# Clone the repository
git clone https://github.com/snehashinde5321/Emart--project.git
cd Emart--project

# Build and start all services
docker-compose build
docker-compose up -d
```

Access the app at: `http://<your-ec2-public-ip>`

---

## 📁 Project Structure

```
emartapp/
├── client/          # Angular frontend
├── nodeapi/         # Node.js backend API
├── javaapi/         # Spring Boot Java API
├── nginx/           # Nginx reverse proxy config
├── docker-compose.yaml
└── Dockerfile
```

---

## 👤 Author

**Sneha Shinde**
GitHub: [snehashinde5321](https://github.com/snehashinde5321)
