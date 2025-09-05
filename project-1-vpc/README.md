# NextWork AWS Networking Project 2 – VPC Traffic Flow and Security

## ✅ Project Overview
In this project, I learned to **configure VPC traffic flow and security**.  
I created **route tables**, made a subnet public, set up **Security Groups** and **Network ACLs**, and verified the setup using a public subnet.

![Step 1: Route Table Settings](screenshots/route-table.png)

## 🛠 Key Services and Concepts
- **Amazon VPC** – Isolating resources inside a private virtual network.  
- **Subnets** – Dividing the VPC into public and private sections.  
- **Route Tables** – Directing traffic inside the VPC and to the internet.  
- **Security Groups** – Resource-level firewall controlling inbound/outbound traffic.  
- **Network ACLs (NACLs)** – Subnet-level traffic control for extra security.  
- **Internet Gateway** – Connecting public subnet resources to the internet.  

![Step 2: Security Group Settings](screenshots/security-group.png)

## 🔧 Steps Completed
1. **Created a route table** for the public subnet.  
   - New route destination: `0.0.0.0/0`  
   - Target: Internet Gateway (NextWork IG)  

2. **Created a security group** for controlling traffic to resources.  
   - Inbound rule: HTTP from Anywhere (0.0.0.0/0)  
   - Outbound rules: All traffic allowed by default  

3. **Created a custom Network ACL** and associated it with the public subnet.  
   - Inbound and Outbound rule: Allow all traffic (Rule 100)  

![Step 3: Network ACL Settings](screenshots/network-acl.png)

## 📌 Key Learnings
- How **route tables** control traffic flow within VPC and to the internet.  
- The difference between **Security Groups** (resource-level) and **Network ACLs** (subnet-level).  
- How **public subnets** communicate with the internet through an Internet Gateway.  
- Understanding inbound and outbound rules for both security groups and NACLs.  

## ⏱ Time Taken
This project took approximately **2 hours**.  
The most challenging part was **understanding route table and NACL logic**, and the most rewarding part was **seeing the subnet become public and accessible via HTTP**.

## 💡 Reflection
I chose this project to **strengthen my AWS networking skills**.  
It gave me hands-on experience in **traffic management, subnet security, and access control**, which is essential for hosting applications securely in AWS.

## 📂 Project Files
- Documentation: [`docs/steps-guide.pdf`](docs/steps-guide.pdf)  
- Screenshots are in the `screenshots` folder:
  - `security-group.png`  
  - `route-table.png`  
  - `network-acl.png`
