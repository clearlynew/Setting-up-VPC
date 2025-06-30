# AWS Networking Architecture Projects

**By Hima Prasobh**  
A step-by-step collection of 9 connected AWS networking projects. These projects build on each other and helped me understand how to create, secure, connect, and monitor my own cloud network. Each project takes approximately 30 mins.

---

## 1. Build a Virtual Private Cloud  
**Goal:** Create the foundation of your network  
- Set up a custom VPC with a defined CIDR block (e.g. `10.0.0.0/16`)  
- Create subnets across different Availability Zones  
- Attach an internet gateway  

---

## 2. VPC Traffic Flow and Security  
**Goal:** Control traffic in your network  
- Set up route tables for public and private subnets  
- Configure security groups and network ACLs  
- Understand the difference between stateful and stateless filtering  

---

## 3. Creating a Private Subnet  
**Goal:** Isolate resources in your VPC  
- Create private subnets without internet access  
- Remove route to internet gateway  
- Launch instances in private subnets  

---

## 4. Launching VPC Resources  
**Goal:** Add servers and services to your network  
- Deploy EC2 instances in both public and private subnets  
- Use security groups to control access  
- Enable auto-assign public IPs for public subnet instances  

---

## 5. Testing VPC Connectivity  
**Goal:** Verify communication inside and outside the VPC  
- Connect to public EC2 via SSH  
- Use it as a Bastion Host to reach private EC2  
- Test ping, curl, or package installs for internet connectivity  

---

## 6. VPC Peering  
**Goal:** Connect multiple VPCs  
- Create two VPCs in the same region  
- Set up VPC peering  
- Update route tables to allow private communication between them  

---

## 7. VPC Monitoring with Flow Logs  
**Goal:** Monitor network traffic  
- Enable VPC Flow Logs to capture IP traffic  
- Send logs to CloudWatch Logs  
- Analyze patterns and spot denied traffic  

---

## 8. Access S3 from a VPC  
**Goal:** Securely connect to AWS storage services  
- Use a private EC2 instance to access S3  
- Test access with and without internet  
- Understand when NAT Gateways or Endpoints are needed  

---

## 9. VPC Endpoints  
**Goal:** Optimize private connections to AWS services  
- Create an Interface VPC Endpoint for services like S3 or DynamoDB  
- Remove internet access and still maintain service access  
- Improve security and reduce data transfer costs  

---

## Summary

These projects guided me through building a secure, scalable, and observable network on AWS using VPCs. I practiced designing network architecture, isolating and securing resources, enabling service access, and tracking traffic. This hands-on experience gave me a strong foundation in cloud networking.
