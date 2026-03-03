📌 Project 5 – EC2 Web Server using CloudFormation (web-stack)
📖 Project Overview
This project demonstrates Infrastructure as Code (IaC) using AWS CloudFormation.
A CloudFormation stack named web-stack was created to automatically provision an EC2 web server.
After stack creation, the EC2 instance was launched successfully and a sample web page was deployed using a User Data script.

🎯 Objective

Automate EC2 instance creation
Use CloudFormation instead of manual provisioning
Install Apache Web Server using User Data
Deploy static HTML page
Access application via public IP

🛠️ AWS Services Used
AWS CloudFormation
Amazon EC2
Amazon VPC
Security Group

🏗️ Architecture
User → Browser → Public IP → EC2 (web-stack) → Apache Web Server → index.html
All infrastructure created through CloudFormation stack web-stack.


🔄 Implementation Steps
Step 1: Create CloudFormation Template
The template includes:
EC2 instance (Name: web-stack)
Instance type: t3.micro
Security Group allowing HTTP (Port 80)
User Data script to install Apache

Step 2: Create Stack
Open AWS CloudFormation
Click Create Stack
Upload template file
Enter Stack name → web-stack
Launch stack
Stack Status: CREATE_COMPLETE ✅

Step 3: EC2 Instance Created
Instance Details:
Name: web-stack
Instance Type: t3.micro
Region: us-east-1
Status: Running
CloudFormation automatically installed Apache using User Data script.

Step 4: Access Application
Copy EC2 Public IP
Open in browser
Output displayed:
CloudFormation Web Server Working

🚀 Final Output
The web server was successfully deployed using Infrastructure as Code without manually launching EC2.
