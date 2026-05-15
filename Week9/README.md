# Azure Environment Technical Documentation

## Overview

This document provides a detailed description of the Azure environment created throughout the project. It includes all deployed resources, their configurations, and how they interact within the system.

---

## Resource Group

- Name: NET731-RG  
- Region: South Africa North  

### Purpose
The resource group is used to logically group all Azure resources for easier management, monitoring, and access control.

---

## Virtual Network

- Name: week5-vnet  
- Region: South Africa North  
- Address Space: 10.50.0.0/16  

### Purpose
Provides network isolation and allows resources to communicate securely.

### Key Configuration
- Subnet: backend-subnet  
- Address range: 10.50.1.0/24  

### Dependencies
- Connected to Virtual Machine  
- Protected by Network Security Group  

---

## Network Security Group (NSG)

- Name: nsg-net731  
- Region: South Africa North  

### Purpose
Controls inbound and outbound traffic to the virtual machine at the network level.

### Key Configuration
- Inbound Rules:
  - Allow SSH (Port 22)  
  - Allow HTTP (Port 80)  
- Outbound:
  - Allow Internet access  

### Dependencies
- Attached to backend-subnet  
- Protects Virtual Machine traffic  

---

## Virtual Machine

- Name: week3-vm  
- Region: South Africa North  
- Size: B2ts_v2  
- OS: Ubuntu Server 22.04 LTS  

### Purpose
Provides compute resources to run workloads and generate monitoring data.

### Key Configuration
- Connected to backend-subnet  
- Public IP enabled  
- SSH access configured  

### Dependencies
- Depends on Virtual Network + Subnet  
- Uses NSG for security  
- Monitored by Azure Monitor  

---

## Storage Account

- Name: net731storage  
- Region: South Africa North  
- Tier: Standard (LRS)  

### Purpose
Stores data and provides blob storage for files.

### Key Configuration
- Containers:
  - internal-docs  
  - public-assets  
- Private access enabled  
- SAS token created for access  

### Dependencies
- Used by applications and users  
- Integrated with Azure security practices  

---

## Azure Monitor

### Purpose
Tracks performance and provides insights into resource usage.

### Key Configuration
- Metrics monitored:
  - CPU usage  
  - Network In/Out  
- Alerts configured:
  - CPU > 80%  

### Dependencies
- Monitors Virtual Machine  
- Connected to Log Analytics Workspace  

---

## Log Analytics Workspace

- Name: week7-law  
- Region: South Africa North  

### Purpose
Centralised logging solution for collecting diagnostic data.

### Key Configuration
- Receives logs from:
  - Network Security Group  
  - Virtual Network  
- Used for querying logs  

### Dependencies
- Integrated with Azure Monitor  
- Receives diagnostics from network resources  

---

## Cost Management (Budget)

- Name: week8-budget  
- Scope: Subscription  
- Budget: $100/month  

### Purpose
Monitors and controls cloud spending.

### Key Configuration
- Alert thresholds:
  - 80% (Actual)  
  - 100% (Forecasted)  
- Email notifications enabled  

### Dependencies
- Linked to Azure subscription  
- Works with Cost Analysis  

---

## Interdependencies Summary

- The Virtual Machine depends on the Virtual Network and Subnet for connectivity.  
- The Network Security Group secures traffic to the Virtual Machine.  
- Azure Monitor collects metrics from the Virtual Machine.  
- Log Analytics Workspace collects logs from NSG and VNet.  
- Storage Account stores application data.  
- Cost Management monitors spending across all resources.  

---

## Conclusion


Task 2:
## Section 2: Security Configuration

### Network Security Group (NSG) Rules

A Network Security Group (NSG) was configured to control traffic to the virtual machine.

#### Inbound Rules:
- Allow SSH  
  - Direction: Inbound  
  - Port: 22  
  - Protocol: TCP  
  - Source: Any  
  - Purpose: Allows secure remote access to the virtual machine  

- Allow HTTP  
  - Direction: Inbound  
  - Port: 80  
  - Protocol: TCP  
  - Source: Any  
  - Purpose: Allows web traffic to reach the virtual machine  

#### Outbound Rules:
- Allow Internet Traffic  
  - Direction: Outbound  
  - Destination: Internet  
  - Purpose: Enables the virtual machine to access external services and updates  

These rules ensure that only required traffic is permitted, improving security by reducing the attack surface.

---

### Identity and Access Management (RBAC)

Role-Based Access Control (RBAC) was implemented to manage user permissions:

- user-ops  
  - Role: Contributor  
  - Purpose: Manage and configure Azure resources  

- user-audit  
  - Role: Reader  
  - Purpose: View resources without making changes  

- user-data  
  - Role: Storage Blob Data Contributor  
  - Purpose: Manage storage data only  



This Azure environment integrates networking, compute, storage, monitoring, and cost management. Each resource plays a specific role and works together to form a secure, scalable, and cost-efficient cloud solution.
``
