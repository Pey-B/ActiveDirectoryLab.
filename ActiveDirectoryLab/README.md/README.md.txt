<!-- Banner Section -->
<p align="center">
  <img src="https://img.shields.io/badge/Windows%20Server%202019-0078D6?style=for-the-badge&logo=windows&logoColor=white" alt="Windows Server 2019"/>
  <img src="https://img.shields.io/badge/Windows%2010-0078D6?style=for-the-badge&logo=windows&logoColor=white" alt="Windows 10"/>
  <img src="https://img.shields.io/badge/VirtualBox-183A61?style=for-the-badge&logo=virtualbox&logoColor=white" alt="VirtualBox"/>
  <img src="https://img.shields.io/badge/PowerShell-5391FE?style=for-the-badge&logo=powershell&logoColor=white" alt="PowerShell"/>
  <img src="https://img.shields.io/badge/Active%20Directory-003366?style=for-the-badge&logo=windows&logoColor=white" alt="Active Directory"/>
</p>

<h1 align="center">🖥️ Active Directory Home Lab (Windows Server 2019 + Windows 10 Client)</h1>

<p align="center">
  <em>A virtualized lab for building and managing an Active Directory domain using Windows Server 2019 and Windows 10 Client in VirtualBox.</em>
</p>

---

## 🧱 Overview

**Purpose:**  
This project demonstrates how to deploy and configure an **Active Directory Domain Services (AD DS)** environment from scratch using **VirtualBox**, simulating a small business network. It includes a domain controller, DHCP/DNS configuration, and a Windows 10 client joined to the domain.

**Technologies Used:**  
- Oracle VirtualBox  
- Windows Server 2019  
- Windows 10 Pro  
- PowerShell  
- Active Directory, DHCP, DNS  

---

## ⚙️ Virtual Machine Configuration

| Role | Hostname | OS | Network | Description |
|------|-----------|----|----------|--------------|
| Domain Controller | DC01 | Windows Server 2019 | Internal + NAT | Hosts AD DS, DNS, DHCP, and NAT |
| Client | CLIENT01 | Windows 10 Pro | Internal | Domain-joined workstation |

---

## 🧩 Configuration Steps & Screenshots

### 1. Created Virtual Machine (Domain Controller)
![Created Virtual Machine DC](screenshots/created_virtual_machine_DC.png)

### 2. Configured Network Interface Cards (NICs)
![Configured NICs](screenshots/configured_NICs.png)

### 3. Set Static IP on Internal Network
![Set Static IP](screenshots/set_static_on_internal_network.png)

### 4. Enabled Active Directory, DNS, and NAT
![Enabled AD and NAT](screenshots/enabled_AD_and_NAT.png)

### 5. Created Organizational Unit (OU) and Added Admin User
![Created OU](screenshots/created_OU_in_AD_and_added_user_to_admin.png)

### 6. Installed DHCP Role
![Installed DHCP](screenshots/installed_DHCP.png)

### 7. Configured IPv4 Scope in DHCP
![Set IPv4 Scope](screenshots/set_IPv4_scope.png)

### 8. Created Users via PowerShell Script
![Created Users](screenshots/created_users_from_script.png)

### 9. Created Client VM
![Created Client VM](screenshots/created_client_VM.png)

### 10. Joined Client to Domain
![Joined Client to Domain](screenshots/joined_client_to_domain.png)

---

## 🧠 Learning Objectives

- Deploy and configure **Active Directory Domain Services (AD DS)**  
- Set up **DHCP** and **DNS** integration with AD  
- Automate **user creation** using PowerShell  
- Join Windows clients to a domain  
- Understand **network segmentation** using NAT + Internal adapters in VirtualBox  

---

## 📂 Repository Structure

