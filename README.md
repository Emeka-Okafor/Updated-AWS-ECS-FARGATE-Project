# AWS ECS Fargate Deployment with Terraform

This project demonstrates how to deploy a containerized application on AWS using Terraform and ECS Fargate.

## Architecture

The infrastructure includes:

- Custom VPC
- Public and private subnets
- Internet Gateway
- NAT Gateway
- Application Load Balancer
- ECS Fargate cluster
- Amazon ECR repository
- Auto scaling
- CloudWatch logging

## Infrastructure as Code

Terraform is used to provision the entire AWS infrastructure.

Location:

terraform/main.tf

## Container

The application container is built using a Dockerfile.

## CI/CD Pipeline

The `pipelines` directory contains an example GitHub Actions workflow that:

- Builds a Docker image
- Pushes the image to Amazon ECR
- Deploys the container to ECS

This pipeline is included for demonstration purposes.

## Technologies Used

- Terraform
- AWS ECS Fargate
- Amazon ECR
- Application Load Balancer
- Docker
- GitHub Actions