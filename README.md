# 🚀 MEAN Stack CRUD Application - Full DevOps Deployment

This project demonstrates containerization and deployment of a full-stack MEAN (MongoDB, Express, Angular, Node.js) CRUD application using Docker, Docker Compose, GitHub Actions CI/CD, and AWS EC2.

---

# 📌 Project Overview

This project includes:

- Angular 15 frontend
- Node.js + Express backend
- MongoDB database
- Docker containerization
- Docker Compose orchestration
- GitHub Actions CI/CD pipeline
- Nginx reverse proxy
- AWS EC2 deployment (Ubuntu)

---

# 🧱 Tech Stack

| Layer       | Technology |
|------------|------------|
| Frontend   | Angular 15 |
| Backend    | Node.js + Express |
| Database   | MongoDB |
| Containers | Docker |
| Orchestration | Docker Compose |
| CI/CD      | GitHub Actions |
| Cloud      | AWS EC2 (Ubuntu) |
| Reverse Proxy | Nginx |

---

# 🐳 Docker Setup (Local Development)

## 1️⃣ Run Application

```bash
docker-compose up --build

Application will be available at:

http://localhost

---

## 📦 Docker Hub Images

Docker images are pushed automatically via CI/CD.

### Backend Image
konireddy21/mean-backend:latest

### Frontend Image
konireddy21/mean-frontend:latest

---

## 🔁 CI/CD Pipeline

CI/CD is implemented using GitHub Actions.

Pipeline steps:
1. Triggered on push to main branch
2. Build backend Docker image
3. Build frontend Docker image
4. Push images to Docker Hub

Workflow file:
.github/workflows/docker-build.yml

---

## 🗄 Database Configuration

MongoDB runs inside a Docker container.

Environment variable used:
MONGO_URI=mongodb://mongodb:27017/ddtask

---

## 🌐 Nginx Configuration

Nginx is used in the frontend container to:
- Handle Angular routing
- Proxy API requests to backend

---

## ☁️ AWS EC2 Deployment

Steps:
1. Launch Ubuntu EC2 instance
2. Install Docker & Docker Compose
3. Clone this repository
4. Run:
docker-compose up -d

Application will be available at:
http://<EC2_PUBLIC_IP>

---

## 📸 Screenshots

The following screenshots are included:
- Docker Hub images
- GitHub Actions pipeline success
- docker-compose.yml
- nginx.conf
- Running containers
- Application UI
- EC2 instance details

---

## ✅ Final Status

✔ Frontend Dockerized  
✔ Backend Dockerized  
✔ MongoDB Containerized  
✔ Docker Compose Working  
✔ CI/CD Implemented  
✔ Production Ready  

---

## 📎 GitHub Repository

https://github.com/manoj-konireddy/mean-crud-dd-task