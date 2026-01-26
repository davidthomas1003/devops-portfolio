![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/davidthomas1003/devops-portfolio/deploy.yml?branch=main)
![Terraform](https://img.shields.io/badge/Terraform-1.5.0-blue)
![Docker](https://img.shields.io/badge/Docker-Verified-blue)
![AWS](https://img.shields.io/badge/AWS-Cloud-orange)

# DevOps Portfolio — ECS Fargate CI/CD

## Overview
This repository demonstrates a production-style DevOps workflow using AWS, Terraform, Docker, and GitHub Actions.

## Architecture
- Dockerized application
- Amazon ECR
- Amazon ECS (Fargate)
- Terraform (Infrastructure as Code)
- GitHub Actions (CI/CD)

## Architecture Diagram

![Architecture](assets/architecture.png)

## Pipeline Example

![Pipeline](assets/pipeline.png)
*GitHub Actions deploying container to ECS successfully*

## Running App

![App Screenshot](assets/app.png)
*Flask app served via ECS Fargate*

## CI/CD Pipeline
- Build Docker image
- Push image to Amazon ECR
- Terraform plan on pull requests
- Terraform apply on main branch

## Branch Strategy
- aphrodite: staging/testing
- main: production (protected)

## Security
- GitHub Secrets for AWS credentials
- Branch protection enabled
 
