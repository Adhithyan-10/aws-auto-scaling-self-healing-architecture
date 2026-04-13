## 📄 Documentation

This folder contains detailed documentation of a production-style AWS architecture built using an Application Load Balancer (ALB) and Auto Scaling Group (ASG).

The project demonstrates how modern cloud systems are designed to achieve high availability, fault tolerance, and self-healing capabilities.

---

### 📑 View Full Documentation

[Open Project Documentation](./project-documentation.pdf)

---

### 📌 Overview

This project extends a basic ALB + EC2 setup by introducing Auto Scaling to create a dynamic and resilient infrastructure.

User requests are routed through an internet-facing Application Load Balancer, which distributes traffic across EC2 instances managed by an Auto Scaling Group. These instances are deployed across multiple Availability Zones to eliminate single points of failure.

The Auto Scaling Group continuously monitors instance health and automatically replaces unhealthy instances, ensuring uninterrupted service.

---

### ⚙️ What This Documentation Covers

* Architecture design and end-to-end request flow
* Launch Template configuration and EC2 automation using user data
* Auto Scaling Group setup with self-healing behavior
* Application Load Balancer and Target Group configuration
* Health checks and traffic routing mechanisms

---

### 💡 Key Highlights

* High availability using **Multi-AZ deployment**
* Self-healing infrastructure using **Auto Scaling**
* Intelligent traffic distribution using **Application Load Balancer**
* Automated EC2 provisioning using **Launch Templates**
* Reliable request routing using **Target Group health checks**

---

### 🔥 Core Concepts Demonstrated

* Auto Scaling maintains desired capacity automatically
* EC2 instances are **disposable and automatically replaced**
* Target Group acts as a bridge between ALB and backend instances
* Health checks control which instances receive traffic
* Security Groups enforce **least privilege access (ALB → EC2 only)**

---

### 🎯 Interview Insight

> “This project showcases how production-grade cloud architectures achieve high availability and fault tolerance by combining load balancing with automated scaling and recovery mechanisms.”

---

### 🚀 Note

> Complete implementation steps, screenshots, and architecture details are included in the full documentation PDF.
