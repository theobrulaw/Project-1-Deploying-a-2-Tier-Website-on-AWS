# Project 1: Deploying a 2-Tier Website on AWS

## Objective

This lab demonstrates how to deploy a highly available 2-tier web application architecture on AWS, separating the web (application) layer from the database layer to improve scalability, security, and reliability.

The project reflects real-world cloud infrastructure patterns used in production environments where frontend services interact securely with backend databases while maintaining performance and fault tolerance.

---

## Architecture / Environment Overview

The environment consists of:

- Amazon EC2 instances hosting the web application layer  
- Amazon RDS (or EC2-based database server) for the database layer  
- Virtual Private Cloud (VPC) with public and private subnets  
- Internet Gateway for public web access  
- Security Groups controlling tier-to-tier communication  

### Core Components

- **Web Tier:** EC2 instance(s) running Apache/Nginx hosting the website  
- **Database Tier:** RDS MySQL/PostgreSQL (or private EC2 DB server)  
- **Networking:** Segmented subnets for security isolation  
- **Security:** Least-privilege inbound and outbound rules  

---

## Prerequisites

- AWS account with EC2, VPC, and RDS permissions  
- Basic understanding of:
  - Linux server administration  
  - VPC networking concepts  
  - Web servers and databases  
- SSH client or AWS console access  

---

## Steps Performed

1. Created a custom VPC with public and private subnets  
2. Deployed EC2 instance in public subnet for the web tier  
3. Installed and configured Apache/Nginx web server  
4. Deployed RDS instance (or private EC2 database server)  
5. Configured security groups for controlled communication  
6. Connected web tier to database tier  
7. Deployed sample website/application  
8. Verified end-to-end functionality  

---

## Validation & Verification

The deployment was confirmed by:

- Successful access to website via EC2 public IP or DNS  
- Database connectivity from web server  
- Application read/write operations functioning correctly  
- Security group rules blocking unauthorized access  

### Key Observations

- Web tier accessible publicly while database remained private  
- Only web server allowed database connections  
- Clear separation of responsibilities between tiers  

---

## Security & Operational Considerations

- Database tier placed in private subnet without internet access  
- Security groups enforced least-privilege access  
- SSH restricted to trusted IP ranges  
- Regular patching applied to EC2 instances  

### Operational Trade-offs

- Single EC2 web server vs horizontal scaling  
- RDS managed service vs self-managed database  
- Cost vs availability considerations  

---

## Lessons Learned

- Tier separation significantly improves security posture  
- VPC subnet design impacts application resilience  
- Proper security group design is critical for cloud workloads  
- Managed services reduce operational overhead  

### Future Improvements

- Add Application Load Balancer for high availability  
- Implement Auto Scaling for web tier  
- Add HTTPS using AWS Certificate Manager  
- Infrastructure as Code deployment  
- Implement backups and monitoring  

---

