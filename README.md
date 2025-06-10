# DevOps CI/CD Automation Pipeline

This project demonstrates a complete CI/CD pipeline for a containerized web application using industry-standard DevOps tools.

## Tech Stack

- **Source Control:** GitHub
- **CI Server:** Jenkins
- **Containerization:** Docker
- **Container Orchestration:** Kubernetes (Minikube)
- **Package Management:** Helm
- **Registry:** Docker Hub 
- **App Language:** Python (Flask)
- **Cloud hosting:** AWS

## Objective

> Automate the build, test, containerization, and deployment of a web application using a reliable CI/CD pipeline.

## Features

- Automated unit testing on each commit
- Docker image build and push to registry
- Kubernetes deployment using Helm
- Manual approval stage for production deployment
- Clean rollback mechanism
- GitHub Actions or Jenkins integration
- Deployment status validation


##  CI/CD Pipeline Overview

1. **Code Commit** ➜ Triggers CI
2. **Unit Tests** ➜ Run automatically
3. **Build Docker Image**
4. **Push Image to Registry**
5. **Deploy via Helm to Minikube**
6. **Manual Approval for Production**
7. **Monitor Rollout Status**

##  How to Run Locally

### Prerequisites

- Docker
- Minikube
- Helm
- Jenkins ( containerized)
- Python for the app

### Steps

```bash
# Clone the repository
git clone https://github.com/your-username/devops-cicd-automation-pipeline.git
cd devops-cicd-automation-pipeline

# Build Docker image
docker build -t yourusername/myapp .

# Push to Docker Hub (after login)
docker push yourusername/myapp

# Start Minikube
minikube start

# Deploy using Helm
helm install myapp ./helm/myapp

# Check rollout status
kubectl get pods



