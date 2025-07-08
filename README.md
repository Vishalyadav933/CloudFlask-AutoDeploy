# 🚀 CloudFlask-AutoDeploy

A **DevOps CI/CD project** by **Vishal Yadav**, demonstrating **automated deployment of a Flask app on AWS EC2 using Docker, Terraform, GitHub Actions, and GHCR**.

---

## 👤 Author

- **Name:** Vishal Yadav
- **Phone:** 7841048227
- **Email:** devops.vishal8227@gmail.com
- [GitHub](https://github.com/Vishalyadav933)

---

## 📌 Project Objective

Deploy a **Flask app on AWS EC2 with automated CI/CD pipelines** to learn and practice **real-world DevOps workflows**.

---

## 🚀 Tech Stack

- **AWS EC2** – Cloud hosting
- **Terraform** – Infrastructure as Code
- **Docker & Docker Compose** – Containerization
- **GitHub Actions** – CI/CD pipeline automation
- **GHCR** – GitHub Container Registry
- **Flask** – Python micro web framework

---

## 🛠️ Step-by-Step Workflow

### ✅ 3️⃣ Docker Compose

**Why?** Simplifies running and managing containers, allows scaling later, and follows DevOps best practices.

Created `docker-compose.yml`:
```yaml
version: '3'
services:
  flaskapp:
    build: .
    ports:
      - "5000:5000"

#Run locally:

docker compose up -d

## Terraform Provisioning on AWS
**Provision EC2 instance and security groups using:**

main.tf

variables.tf

outputs.tf

**Commands**

terraform init
terraform apply
## Docker Setup on EC2
SSH into EC2:

ssh -i nv-key.pem ubuntu@<EC2-PUBLIC-IP>


## Install Docker:

sudo apt update
sudo apt install docker.io -y
sudo systemctl enable docker
sudo systemctl start docker


## Git & GitHub Integration
Pushed project to:

https://github.com/Vishalyadav933/CloudFlask-AutoDeploy

**Commands:**

git init
git remote add origin <repo-url>
git add .
git commit -m "Initial commit"
git push -u origin main 


## GitHub Actions CI/CD Pipeline
Added .github/workflows/deploy.yml to automate:

Build Docker image

Push to GHCR

SSH into EC2

Pull and restart container automatically

## Verification
**Access your deployed Flask app:**

http://<EC2-PUBLIC-IP>:5000
to verify automated CI/CD deployment


# Project Structure
CloudFlask-AutoDeploy/
│
├── app/                       # Flask app with Docker
│   ├── app.py
│   ├── requirements.txt
│   ├── Dockerfile
│   └── docker-compose.yml     # ✅ 3️⃣ Docker Compose
│
├── terraform/                 # ✅ 4️⃣ Terraform AWS Provisioning
│   ├── main.tf
│   ├── variables.tf
│   ├── outputs.tf
│
└── .github/
    └── workflows/
        └── deploy.yml         # ✅ 7️⃣ GitHub Actions CI/CD Pipeline


## Features
CI/CD pipeline for Flask app on AWS EC2

Infrastructure management with Terraform

Containerization with Docker & Docker Compose

Automated deployment with GitHub Actions + GHCR

Clean, repeatable DevOps workflow


## Licine
This project is created for learning, DevOps practice, and portfolio building.


## Push to GitHub:
After adding this file:

git add README.md
git commit -m "Add final structured README with workflow and features"
git push origin main
