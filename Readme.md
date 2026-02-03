# Cloud Basics Using AWS Free Tier

## Overview
This project demonstrates **basic cloud computing concepts** using the **AWS Free Tier**.  
An **EC2 Linux instance** was launched, accessed using SSH, and configured with a basic web server.

---

## Services
- **EC2 Instance**: Linux virtual machine launched using AWS EC2 Free Tier
- **Web Server**: Apache (httpd) installed on EC2 instance

---

## Service Interaction
- User connects to EC2 instance using SSH and key pair
- Security groups allow SSH (22) and HTTP (80) access
- Web application is accessed using EC2 public IP
- AWS resources are managed through AWS Console

---

## Commands Used
```bash
ssh -i keypair.pem ec2-user@<public-ip>
sudo yum update -y
sudo yum install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd
