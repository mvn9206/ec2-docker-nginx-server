# EC2 + Docker + Nginx Web Server on AWS

## Overview
Deployed a live web server on AWS EC2 using Docker and Nginx.
Accessible from the public internet via HTTP.

## What I Built
- Launched EC2 instance (Amazon Linux 2023) in Mumbai region
- SSH'd into server via AWS EC2 Instance Connect
- Installed Docker on Linux server
- Pulled and ran Nginx inside a Docker container
- Configured Security Group to allow HTTP port 80
- Web server live and accessible from public IP

## Architecture
Browser → Public IP → EC2 Security Group (Port 80) → 
Docker Container → Nginx Web Server

## AWS Services Used
- Amazon EC2 (t3.micro, Mumbai region)
- Security Groups (Inbound rules)
- EC2 Instance Connect (SSH)

## Commands Used
sudo yum install docker -y
sudo systemctl start docker
sudo docker run -d -p 80:80 nginx

## Screenshots
<img width="1878" height="773" alt="EC2 RUNNING" src="https://github.com/user-attachments/assets/74031d00-34b4-4dfe-ae4c-e5a0ead2d50e" />
<img width="1893" height="830" alt="docker commands" src="https://github.com/user-attachments/assets/e0ab9d97-c1e0-4aa6-a028-6d9dd063b08e" />
<img width="1873" height="707" alt="nginx" src="https://github.com/user-attachments/assets/b1b61c69-710d-4e64-af65-0fb5e03c92fd" />


## Key Concepts Demonstrated
- Cloud compute provisioning
- Linux server administration
- Docker containerization
- Network security with security groups
- Web server deployment
