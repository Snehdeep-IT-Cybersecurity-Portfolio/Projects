# Slow Computer Performance (CompTIA A+ 6-Step Process)

**Issue:** Computer running very slowly.

**Step 1: Identify the Problem**  
- User reports system lag and slow application loading.  
- Checked Task Manager: high CPU and memory usage.  
- Noted multiple startup programs running.  
- Disk usage is high, and temporary files are taking up space.

**Step 2: Establish a Theory of Probable Cause**  
- Too many startup programs consuming system resources  
- Pending Windows updates  
- Temporary files filling storage  
- Possible malware infection

**Step 3: Test the Theory**  
- Disabled unnecessary startup programs via Task Manager → `Ctrl + Shift + Esc` → Startup tab.  
- Ran Disk Cleanup to remove temporary files.  
  **Simulated output:**
```

Disk Cleanup completed.

1. Temporary files removed: 250 MB
2. Recycle Bin cleared
3. System cache cleared

```
- Performed full system malware scan using Windows Defender.  
**Simulated output:**
```

Windows Defender Scan Complete
No threats detected

```
- Issue partially improved after performing above steps.

**Step 4: Establish a Plan of Action and Implement the Solution**  
- Disabled remaining unnecessary startup programs.  
- Installed pending Windows updates.  
**Simulated output:**
```

Windows Update Completed
5 updates installed
Reboot required

```
- Cleared temporary files and system cache.  
- Rebooted system.

**Step 5: Verify Full System Functionality**  
- System performance improved significantly.  
- Applications open normally, and system responds quickly.  
- User confirmed improvement in workflow.

**Step 6: Document Findings, Actions, and Outcomes**  
- Root Cause: Excessive startup programs consuming system memory  
- Resolution Time: ~20 minutes  
- Action Taken: Disabled startup apps, installed updates, cleared temporary files, rebooted system  
- Outcome: System performance restored, user satisfied
  
---
