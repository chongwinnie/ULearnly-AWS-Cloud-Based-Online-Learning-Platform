# ☁️ ULearnly: AWS Cloud-Based Online Learning Platform
A scalable, secure, and high-availability **cloud architecture** hosted on **AWS**, designed to support an online learning platform. Built using AWS EC2, ELB, RDS, EFS, VPC, and Auto Scaling for performance, security, and cost efficiency.

---

## 📦 Project Deliverables
- 📦 [`moodle.zip`](https://github.com/QiYang102/ULearnly-AWS-Cloud-Based-Online-Learning-Platform/releases/latest) — Moodle deployment package (download from GitHub Release)
- 📄 `G10_AWS_Architecture_Report.docx` — Full technical documentation
- 🖼️ `solution-architecture.png` — Final AWS infrastructure diagram

---

## 📦 moodle.zip Contents

This file contains the complete Moodle website project setup.
moodle.zip
- ├── moodle/ # Moodle website folder (code, config, themes, plugins)
- └── rds_moodle_backup.sql # Moodle MySQL database export (from AWS RDS)

---
## 🧱 AWS Services Used

| Category           | AWS Services                                           |
|--------------------|--------------------------------------------------------|
| Compute            | EC2, Auto Scaling                                      |
| Database           | RDS (Aurora MySQL)                                     |
| Storage            | EFS                                                    |
| Networking         | VPC, NAT Gateway, Security Groups, ELB                 |
| DevOps             | AMI, SSH Key Pairs                                     |
| Monitoring         | CloudWatch (optional), Health Checks                   |
| Security & Access  | IAM, Security Groups, VPC Firewall Rules               |

---

## 🖥️ Architecture Overview

The project hosts a Moodle-based online learning platform. It features:

- **EC2 instances (Web, App, Admin)** deployed across 2 AZs
- **Elastic Load Balancer (ELB)** distributes HTTP traffic
- **Amazon Aurora RDS** for backend database
- **Amazon EFS** for shared Moodle file storage
- **Auto Scaling Group** for high availability
- **Custom VPC** with public/private subnets and NAT Gateway

![Architecture Diagram](solution-architecture.png)

---

## 🧪 How to Run Locally with XAMPP

1. **Extract `moodle.zip`**  
   Unzip it to get the `moodle/` folder and `rds_moodle_backup.sql`.

2. **Move `moodle/` into your XAMPP htdocs directory**

3. **Start XAMPP Control Panel**
- Start **Apache**
- Start **MySQL**

4. **Import the database**
- Go to: `http://localhost/phpmyadmin`
- Create a new database (e.g., `moodle-databse`)
- Click on the new DB → Click **Import**
- Select `rds_moodle_backup.sql`
- Click **Go**

5. **Access Moodle via browser**


✅ Once setup is done, you’ll have a fully functional local Moodle site running from your `moodle/` folder and connected to your restored database.

---

## 🎬 Project Demo

Watch the demonstration of **ULearnly: AWS Cloud-Based Online Learning Platform**.
▶️ **[Watch the Full Project Demo on YouTube](https://youtu.be/VnRl-CAEutY)**


