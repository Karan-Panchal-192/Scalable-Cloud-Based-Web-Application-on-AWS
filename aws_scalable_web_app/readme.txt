# 🚀 Scalable AWS DevOps Web Application

## 📌 Overview
Designed and deployed a production-style, scalable, and secure web application on AWS using core DevOps and cloud services.

The system is fault-tolerant, auto-healing, monitored, and cost-optimized.

---

## 🏗️ Architecture
**Internet → Route 53 → ALB → Auto Scaling EC2 → RDS (Private Subnet)**

- Multi-AZ deployment
- Private database layer
- Monitoring and alerting enabled

---

## 🧰 AWS Services Used
- EC2
- Auto Scaling Group
- Application Load Balancer
- VPC (Public & Private Subnets)
- RDS (MySQL)
- S3 (Versioning + Lifecycle)
- IAM
- CloudWatch
- SNS

---

## ⚙️ Key Features
- Auto-healing infrastructure
- CPU-based auto scaling
- Private RDS with security-group access
- Email alerts on failures
- Secure S3 storage with lifecycle rules

---

## 🧪 Validation
- Verified EC2 → RDS private connectivity using MySQL client
- Tested auto-healing by terminating instances
- Triggered CloudWatch alarms via CPU stress

---

## 📸 Screenshots
(See `/screenshots` folder)

---

## 📚 What I Learned
- Designing production AWS architecture
- Networking & security best practices
- Monitoring and alerting in DevOps
- Cost-aware cloud design
