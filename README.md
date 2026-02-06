🌐 Scalable Cloud-Based Web Application on AWS
📌 Project Description

This project demonstrates a production-grade AWS cloud architecture for a scalable, highly available, and secure web application. It is designed using AWS best practices and core DevOps principles such as automation, fault tolerance, security, and scalability.

The architecture uses Auto Scaling, Application Load Balancer, custom AMIs, IAM roles, RDS, and S3 to simulate a real enterprise deployment.

🏗️ Architecture Overview

The application is deployed inside a custom VPC (devops-vpc) spanning multiple Availability Zones to ensure high availability.

Key Flow:
User → Application Load Balancer → EC2 Auto Scaling Group → RDS (MySQL)
                               → Amazon S3 (via IAM Role)

🚀 AWS Services Used

Amazon VPC – Custom networking with public & private subnets

Application Load Balancer (ALB) – Traffic distribution & health checks

Auto Scaling Group (ASG) – Self-healing and scaling

Amazon EC2 – Web servers using custom AMI

Launch Templates – Immutable infrastructure

Amazon RDS (MySQL) – Private database layer

Amazon S3 – Secure object storage

IAM Roles – Credential-less secure access

Security Groups – Controlled traffic flow

🔐 Security Best Practices Implemented

No hard-coded AWS credentials

IAM Role-based access for EC2 → S3

RDS deployed in private subnets (no public access)

Security Group to Security Group communication

IMDSv2 enforced on EC2

Encrypted S3 bucket with versioning enabled

⚙️ Automation & Reliability

Auto Scaling replaces unhealthy EC2 instances automatically

ALB performs health checks

Launch Templates ensure consistent instance configuration

Custom AMI enables fast, repeatable deployments

🧪 Verified Functionality

Auto Scaling launches instances across AZs

EC2 instances serve traffic via ALB

EC2 uploads files to S3 using IAM Role (no access keys)

Database accessible only from application layer
