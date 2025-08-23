# Blue Screen of Death (BSOD) Troubleshooting (CompTIA A+ 6-Step Process)

**Issue:** System crashes with a blue screen error.

**Step 1: Identify the Problem**  
- User reports system crashes with stop code "CRITICAL_PROCESS_DIED".  
- System is unstable and cannot boot normally.  
- Noted that the crashes happen randomly during startup and while running applications.

**Step 2: Establish a Theory of Probable Cause**  
- Corrupted system files  
- Outdated or incompatible drivers  
- Failing hardware (RAM or hard drive)

**Step 3: Test the Theory**  
- Booted into Safe Mode by pressing `F8` during startup.  
- Ran System File Checker to repair system files: `sfc /scannow`  
  **Simulated output:**
```

Beginning system scan...
Windows Resource Protection found corrupt files and successfully repaired them.

```
- Checked disk integrity with `chkdsk /f`  
**Simulated output:**
```

Stage 1: Examining basic file system structure...
Stage 2: Examining file name linkage...
Stage 3: Examining security descriptors...
Windows has scanned the file system and found no problems.

```
- Checked Device Manager for outdated drivers; found one outdated graphics driver.

**Step 4: Establish a Plan of Action and Implement the Solution**  
- Repaired corrupted system files using `sfc /scannow`.  
- Updated the outdated graphics driver.  
- Rebooted the system.

**Step 5: Verify Full System Functionality**  
- System restarted successfully.  
- No further BSODs observed.  
- User confirmed system stability and normal operation.

**Step 6: Document Findings, Actions, and Outcomes**  
- Root Cause: Corrupted system files and outdated driver  
- Resolution Time: ~30 minutes  
- Action Taken: Repaired system files, updated driver, rebooted system  
- Outcome: System restored and stable

---
