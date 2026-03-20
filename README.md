# aws-mysecure-vpc-architecture
# Secure VPC Architecture with Bastion Host

## Objective
I designed and implemented a secure AWS VPC architecture with controlled access to private resources.

## Architecture 
(MY VPC aRCHITECTURE(2).jpg)

## Services Used
- VPC
- EC2
- Security Groups
- Internet Gateway

## Network Design

- Public Subnet (10.0.1.0/24)
- Private Subnet (10.0.2.0/24)
- Bastion host in public subnet
- Private EC2 in private subnet

## Security Controls

- SSH access restricted to trusted IP
- Private EC2 has no public IP
- Access only via bastion host
- Network segmentation enforced

## Validation

- Direct SSH to private EC2 blocked
- SSH via bastion successful
- Private EC2 has no internet access

## Lessons Learned

- Importance of subnet isolation
- How bastion hosts secure access
- Role of route tables in defining public/private subnets
