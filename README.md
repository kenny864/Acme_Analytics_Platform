# Acme_Analytics_Platform

> A production-inspired AWS Cloud Engineering portfolio demonstrating how a fictional startup's cloud infrastructure evolves from a single Terraform deployment into a scalable, secure, and automated platform.

---

## Overview

**Acme Analytics** is a fictional SaaS startup that provides data analytics solutions to business customers.

This repository serves as the central documentation hub for the company's cloud infrastructure portfolio. Each project represents a realistic engineering milestone in the startup's growth, showcasing how AWS infrastructure can be designed, automated, secured, and operated using Infrastructure as Code (IaC).

The goal of this portfolio is to demonstrate practical cloud engineering skills through production-inspired Terraform projects that build upon one another.

---

# Platform Evolution

```text
Project 1
AWS IAM User Provisioning
│
├── Automated user creation
├── IAM Groups
└── MFA Enforcement
        │
        ▼
Project 2
Network Foundation
│
├── VPC
├── Public & Private Subnets
├── NAT Gateway
└── Security Groups
        │
        ▼
Project 3
Marketing Website
│
├── Amazon S3
├── CloudFront
├── ACM
└── Route 53
        │
        ▼
Project 4
Three-Tier Application
│
├── ALB
├── Auto Scaling
├── EC2
└── Amazon RDS
        │
        ▼
Project 5
Remote Terraform Backend
│
├── Amazon S3
└── DynamoDB
        │
        ▼
Project 6
Terraform Modules
        │
        ▼
Project 7
Multi-Environment Infrastructure
        │
        ▼
Project 8
GitHub Actions CI/CD
        │
        ▼
Project 9
Amazon ECS on AWS Fargate
        │
        ▼
Project 10
Serverless Customer API
        │
        ▼
Project 11
Monitoring & Alerting
        │
        ▼
Project 12
Amazon EKS Kubernetes Platform
```

---

# Repository Roadmap

| Project                          | Repository                        | Status     |
| -------------------------------- | --------------------------------- | ---------- |
| IAM User Provisioning            | terraform-acme-iam-provisioning   | ✅ Complete |
| Network Foundation               | terraform-acme-network-foundation | ⏳ Planned  |
| Static Website                   | terraform-acme-static-website     | ⏳ Planned  |
| Three-Tier Application           | terraform-acme-three-tier-app     | ⏳ Planned  |
| Remote Terraform Backend         | terraform-acme-remote-state       | ⏳ Planned  |
| Terraform Modules                | terraform-acme-modules            | ⏳ Planned  |
| Multi-Environment Infrastructure | terraform-acme-multi-environment  | ⏳ Planned  |
| GitHub Actions CI/CD             | terraform-acme-github-actions     | ⏳ Planned  |
| Amazon ECS on AWS Fargate        | terraform-acme-ecs-fargate        | ⏳ Planned  |
| Serverless Customer API          | terraform-acme-serverless-api     | ⏳ Planned  |
| Monitoring & Alerting            | terraform-acme-monitoring         | ⏳ Planned  |
| Amazon EKS Platform              | terraform-acme-eks-platform       | ⏳ Planned  |

---

# Overall AWS Architecture

```text
                                Internet
                                    │
                             Amazon Route 53
                                    │
                              Amazon CloudFront
                                    │
                       Static Website (Amazon S3)
                                    │
                                    ▼
                    Application Load Balancer (ALB)
                                    │
               ┌────────────────────┴────────────────────┐
               │                                         │
         Amazon ECS (Fargate)                    Amazon EC2
               │                                         │
               └────────────────────┬────────────────────┘
                                    │
                               Amazon RDS
                                    │
                               Amazon S3
                                    │
             API Gateway ──► AWS Lambda ──► DynamoDB

                    CloudWatch • SNS • IAM • GitHub Actions
```

---

# AWS Services Used

## Compute

* Amazon EC2
* Amazon ECS
* AWS Fargate
* AWS Lambda
* Amazon EKS

## Networking

* Amazon VPC
* Public & Private Subnets
* Internet Gateway
* NAT Gateway
* Route Tables
* Security Groups
* Application Load Balancer

## Storage

* Amazon S3
* Amazon DynamoDB

## Databases

* Amazon RDS (MySQL)

## Identity & Security

* AWS IAM
* IAM Policies
* IAM Groups
* MFA Enforcement

## Monitoring

* Amazon CloudWatch
* Amazon SNS

## DevOps

* Terraform
* GitHub Actions
* Docker

---

# Skills Demonstrated

## Infrastructure as Code

* Terraform
* Modular Infrastructure
* Variables
* Outputs
* Remote State
* State Locking

## Cloud Architecture

* High Availability
* Multi-AZ Deployments
* Layered Network Design
* Secure Application Architecture

## Security

* Least Privilege Access
* IAM Policy Design
* MFA Enforcement
* Security Groups
* Private Networking
* Encryption

## Automation

* Infrastructure Automation
* User Provisioning
* CI/CD Pipelines
* GitHub Actions

## Containers

* Docker
* Amazon ECS
* AWS Fargate
* Amazon EKS

## Serverless

* API Gateway
* AWS Lambda
* DynamoDB

---

# Architecture Diagrams

Each repository includes:

* AWS architecture diagrams
* Terraform project structure
* Deployment screenshots
* AWS Console screenshots
* Infrastructure documentation

---

# Repository Standards

Every project in this portfolio includes:

* Professional README
* Business scenario
* Project requirements
* Architecture diagram
* Terraform source code
* Deployment instructions
* Example outputs
* Screenshots
* Lessons learned
* Future improvements

---

# Why This Portfolio?

Rather than creating isolated Terraform tutorials, this portfolio demonstrates how cloud infrastructure evolves as a company grows.

Beginning with identity management and networking, the projects gradually introduce scalable web applications, CI/CD pipelines, containers, serverless services, monitoring, and Kubernetes. Each project builds on previous work to reflect how infrastructure is developed in real engineering environments.

---

# About the Author

Hi, I'm **Kenny Jean-Baptiste**.

I'm an AWS Cloud Engineer focused on building secure, automated, and production-inspired cloud infrastructure using Terraform and AWS. This portfolio documents my hands-on journey developing practical cloud engineering skills through realistic infrastructure projects.

Feel free to explore the individual repositories to see each stage of the Acme Analytics platform in detail.

---

## License

This project is licensed under the MIT License.
