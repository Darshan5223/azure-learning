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

## Task 2: Create ManufacturingVnet using ARM Template (Completed)

### Summary
- Reused exported ARM template from Task 1
- Modified address space and subnet ranges
- Deployed ManufacturingVnet using Infrastructure as Code
- Validated network isolation and deployment success

### Configuration
- Virtual Network: ManufacturingVnet
- Address Space: 10.30.0.0/16
- Subnets:
  - SensorSubnet1 (10.30.20.0/24)
  - SensorSubnet2 (10.30.21.0/24)
- Region: East US

### Concepts Covered
- Infrastructure as Code (ARM Templates)
- Reusable network deployments
- CIDR-based address planning
- Environment isolation

### Documentation
- 📄 **Detailed Notes:**  
  Documented as part of Lab 04 Task 2

---

## Task 3: Configure NSG and ASG Communication (Completed)

### Summary
- Implemented subnet-level security using Network Security Groups
- Used Application Security Groups for scalable rule management
- Allowed inbound HTTP/HTTPS traffic from ASG
- Denied outbound internet traffic

### Concepts Covered
- NSG rule evaluation
- ASG-based security
- Inbound and outbound traffic control

---

## Task 4: Configure Public and Private Azure DNS (Completed)

### Summary
- Created public DNS zone with A records
- Created private DNS zone for internal name resolution
- Linked private DNS zone to ManufacturingVnet
- Verified DNS resolution

### Concepts Covered
- Public vs Private DNS
- DNS record sets
- VNet DNS linking

---

## Lab Status
- Task 1: ✅ Completed
- Task 2: ✅ Completed
- Task 3: ✅ Completed
- Task 4: ✅ Completed

