<p align="center">
  <img src="assets/profile.png" width="140" style="border-radius:50%;" />
</p>

<h1 align="center">Fawad Ul Haq</h1>
<h3 align="center">DevOps Engineer | Cloud Infrastructure | Platform Engineering</h3>

<p align="center">
Designing scalable, secure, and highly available cloud-native systems using modern DevOps & SRE practices.
</p>

---

## 🧠 Executive Summary

DevOps Engineer specializing in cloud infrastructure automation, CI/CD pipeline engineering, and Kubernetes-based distributed systems.  
Experienced in building production-grade, observable, and fault-tolerant platforms using Infrastructure as Code and GitOps principles.

---

## 🏆 Core Expertise

- Cloud Platforms: AWS  
- Containers & Orchestration: Kubernetes, OpenShift, Docker  
- Infrastructure as Code: Terraform, Ansible  
- CI/CD: GitHub Actions, Jenkins  
- Observability: Prometheus, Grafana  
- Networking: Ingress Controllers, Service Mesh (Istio)  
- Security: JWT Authentication, Secure Deployment Pipelines  
- Architecture: Microservices, Distributed Systems  
- Practices: GitOps, SRE, High Availability, Fault Tolerance  

---

## 🚀 Featured Project — OpenShift Microservices Platform

GitHub Repository:  
https://github.com/Faddy01/openshift-microservices-platform

---

## 🏗️ System Architecture

```mermaid
flowchart LR

User[User / Client] --> Ingress[Ingress Controller]

Ingress --> Frontend[Frontend Service]
Frontend --> Backend[Backend API Service]

Backend --> Auth[JWT Authentication Layer]
Backend --> DB[(MongoDB Database)]

subgraph Kubernetes/OpenShift Cluster
Frontend
Backend
Auth
DB
Monitoring[Prometheus + Grafana]
Istio[Istio Service Mesh]
end

Ingress --> Istio
Istio --> Backend
Istio --> Frontend
