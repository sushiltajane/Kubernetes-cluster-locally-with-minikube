# Kubernetes-cluster-locally-with-minikube
# Kubernetes Deployment Example

This repository demonstrates a basic Kubernetes setup using **Minikube** to deploy an Nginx web application with a NodePort service.

## 🚀 Task Overview

- Create `deployment.yaml` to deploy an Nginx container
- Create `service.yaml` to expose the app via a NodePort
- Deploy everything using `kubectl` on a Minikube cluster
- Verified service accessibility through Minikube

---

## 📁 Files

- `deployment.yaml` – Kubernetes deployment for Nginx
- `service.yaml` – Kubernetes service of type NodePort

---

## 🛠️ Setup Instructions

### 1. Start Minikube

```bash
minikube start --driver=docker
2. Deploy Resources
bash
Copy
Edit
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
3. Check Deployment Status
bash
Copy
Edit
kubectl get pods
kubectl get svc
4. Access the Application
bash
Copy
Edit
minikube service my-service
This will open the app in your browser via NodePort.

🧹 Teardown
To stop and delete the cluster:

bash
Copy
Edit
minikube delete
✅ Requirements
Docker

Minikube

kubectl
