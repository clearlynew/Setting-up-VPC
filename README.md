# AWS Networking Architecture Projects

**By Hima Prasobh**  
A step-by-step collection of 9 connected AWS networking projects. These projects build on each other and helped me understand how to create, secure, connect, and monitor my own cloud network. Each project takes approximately 30 minutes to complete.

---

## 1. Build a Virtual Private Cloud  
**Goal:** Create the foundation of your network  
- Set up a custom VPC with a defined CIDR block (e.g., `10.0.0.0/16`)  
- Create subnets in an Availability Zone  
- Attach an internet gateway for connectivity  

---

## 2. VPC Traffic Flow and Security  
**Goal:** Control traffic in your network  
- Create route tables and associate them with subnets  
- Configure security groups to allow HTTP traffic  
- Use network ACLs to control traffic at the subnet level  

---

## 3. Creating a Private Subnet  
**Goal:** Isolate resources in your VPC  
- Create a subnet with no route to the internet  
- Leave the default network ACL (denies all traffic)  
- Keep the subnet fully private for internal-only resources  

---

## 4. Launching VPC Resources  
**Goal:** Add servers and services to your network  
- Launch EC2 instances in both public and private subnets  
- Attach security groups for HTTP access  
- Enable auto-assign public IPs for instances in public subnets  

---

## 5. Testing VPC Connectivity  
**Goal:** Verify communication within the VPC and with the internet  
- Connect to EC2 in the public subnet using SSH  
- Use it as a Bastion Host to reach private instances  
- Test internet access with `ping` and `curl` commands  

---

## 6. VPC Peering  
**Goal:** Connect multiple VPCs together  
- Create two VPCs in the same region  
- Set up a VPC peering connection  
- Update route tables to allow private cross-VPC communication  

---

## 7. VPC Monitoring with Flow Logs  
**Goal:** Track and analyze network traffic  
- Enable VPC Flow Logs to capture traffic metadata  
- Send logs to Amazon CloudWatch  
- Monitor accepted and rejected traffic across subnets  

---

## 8. Access S3 from a VPC  
**Goal:** Securely connect to AWS storage services from within a VPC  
- Access S3 from a private EC2 instance  
- Test access with and without internet connectivity  
- Understand the need for NAT Gateways or VPC Endpoints  

---

## 9. VPC Endpoints  
**Goal:** Optimize private access to AWS services  
- Create an Interface VPC Endpoint (PrivateLink)  
- Access S3 or DynamoDB without a public IP or NAT  
- Improve security and reduce data transfer costs  

---

## Summary

These projects guided me through building a secure, scalable, and observable network on AWS using VPCs. I gained hands-on experience designing cloud architecture, isolating and securing resources, enabling service access, and monitoring network activity. This helped build a strong foundation in cloud networking.
