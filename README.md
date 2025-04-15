# AWS_Network_Architecture

<img src="https://github.com/user-attachments/assets/92a29457-5e65-4ce0-9eae-0e8053bc2cd4" alt="Networking" width="400"/>


This project demonstrates the implementation of a **secure and efficient Virtual Private Cloud (VPC)** architecture on AWS, using both public and private subnets across multiple Availability Zones. The architecture follows AWS best practices for **isolation, controlled access, and high availability**.

## 🚀 Project Overview

- **Multi-AZ Deployment**: VPC spans multiple Availability Zones to ensure high availability and fault tolerance.
- **Public Subnet**: Contains an EC2 instance accessible from the internet via an **Internet Gateway (IGW)**.
- **Private Subnet**: Hosts an EC2 instance that is **isolated from direct internet access**, enhancing security.
- **NAT Gateway**: Enables instances in the private subnet to initiate outbound internet connections **securely**.
- **Custom Route Tables**:
  - Public subnet routes traffic through the **IGW**.
  - Private subnet routes traffic through the **NAT Gateway**.

## 🔧 Key Components

- Amazon VPC
- Public and Private Subnets
- Internet Gateway (IGW)
- NAT Gateway
- Route Tables
- EC2 Instances
- Availability Zones (Multi-AZ)

## 🔐 Security & Best Practices

- **Network Isolation**: Separate public and private subnets to isolate internet-facing and internal resources.
- **Controlled Internet Access**: Use of NAT Gateway ensures only **outbound** internet access from private resources.
- **High Availability**: Subnets and gateways are distributed across multiple Availability Zones to minimize downtime.

## 📚 Use Cases

- Hosting secure backend services or databases in a private subnet.
- Deploying public-facing web servers while keeping internal services isolated.
- Creating a scalable and production-ready AWS network foundation.

