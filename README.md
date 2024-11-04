README.md
# VPC Setup for a Web Application

## Project Overview
This project sets up a Virtual Private Cloud (VPC) on AWS using Terraform. It includes public and private subnets, an internet gateway, and route tables to manage traffic.

## Objectives
- Create a VPC with public and private subnets.
- Configure an Internet Gateway for external access.
- Set up route tables for public and private subnets.

## Terraform Configuration
The Terraform code is located in `main.tf` and includes:
- VPC creation with a CIDR block of `10.0.0.0/16`.
- Two public subnets and two private subnets across different availability zones.
- An internet gateway attached to the VPC.
- Route tables for managing traffic.

## How to Deploy
1. Ensure you have [Terraform](https://www.terraform.io/downloads.html) installed.
2. Configure your AWS credentials.
3. Run `terraform init` to initialize the project.
4. Run `terraform plan` to see what will be created.
5. Run `terraform apply` to create the resources.

## Cleanup
To remove all resources, run:
```bash
terraform destroy