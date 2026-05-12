BuildRight – Cloud-Native Full Stack Web Application

📌 Project Overview

BuildRight is a full-stack, cloud-enabled web application designed for managing architectural projects, plans, galleries, and client inquiries through a modern admin dashboard.
The project is built using scalable AWS cloud infrastructure with automated CI/CD practices for deployment and management.

The platform enables:

Architecture project showcase management
Plan and gallery management
Secure admin operations
Client inquiry handling
Cloud-based scalable deployment
Automated infrastructure provisioning using Terraform
CI/CD integration for seamless deployment
🏗️ System Architecture
AWS Architecture Overview

The application is deployed using a secure and scalable AWS cloud architecture.

Architecture Components
Amazon CloudFront
Global CDN for faster content delivery
Amazon API Gateway
Secure API routing and management
Amazon S3
Static frontend hosting (React.js)
Storage for images, plans, reports, and PDFs
Application Load Balancer (ALB)
Distributes traffic across backend instances
Amazon EC2 Auto Scaling Group
Hosts Spring Boot backend applications
Automatically scales based on traffic
Amazon RDS (MySQL)
Managed relational database service
AWS IAM
Secure access management and permissions
Amazon CloudWatch
Monitoring and logging
AWS CloudTrail
Auditing and activity tracking
NAT Gateway
Internet access for private subnet resources
📷 Architecture Diagram

🚀 Tech Stack
Frontend
React.js
HTML5
CSS3
JavaScript
Backend
Spring Boot
REST APIs
Java
Database
MySQL (Amazon RDS)
Cloud & DevOps
AWS EC2
AWS S3
AWS CloudFront
AWS API Gateway
AWS ALB
AWS IAM
AWS CloudWatch
AWS CloudTrail
Terraform
GitHub Actions / CI-CD Pipeline
☁️ AWS Infrastructure
VPC Design
Public Subnet
Private Subnet
Internet Gateway
NAT Gateway
Security Groups
Compute Layer
EC2 instances in Auto Scaling Group
Spring Boot application deployment
Storage Layer
S3 bucket for frontend hosting
S3 bucket for reports and documents
Database Layer
Amazon RDS MySQL in private subnet
🔄 CI/CD Pipeline

The project follows a cloud-native CI/CD workflow.

Pipeline Flow
Developer pushes code to GitHub
CI pipeline triggers automatically
Terraform provisions infrastructure
Backend services deploy to EC2
Frontend deploys to S3
CloudFront distributes content globally
📁 Project Structure
BuildRight/
│
├── frontend/                 # React Frontend
├── backend/                  # Spring Boot Backend
├── terraform/                # Infrastructure as Code
│   ├── alb.tf
│   ├── ec2.tf
│   ├── rds.tf
│   ├── vpc.tf
│   ├── security.tf
│   ├── iam.tf
│   ├── s3.tf
│   ├── variables.tf
│   └── outputs.tf
│
├── .github/workflows/        # CI/CD Pipelines
├── README.md
└── architecture.png
⚙️ Terraform Deployment Steps
Initialize Terraform
terraform init
Validate Configuration
terraform validate
Preview Infrastructure
terraform plan
Deploy Infrastructure
terraform apply
🔐 Security Features
IAM role-based access control
Security Groups for network isolation
Private subnet for database
HTTPS communication
CloudTrail auditing
CloudWatch monitoring
📊 Monitoring & Logging
Amazon CloudWatch
Application monitoring
EC2 metrics
Log collection
AWS CloudTrail
AWS API activity tracking
Security auditing
🌟 Key Features

✅ Scalable AWS Architecture
✅ Full Stack Web Application
✅ Infrastructure as Code (Terraform)
✅ Auto Scaling Backend
✅ Secure Cloud Deployment
✅ CI/CD Automation
✅ Global Content Delivery using CloudFront
✅ Managed Database with Amazon RDS
✅ Modern Admin Dashboard

📌 Future Enhancements
Docker containerization
Kubernetes (EKS) deployment
Multi-region deployment
AI-powered architecture recommendations
Real-time analytics dashboard
