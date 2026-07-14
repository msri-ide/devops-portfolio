# DevOps Portfolio

## 📌 Overview

This project demonstrates an end-to-end deployment of a containerized web application on Amazon EKS using production-style Kubernetes networking.

The application is containerized using Docker, stored in Amazon ECR, deployed on Amazon EKS, and exposed to the internet through an AWS Application Load Balancer (ALB) using Kubernetes Ingress.

To securely allow Kubernetes workloads to access AWS services, OIDC and IAM Roles for Service Accounts (IRSA) are implemented. The AWS Load Balancer Controller is installed using Helm to automatically provision and manage the Application Load Balancer.

---

## 🛠️ Tech Stack

- Linux
- AWS EC2
- Amazon ECR
- Amazon EKS
- Docker
- Kubernetes
- kubectl
- eksctl
- Helm
- OIDC
- IAM Roles for Service Accounts (IRSA)
- AWS Load Balancer Controller
- Kubernetes Ingress

---

## 🏗️ Architecture

```text
Developer
    │
    ▼
Docker Build
    │
    ▼
Amazon ECR
    │
    ▼
Amazon EKS
    │
    ▼
Kubernetes Deployment
    │
    ▼
Pods
    │
    ▼
ClusterIP Service
    │
    ▼
Ingress
    │
    ▼
AWS Load Balancer Controller
    │
    ▼
Application Load Balancer (ALB)
    │
    ▼
Browser
```

---

## 📂 Repository Structure

```text
app/
├── Dockerfile
├── index.html
└── style.css

kubernetes/
├── deployment.yaml
├── service.yaml
└── ingress.yaml

screenshots/
└── devops-portfolio.png

README.md
```

---

## 📸 Deployment Screenshot

![Amazon EKS Deployment](screenshots/devops-portfolio.png)

---

## 🚀 Features

- ✅ Dockerized Nginx Web Application
- ✅ Amazon ECR Image Repository
- ✅ Amazon EKS Cluster
- ✅ Kubernetes Deployment & ReplicaSet
- ✅ ClusterIP Service
- ✅ Kubernetes Ingress
- ✅ OIDC Integration
- ✅ IAM Roles for Service Accounts (IRSA)
- ✅ AWS Load Balancer Controller (Helm)
- ✅ Internet-facing Application Load Balancer (ALB)

---

## 📚 Key Concepts Implemented

- Docker Image Build & Push to Amazon ECR
- Kubernetes Deployments
- ReplicaSets & Pods
- ClusterIP Service
- Kubernetes Ingress
- Amazon EKS
- OIDC Provider
- IAM Roles for Service Accounts (IRSA)
- AWS Load Balancer Controller
- Helm Package Management
- Application Load Balancer (ALB) Integration

---

## 🎯 Learning Outcome

This project demonstrates a production-oriented deployment workflow on Amazon EKS by integrating Docker, Kubernetes, Amazon ECR, OIDC, IRSA, Helm, AWS Load Balancer Controller, and Application Load Balancer (ALB) to securely deploy and expose containerized applications.
