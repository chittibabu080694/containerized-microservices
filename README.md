# Containerized Microservices Deployment with Docker & AWS ECS/EKS

A production-ready microservices architecture leveraging **Docker**, **Python (Flask)**, and container orchestration workflows on **AWS ECS or EKS**. This project demonstrates containerization best practices, multi-stage or slim image builds, and cloud deployment pipelines.

---

## 🏗️ Architecture Flow

1. **Application Layer:** A lightweight Python [Flask](https://github.com/chittibabu080694/containerized-microservices/blob/main/app/app.py) microservice handling HTTP requests.
2. **Containerization:** Packaged via a dedicated [Dockerfile](https://github.com/chittibabu080694/containerized-microservices/blob/main/app/Dockerfile) utilizing an optimized `python:3.11-slim` base image.
3. **Registry & Orchestration:** Images are pushed to Amazon ECR and deployed onto managed clusters via Amazon ECS (Fargate) or Kubernetes (EKS).

---

## 📁 Repository Structure

```text
containerized-microservices/
├── app/                        # Application Source Code & Configs
│   ├── app.py                  # Core Flask microservice application
│   ├── requirements.txt        # Python dependency manifest
│   └── Dockerfile              # Container build instructions
└── README.md                   # Project documentation
