# AZ-104 Lab 04 – Implement Virtual Networking

## Objective
Design and implement Azure virtual networking with proper IP planning, subnetting,
and scalability to support enterprise workloads.

---

## Task 1: Create CoreServicesVnet (Completed)

### Summary
- Created a core Azure Virtual Network using the Azure Portal
- Designed a scalable IP addressing scheme using CIDR notation
- Implemented subnet segmentation for shared services and database workloads
- Avoided overlapping IP address ranges
- Exported the Virtual Network configuration as an ARM template for future reuse

### Configuration Details
- **Virtual Network Name:** CoreServicesVnet  
- **Resource Group:** az104-rg4  
- **Region:** East US  
- **Address Space:** 10.20.0.0/16  

**Subnets**
- **SharedServicesSubnet:** 10.20.10.0/24  
- **DatabaseSubnet:** 10.20.20.0/24  

### Concepts Covered
- Azure Virtual Networks
- IP Address Planning (CIDR)
- Subnet Design and Segmentation
- Azure Reserved IP Addresses
- Network Design Best Practices
- Infrastructure as Code (Export ARM Template)

### Key Learnings
- Proper IP planning prevents future network redesign
- Larger address spaces support scalability
- Subnets enable workload isolation and security
- Any Azure resource can be represented as code

### Documentation
- 📄 **Detailed Notes (PDF):**  
  `AZ104_Lab04_Task01_Virtual_Networking_Notes.pdf`

---

## Status
- Task 1: ✅ Completed
- Task 2: ⏳ Pending
- Task 3: ⏳ Pending
- Task 4: ⏳ Pending
