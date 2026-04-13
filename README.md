# 🚀 Infrastructure as Code on AWS using Terraform

## 📌 Overview

This project demonstrates how to provision and manage AWS infrastructure using **Terraform** with integrated **monitoring and alerting**.

The goal is to create a **scalable, repeatable, and production-like cloud environment** using Infrastructure as Code (IaC) principles.

---

## 🏗️ Architecture

![Architecture Diagram](./assets/architecture.png)

**Key Components:**

* VPC with public/private subnets
* EC2 instances for application hosting
* Security Groups and IAM roles for secure access
* S3 bucket for storage / backend (optional)
* CloudWatch for monitoring and alerts

---

## ⚙️ Tech Stack

* **Cloud Provider:** AWS
* **IaC Tool:** Terraform
* **Monitoring:** AWS CloudWatch / Prometheus + Grafana
* **OS:** Linux (Ubuntu/Amazon Linux)
* **Optional Tools:** Ansible, Docker

---

## 📁 Project Structure

```
.
├── main.tf
├── variables.tf
├── outputs.tf
├── provider.tf
├── terraform.tfvars
├── modules/
│   ├── vpc/
│   ├── ec2/
│   └── security/
├── scripts/
│   └── install_dependencies.sh
└── assets/
    └── architecture.png
```

---

## 🚀 Getting Started

### 1️⃣ Prerequisites

* AWS Account
* Terraform installed (`>= 1.x`)
* AWS CLI configured (`aws configure`)
* SSH key pair

---

### 2️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/terraform-aws-iac.git
cd terraform-aws-iac
```

---

### 3️⃣ Initialize Terraform

```bash
terraform init
```

---

### 4️⃣ Preview Changes

```bash
terraform plan
```

---

### 5️⃣ Apply Configuration

```bash
terraform apply
```

---

### 6️⃣ Destroy Resources (Cleanup)

```bash
terraform destroy
```

---

## 🔐 Security Best Practices

* Used **IAM roles** instead of hardcoded credentials
* Applied **least privilege principle**
* Restricted access via **Security Groups**
* Sensitive variables stored securely (not committed to Git)

---

## 📊 Monitoring & Alerts

* Configured **CloudWatch metrics and alarms** for:

  * CPU utilization
  * Network traffic
  * Instance health
* Optional integration with **Grafana dashboards**
* Alerts can be sent via **SNS (email notifications)**

---

## 🌍 Features

* Infrastructure provisioning using reusable Terraform modules
* Environment consistency and reproducibility
* Scalable cloud architecture
* Monitoring and alerting for observability

---

## 🔄 Future Improvements

* Add **remote backend (S3 + DynamoDB)**
* Implement **Auto Scaling Groups**
* Add **multi-environment support (dev/staging/prod)**
* Integrate **CI/CD pipeline for Terraform deployments**
* Add **logging with ELK stack or CloudWatch Logs**

---

## 📸 Screenshots

| Terraform Apply                   | CloudWatch Dashboard                   |
| --------------------------------- | -------------------------------------- |
| ![](./assets/terraform-apply.png) | ![](./assets/cloudwatch-dashboard.png) |

---

## 🧠 Key Learnings

* Hands-on experience with Infrastructure as Code
* Deep understanding of AWS networking (VPC, subnets, routing)
* Implementing monitoring and alerting systems
* Writing modular and reusable Terraform code

---

## 🤝 Contributing

Feel free to fork this repo and submit pull requests.

---

## 📜 License

This project is licensed under the MIT License.

---

## 👤 Author

**Parthasarathy-G**

* GitHub: https://github.com/Parthasarathy-G
* LinkedIn: https://linkedin.com/in/parthasarathyg28

---
