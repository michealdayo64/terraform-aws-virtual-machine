# Terraform AWS VM

## Project Description
This project contains Terraform code to provision a virtual machine (VM) on Amazon Web Services (AWS). The VM can be used for various purposes, such as hosting applications, running scripts, or testing configurations.

The project includes Terraform configuration files that define the necessary resources, such as EC2 instances, security groups, and networking components. It also includes a `.gitignore` file to exclude sensitive files and directories from version control.

## Infrastructure Architecture
The infrastructure architecture consists of the following components:
- **VPC (Virtual Private Cloud)**: A logically isolated network in AWS where the VM will be deployed.
- **Availability Zones**: Physical locations within a region where AWS resources can be deployed.   
- **Subnet**: A segment of the VPC that allows you to group resources based on security and operational needs.
- **EC2 Instance**: A virtual machine running on AWS, which can be configured with specific instance types, AMIs, and other settings.
- **Security Groups**: Firewall rules that control inbound and outbound traffic to the EC2 instance

## Terraform Rules
1. inspect the main.tf file to understand the resources being created and their configurations.
2. Do not modify the Terraform state files (`terraform.tfstate` and `terraform.tfstate.backup`) directly. Use Terraform commands to manage the state.
3. Do not duplicate resources unnecessarily. Reuse existing resources when possible to avoid conflicts and maintain a clean infrastructure.
4. preserve the terraform state files in the `.gitignore` file to prevent sensitive information from being exposed in version control.
5. run the following commands to initialize and validate the Terraform configuration:
```bash
terraform init
terraform validate
terraform plan
```
6. never automatically run `terraform apply` and `terraform destroy` without explicit approval.