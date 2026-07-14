# 📖 DevOps & AWS Cloud Technical Handbook

> A comprehensive technical handbook covering **DevOps**, **AWS Cloud**, **Kubernetes**, **CI/CD**, **Infrastructure as Code (IaC)**, **Monitoring**, **Networking**, **Security**, and modern cloud-native technologies.

---

# 📚 Table of Contents

1. Messaging & Notification Services
2. Storage & Container Registries
3. Container Orchestration & Scaling
4. CI/CD Automation
5. Infrastructure as Code
6. Version Control & Security
7. Monitoring & Caching
8. Networking, Compute & Governance
9. Traffic Management & DNS

---

# 1️⃣ Messaging & Notification Services

## Amazon SQS (Simple Queue Service)

Amazon SQS is a fully managed message queuing service used to decouple distributed applications and microservices.

### Features

- Buffers requests during traffic spikes.
- Supports asynchronous communication.
- Maximum **10 messages per batch**.
- Maximum payload size: **256 KB**.
- Supports unlimited throughput for **Standard Queues**.
- FIFO queues support ordered processing with exactly-once delivery.

### Queue Types

#### Standard Queue

- At-least-once delivery
- Best effort ordering
- Nearly unlimited throughput

#### FIFO Queue

- Exactly-once processing
- Strict message ordering
- Default throughput: **300 messages/sec**

---

## Amazon SNS (Simple Notification Service)

Amazon SNS is a fully managed publish/subscribe messaging service.

### Features

- Fan-out architecture
- Push-based messaging
- Supports multiple subscribers

### Supported Subscribers

- Amazon SQS
- AWS Lambda
- HTTP / HTTPS
- Email
- SMS

---

## Amazon SES (Simple Email Service)

Cloud-based email service for sending transactional and marketing emails.

### Use Cases

- Password Reset
- OTP Emails
- Notifications
- Marketing Campaigns

---

# 2️⃣ Storage & Container Registries

## Velero

Backup and Disaster Recovery solution for Kubernetes clusters.

### Components

- Velero Server
- Velero CLI
- Backup Storage Plugins
- Volume Snapshots

---

## MinIO

High-performance S3-compatible object storage.

### Features

- 100% Amazon S3 Compatible
- Distributed Storage
- High Availability
- Object Versioning

---

## Amazon ECR (Elastic Container Registry)

Managed Docker container image registry.

### Features

- Private repositories
- Image vulnerability scanning
- Lifecycle policies
- IAM integration

---

# 3️⃣ Container Orchestration & Scaling

## Amazon ECS

AWS native container orchestration service.

### Components

- Task Definition
- Cluster
- Service
- Task
- Capacity Providers

---

## Amazon EKS

Managed Kubernetes service.

### Components

- Managed Control Plane
- Worker Nodes
- Node Groups
- Fargate Support

---

## Karpenter

High-performance Kubernetes autoscaler.

### Features

- Dynamic EC2 provisioning
- Fast scaling
- Cost optimization

---

## Podman

Daemonless container engine.

### Features

- Rootless Containers
- OCI Compatible
- Docker Compatible CLI

---

# 4️⃣ CI/CD Automation

## GitLab CI/CD

Pipeline automation built directly into GitLab.

### Components

- `.gitlab-ci.yml`
- Stages
- Jobs
- Runners

---

## Jenkins

Open-source automation server.

### Components

- Controller (Master)
- Agents
- Jenkinsfile
- Plugins
- Credentials Store

---

## AWS CodePipeline

Fully managed Continuous Delivery service.

### Stages

- Source
- Build
- Test
- Deploy

---

# 5️⃣ Infrastructure as Code

## Terraform

Declarative Infrastructure as Code tool by HashiCorp.

### Components

- Providers
- Resources
- Variables
- Modules
- State File (`terraform.tfstate`)

### Common Commands

```bash
terraform init

terraform plan

terraform apply

terraform destroy
```

---

## Ansible

Agentless configuration management tool.

### Components

- Inventory
- Playbooks
- Roles
- Handlers

### Common Commands

```bash
ansible all -m ping -i inventory.ini

ansible-playbook -i inventory.ini site.yml

ansible-galaxy collection install community.aws
```

