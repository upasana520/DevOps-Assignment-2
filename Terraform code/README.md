# AWS VPC Creation with Terraform
This module creates a VPC alongside a variety of related resources, including:

- Public and private subnets
- Public and private route tables
- Elastic IPs
- Network Interfaces
- NAT Gateways
- An Internet Gateway
- A VPC Endpoint
- A bastion EC2 instance




Modules:

- ssh-key: Generates an ssh key pair
- network: Sets up a VPC with IGWs, NAT GWs, 2 public subnets, 2 private subnets, Elastic IPs,Bastion EC2 instance, Elastic IP
- ec2: Currently creates ec2 instance in a public subnet and ec2 instance in a private subnet
- each subnet is in a different AZ
- ALB: This module creates ALB in AWS,Target Group.
- private key is copied over to the bastion ec2 instance so it can ssh into the private subnet
- ec2 in private subnet has outgoing network access though the NAT gateway
- 


