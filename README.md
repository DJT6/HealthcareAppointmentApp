# Cloud-Based Appointment Management System

A **full-stack healthcare-style appointment booking system** deployed on AWS, demonstrating modern **multi-tier cloud architecture** and **CI/CD automation**.  
Patients can securely book, manage, and cancel appointments via a responsive frontend, while backend operations run on AWS with high availability and scalability.

---

## Overview

This project simulates a real-world healthcare scheduling system deployed entirely on AWS.  
It uses a **multi-tier architecture** integrating EC2, DynamoDB, Route 53, and Nginx for secure and scalable access.  
It also features **CI/CD pipelines** through GitHub Actions for automated deployments, and **CloudWatch monitoring** for observability.

---

## Architecture

**Architecture Components:**
- **Frontend:** Hosted via AWS S3 + CloudFront with custom domain (HTTPS via Route 53)
- **Backend:** Node.js/Express API running on EC2 with Nginx reverse proxy
- **Database:** DynamoDB for storing appointment data
- **Monitoring:** CloudWatch logs and alarms for backend/API health
- **Security:** IAM roles with least-privilege access, SSL via Route 53 + Nginx
- **Automation:** CI/CD pipeline integrated with GitHub Actions for continuous deployment

### System Diagram
Client → Route 53 → CloudFront → Nginx (EC2) → Node.js API → DynamoDB

## Auther
Deion Jose Tulcidas
- AWS Cloud Certified | Business Information Systems Major @ University of Pittsburgh 
  Building scalable, cloud-native applications on AWS 
