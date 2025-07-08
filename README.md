# CloudFlask-AutoDeploy 🚀

A **DevOps CI/CD project** by **Vishal Yadav**, demonstrating **automated deployment of a Flask app on AWS EC2 using Docker, Terraform, GitHub Actions, and GHCR**.

---

##  Author
- **Name:** Vishal Yadav
- **Phone:** 7841048227
- **Email:** devops.vishal8227@gmail.com
- [GitHub](https://github.com/Vishalyadav933)

---

## 📌 Project Objective

To **learn and practice real-world DevOps** by:
✅ Building a Python Flask app.  
✅ Provisioning AWS EC2 using Terraform.  
✅ Containerizing with Docker & Docker Compose.  
✅ Automating deployments using GitHub Actions and GHCR.

---

## 🚀 Tech Stack

✅ AWS EC2 – Cloud hosting  
✅ Terraform – Infrastructure as Code (IaC)  
✅ Docker & Docker Compose – Containerization  
✅ GitHub Actions – CI/CD pipelines  
✅ GitHub Container Registry (GHCR) – Image registry  
✅ Flask – Python micro web framework

---

## 🛠️ Step-by-Step Implementation

### ✅ 1️⃣ Created Flask Application
- Developed `app/app.py` displaying “Hello, DevOps-Flask-Demo!”.
- Added `requirements.txt` for dependencies.

### ✅ 2️⃣ Containerized with Docker
- Wrote `Dockerfile` for Flask app.
- Built and tested locally using:
  ```bash
  docker build -t flaskapp .
  docker run -p 5000:5000 flaskapp

#Added Docker Compose

Created docker-compose.yml for simplified deployment.

Provisioned AWS EC2 with Terraform

Wrote terraform/main.tf, variables.tf, outputs.tf.

#Ran:


terraform init
terraform apply

Installed Docker on EC2

SSH into EC2:

ssh -i nv-key.pem ubuntu@<EC2-PUBLIC-IP>


#Installed Docker:

sudo apt update
sudo apt install docker.io -y
sudo systemctl enable docker
sudo systemctl start docker

#Configured Git & GitHub

git init
git remote add origin https://github.com/Vishalyadav933/CloudFlask-AutoDeploy.git    # Committed and pushed code.

#Set Up GitHub Actions CI/CD

Created .github/workflows/deploy.yml:

 #On push to main:

Builds Docker image.

Pushes to GHCR.

SSH into EC2.

Pulls latest image and restarts using Docker Compose.

Verified Deployment: http://<EC2-PUBLIC-IP>:5000



#Project Structure:

CloudFlask-AutoDeploy/
│
├── app/
│   ├── app.py
│   ├── requirements.txt
│   ├── Dockerfile
│   └── docker-compose.yml
│
├── terraform/
│   ├── main.tf
│   ├── variables.tf
│   ├── outputs.tf
│
└── .github/
    └── workflows/
        └── deploy.yml


#Features:

✅ End-to-end CI/CD pipeline for Flask app.
✅ Containerized deployment ensuring consistency.
✅ Infrastructure as Code for AWS provisioning.
✅ Uses free, industry-standard DevOps tools.
✅ Suitable for resume and LinkedIn portfolio projects.

What i learned:

✅ Hands-on AWS provisioning with Terraform.
✅ Docker image building and management.
✅ Configuring CI/CD using GitHub Actions.
✅ Managing cloud permissions, SSH keys, and deployments.
✅ Debugging real-world deployment issues.


#License:

This project is for learning, practice, and portfolio building only by Vishal Yadav.
