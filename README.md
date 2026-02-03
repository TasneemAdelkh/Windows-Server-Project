# Windows-Server-Project
Enterprise Windows Server Active Directory project implementing a multi-domain infrastructure with AD DS, DNS, DHCP, Group Policy, delegation, roaming profiles, automation, and WDS — documented as part of an MCSA-focused training project.
# Windows Server Active Directory Infrastructure Project

## Overview
This project documents the design and implementation of a **Windows Server Active Directory infrastructure** that simulates a real enterprise environment.  
It was completed as part of a **Windows Server / MCSA-focused course** and demonstrates core concepts used in production Microsoft-based networks.

The project focuses on **domain architecture, centralized management, security policies, automation, and service integration**, using a structured forest with parent and child domains.

> 📌 **Note:**  
> This repository is **documentation-based**. The full project documentation is maintained as a PDF and is **not publicly uploaded**.

---

## Project Scope & Key Features

### 🔹 Active Directory & Domain Design
- Forest root domain: `iti.local`
- Child domains for branch offices:
  - `ALEX.iti.local`
  - `ISMAILIA.iti.local`
- Multiple Domain Controllers for redundancy
- Read-Only Domain Controller (RODC) for branch security
- Global Catalog configuration
- Domain trust and hierarchy design

---

### 🔹 Core Infrastructure Services
- **DNS**
  - Forward lookup zones
  - Conditional forwarding
  - Name resolution across domains
- **DHCP**
  - Centralized IP address management
  - Scope configuration and lease verification
- **IIS Web Services**
  - Internal websites hosting
  - DNS-integrated site access
- **FTP Services**
  - File retrieval validation via DNS records

---

### 🔹 Group Policy & Security Enforcement
- User logon time restrictions
- Blocking Control Panel access
- Removable storage (USB) restrictions
- Mandatory corporate wallpaper enforcement
- Software deployment using Group Policy (WinRAR)
- Policy scoping using Organizational Units (OUs)

---

### 🔹 Delegation & Remote Access
- Controlled delegation of Remote Desktop access
- Secure non-administrative RDP access to Domain Controllers
- Permission verification and validation

---

### 🔹 User Profiles & Automation
- Roaming profiles across parent and child domains
- Centralized profile storage with NTFS permissions
- PowerShell automation:
  - Bulk creation of users from CSV files
  - OU-based user placement

---

### 🔹 Windows Deployment Services (WDS)
- Network-based OS deployment
- PXE boot authentication
- DHCP integration during deployment
- Boot and install image configuration
- Deployment verification

---

## Project Contributors
This project was completed as a **team effort**, with collaboration on planning, configuration, testing, and documentation.

- Tasneem Adel 
- Abdelrahim Badr  
- Emad Singab  
- Islam Yasser  
- Yasmeen Mohamed  

---

## Instructor Acknowledgment
Special thanks to **Mohamed Abosehly** for his guidance, technical explanations, and continuous support throughout the course.

---

## Documentation Availability
📄 The complete project documentation is maintained as a **PDF** and can be shared **upon request**.

---

## Disclaimer
This project was built for **learning and demonstration purposes**.  
All configurations, IP addresses, domain names, and users are part of a **lab environment**, not a production system.

