# Full Stack Chat Application DevOps Project

A full stack real time chat application deployed using Docker, Kubernetes, GitHub Actions CI/CD, Minikube, and AWS EKS.

This project focuses on practical DevOps implementation including containerization, orchestration, CI/CD automation, Kubernetes deployment, and cloud infrastructure deployment.

---

# Tech Stack

## Frontend

* React.js
* Vite

## Backend

* Node.js
* Express.js
* Socket.IO

## Database

* MongoDB

## DevOps & Cloud

* Docker
* Docker Compose
* Kubernetes
* Minikube
* AWS EC2
* AWS EKS
* GitHub Actions
* Docker Hub
* NGINX Ingress Controller

---

# Features

* Real time chat functionality
* User authentication
* Containerized frontend and backend
* Kubernetes deployment using YAML manifests
* CI/CD automation using GitHub Actions
* Docker image build and push automation
* Kubernetes namespace isolation
* Ingress based routing
* MongoDB deployment in Kubernetes
* Local deployment using Minikube
* Cloud deployment using AWS EKS

---

# Project Structure

```bash id="m2mx29"
full-stack_chatApp/
│
├── .github/workflows/
├── backend/
├── frontend/
├── k8s/
├── docker-compose.yml
├── .gitignore
├── LICENSE
└── README.md
```

---

# Docker Setup

## Build Backend Image

```bash id="h3hlnv"
docker build -t chatapp-backend ./backend
```

## Build Frontend Image

```bash id="m9chps"
docker build -t chatapp-frontend ./frontend
```

## Run Containers

```bash id="cgtq0n"
docker-compose up -d
```

---

# Kubernetes Deployment

## Start Minikube

```bash id="n7h6k9"
minikube start
```

## Apply Kubernetes Manifests

```bash id="p7r0wq"
kubectl apply -f k8s/
```

## Check Kubernetes Resources

```bash id="ukpr4s"
kubectl get all -n chat-app
```

## Check Running Pods

```bash id="vf5n9l"
kubectl get pods -n chat-app
```

---

# CI/CD Pipeline

GitHub Actions workflow automates:

* Docker image build
* Docker Hub image push
* Continuous Integration workflow

Workflow location:

```bash id="utllaq"
.github/workflows/
```

---

# AWS EKS Deployment

The application was also deployed on AWS EKS for managed Kubernetes orchestration.

Commands used:

```bash id="4du0n9"
eksctl create cluster
kubectl get nodes
kubectl top nodes
```

---

# Ingress Routing

NGINX Ingress Controller was used to expose the application externally.

Ingress handled:

* frontend routing
* backend API routing
* service communication

---

# Learning Outcomes

Through this project I learned:

* Docker containerization
* Kubernetes architecture and workloads
* Kubernetes Services and Ingress
* CI/CD pipeline automation
* GitHub Actions workflow management
* AWS EKS deployment
* Troubleshooting Kubernetes networking and deployment issues
* Managing real world DevOps workflows

---

# Author

## Mujtaba Shaikh

Aspiring DevOps & Cloud Engineer
