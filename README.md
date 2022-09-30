# Amazon EKS using Terraform

**This project provides you how to setup a Kubernetes Cluster on AWS using Terraform **

versions.tf sets the Terraform version. It also sets versions for the providers used by the configuration.

variables.tf contains a region variable that controls where to create the EKS cluster.

vpc.tf provisions a VPC, subnets, and availability zones using the AWS VPC Module. 

security-groups.tf provisions the security groups the EKS cluster will use.

eks-cluster.tf uses the AWS EKS Module to provision an EKS cluster and other required resources, including Auto Scalling Groups, Security Groups, IAM Roles and IAM Policies.

outputs.tf defines the output values for this configuration.

main.tf describes everything about the cluster.