
# 🚀 Day 13 – Setting Up the DevOps Environment for a Three-Tier Application

## 📌 Project Overview

On Day 13, I prepared the DevOps environment required to deploy a three-tier application on **Amazon EKS**. The focus was on installing and configuring the essential DevOps tools that would be used in the CI/CD pipeline, GitOps deployment, code quality analysis, and monitoring.

---

## 🎯 Objectives

* Prepare the AWS environment for deployment.
* Install and configure Jenkins for Continuous Integration.
* Install and configure SonarQube for code quality analysis.
* Install and configure Argo CD for GitOps-based deployments.
* Install Prometheus for monitoring Kubernetes resources.
* Install Grafana for visualizing metrics and dashboards.
* Verify that all services were running successfully.

---

## 🛠️ Technologies Used

* AWS
* Amazon EC2
* Amazon EKS
* Docker
* Kubernetes
* Jenkins
* SonarQube
* Argo CD
* Prometheus
* Grafana
* Helm
* kubectl
* Git
* GitHub

---

## ✅ Tasks Completed

### Jenkins

* Installed Jenkins on the server.
* Accessed the Jenkins web interface.
* Verified successful installation.

### SonarQube

* Installed SonarQube.
* Accessed the SonarQube dashboard.
* Verified the server was running successfully.

### Argo CD

* Installed Argo CD in the Kubernetes cluster.
* Accessed the Argo CD web interface.
* Verified that Argo CD components were running.

### Prometheus

* Installed Prometheus using Helm.
* Verified Prometheus was collecting Kubernetes metrics.

### Grafana

* Installed Grafana using Helm.
* Logged into the Grafana dashboard.
* Verified successful integration with Prometheus.

---

## 📸 Screenshots
### IAM User
![IAM User](screenshots/iam-user.png)

### Jenkins Dashboard

![Jenkins Dashboard](screenshots/jenkins-dashboard.png)

### SonarQube Dashboard

![SonarQube Dashboard](screenshots/sonarqube-dashboard.png)

### Argo CD Login

![Argo CD Login](screenshots/argocd-login.png)

### Prometheus Dashboard

![Prometheus Dashboard](screenshots/prometheus-dashboard.png)

### Grafana Login

![Grafana Login](screenshots/grafana-login.png)

---

## 📚 Learning Outcomes

* Learned how to install and configure Jenkins for CI.
* Understood the role of SonarQube in code quality analysis.
* Configured Argo CD for GitOps-based deployments.
* Installed Prometheus for Kubernetes monitoring.
* Configured Grafana dashboards for metrics visualization.
* Gained practical experience with DevOps tools on AWS.

---

## 🚀 Next Steps

On **Day 14**, I will:

* Connect Argo CD to the GitHub repository.
* Deploy the three-tier application to Amazon EKS.
* Verify application deployment.
* Monitor the application using Prometheus and Grafana.
* Validate the complete CI/CD and GitOps workflow.
