# DevOps CI/CD Platform

An end-to-end DevOps CI/CD platform that automates building, testing, analyzing, containerizing, and deploying a Java application to AWS EKS using modern DevOps tools and best practices.

---

## Project Overview

The platform covers the complete software delivery lifecycle:

- Infrastructure provisioning with Terraform
- Continuous Integration using Jenkins
- Code quality analysis with SonarQube
- Artifact management with Nexus Repository
- Docker image build and push to Amazon ECR
- Continuous Deployment to Kubernetes (Amazon EKS)

All required tools are installed automatically using custom shell scripts inside /scripts folder.

---

## Architecture

Java Code → GitHub → Jenkins CI/CD Pipeline  
- SonarQube (Code Quality)  
- Maven Build  
- Nexus Repository (Artifacts)  
- Docker Image  
- Amazon ECR  
- Amazon EKS (Kubernetes Deployment)

---

## Tech Stack

### CI/CD & Build
- Jenkins
- GitHub
- Maven

### Code Quality & Artifacts
- SonarQube
- Nexus Repository Manager

### Containers & Orchestration
- Docker
- Kubernetes
- Amazon EKS
- kubectl
- eksctl

### Cloud & Infrastructure
- AWS (EC2, EKS, ECR, IAM, VPC)
- Terraform (Infrastructure as Code)

### Configuration & Automation
- Bash scripting
- Ansible

---

## CI/CD Pipeline Stages

1. Checkout source code from GitHub
2. Run SonarQube static code analysis
3. Build Java application using Maven
4. Upload artifacts to Nexus Repository
5. Build Docker image
6. Push Docker image to Amazon ECR
7. Deploy application to Amazon EKS using Kubernetes manifests.

## Tool Installation

All tools are installed using scripts in the `scripts/` directory:
- Jenkins
- Docker
- Terraform
- Ansible
- kubectl
- eksctl
- SonarQube
- Nexus Repository
