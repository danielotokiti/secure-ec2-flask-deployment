# Day 3 – Custom VPC, Bastion Host, and Private EC2

Tasks Completed:
- Created a custom VPC with CIDR block `10.0.0.0/16`
- Created two subnets:
  - Public Subnet: `10.0.1.0/24`
  - Private Subnet: `10.0.2.0/24`
- Created and attached an Internet Gateway to the VPC
- Configured a Route Table for the Public Subnet with route to IGW
- (Optional) Created NAT Gateway for Private Subnet internet access
- Launched a **Bastion Host EC2** in the Public Subnet
- Launched a **Private EC2** instance in the Private Subnet
- Created Security Groups:
  - Bastion SG: Allow SSH from my IP
  - Private SG: Allow SSH only from Bastion’s SG
- Successfully connected to the Private EC2 via SSH through the Bastion

## Screenshots:
- VPC summary page showing CIDR
- Subnet list (Public + Private) with CIDRs
- Internet Gateway page showing attachment
- Route table with 0.0.0.0/0 → IGW for Public Subnet
- NAT Gateway config (if used)
- Route table for Private Subnet (0.0.0.0/0 → NAT GW)
- EC2 Instance Summary: Bastion Host
- EC2 Instance Summary: Private EC2
- Security Group rules for Bastion and Private instances
- Terminal screenshot: SSH from local → Bastion → Private EC2
