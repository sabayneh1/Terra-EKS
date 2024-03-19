# Kubernetes EKS Cluster Deployment with Terraform

This project contains Terraform configurations for deploying a highly available Amazon EKS (Elastic Kubernetes Service) cluster with custom modules for VPC, IAM roles, EKS cluster configuration, and worker node management. It also includes a data source for fetching an EKS authentication token and configures the Kubernetes provider to interact with the cluster.

## Prerequisites

- AWS Account and CLI: Ensure you have an AWS account and have configured the AWS CLI with the necessary permissions.
- Terraform: Ensure Terraform is installed on your machine.
- kubectl: Required for interacting with the Kubernetes cluster.
- jq: Used for processing JSON data in command line scripts.
- AWS IAM Authenticator: Required for authentication to the EKS cluster.

## Project Structure

- `modules/`: Contains the custom modules used for the EKS cluster deployment.
  - `vpc/`: Defines the VPC configuration for the EKS cluster.
  - `iam-roles/`: Manages the IAM roles required for EKS.
  - `eks-cluster/`: Configures the EKS cluster.
  - `eks-worker-nodes/`: Manages the EKS worker nodes.

- `main.tf`: The main Terraform configuration file for deploying the EKS cluster.
- `variables.tf`: Defines the variables used in the configurations.
- `outputs.tf`: Specifies the output information from the Terraform deployment.
- `README.md`: This file, providing documentation and instructions.

## Setup and Deployment

1. **Initialize Terraform**:

terraform init

2. **Review Terraform**:
   
 terraform plan

3. **APPLY Terraform**:

 terraform apply

