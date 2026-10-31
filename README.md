# AWS-Internship-VPC-Peering
AWS Cloud Infrastructure lab implementing a secure cross-VPC network architecture using VPC Peering, customized private route tables, stateful Security Groups, and multi-hop SSH proxy jump validation.
# AWS Internship - VPC Peering & Network Security Project

## 📋 Project Architecture
- **VPC-A:** `10.10.0.0/16` with Public Subnet (`10.10.1.0/24`) and Private Subnet (`10.10.2.0/24`)
- **VPC-B:** `10.20.0.0/16` with Private Subnet (`10.20.1.0/24`)
- **Peering Connection:** `ewb-a-b-peer` linking VPC-A and VPC-B securely
- **Compute nodes:** 1 Public Bastion Host (`10.10.1.10`), 2 Private App Instances (`10.10.2.10` & `10.20.1.10`)

## 🔍 Validation Logs
The architecture was validated via an internal ICMP ping test from `ewb-app-a` to `ewb-app-b` across the peering bridge, achieving **0% packet loss** under symmetric routing configurations.

*All structural verification images, including the EC2 dashboard configurations, active peering states, and successful terminal outputs, are uploaded directly within this repository.*
