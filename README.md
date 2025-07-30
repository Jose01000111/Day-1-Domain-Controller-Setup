# 🏦 Day 1 — Domain Controller Setup  
## Chicago Bank Branch Active Directory Lab (Hyper-V)

Welcome to Day 1 of my **5-Day Active Directory Lab** project!  
I’m building out a realistic domain controller environment for a fictional Chicago bank branch using **Hyper-V** and **Windows Server 2022**. Here's how I set it all up — step by step!

---

## 🛠️ Environment

- 💻 **Host OS**: Windows 10 with **Hyper-V** pre-installed  
- 🖥️ **VM OS**: Windows Server 2022 Datacenter (Eval)  
- 🌐 **Domain**: `chicago.bankcorp.local` (child domain of `bankcorp.local`)  
- 🧑‍💼 **Admin Account**: Jose Guerrero  
- 🧰 **Tools**: Server Manager, ADUC, Group Policy

---

## ✅ What I Did:

- 🔽 **Downloaded Windows Server 2022 ISO**  
  Got it from the official Microsoft Evaluation Center  
  ![Screenshot: ISO Download Confirmation](./screenshots/iso-download.png)

- 💻 **Created a New Virtual Machine in Hyper-V**  
  Named it `CHICAGO-DC01` and mounted the Windows Server 2022 ISO  
  ![Screenshot: Hyper-V VM Settings](./screenshots/hyperv-vm-setup.png)

- 🏁 **Installed Windows Server 2022**  
  Chose Desktop Experience and set the local admin password  
  ![Screenshot: Windows Server Installation Complete](./screenshots/windows-install.png)

- 🖥️ **Renamed the Computer to `CHICAGO-DC01`**  
  Changed computer name via System Properties and restarted  
  ![Screenshot: System Properties with New Hostname](./screenshots/rename-computer.png)

- 🌐 **Assigned a Static IP Address**  
  Configured IPv4 manually (e.g., 192.168.1.10) in Network Adapter settings  
  ![Screenshot: Static IP Settings](./screenshots/static-ip.png)

- 🧑‍💻 **Enabled Remote Desktop**  
  Enabled Remote Desktop and allowed through firewall  
  ![Screenshot: Remote Desktop Enabled](./screenshots/remote-desktop.png)

- 🛠️ **Installed Active Directory Domain Services (AD DS) Role**  
  Used Server Manager to add the AD DS role  
  ![Screenshot: AD DS Role Installation](./screenshots/ad-ds-install.png)

- 🏛️ **Promoted Server to Domain Controller**  
  Created new forest `bankcorp.local` with child domain `chicago.bankcorp.local`  
  Set DSRM password and rebooted  
  ![Screenshot: Domain Controller Promotion](./screenshots/dc-promotion.png)

- 🔍 **Verified Domain Controller Setup**  
  Opened Active Directory Users and Computers and confirmed domain presence  
  ![Screenshot: ADUC Domain View](./screenshots/aduc-domain.png)

---

---
