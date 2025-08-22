# AWS Route 53 & SSL Certificate Demo Setup

## 📋 Overview

I walked through the complete AWS infrastructure setup process without actually buying a domain - here's how I did it and what I learned.

## 🛠 My Setup Process

### Route 53 Hosted Zone
- Created a hosted zone for my demo domain
- Got nameservers and DNS management capabilities
- Learned DNS infrastructure without owning the domain

### SSL Certificate with ACM
- Requested SSL certificate through AWS Certificate Manager
- Set up DNS validation process
- Learned complete certificate request and validation workflow

### VPC Infrastructure
- Built custom VPC with public/private subnets across multiple AZs
- Configured internet gateway and route tables
- Set up security groups for proper communication

### Load Balancer Setup
- Created Application Load Balancer targeting my EC2 instance
- Configured SSL certificate integration
- Set up HTTP/HTTPS traffic handling across multiple AZs

### Health Checks & DNS Records
- Configured Route 53 health checks for EC2 endpoint monitoring
- Created A records pointing to load balancer
- Set up failover routing policies for high availability

## ✅ Key Takeaways

- ✨ Practiced entire SSL and load balancer setup without domain purchase costs
- 🔗 Learned seamless integration between Route 53, ACM, VPC, and ALB
- 📚 Understood complete workflow from DNS to certificate validation to traffic routing
- 🛡️ Gained hands-on experience with AWS networking and security configurations

## ⚠️ CloudFront Limitation

Since I didn't have a registered domain, I couldn't set up custom CloudFront for this demo. However, I successfully implemented CloudFront with a custom domain in my **Week 8 task**.
