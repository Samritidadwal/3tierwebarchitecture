# 3tierwebarchitecture
 
# 🌐 Three-Tier Web Architecture on AWS

## 📘 Overview

This project demonstrates a **Three-Tier Web Application Architecture** deployed on **AWS Cloud**, designed for scalability, modularity, and security. The architecture separates the presentation, application logic, and data layers to ensure maintainability and performance.

## 🏗️ Architecture Diagram

```
[Client (Browser)]
        |
     [Route 53 / CloudFront]
        |
     [External ALB (Application Load Balancer)]
        |
     [Web Tier: EC2 or Lambda (Nginx/React)]
        |
     [Internal ALB (Application Load Balancer)]
        |
     [App Tier: EC2 or Lambda (Node.js/Python)]
        |
     [DB Tier: RDS (MySQL/PostgreSQL) or DynamoDB]
 

## 🔧 Technologies Used

### ☁️ AWS Services:
- **EC2** – Hosts web and app servers
- **RDS / DynamoDB** – Database layer for storing application data
- **S3** – For static assets (if any)
- **Elastic Load Balancer (ALB)** – Distributes traffic across web/app tier
- **VPC** – With public and private subnets
- **Security Groups & IAM** – Secure access and role-based permissions
- **CloudWatch** – Logging and monitoring
- **Auto Scaling Groups** – High availability

### 🛠️ Application Stack:
- **Frontend**: HTML, CSS, JS / React
- **Backend**: Node.js / Python (Flask or Django)
- **Database**: MySQL / PostgreSQL / DynamoDB

---

## 🚀 Features

- 📦 Modular architecture with clear separation of concerns
- 🔒 Secure environment with VPC isolation and IAM roles
- 📈 Auto-scaling and fault-tolerant setup
- 🔄 CI/CD Integration with GitHub Actions / CodePipeline (optional)
- 🧠 Scalable backend with optional ML integration

---

## ⚙️ Deployment Options

### 🧑‍💻 Manual Deployment:
- Launch EC2 instances via AWS Console
- Configure Load Balancer and Target Groups
- Connect backend to RDS / DynamoDB
- Use SSH / SCP to deploy application files

### 📦 Infrastructure as Code (Recommended):
- Terraform / CloudFormation templates provided
- Easily reproducible and version-controlled
- Just run:
  ```bash
  terraform init
  terraform apply
  ```

---

## 📂 Folder Structure (Example)
```
/three-tier-architecture
│
├── terraform/                # IaC scripts
├── web-tier/                 # Frontend code
├── app-tier/                 # Backend logic (API/Business Logic)
├── db-scripts/               # DB schema, seed scripts
├── assets/                   # Diagrams or static files
├── README.md                 # You're here!
```

## 📊 Monitoring & Logging

- Application logs: CloudWatch
- Metrics: CPU, Memory, Request Count
- Alerts: Configurable via SNS/CloudWatch

---

## 👩‍💻 Author

**Samriti Dadwal**  
Cloud Solution Architect | AWS Certified | DevOps & Serverless Specialist  
📧 [dadwalsamrititech@gmail.com](mailto:dadwalsamrititech@gmail.com)  
🔗 [LinkedIn](https://linkedin.com/in/samriti-dadwal-78354026a)

---

## 📝 License

This project is open-source under the MIT License.
