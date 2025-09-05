\# NextWork AWS Networking Project 2 – VPC Traffic Flow and Security



\## ✅ Project Overview

In this project, I learned to \*\*configure VPC traffic flow and security\*\*.  

This involved creating/modifying \*\*route tables\*\*, making one subnet public and another private, setting up \*\*Security Groups\*\* and \*\*Network ACLs\*\*, and verifying the setup with a test EC2 instance.



\## 🛠 Key Services and Concepts

\- \*\*Amazon VPC\*\* – Private, isolated network for resources  

\- \*\*Subnets\*\* – Public vs private sections in the VPC  

\- \*\*Internet Gateway\*\* – Connects public subnet to the internet  

\- \*\*Route Tables\*\* – Directs traffic within and outside the VPC  

\- \*\*Security Groups\*\* – Acts as a virtual firewall for resources  

\- \*\*Network ACLs (NACLs)\*\* – Subnet-level traffic control  



\## 🔧 Steps Completed



\### Step 0 – Prep

Understand project goals: configure traffic flow, security, subnets, and verify with EC2.



\### Step 1 – Set up VPC basics

Created a VPC, added subnets, and attached an internet gateway to allow public internet access.



\### Step 2 – Create Route Table

Created a route table and associated it with the public subnet.  

\*\*New route destination:\*\* `0.0.0.0/0`  

\*\*Target:\*\* Internet Gateway (NextWork IG)  



!\[Route Table](screenshots/route-table.png)



\### Step 3 – Create Security Group

Created a security group for controlling traffic to resources.  

\*\*Inbound rule:\*\* HTTP from Anywhere (0.0.0.0/0)  

\*\*Outbound rules:\*\* All traffic allowed by default  



!\[Security Group](screenshots/security-group.png)



\### Step 4 – Create Network ACL

Created a custom Network ACL and associated it with the public subnet.  

\*\*Inbound/Outbound rule:\*\* Allow all traffic (Rule 100)  



!\[Network ACL](screenshots/network-acl.png)



\## 📂 Project Files

\- Documentation: \[`docs/steps-guide.pdf`](docs/steps-guide.pdf)  

\- Screenshots: `screenshots/security-group.png`, `screenshots/route-table.png`, `screenshots/network-acl.png`



\## ⏱ Time Taken

This project took approximately \*\*2 hours\*\*.  

Most challenging part: Understanding route table logic.  

Most rewarding part: Seeing traffic flow correctly and subnet become public.



\## 💡 Reflection

This project strengthened my understanding of \*\*AWS networking and security best practices\*\*, including the use of route tables, security groups, and network ACLs.  

I now have a working public subnet connected to the internet, secured by a security group and network ACL, ready for hosting an EC2 instance or web app.



