# Node.js Todo Application Deployment on AWS ECS & ECR

Deploying a Node.js Todo Application using Docker, Amazon ECR, ECS Fargate and CloudWatch Logs.

## 📌 Project Overview

This project demonstrates the deployment of a containerized Node.js Todo Application on AWS using Docker, Amazon ECR, Amazon ECS (Fargate), IAM, Security Groups, and CloudWatch Logs.

The application was first containerized using Docker, stored in Amazon Elastic Container Registry (ECR), deployed using Amazon Elastic Container Service (ECS), and monitored through CloudWatch Logs.

---

## Architecture

```text
Developer
    │
    ▼
GitHub Repository
    │
    ▼
Docker Build
    │
    ▼
Amazon ECR
(Container Registry)
    │
    ▼
Amazon ECS (Fargate)
(Container Deployment)
    │
    ▼
Security Group + Networking
    │
    ▼
Node.js Todo Application
    │
    ▼
Amazon CloudWatch Logs
```

---

## Technologies & AWS Services Used

### Development
- Node.js
- HTML
- CSS
- JavaScript

### DevOps Tools
- Git
- GitHub
- Docker

### AWS Services
- Amazon ECS
- Amazon ECR
- IAM
- CloudWatch Logs
- Security Groups
- VPC Networking

---

## Project Workflow

### Step 1: Application Development
- Created a Todo Application using Node.js.
- Developed frontend using HTML, CSS, and JavaScript.

### Step 2: Version Control
- Stored source code in GitHub repository.
- Managed project versions using Git.

### Step 3: Docker Containerization
- Created a Dockerfile.
- Built a Docker image for the application.

```bash
docker build -t node-todo .
```

### Step 4: Amazon ECR
- Created an ECR repository.
- Authenticated Docker with ECR.
- Tagged and pushed Docker image.

```bash
docker tag node-todo:latest <ecr-repository-uri>
docker push <ecr-repository-uri>
```

### Step 5: Amazon ECS
- Created ECS Cluster.
- Created ECS Task Definition.
- Configured CPU, Memory, Container Image and Ports.
- Deployed application using ECS Fargate.

### Step 6: IAM Configuration
- Configured ECS Task Execution Role.
- Allowed ECS to pull images from ECR.
- Allowed ECS to send logs to CloudWatch.

### Step 7: Networking & Security
- Configured VPC Networking.
- Assigned Public IP.
- Updated Security Group rules.
- Allowed inbound traffic on application port.

### Step 8: Monitoring
- Integrated CloudWatch Logs.
- Verified application logs and container status.

---

## 📸 Project Screenshots

### ECS Cluster
![ECS Cluster](Screenshots/ecs-cluster.png)

### ECS Task Running
![ECS Task](Screenshots/ecs-task-running.png)

### CloudWatch Logs
![CloudWatch Logs](Screenshots/cloudwatch-logs.png)

### Security Group Configuration
![Security Group](Screenshots/security-group.png)

### Application Output
![Application](Screenshots/application-output.png)

---

## Deployment Steps

1. Create Node.js Application
2. Create Dockerfile
3. Build Docker Image
4. Create ECR Repository
5. Push Image to ECR
6. Create ECS Cluster
7. Create Task Definition
8. Configure Networking
9. Configure IAM Role
10. Enable CloudWatch Logs
11. Run ECS Task
12. Configure Security Group
13. Access Application using Public IP

---

## Learning Outcomes

Through this project I gained hands-on experience in:

- Docker Containerization
- Amazon ECR
- Amazon ECS Fargate
- IAM Roles & Permissions
- CloudWatch Monitoring
- Security Group Management
- AWS Networking Basics
- Container Deployment Workflow
- Real-world DevOps Practices

---

## Author

**Vedashri Giri**

Aspiring DevOps Engineer | AWS Learner | Docker | Linux | Git | GitHub | ECS | ECR | CloudWatch
