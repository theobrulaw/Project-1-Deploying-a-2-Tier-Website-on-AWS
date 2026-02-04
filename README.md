# Scalable Web Application on AWS

This repository contains hands-on projects demonstrating the design,
deployment, and operation of a highly available and scalable web application
on AWS using best practices for reliability, performance, and cost efficiency.

The focus is on building cloud-native architectures that can scale on demand,
handle failures gracefully, and support real-world production workloads.

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
