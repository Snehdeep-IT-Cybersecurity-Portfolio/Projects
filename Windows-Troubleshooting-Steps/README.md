# 🖥️ Windows Troubleshooting Steps  

This repository contains **Windows troubleshooting guides** following the **CompTIA A+ 6-Step troubleshooting methodology**.  
These guides are designed for **IT support professionals** 🧑‍💻, particularly for **Service Desk or Help Desk** roles, to demonstrate common troubleshooting skills in a structured and documented manner.  

---

## 📋 Overview  

Each troubleshooting guide includes:  

1. 🔍 **Identify the Problem** – Gather information about the issue.  
2. 🤔 **Establish a Theory of Probable Cause** – Determine possible causes of the problem.  
3. 🧪 **Test the Theory** – Perform diagnostic tests or run commands to verify the theory.  
4. 🛠️ **Establish a Plan of Action & Implement the Solution** – Execute corrective measures.  
5. ✅ **Verify Full System Functionality** – Confirm the problem is resolved.  
6. 📝 **Document Findings, Actions, and Outcomes** – Record the resolution steps and results.  

---

## 📚 Troubleshooting Guides  

1. 📶 [**Wi-Fi Connectivity**](Wifi-Troubleshooting.md)  
   - Fix network issues using commands like `ipconfig /release`, `ipconfig /renew`, `ipconfig /flushdns`, and `netsh int ip reset`.  

2. 🐢 [**Slow Computer Performance**](Slow-Performance.md)  
   - Improve system speed by disabling startup programs, clearing temporary files, and applying updates.  

3. 💻💥 [**Blue Screen of Death (BSOD)**](BSOD-Troubleshooting.md)  
   - Diagnose system crashes with `sfc /scannow`, `chkdsk /f`, and driver updates.  

4. 🖨️ [**Printer Issues**](Printer-Issue.md)  
   - Resolve printer problems by restarting the Print Spooler, reinstalling drivers, and checking port configs.  

5. 🔒 [**Account Lockout**](Account-Lockout.md)  
   - Unlock accounts in Active Directory, reset passwords, and verify user access.  

---

## ⚡ Windows Troubleshooting Scripts  

PowerShell scripts help **automate repetitive support tasks** 🤖.  

- 🔄 **Reset TCP/IP Stack:** `netsh int ip reset`  
- 🌐 **Release/Renew IP Address:** `ipconfig /release` & `ipconfig /renew`  
- 🧹 **Flush DNS Cache:** `ipconfig /flushdns`  
- 🔁 **Restart Services:** e.g., `net stop spooler` & `net start spooler`  

**✨ Benefits:**  
- ⏱️ Saves time & ensures consistency  
- 🛡️ Reduces human error  
- ⚙️ Quickly fixes common issues  

---
