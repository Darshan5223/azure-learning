AZ-104 – LAB 04 (TASK 1)
FULL DETAILED NOTES (PDF CONTENT)

Below is the final, polished content that should go into your PDF.

1️⃣ Lab Title

AZ-104 – Lab 04: Implement Virtual Networking
Task 1: Create CoreServicesVnet

2️⃣ Objective

Design and deploy a scalable Azure Virtual Network with proper IP address planning and subnet segmentation to support enterprise workloads and future growth.

3️⃣ Why This Task Is Important

Virtual networking is the foundation of all Azure workloads. Poor network design leads to IP conflicts, security issues, and costly redesigns. This task introduces best practices for planning, subnetting, and future scalability.

4️⃣ Configuration Summary

Virtual Network Name: CoreServicesVnet

Resource Group: az104-rg4

Region: East US

Address Space: 10.20.0.0/16

Subnets:

SharedServicesSubnet – 10.20.10.0/24

DatabaseSubnet – 10.20.20.0/24

5️⃣ Key Concepts Explained
Azure Virtual Network (VNet)

A VNet is a logically isolated private network in Azure that enables communication between Azure resources such as virtual machines, databases, and services.

IP Address Planning (CIDR)

The CIDR block 10.20.0.0/16 provides 65,536 IP addresses, allowing significant room for future expansion. Choosing a larger address space early avoids reconfiguration later.

Subnet Design

Subnets divide a VNet into logical segments. Separating shared services and databases improves security, performance, and manageability.

Azure Reserved IP Addresses

Azure reserves five IP addresses in each subnet for platform services. This must be considered when designing subnet sizes.

6️⃣ Infrastructure as Code (Export Template)

After creating the virtual network via the Azure portal, the configuration was exported as an ARM template. This enables reuse, automation, and consistency across environments.

7️⃣ Interview-Ready Questions & Answers

Q: What is an Azure Virtual Network?
A: A private, isolated network in Azure that enables secure communication between resources.

Q: Why is CIDR planning important?
A: It prevents IP exhaustion and overlapping address space issues.

Q: Why use a /16 address space for core services?
A: To support long-term scalability and multiple subnets.

Q: Why separate subnets for services and databases?
A: For security isolation and traffic management.

Q: Why export the ARM template?
A: To enable Infrastructure as Code and repeatable deployments.

8️⃣ Key Takeaways

Proper virtual network design is critical for scalable and secure Azure environments. Task 1 establishes the foundation for advanced networking concepts such as NSGs, ASGs, DNS, and hybrid connectivity.