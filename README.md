# 🚀 Task 3 – Infrastructure as Code (IaC) with Terraform

## Elevate Labs – DevOps Internship

---

## 📌 Project Overview

This project demonstrates Infrastructure as Code (IaC) using Terraform to provision a local Docker container.

Terraform was used to manage a Docker NGINX image and container through the Docker provider.

The container was successfully deployed and accessed through a web browser.

---

## 🎯 Objective

The objective of this task is to understand Infrastructure as Code and provision a local Docker container using Terraform.

---

## 🛠️ Tools Used

- Terraform

- Docker

- Docker Provider

- Git Bash

- GitHub

- NGINX

---

## 📁 Project Structure


terraform-docker/

│

├── main.tf

├── README.md

├── .gitignore

│

└── screenshots/

&#x20;   ├── 01-terraform-init.png

&#x20;   ├── 02-terraform-plan.png

&#x20;   ├── 03-terraform-apply.png

&#x20;   ├── 04-nginx-browser.png

&#x20;   ├── 05-terraform-state.png

&#x20;   └── 06-terraform-destroy.png



⚙️ Terraform Configuration

The main.tf file contains the Terraform configuration for:

1\. Docker provider

2\. NGINX Docker image

3\. NGINX Docker container

4\. Port mapping

The NGINX container was exposed through port 8081 on the host and port 80 inside the container.



🔄 Terraform Commands Used:

1\. Initialize Terraform:

terraform init



Initializes the Terraform working directory and downloads the required Docker provider.



2\. Validate Configuration:

terraform validate



Checks whether the Terraform configuration is valid.



3\. Create Execution Plan:

terraform plan



Shows the infrastructure changes Terraform plans to make.



4\. Apply Configuration:

terraform apply



Creates the Docker image and Docker container.



5\. Check Docker Container:

docker ps



Used to verify that the NGINX container was running.



6\. Verify Application:

The application was accessed using:

http://localhost:8081



The NGINX welcome page was displayed successfully.



7\. Check Terraform State:

terraform state list



Used to view the resources managed by Terraform.

terraform show



Used to display detailed information about the Terraform-managed infrastructure.



8\. Destroy Infrastructure:

terraform destroy



Used to remove the Docker container and Docker image created by Terraform.



📸 Execution Evidence:

Terraform Plan:

Terraform successfully generated an execution plan for the Docker image and container.

Terraform Apply:

Terraform successfully created the Docker NGINX image and container.

NGINX Application



The NGINX application was successfully accessed at:

http://localhost:8081



Terraform State:

The Terraform state showed:

docker\_container.nginx

docker\_image.nginx



Terraform Destroy:

The infrastructure was successfully removed.

Terraform displayed:

Destroy complete! Resources: 2 destroyed.



🧠 What I Learned:

Through this task, I learned:

\- What Infrastructure as Code (IaC) means

\- How Terraform works

\- What Terraform providers are

\- How to use the Docker provider

\- How to create Docker resources using Terraform

\- How terraform init works

\- How terraform plan previews changes

\- How terraform apply provisions infrastructure

\- How to inspect Terraform state

\- How terraform destroy removes infrastructure

\- How Terraform can automate infrastructure provisioning





✅ Conclusion:

This task provided practical experience with Infrastructure as Code using Terraform and Docker. I successfully provisioned an NGINX Docker container using Terraform, verified the application through a browser, inspected the Terraform state, and destroyed the infrastructure after completing the deployment.

