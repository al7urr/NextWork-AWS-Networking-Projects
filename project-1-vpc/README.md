# NextWork AWS Networking Project 1 – Build a VPC

## ✅ Project Overview
In this project, I learned to **create a Virtual Private Cloud (VPC)** and connect it to the internet.  
I divided the VPC into **subnets** and then attached an **internet gateway** so resources inside the VPC could communicate with the outside world.

![Step 1: VPC Settings](project-1-vpc/screenshots/vpc-settings)

## 🛠 Key Services and Concepts
- **Amazon VPC** – Isolating resources inside a private virtual network.  
- **Subnets** – Dividing the VPC into smaller sections (public vs private).  
- **CIDR Blocks** – Defining the IP address ranges for VPCs and subnets.  
- **Internet Gateway** – Allowing communication between the VPC and the internet.  
- **Availability Zones** – Placing resources across multiple AZs for reliability.  

![Step 2: Subnet Settings](project-1-vpc/screenshots/subnet-settings)

## 🔧 Steps Completed
1. **Created a VPC** with a CIDR block to define its private IP range.  
2. **Created a subnet** inside the VPC, linked to a specific Availability Zone.  
3. **Attached an Internet Gateway** to the VPC to enable internet access.  

![Step 3: Internet Gateway](project-1-vpc/screenshots/internet-gateway

## 📌 Key Learnings
- Why **VPCs are essential** for secure and organized cloud networking.  
- How **subnets** help separate resources by purpose (public vs private).  
- How an **internet gateway** connects private AWS resources to the internet.  
- The role of **Availability Zones** in improving reliability.  

## ⏱ Time Taken
This project took approximately **1 hour**.  
The most challenging part was **understanding CIDR blocks**, and the most rewarding part was **seeing the VPC fully connected to the internet**.

## 💡 Reflection
I chose this project to **build a strong foundation in AWS networking**.  
It gave me hands-on experience in **network design, security, and connectivity**, which will be essential for the upcoming projects in this series.

## 📂 Project Files
- Documentation: [`steps.md`](project-1-vpc/docs/steps.md)  
- Screenshots are in the `screenshots` folder.  

