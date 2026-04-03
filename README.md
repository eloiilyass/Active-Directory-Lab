# 🏢 Active Directory Lab (Infrastructure Setup)

## 📌 Project Overview

This project simulates the deployment of a **Windows Server infrastructure** and the implementation of **Active Directory Domain Services (AD DS)** in a virtual environment.

It demonstrates the full process of building a domain from scratch, including server installation, network configuration, and domain management.

---

## 🧱 Lab Architecture

* **Domain Controller:** Windows Server 2025
* **Client Machine:** Windows 10
* **Network Type:** Host-only (isolated internal network)

---

## ⚙️ Technologies & Tools

* VMware Workstation
* Windows Server 2025
* Windows 10
* Active Directory Domain Services (AD DS)
* DNS Configuration

---

# 🔹 Part 1: Windows Server Installation

## 🎯 Objectives

* Install Windows Server
* Configure virtual machine resources
* Prepare system for domain deployment

---

### 🖥️ Screen 1: VMware Setup

This step shows the creation and configuration of the virtual machine.

![VM Setup](./vm-setup.png)

---

### 🖥️ Screen 2: VM Configuration (BIOS & Resources)

This step shows CPU, memory, and BIOS configuration before installation.

![VM BIOS](./vm-bios.png)

---

### 🖥️ Screen 3: Windows Server Boot

This step shows the system boot process before installation.

![Boot](./windows-boot.png)

---

### 🖥️ Screen 4: Windows Server Edition Selection

Selection of Windows Server Standard (Desktop Experience).

![Edition](./windows-edition.png)

---

### 🖥️ Screen 5: First Boot

This step confirms successful installation of Windows Server.

![Desktop](./windows-desktop.png)

---

### 🖥️ Screen 5.1: Network Configuration

Configuration of static IP and DNS:

* IP Address: 192.168.56.10
* Subnet Mask: 255.255.255.0
* DNS Server: 192.168.56.10

![Network](./server-network.png)

---

# 🔹 Part 2: Active Directory Deployment

## 🎯 Objectives

* Install Active Directory Domain Services
* Promote server to Domain Controller
* Create domain environment

---

### 🖥️ Screen 6: Server Manager

Access to server management dashboard.

![Server Manager](./server-manager.png)

---

### 🖥️ Screen 7: Add Roles and Features

Launching the installation wizard.

![Install AD](./ad-install.png)

---

### 🖥️ Screen 8: AD DS Selection

Selecting Active Directory Domain Services.

![AD DS](./ad-ds.png)

---

### 🖥️ Screen 9: Confirm Installation

Validation before installation.

![Confirm](./ad-confirm.png)

---

### 🖥️ Screen 10: Promote to Domain Controller

Initiating domain controller setup.

![Promote](./promote.png)

---

### 🖥️ Screen 11: Domain Controller Setup

Configuration of domain and DNS.

![DC Install](./dc-install.png)

---

### 🖥️ Screen 12: Domain Login

Successful login using domain credentials.

![Login](./dc-login.png)

---

# 🔹 Part 3: Active Directory Management

## 🎯 Objectives

* Manage users and OUs
* Structure domain

---

### 🖥️ Screen 13: AD Users and Computers

Opening AD management console.

![AD Users](./ad-users.png)

---

### 🖥️ Screen 14: Create Organizational Units

Creation of OUs for structuring the domain.

![OU](./ou.png)

---

### 🖥️ Screen 15: Create Users

Adding domain users.

![User](./user.png)

---

# 🔹 Part 4: Client Configuration

## 🎯 Objectives

* Install Windows 10
* Join domain
* Test connectivity

---

### 🖥️ Screen 17: Windows 10 Installation

Selecting Windows 10 edition.

![Win10](./win10-edition.png)

---

### 🖥️ Screen 18: First Boot

Windows 10 ready for configuration.

![Desktop](./win10-desktop.png)

---

### 🖥️ Screen 18.1: Network Configuration

Client configured with:

* IP Address: 192.168.56.20
* DNS: 192.168.56.10

![Client Network](./client-network.png)

---

### 🖥️ Screen 19: Join Domain

Successful domain join process.

![Join Domain](./join-domain.png)

---

### 🖥️ Screen 20: Domain Login

Login using domain user.

![Client Login](./client-login.png)

---

# ✅ Key Achievements

* Installed and configured Windows Server
* Deployed Active Directory Domain Services
* Configured DNS and networking
* Created domain users and OUs
* Joined client machine to domain

---

# 🎯 Skills Demonstrated

* Windows Server Administration
* Active Directory Deployment
* Network Configuration
* DNS Setup
* Virtualization (VMware)

---

# 📌 Conclusion

This project demonstrates the complete setup of a **Windows Server domain infrastructure** from installation to client integration.

It provides a strong foundation for system administration and enterprise network management.
