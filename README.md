# 🐳 Basic Pod Deployment (Minikube)

A minimal Kubernetes project showcasing how to define and deploy a single pod using **Minikube**. This example is ideal for beginners who want to understand how pod specifications work at the most fundamental level.

---

## 📌 Project Overview

* **Name**: basic-pod-minikube
* **Stack**: Kubernetes YAML, Minikube
* **Goal**: Deploy a standalone pod in a local Kubernetes cluster
* **Use Case**: Introductory DevOps or Kubernetes lab exercise

---

## 📁 Project Structure

```
├── pod.yaml        # YAML manifest defining a single nginx pod
```

---

## 🚀 Getting Started

### Prerequisites

* [Minikube](https://minikube.sigs.k8s.io/docs/start/)
* [kubectl](https://kubernetes.io/docs/tasks/tools/)

### Installation Steps

```bash
# 1. Start Minikube
minikube start

# 2. Apply the pod definition
kubectl apply -f pod.yaml

# 3. Check that the pod is running
kubectl get pods

# 4. Optional: Describe the pod to inspect configuration
kubectl describe pod nginx

# 5. Optional: Access pod logs
kubectl logs nginx
```

---

## 📦 Technologies Used

* **Kubernetes** – Container orchestration
* **Minikube** – Local development cluster
* **YAML** – Declarative syntax for infrastructure as code

---

## 🧪 Testing and Coverage

> Manual validation using `kubectl` CLI to check pod status, logs, and descriptions.

---

## 🧠 Key Challenges & Learnings

* Learned how to define a `Pod` spec with custom labels and container settings
* Understood lifecycle and status transitions (Pending → Running)
* Practiced inspecting logs and resource descriptions for debugging

---

## 📷 Screenshots or Live Demo

> Sample CLI output:

```bash
kubectl get pods
NAME    READY   STATUS    RESTARTS   AGE
nginx   1/1     Running   0          15s
```

---

## 📜 License

[MIT](https://opensource.org/licenses/MIT)

---

> Developed by [David Hernández](https://github.com/davidhernandez-adm) as a starting point for Kubernetes pod experimentation.
