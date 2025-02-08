# Terraform AWS VPC & EC2 Setup

This Terraform project provisions an AWS infrastructure with the following:
- A VPC with CIDR '10.0.0.0/16'
- Three public subnets across different availability zones
- Three private subnets across different availability zones
- An Internet Gateway for public subnet connectivity
- A NAT Gateway for private subnet internet access
- A Security Group allowing HTTP (port 80) traffic
- An EC2 instance deployed in a public subnet

The EC2 instance can be accessed via its public IP.

## Prerequisites

Ensure you have the following installed:

- Terraform (">= 1.0")
- AWS CLI (">= 2.0")
- An AWS account with appropriate IAM permissions
- A configured AWS profile ("aws configure")

## Deployment Steps

1. Clone the repository:
   
   git clone https://github.com/your-repo/terraform-aws-vpc.git
   cd terraform-aws-vpc

2. Initialize Terraform:
	terraform init

3. Review the execution plan:
	terraform plan

4. Apply the configuration:
	terraform apply -auto-approve

