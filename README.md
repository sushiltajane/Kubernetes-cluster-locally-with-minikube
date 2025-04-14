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

minikube start --driver=docker

### 2. Deploy Resources

kubectl apply -f deployment.yaml kubectl apply -f service.yaml

### 3. Check Deployment Status

kubectl get pods kubectl get svc

### 4. Access the Application

minikube service my-service

> This will open the Nginx app in your browser via NodePort.

---

## 🧹 Teardown

To delete the cluster and free resources:

minikube delete


---

## ✅ Requirements

- [Docker](https://www.docker.com/)  
- [Minikube](https://minikube.sigs.k8s.io/docs/start/)  
- [kubectl](https://kubernetes.io/docs/tasks/tools/)  

---

## 📸 Screenshot

![Screenshot 2025-04-14 175233](https://github.com/user-attachments/assets/12629704-1687-438b-96aa-c3c506fe4b3d)



