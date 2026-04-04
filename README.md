# 🏢 Active Directory Lab — Windows Server Infrastructure Setup

> **Windows Server 2025 · Active Directory DS · DNS · Domain Controller · VMware · Windows 10**

![Status](https://img.shields.io/badge/Status-Completed-2ea44f?style=flat-square)
![Platform](https://img.shields.io/badge/Platform-Windows%20Server%202025-0078D4?style=flat-square&logo=windows)
![Tool](https://img.shields.io/badge/Virtualization-VMware%20Workstation-607078?style=flat-square)
![Type](https://img.shields.io/badge/Lab-Domain%20Infrastructure%20Build-6e40c9?style=flat-square)

---

## 📌 Overview

This project demonstrates the **complete build of a Windows Server domain infrastructure from scratch** in an isolated virtual environment.

It covers every step from VM provisioning and OS installation to Active Directory deployment, domain controller promotion, and client integration — reflecting the full skill set required for **Junior Sysadmin**, **IT Support**, and **Network Administrator** roles.

---

## 🧱 Lab Architecture

| Component | Details |
|---|---|
| Domain Controller | Windows Server 2025 (Standard Desktop Experience) |
| Client Machine | Windows 10 |
| Network Type | Host-only — isolated internal network |
| Virtualization | VMware Workstation |

### Network Configuration

| Machine | IP Address | DNS |
|---|---|---|
| Windows Server 2025 | 192.168.56.10 | 192.168.56.10 (self) |
| Windows 10 Client | 192.168.56.20 | 192.168.56.10 |

---

## ⚙️ Technologies & Tools

`Windows Server 2025` · `Active Directory DS` · `DNS` · `Domain Controller` · `Server Manager` · `VMware Workstation` · `Windows 10` · `ADDS Role`

---

## 🗂️ Project Structure

```
Lab
├── Part 1 — Windows Server Installation & Network Configuration
├── Part 2 — Active Directory Deployment & DC Promotion
├── Part 3 — Active Directory Management (OUs & Users)
└── Part 4 — Windows 10 Client Setup & Domain Join
```

---

## 🔹 Part 1 — Windows Server Installation

Provisioned a VMware virtual machine and installed Windows Server 2025 with full Desktop Experience, then configured a static IP for the domain environment.

| Setting | Value |
|---|---|
| Edition | Windows Server 2025 Standard (Desktop Experience) |
| IP Address | 192.168.56.10 |
| Subnet Mask | 255.255.255.0 |
| DNS Server | 192.168.56.10 (loopback — DC is its own DNS) |

> 📸 **Screen 1** — VMware VM creation

![VM Setup](./vm-setup.png)

> 📸 **Screen 2** — CPU, memory, and BIOS configuration

![VM BIOS](./vm-bios.png)

> 📸 **Screen 3** — Windows Server boot process

![Boot](./windows-boot.png)

> 📸 **Screen 4** — Windows Server edition selection

![Edition](./windows-edition.png)

> 📸 **Screen 5** — First boot — installation confirmed

![Desktop](./windows-desktop.png)

> 📸 **Screen 5.1** — Static IP and DNS configuration

![Network](./server-network.png)

---

## 🔹 Part 2 — Active Directory Deployment

Installed the AD DS role via Server Manager and promoted the server to a **Domain Controller**:

| Step | Action | Result |
|---|---|---|
| Add Roles & Features | Selected AD DS role | ✅ Installed |
| Promote to DC | New forest creation | ✅ Promoted |
| DNS Integration | Auto-configured with AD | ✅ Active |
| Domain Login | Authenticated via domain | ✅ Success |

> 📸 **Screen 6** — Server Manager dashboard

![Server Manager](./server-manager.png)

> 📸 **Screen 7** — Add Roles and Features wizard

![Install AD](./ad-install.png)

> 📸 **Screen 8** — Active Directory DS role selection

![AD DS](./ad-ds.png)

> 📸 **Screen 9** — Installation confirmation

![Confirm](./ad-confirm.png)

> 📸 **Screen 10** — Domain Controller promotion initiated

![Promote](./promote.png)

> 📸 **Screen 11** — DC setup and DNS configuration

![DC Install](./dc-install.png)

> 📸 **Screen 12** — Successful domain login

![Login](./dc-login.png)

---

## 🔹 Part 3 — Active Directory Management

Managed the domain structure using Active Directory Users and Computers (ADUC):

- Opened **AD Users and Computers** console
- Created **Organizational Units** to structure the domain
- Added **domain users** assigned to their respective OUs

> 📸 **Screen 13** — Active Directory Users and Computers console

![AD Users](./ad-users.png)

> 📸 **Screen 14** — Organizational Units created

![OU](./ou.png)

> 📸 **Screen 15** — Domain users added

![User](./user.png)

---

## 🔹 Part 4 — Client Configuration & Domain Join

Installed Windows 10 on a second VM, configured networking, and successfully joined the domain:

| Step | Configuration | Result |
|---|---|---|
| Windows 10 install | Standard edition | ✅ Installed |
| Network setup | IP: 192.168.56.20 · DNS: 192.168.56.10 | ✅ Configured |
| Domain join | Joined domain via System Properties | ✅ Success |
| Domain login | Authenticated with domain user | ✅ Pass |

> 📸 **Screen 17** — Windows 10 edition selection

![Win10](./win10-edition.png)

> 📸 **Screen 18** — Windows 10 first boot

![Desktop](./win10-desktop.png)

> 📸 **Screen 18.1** — Client network configuration

![Client Network](./client-network.png)

> 📸 **Screen 19** — Domain join completed

![Join Domain](./join-domain.png)

> 📸 **Screen 20** — Domain login from client

![Client Login](./client-login.png)

---

## ✅ Key Achievements

- Provisioned and configured **Windows Server 2025** from scratch in VMware
- Deployed **Active Directory Domain Services** and promoted server to **Domain Controller**
- Configured **DNS** integrated with Active Directory
- Created **Organizational Units** and **domain users**
- Installed **Windows 10** client and successfully **joined the domain**
- Validated end-to-end **domain authentication** from client machine

---

## 🎯 Skills Demonstrated

| Category | Skills |
|---|---|
| Windows Server | Installation, configuration, Server Manager, roles & features |
| Active Directory | AD DS deployment, DC promotion, ADUC, OUs, user management |
| DNS | Active Directory-integrated DNS, static IP, DNS resolution |
| Networking | Static IP configuration, client-server connectivity |
| Virtualization | VMware Workstation, multi-VM lab design |

---

## 💼 Target Roles

This project directly demonstrates skills required for:

- **Junior System Administrator**
- **IT Support Technician**
- **Network Administrator**

---

*Lab built in an isolated VMware environment — all configurations documented with screenshots and test results.*
