# AWS Automated Static Website Hosting
An automated, production-grade infrastructure-as-code (IaC) project for hosting highly available, secure static websites on AWS.

##  Project Overview
This project automates the deployment of a static website using **Terraform**. It leverages **Amazon S3** for storage and **AWS CloudFront** for global content delivery, secured with the modern **Origin Access Control (OAC)** protocol.

### Key Features
* **Zero Public S3 Access:** The bucket is completely private; traffic is only allowed through CloudFront.
* **Global Latency Reduction:** Uses CloudFront Edge locations for fast loading worldwide.
* **Security First:** Implements AWS SigV4 signing via OAC.
* **Automated Content Sync:** Terraform handles both infrastructure provisioning and file uploads.

##  Architecture


* **S3:** Hosts the static assets (HTML/CSS).
* **CloudFront:** Acts as the CDN and SSL termination point.
* **OAC:** Secures the "handshake" between CloudFront and S3.
* **Terraform:** Manages the entire lifecycle of the resources.

##  Tech Stack
| Tool | Purpose |
| :--- | :--- |
| **Terraform** | Infrastructure as Code |
| **AWS S3** | Object Storage |
| **AWS CloudFront** | Content Delivery Network (CDN) |
| **Git/GitHub** | Version Control |


