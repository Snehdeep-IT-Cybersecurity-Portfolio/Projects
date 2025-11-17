# 5️⃣ Windows 10 Client – Join to Domain

**Goal:** Join a Windows 10 client VM to the domain `mydomain.local` and verify successful authentication + policy application.

---

## ✔️ Steps Taken

### **1️⃣ Configure Client Network**

Set client to **Host-Only Adapter** (same network as server):

- Windows Server: `192.168.56.10`
- Windows 10 Client: `192.168.56.20`
- Subnet: `255.255.255.0`
- DNS: **192.168.56.10** (must point to the Domain Controller)

Verify:

```cmd
ipconfig /all
ping 192.168.56.10
```
2️⃣ Join Client to Domain
Open System Properties → Domain Join
or use command:

```powershell

Add-Computer -DomainName "mydomain.local" -Credential MyDomain\Administrator
```
Restart-Computer
Client reboots and now you can sign in using:

mydomain\AliceIT
mydomain\BobHR
mydomain\CarolSales
3️⃣ Verify Domain Login
After reboot:

Press Other User

Enter domain username + password

Confirm login success

4️⃣ Verify Group Policies
Check applied policies:

```

gpresult /r

```
Check if HR restrictions applied (for HR user).

5️⃣ Confirm Organizational Unit Placement
On the server:

```powershell

Get-ADComputer -Identity "CLIENTPC"
```
Ensure it appears under the correct OU (default is Computers).
