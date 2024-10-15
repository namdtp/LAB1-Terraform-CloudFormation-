# LAB1 - Using Terraform and CloudFormation to manage and deploy AWS infrastructure
This project made by group 22 - CLASS Code : NT548.P11  
Menber : 
| No. | Name | ID | Task |
|-------|-------|-------|-------|
| 01 | Đỗ Trần Phương Nam | 19520742 | Cloudformation |
| 02 | Nguyễn Trọng Nhân | 19520801 | Terraform |

## Task requirements:

### 1. VPC: Create a VPC that includes the following components :  
- Subnets: include Public Subnet (connect Internet Gateway) and Private Subnet (using NAT Gateway for connect to network).  
- Internet Gateway: Conecet Public Subnet to allow internal resources to access Internet.  
- Default Security Group: create Security Group defaul for VPC  
### 2. Route Tables: Create Route Tables for Public and Private Subnet  
 - Public Route Table: Route Internet traffic via Internet Gateway.
- Private Route Table: Route Internet traffic via NAT Gateway.
### 3. EC2: Create instances in Public và Private Subnet, make sure Public instance is allowed accessible from the Internet, while Private instances can only be accessed from Public instances via SSH or other secure methods.
### 4.Security Groups: Create Security Groups to control traffic in/out of the EC2 instances  
- Public EC2 Security Group: Only allow SSH connections (port 22) from a specific IP (or user's IP)  
- Private EC2 Security Group: Allows connection from Public EC2 instance via necessary port (SSH or other ports if needed).
