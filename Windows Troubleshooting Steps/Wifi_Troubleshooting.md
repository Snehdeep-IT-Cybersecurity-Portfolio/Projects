# Wi-Fi Troubleshooting (CompTIA A+ 6-Step Process)

**Issue:** User cannot connect to Wi-Fi.

**Step 1: Identify the Problem**  
- User reports "No Internet Access".  
- Other devices are working fine on the same network.  
- Verified that the Wi-Fi adapter is enabled on the laptop.  
- Confirmed the device is within range of the access point.

**Step 2: Establish a Theory of Probable Cause**  
- Corrupted TCP/IP stack  
- Incorrect IP configuration  
- DHCP server not assigning addresses  
- Outdated or faulty wireless driver

**Step 3: Test the Theory**  
- Release and renew IP address by typing `ipconfig /release` followed by `ipconfig /renew`.  
  **Simulated output:**
```

Windows IP Configuration

Ethernet adapter Wi-Fi:


 Connection-specific DNS Suffix  . :
 IPv4 Address. . . . . . . . . . . : 192.168.1.25
 Subnet Mask . . . . . . . . . . . : 255.255.255.0
 Default Gateway . . . . . . . . . : 192.168.1.1


```
- Flush DNS cache by typing `ipconfig /flushdns`.  
**Simulated output:**

```

Windows IP Configuration
Successfully flushed the DNS Resolver Cache.

```

- Reset TCP/IP stack by typing `netsh int ip reset`.  
**Simulated output:**
```

Resetting Global, OK!
Resetting Interface, OK!
Resetting Unicast Address, OK!
Resetting Neighbor, OK!
Resetting Path, OK!
Restart the computer to complete this action.

```
- Reboot system. Issue resolved.

**Step 4: Establish a Plan of Action and Implement the Solution**  
- Performed TCP/IP reset and rebooted the system.  
- Verified DHCP assigned a valid IP address.  

**Step 5: Verify Full System Functionality**  
- User successfully reconnected to Wi-Fi.  
- Confirmed ability to browse the internet and access shared network resources.  

**Step 6: Document Findings, Actions, and Outcomes**  
- Root Cause: Corrupted TCP/IP stack  
- Resolution Time: ~10 minutes  
- Action Taken: Reset TCP/IP stack, verified DHCP lease, tested connectivity  
- Outcome: User confirmed issue resolved