---

# 6️⃣ Version Control & Security

## Git & GitHub

Distributed Version Control System.

### Common Commands

```bash
git init

git add .

git commit -m "Initial Commit"

git push origin main
```

---

## Trivy

Open-source vulnerability scanner.

### Scan Image

```bash
trivy image nginx
```

### Scan Configuration

```bash
trivy config .
```

---

# 7️⃣ Monitoring & Caching

## Prometheus

Time-series monitoring system.

### Features

- Pull Model
- PromQL
- AlertManager
- Exporters

---

## Grafana

Visualization platform.

### Features

- Dashboards
- Alerts
- Data Sources
- Panels

---

## Redis

In-memory database and cache.

### Data Structures

- Strings
- Lists
- Hashes
- Sets
- Sorted Sets

### Persistence

- RDB
- AOF

---

# 8️⃣ Networking, Compute & Governance

## AWS VPC

Virtual private network inside AWS.

### Components

- CIDR Block
- Subnets
- Route Tables
- Internet Gateway
- NAT Gateway
- Security Groups
- Network ACL

---

## Amazon EC2

Elastic virtual servers.

### Components

- AMI
- Instance Types
- EBS
- Elastic IP
- Key Pair

---

## AWS Lambda

Serverless compute service.

### Components

- Function
- Layers
- Triggers
- Destinations

---

## AWS IAM

Identity and Access Management.

### Components

- Users
- Groups
- Roles
- Policies

---

## Amazon RDS

Managed relational database service.

### Supported Engines

- MySQL
- PostgreSQL
- MariaDB
- Oracle
- SQL Server

---

# 9️⃣ Traffic Management & DNS

## NGINX

High-performance web server and reverse proxy.

### Components

- Master Process
- Worker Processes
- Reverse Proxy
- Load Balancer

---

## AWS Elastic Load Balancer (ELB)

Distributes incoming traffic across multiple targets.

### Types

### Application Load Balancer (ALB)

- Layer 7
- HTTP / HTTPS
- Path-based Routing
- Host-based Routing

### Network Load Balancer (NLB)

- Layer 4
- TCP / UDP
- Ultra Low Latency

### Classic Load Balancer (CLB)

- Legacy Load Balancer

---

## Amazon Route 53

Highly available DNS service.

### Components

- Hosted Zones
- Record Sets
- Health Checks

### Routing Policies

- Simple Routing
- Weighted Routing
- Latency Routing
- Failover Routing
- Geolocation Routing
- Geoproximity Routing
- Multi-Value Routing

---
# 🛠️ Technologies Covered

- AWS Cloud
- Kubernetes
- Docker
- Podman
- ECS
- EKS
- Terraform
- Ansible
- Git
- GitHub
- Jenkins
- GitLab CI/CD
- AWS CodePipeline
- Prometheus
- Grafana
- Redis
- Trivy
- NGINX
- Route 53
- ELB
- EC2
- Lambda
- IAM
- RDS
- SQS
- SNS
- SES
- MinIO
- Velero
- Amazon ECR

---
---

# 📄 License

MIT License

Copyright (c) 2026 Abhishek Singh Parihar

This project is licensed under the **MIT License**.

# 📄 Copyright & Usage

**Copyright © 2026 Abhishek Singh Parihar. All Rights Reserved.**

This repository contains educational documentation and PDF materials related to **DevOps & AWS Cloud**.

## 📚 Learning & Educational Purpose

This handbook is provided **free of charge** for **learning, educational, and personal reference purposes**.

### ✅ You are allowed to:

- Download the PDF.
- Read and study the content.
- Use it for personal learning and educational purposes.
- Share the GitHub repository link with others.

### ❌ You are NOT allowed to:

- Copy, reproduce, or republish the PDF or documentation as your own work.
- Modify the content and redistribute it under your own name.
- Sell or use this material for commercial purposes without the author's permission.
- Misuse the content in any way, including plagiarism or unauthorized redistribution.

By using this repository, you agree to respect the author's work and use these materials responsibly.

For permissions beyond personal learning or educational use, please contact the author.

**Author:** Abhishek Singh Parihar
