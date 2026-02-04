# Amazon S3 Static Website Hosting (Cloud Infrastructure Lab)

This repository documents hands-on labs and exercises using Amazon S3
to deploy and manage static websites in AWS, focusing on cloud storage,
security configuration, access control, and scalable web hosting
within a production-style cloud environment.

The focus is on developing practical AWS skills that support CloudOps,
DevOps, and cloud infrastructure engineering roles.

---

## Technologies & Services Used

- Amazon EC2
- Application Load Balancer (ALB)
- Auto Scaling Groups (ASG)
- Amazon VPC (Public & Private Subnets)
- Amazon RDS (Multi-AZ)
- Amazon S3
- Amazon CloudFront
- AWS Route 53
- AWS Certificate Manager (ACM)
- Amazon CloudWatch
- AWS IAM
- Git & GitHub

---

## Architecture & Design Principles

- High availability across multiple Availability Zones
- Horizontal scaling with Auto Scaling Groups
- Layered architecture (Web, Application, Database)
- Fault tolerance and self-healing infrastructure
- Secure networking using VPC isolation
- Observability through logging and monitoring
- Cost-aware resource design

---

## Featured Labs & Projects

- Web application deployment using EC2 behind an Application Load Balancer
- Auto Scaling configuration based on CPU and traffic metrics
- Multi-AZ database deployment for high availability
- Secure networking with public and private subnets
- CloudFront integration for performance optimization
- HTTPS enforcement using ACM
- Route 53 DNS configuration with alias records
- CloudWatch alarms and scaling policies
- Failure simulation and recovery testing

---

## Repository Structure

```text
Scalable-Web-App-on-AWS/
├── networking/
├── compute/
├── load-balancing/
├── auto-scaling/
├── database/
├── monitoring/
├── diagrams/
└── documentation/
# Scalable-Web-App-on-AWS
Deployed a containerized Node.js app using ECS, ALB, and RDS. Implemented CI/CD using GitHub Actions.
