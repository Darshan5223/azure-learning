# AZ-104 Lab 09b – Implement Azure Container Instances (ACI)

## 📌 Lab Objective
Understand how to deploy and validate a containerized web application using **Azure Container Instances**, a serverless container platform that removes infrastructure management.

---

## 🧠 Core Concepts Explained

### 🔹 What is a Container?
A container packages:
- Application code
- Runtime
- Dependencies  
into a lightweight, isolated unit.

Unlike VMs, containers **share the host OS kernel**, making them faster and cheaper.

---

### 🔹 What is Azure Container Instances (ACI)?
ACI allows you to:
- Run containers directly in Azure
- Without VMs
- Without Kubernetes
- Without cluster management

It is **serverless compute for containers**.

---

## 🛠️ Task Breakdown

### ✅ Task 1: Deploy Azure Container Instance

**Steps Performed**
1. Created a Container Instance
2. Selected **Quickstart Image**
3. Used Docker image: mcr.microsoft.com/azuredocs/aci-helloworld:latest
4. Configured:
- Linux container
- Public DNS name
- Port 80
5. Disabled container logs for simplicity

**Result**
- Container deployed in ~2 minutes
- No VM, OS, or infrastructure configuration required

---
### ✅ Task 2: Test & Verify Container

**Verification Steps**
- Checked container status → **Running**
- Accessed application using: http://<dns-name>.<region>.azurecontainer.io

- Verified **“Welcome to Azure Container Instance”**
- Viewed HTTP logs from: Container Instance → Containers → Logs



---

## 📌 Key Takeaways

- ACI is best for:
- Short-lived workloads
- Stateless applications
- Dev/Test
- CI/CD jobs
- No autoscaling or orchestration
- Pay only for:
- CPU seconds
- Memory used

---

## 🧪 Interview Questions & Answers

**Q1: When should I choose ACI over AKS?**  
Use ACI when you don’t need orchestration, scaling, or microservices.

---

**Q2: Is ACI suitable for production?**  
Yes, for small, stateless, low-traffic applications.

---

**Q3: Does ACI support persistent storage?**  
Limited support using Azure Files.

---

**Q4: How is ACI billed?**  
Per second, based on CPU and memory usage.

---

## 🧹 Cleanup Strategy
Deleted the resource group after lab completion to avoid costs.

---

## 🎯 AZ-104 Exam Tip
If the question says:
- **“Run a container quickly”**
- **“No infrastructure management”**
- **“No Kubernetes”**

👉 Answer is **Azure Container Instances**


