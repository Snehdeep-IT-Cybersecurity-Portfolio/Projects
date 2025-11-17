# 🖥️ Server Core Active Directory Lab

This project demonstrates an **Active Directory lab setup** using **Windows Server Core** and **PowerShell**.  
It showcases how to simulate a corporate environment with domain controllers, organizational units, users, groups, and GPOs.

---

## 📋 Project Overview

**Objective:**  
To practice and demonstrate core Active Directory administration skills in a Server Core environment.

**Key Features Implemented:**

**Key Features Implemented:**

- 🖥️ Configured **Windows Server 2022 Core** as a Domain Controller  
- 💻 Used **Windows 10 client** joined to the domain  
- 🌐 Created domain: `mydomain.local`  
- 🏢 Created **Organizational Units (OUs)**: IT, HR, Sales  
- 👤 Created **users** and assigned them to **groups**  
- 🔒 Linked **GPOs** to OUs to enforce department policies  

All steps were performed using **PowerShell commands** without GUI.

---

## 📁 Project Structure

```

ServerCore-AD-Lab/
├── steps/      # Step-by-step commands and screenshots
├── scripts/    # Optional: PowerShell scripts used
└── README.md   # Project overview

```

- `steps/` contains all commands, outputs, and screenshots demonstrating the implementation.  
- `scripts/` (optional) can store reusable PowerShell scripts for setting up the lab.

---

## 💡 Notes

- The lab demonstrates practical **AD management** on Server Core.  
- Screenshots and detailed commands are organized in the `steps/` folder.  
- Focus is on **PowerShell-driven administration**, suitable for labs, learning, or portfolio showcase.

