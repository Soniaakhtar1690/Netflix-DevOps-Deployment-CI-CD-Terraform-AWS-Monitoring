<img width="1536" height="1024" alt="0093f85d-e162-4dd1-8b0e-8b89eb9e556e" src="https://github.com/user-attachments/assets/80d10fb7-0c07-4470-9ce9-07a06ad0d2e6" /># 🚀 Netflix DevOps Deployment – CI/CD, Terraform, AWS, Monitoring

This repository showcases a **hands-on DevOps project** that simulates a real-world deployment workflow by deploying a Netflix clone application with **automated CI/CD pipelines**, **infrastructure as code**, and **monitoring/observability** on AWS.

---

## 🔹 Project Overview

- **AWS Organization Setup** – Multi-service foundation for deployment  
- **Infrastructure Provisioning (Terraform via HCP)** – Provisioned 4 servers:  
  - Jenkins (CI/CD)  
  - Prometheus + Grafana (Monitoring stack)  
  - 2 Tomcat + Node Exporter servers (Application + Metrics)  
- **CI/CD Pipeline in Jenkins**  
  - Pulled the Netflix app source code from GitHub  
  - Built & tested with Maven  
  - Packaged WAR artifact and stored in an **S3 bucket**  
- **Automated Deployment**  
  - Jenkins pipeline deployed the Netflix app onto Tomcat servers  
- **Monitoring & Observability**  
  - Node Exporter + Prometheus for system metrics  
  - Grafana dashboards for real-time visualization  

✨ **Outcome:** A fully automated Netflix deployment pipeline with monitoring and alerting on AWS.

---

## 🏗️ Architecture

![Architecture] [Uploading 0093f85d-e162-4dd1-8b0e-8b89eb9e556e.png…]


---

## ⚙️ Tech Stack

- **AWS (EC2, S3, IAM, VPC)**  
- **Terraform (IaC via HCP)**  
- **Jenkins (CI/CD)**  
- **Tomcat (App Server)**  
- **Maven (Build tool)**  
- **Prometheus + Grafana (Monitoring & Observability)**  
- **Node Exporter (Metrics Collection)**  

---

## 📌 Key Features

✔ Infrastructure as Code (IaC) with Terraform  
✔ End-to-End CI/CD pipeline using Jenkins  
✔ Netflix app deployment on Tomcat  
✔ Artifact storage on AWS S3  
✔ System metrics collection with Prometheus  
✔ Real-time dashboards with Grafana  

---

## 🚀 Setup Instructions

### 1. Clone this Repository
```bash
git clone https://github.com/your-username/netflix-devops-deployment.git
cd netflix-devops-deployment
2. Provision Infrastructure with Terraform
bash
Copy code
cd terraform
terraform init
terraform apply
3. Configure Jenkins
Install required plugins: Git, Maven, Pipeline, AWS CLI

Create a pipeline using the provided Jenkinsfile

4. Deploy Netflix App
Jenkins pipeline builds the WAR and pushes to S3

WAR file gets deployed automatically on Tomcat servers

5. Setup Monitoring
Start Prometheus with prometheus.yml

Import Grafana dashboard from grafana-dashboards.json

📊 Monitoring Example

Prometheus: http://<prometheus-server>:9090
Grafana: http://<grafana-server>:3000

📷 Screenshots
✅ Jenkins pipeline execution
🎬 Netflix app running on Tomcat
📈 Grafana dashboards with metrics
[1756962902048](https://github.com/user-attachments/assets/e2b6211a-a60f-4496-818c-64203fff28d6)
[1756962903707](https://github.com/user-attachments/assets/d596212a-5585-4421-948e-f26f6d744ee2)
[1756962901785](https://github.com/user-attachments/assets/76e4b43a-e4f9-4b92-989a-e01f57d98562)
[1756962902305](https://github.com/user-attachments/assets/38e6afcc-a645-4f8a-b78b-b0075f336e53)
[1756962901826](https://github.com/user-attachments/assets/07282828-6415-4b06-9798-c5711f45f086)
[1756962903078](https://github.com/user-attachments/assets/a40b0a47-b99e-4cfe-b1aa-a534ad0ded93)
[1756962903707 (1)](https://github.com/user-attachments/assets/4301e866-cba3-417c-8db2-23f0df44a486)
[1756962902077](https://github.com/user-attachments/assets/b022459d-6b36-4202-8d49-0c40ae0c8ccb)


📚 Learnings

-->Infrastructure as Code (IaC)
-->CI/CD Automation
-->Application Deployment Strategies
-->Monitoring & Observability

🏁 Outcome
A production-like DevOps workflow that automates Netflix application deployment, integrates monitoring/alerting, and runs on AWS infrastructure.
![1756962905474](https://github.com/user-attachments/assets/0514f133-c17c-4815-836a-81bd48f925bb)


Author Sonia Akhtar
