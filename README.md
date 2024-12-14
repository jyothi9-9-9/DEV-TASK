# Cloud & DevOps Engineer Assessment - Web Application Deployment on EKS

This repository contains the solution for deploying a simple web application on AWS EKS using Kubernetes. The application is exposed via an AWS LoadBalancer.

## Steps to Deploy the Solution

1. **Set up AWS Infrastructure:**
   - Use Terraform to provision the AWS infrastructure.
   - Run `terraform init` and `terraform apply` to create the necessary resources.

2. **Build and Push Docker Image:**
   - Build the Docker image for the web application.
   - Push it to Docker Hub or Amazon ECR.

3. **Deploy to Kubernetes:**
   - Apply the Kubernetes deployment and service YAML files to the EKS cluster.
   - `kubectl apply -f deployment.yaml`
   - `kubectl apply -f service.yaml`

4. **Verify the Web Application:**
   - Once the LoadBalancer is provisioned, access the web app using the external DNS name or IP.

## Technologies Used

- AWS (EKS, IAM, VPC, EC2)
- Kubernetes
- Terraform
- Docker
- Helm
- Prometheus & Grafana (For monitoring)

