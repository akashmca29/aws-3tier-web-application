# AWS 3-Tier Web Application
- Web Tier EC2 Instances
- Application Tier EC2 Instances
- Amazon RDS Database
- Bastion Host
- CloudWatch Monitoring
- SNS Email Alerts

---

## Architecture Diagram

![Architecture Diagram](architecture-diagram.png)

---

## Project Flow

1. User accesses application through Route 53 domain.
2. CloudFront improves speed and caching.
3. HTTPS ALB distributes traffic to Web Tier EC2 instances.
4. Web Tier forwards requests to Application Tier.
5. Application Tier connects to Amazon RDS database.
6. Bastion Host is used for secure private access.
7. CloudWatch monitors infrastructure.
8. SNS sends email notifications.

---

## AWS Services Used

- Amazon EC2
- Application Load Balancer
- Auto Scaling Group
- Amazon RDS
- Amazon VPC
- Route 53
- CloudFront
- Bastion Host
- CloudWatch
- SNS

---

## Security Features

- HTTPS using SSL certificate
- Private subnets for Application Tier and RDS
- Bastion Host for SSH access
- Security Groups for restricted access
- CloudFront for secure delivery

---

## Resume Points

- Designed a 3-tier web application architecture using EC2, ALB, and RDS.
- Implemented private subnets for secure application and database layers.
- Configured Bastion Host for administrative access.
- Integrated Route 53 and CloudFront for secure content delivery.
- Configured CloudWatch alarms and SNS notifications.

---

## Interview Questions

1. What is a 3-tier architecture?
2. Why are private subnets used?
3. What is the role of Bastion Host?
4. Why use ALB?
5. How does CloudFront improve performance?
6. What happens if one EC2 instance fails?
7. Why place RDS in private subnet?
8. What is the difference between Web Tier and App Tier?
