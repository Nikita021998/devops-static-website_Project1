# AWS DevOps CI/CD Portfolio Project 🚀

## Overview

This project demonstrates an end-to-end CI/CD deployment pipeline for a static portfolio website using AWS and DevOps tools.

The application source code is managed using GitHub and automatically deployed through Jenkins CI/CD pipeline. The application is containerized using Docker and hosted on an AWS EC2 instance with Nginx as the web server.

---

# Architecture

```
Developer
    |
    |
    v
GitHub Repository
    |
    |
    v
Jenkins CI/CD Pipeline
    |
    |
    v
Docker Image Build
    |
    |
    v
Docker Container
    |
    |
    v
AWS EC2 Instance
    |
    |
    v
Nginx Web Server
    |
    |
    v
Live Website
```

---

# Technologies Used

| Technology | Purpose |
|------------|---------|
| AWS EC2 | Cloud infrastructure for hosting application |
| Ubuntu Linux | Server operating system |
| GitHub | Source code management |
| Jenkins | CI/CD pipeline automation |
| Docker | Application containerization |
| Nginx | Web server |
| Shell Script | Server automation |

---

# Project Workflow

## 1. Source Code Management

- Created a static portfolio website using HTML and CSS.
- Managed source code using Git and GitHub repository.

## 2. CI/CD Pipeline

Jenkins automates the deployment process:

1. Developer pushes code changes to GitHub.
2. Jenkins automatically fetches the latest source code.
3. Docker image is created.
4. Docker container is deployed.
5. Nginx serves the application.
6. Updated changes become available on the live website.

---

# Project Structure

```
AWS-DevOps-Portfolio-Project

├── index.html
├── style.css
├── Dockerfile
├── Jenkinsfile
├── README.md
└── screenshots
    ├── website-output.png
    ├── ec2-instance.png
    └── jenkins-success.png
```

---

# Docker Deployment

## Build Docker Image

```bash
docker build -t devops-portfolio .
```

## Run Docker Container

```bash
docker run -d -p 80:80 devops-portfolio
```

## Check Running Container

```bash
docker ps
```

---

# Jenkins Pipeline

Pipeline stages:

```
Checkout Code
      |
      |
Build Docker Image
      |
      |
Run Docker Container
      |
      |
Deploy Application
```

---

# AWS Deployment

The application is deployed on:

- AWS EC2 Instance
- Ubuntu Server
- Docker Runtime
- Nginx Web Server

Security configuration:

- HTTP Port 80 enabled
- SSH Port 22 enabled

---

# Screenshots

## Website Output

![Website](screenshots/website-output.png)


## AWS EC2 Instance

![EC2](screenshots/ec2-instance.png)


## Jenkins Pipeline Success

![Jenkins](screenshots/jenkins-success.png)


---

# Challenges Faced & Solutions

### 1. Jenkins-GitHub Integration

**Challenge:** Connecting Jenkins with GitHub repository.

**Solution:** Configured Git repository URL and automated source code checkout.


### 2. Docker Deployment

**Challenge:** Running application inside a container.

**Solution:** Created Dockerfile and automated container deployment.


### 3. AWS Server Configuration

**Challenge:** Hosting application securely on EC2.

**Solution:** Configured Ubuntu server, security groups, Docker and Nginx.

---

# Future Improvements

- Add Terraform for AWS infrastructure automation.
- Add AWS Route 53 custom domain.
- Add HTTPS using AWS Certificate Manager.
- Add monitoring using CloudWatch.
- Implement Kubernetes deployment.

---

# Interview Explanation

"I built an AWS DevOps CI/CD pipeline for deploying a portfolio website. The source code is maintained in GitHub, Jenkins automates the build and deployment process, Docker is used for containerization, and the application is hosted on AWS EC2 using Nginx. This project helped me understand real-world DevOps practices including CI/CD automation, cloud deployment, and Linux server management."

---

# Author

**Nikita Sumant**

- AWS DevOps Engineer (Aspiring)
- GitHub: https://github.com/Nikita021998
- Project: AWS DevOps CI/CD Portfolio Project
