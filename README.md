# Local Kubernetes Cluster with Kind

**Hands-on Kubernetes learning using Kind (Kubernetes IN Docker)**

![Nginx Running](screenshots/1-nginx-welcome.png)

---

## 📋 Project Summary

Set up a complete local Kubernetes environment using **Kind** and deployed a sample Nginx web application. This project demonstrates core container orchestration concepts without needing cloud resources.

**Status**: Successfully Completed

---

## 🎯 Objectives & Achievements

- Installed and configured a local Kubernetes cluster using Kind
- Deployed a containerized application (Nginx)
- Learned key Kubernetes resources: Pods, Deployments, Services
- Accessed the application locally via port forwarding
- Understood the difference between Minikube and Kind

---

## 🛠️ Technologies Used

- **Kind** – Kubernetes IN Docker
- **kubectl** – Kubernetes CLI
- **Docker** – Container runtime
- **Nginx** – Sample web server

---

## 📸 Project Screenshots

### 1. Nginx Welcome Page
![Nginx Running](screenshots/1-nginx-welcome.png)

### 2. Kubernetes Nodes
![kubectl get nodes](screenshots/2-kubectl-nodes.png)

### 3. Pods and Services
![kubectl get all](screenshots/3-kubectl-get-all.png)

### 4. Kind Cluster Creation
![Kind Create](screenshots/4-kind-create.png)

---

## 🧩 What I Learned

- How to run Kubernetes locally without heavy VM overhead
- Basic Kubernetes workflow (`create deployment`, `expose`, `port-forward`)
- Difference between control plane and worker nodes
- Importance of port forwarding for local testing

---

## 🚀 Commands Used

```bash
kind create cluster
kubectl create deployment nginx --image=nginx
kubectl expose deployment nginx --type=NodePort --port=80
kubectl port-forward svc/nginx 8080:80
