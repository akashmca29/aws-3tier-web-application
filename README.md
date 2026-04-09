# AWS 3-Tier Web Application
- Web Tier EC2 Instances
- Application Tier EC2 Instances
- Amazon RDS Database
- Bastion Host
- CloudWatch Monitoring
- SNS Email Alerts

---
aws-3tier-web-application/
│
├── README.md
├── architecture-diagram.png
├── screenshots/
│   ├── vpc.png
│   ├── public-subnet.png
│   ├── private-subnet.png
│   ├── alb.png
│   ├── ec2-web-tier.png
│   ├── ec2-app-tier.png
│   ├── rds.png
│   ├── cloudfront.png
│   ├── route53.png
│   ├── sns.png
│   └── cloudwatch.png
├── web-tier/
│   ├── index.html
│   └── style.css
├── app-tier/
│   └── app.py
├── userdata-script/
│   ├── webserver-install.sh
│   └── appserver-install.sh
├── deployment-steps.md
├── security-group-rules.md
├── interview-questions.md
├── resume-points.md
└── cost-estimation.md
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

