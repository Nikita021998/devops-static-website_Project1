# AWS DevOps CI/CD Portfolio Project

## Project Overview

This project demonstrates a complete CI/CD deployment pipeline using AWS and DevOps tools.

The static portfolio website is deployed on AWS EC2 using Docker, Jenkins, and Nginx.

---

## Architecture

```
Developer
    |
    |
GitHub Repository
    |
    |
Jenkins CI/CD Pipeline
    |
    |
Docker Container
    |
    |
AWS EC2 Instance
    |
    |
Nginx Web Server
    |
    |
Live Website
```

---

## Technologies Used

- AWS EC2
- Ubuntu Linux
- GitHub
- Jenkins
- Docker
- Nginx
- Shell Scripting
- CI/CD Pipeline

---

## CI/CD Workflow

1. Developer pushes code to GitHub

2. Jenkins automatically pulls the latest code

3. Docker image is created

4. Application container is deployed

5. Nginx serves the website

---

## Project Structure

```
.
├── index.html
├── style.css
├── Dockerfile
├── Jenkinsfile
└── README.md
```

---

## Deployment Commands

### Build Docker Image

```
docker build -t devops-portfolio .
```

### Run Docker Container

```
docker run -d -p 80:80 devops-portfolio
```

---

## Project Screenshots

(Add screenshots here)

Example:

```
screenshots/
├── website-output.png
├── ec2-instance.png
└── jenkins-success.png
```

---

## Interview Explanation

"I created a DevOps CI/CD pipeline where source code is managed using GitHub. Jenkins automates the build and deployment process. The application is containerized using Docker and deployed on AWS EC2 with Nginx as the web server."
