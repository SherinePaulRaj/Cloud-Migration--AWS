
# Cloud Security Architecture on AWS

## Author

- **Sherine Paul Raj**
- UID: 119362921
- Email: sherpaul@umd.edu

## Problem Statement

The CobraKai team recognized the importance of migrating to the cloud. This project discusses the implementation of cloud architecture and associated services to enhance the security and scalability of the CobraKai infrastructure using AWS.

## Table of Contents

1. [Virtualizing the Network Architecture](#virtualizing-the-network-architecture)
2. [Security Best Practices](#security-best-practices)
3. [Resource Monitoring and Cost Management](#resource-monitoring-and-cost-management)
4. [Conclusion](#conclusion)

## Virtualizing the Network Architecture

1. **Creating a VPC**:
   - Define and configure a Virtual Private Cloud (VPC) using AWS's VPC dashboard.
   - Specify the IP range to ensure the network functions within a controlled environment.

2. **Internet Gateway**:
   - Attach an Internet Gateway to enable virtual servers to connect to the internet.

3. **Subnets**:
   - Divide the VPC's CIDR range into smaller subnets for enhanced availability.
   - Create multiple subnets (e.g., for web and app servers) with different IP address ranges.

4. **Routing Tables**:
   - Configure routing tables to efficiently direct internet traffic to and from the subnets.

5. **Security Groups & Network ACLs**:
   - Apply security groups to control inbound and outbound traffic at the instance level.
   - Utilize Network ACLs to provide an additional layer of security at the subnet level.

## Security Best Practices

- **IAM Role Management**:
  - Create specific IAM roles for different teams, ensuring the principle of least privilege.
- **Data Encryption**:
  - Encrypt data at rest using AWS Key Management Service (KMS) and in transit using TLS.
- **Monitoring & Logging**:
  - Enable AWS CloudTrail and AWS CloudWatch for tracking activities and maintaining logs.

## Resource Monitoring and Cost Management

- **AWS Trusted Advisor**:
  - Use AWS Trusted Advisor to optimize performance and monitor cloud usage.
- **Cost Allocation Tags**:
  - Implement tagging to manage and track resource usage and expenses efficiently.

## Conclusion

The project outlines the steps for setting up a secure cloud architecture on AWS, addressing the network structure, security practices, and monitoring mechanisms. By following these guidelines, CobraKai can leverage the cloud's flexibility and scalability while maintaining robust security.
