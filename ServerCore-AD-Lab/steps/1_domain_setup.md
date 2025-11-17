# 1️⃣ Domain Setup – Windows Server 2022 Core

**Goal:** Set up **Windows Server 2022 Core** as a **Domain Controller** and create the domain `mydomain.local`.

---

## Steps Taken:

```powershell
# Install Active Directory Domain Services
Install-WindowsFeature AD-Domain-Services

# Promote Server Core to Domain Controller and create domain
Install-ADDSForest -DomainName "mydomain.local"
Notes:
The server is now configured as the primary domain controller.

Ready for creating OUs, users, and groups.

All configuration is done via PowerShell, no GUI required.

```
![Domain Setup](screenshots/domain_setup.png)
