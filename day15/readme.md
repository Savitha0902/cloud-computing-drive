
# Day 15 – Three-Tier Application Deployment on AWS using DevOps Tools

## Overview

On Day 15, I completed the documentation of my end-to-end Three-Tier Application deployment on AWS. This project demonstrates a production-style DevOps workflow using Infrastructure as Code, CI/CD, Kubernetes, GitOps, containerization, monitoring, and security tools.

The deployment automates infrastructure provisioning, application build and deployment, monitoring, and continuous delivery using modern DevOps practices.

---

## Technologies Used

* AWS IAM
* Terraform
* AWS CLI
* Amazon EC2
* Jenkins
* Docker
* Docker Compose
* SonarQube
* Trivy
* Amazon ECR
* Amazon EKS
* Kubernetes
* Helm
* Prometheus
* Grafana
* Argo CD
* Cloudflare DNS
* Persistent Volumes (PV)
* Persistent Volume Claims (PVC)
* Git & GitHub

---

## Project Workflow

### 1. IAM User Setup

Created an IAM user with the required permissions for:

* Amazon EC2
* Amazon EKS
* Amazon ECR
* Amazon S3
* DynamoDB

---

### 2. Terraform & AWS CLI Installation

* Installed Terraform
* Installed AWS CLI
* Configured AWS CLI using IAM credentials

---

### 3. Remote Terraform Backend

Created:

* S3 Bucket for Terraform state storage
* DynamoDB Table for Terraform state locking

---

### 4. Infrastructure Provisioning

Provisioned the Jenkins EC2 instance using Terraform.

---

### 5. Jenkins Server Configuration

Installed and configured:

* Jenkins
* Docker
* Docker Compose
* Terraform
* Kubectl
* AWS CLI
* Trivy
* SonarQube

---

### 6. Jenkins Plugins

Configured the required plugins:

* AWS Credentials
* AWS Steps
* Docker
* Docker Pipeline
* Eclipse Temurin Installer
* NodeJS
* OWASP Dependency Check
* SonarQube Scanner

---

### 7. SonarQube Integration

Integrated SonarQube into the Jenkins pipeline for static code analysis and code quality checks.

---

### 8. Amazon ECR

Created separate repositories for:

* Frontend Docker Image
* Backend Docker Image

Configured Jenkins to build Docker images and push them to Amazon ECR.

---

### 9. Amazon EKS Deployment

Provisioned the Kubernetes cluster using Terraform, including:

* VPC
* Public and Private Subnets
* Internet Gateway
* Security Groups
* IAM Roles
* Worker Nodes

---

### 10. Monitoring Setup

Installed Prometheus and Grafana using Helm for:

* Cluster Monitoring
* Pod Monitoring
* Resource Usage
* Dashboard Visualization

---

### 11. Jenkins CI/CD Pipeline

Created separate pipelines for Frontend and Backend.

Pipeline stages included:

* Source Code Checkout
* Dependency Installation
* Build
* SonarQube Analysis
* Dependency Check
* Trivy Scan
* Docker Build
* Push Image to Amazon ECR
* Update Kubernetes Manifests
* Trigger GitOps Deployment

---

### 12. GitOps with Argo CD

Installed Argo CD on the EKS cluster.

Configured automatic synchronization between GitHub and Kubernetes to deploy application updates.

---

### 13. DNS Configuration

Configured Cloudflare DNS to expose the application through a custom subdomain pointing to the Kubernetes Load Balancer.

---

### 14. Persistent Storage

Configured:

* Persistent Volumes (PV)
* Persistent Volume Claims (PVC)

to provide persistent storage for the database.

---

### 15. Final Validation

Verified:

* Infrastructure provisioning
* CI/CD pipeline execution
* Docker image creation
* ECR image push
* Kubernetes deployment
* Argo CD synchronization
* Prometheus monitoring
* Grafana dashboards
* Application accessibility

---


ion on Amazon EKS using Terraform, Jenkins, Docker, SonarQube, Trivy, Amazon ECR, Argo CD, Prometheus, Grafana, and Cloudflare with an automated CI/CD and GitOps workflow.
