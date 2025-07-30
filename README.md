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

## 🔽 **Downloaded Windows Server 2022 ISO**  
  Got it from the official Microsoft Evaluation Center
  
 <img width="1138" height="450" alt="RFUwNvF" src="https://github.com/user-attachments/assets/3b12d9fb-6de2-4b12-8aa7-1a143f3381aa" />

 ---
 
<img width="1016" height="697" alt="mLu6spL" src="https://github.com/user-attachments/assets/cfe7a324-ffd9-47b7-bd27-99d81a3d6edd" />

## 💻 **Created a New Virtual Machine in Hyper-V**  
  Named it `CHICAGO-DC01` and mounted the Windows Server 2022 ISO  

 <img width="1229" height="675" alt="mAZCQwo" src="https://github.com/user-attachments/assets/1b81c303-3abc-4194-8c91-450375ea9442" />

- 🏁 **Installed Windows Server 2022**  
  Chose Desktop Experience and set the local admin password

  <img width="1016" height="697" alt="mLu6spL" src="https://github.com/user-attachments/assets/310d7e03-a354-47a9-bd51-823f9b51ace2" />

- 🖥️ **Renamed the Computer to `CHICAGO-DC01`**  
  Changed computer name via System Properties and restarted  

<img width="401" height="470" alt="Nuf3dee" src="https://github.com/user-attachments/assets/11e214d4-6e8f-4c7c-a97e-42b3ea4f647f" />

- 🌐 **Assigned a Static IP Address**  
  Configured IPv4 manually (e.g., 192.168.1.10) in Network Adapter settings  

<img width="1143" height="647" alt="onMkCnS" src="https://github.com/user-attachments/assets/5b16f706-360b-4839-9af4-39ce6bdf1b96" />

---

<img width="1218" height="661" alt="wzEh0Gl" src="https://github.com/user-attachments/assets/3a5d25ff-1101-4186-bafc-8ed1365b1a0d" />

- 🧑‍💻 **Enabled Remote Desktop**  
  Enabled Remote Desktop and allowed through firewall  

<img width="1076" height="516" alt="YDC539W" src="https://github.com/user-attachments/assets/ac63e465-96a6-4fb7-bced-cb441256a3c2" />

- 🛠️ **Installed Active Directory Domain Services (AD DS) Role**  
  Used Server Manager to add the AD DS role  

<img width="1128" height="637" alt="VUTgu3X" src="https://github.com/user-attachments/assets/95883f56-5304-4c46-abe6-b000f578e4a4" />

- 🏛️ **Promoted Server to Domain Controller**  
  Created new forest `bankcorp.local` with child domain `chicago.bankcorp.local`  
  Set DSRM password and rebooted  

<img width="755" height="435" alt="YfQvEIC" src="https://github.com/user-attachments/assets/b39a69ca-9243-4d94-b88e-7fff2d6cfa32" />

---

<img width="768" height="559" alt="Oeip7ax" src="https://github.com/user-attachments/assets/e05aa74a-3c7a-4811-9b78-4433110f7076" />

- 🔍 **Verified Domain Controller Setup**  
  Opened Active Directory Users and Computers and confirmed domain presence  

<img width="1213" height="441" alt="rMtXfOJ" src="https://github.com/user-attachments/assets/cf4ff3ce-15ae-4a01-b465-7fc1a15d69fe" />

---
