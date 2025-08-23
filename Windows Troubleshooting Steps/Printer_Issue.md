# Printer Not Printing Troubleshooting (CompTIA A+ 6-Step Process)

**Issue:** User unable to print.

**Step 1: Identify the Problem**  
- User reports printer shows as online but print jobs remain stuck in the queue.  
- Other users on the network can print normally.  
- Checked printer queue: multiple jobs pending indefinitely.

**Step 2: Establish a Theory of Probable Cause**  
- Stuck Print Spooler service  
- Corrupted or outdated printer driver  
- Incorrect printer port configuration

**Step 3: Test the Theory**  
- Restarted Print Spooler service by typing `net stop spooler` and `net start spooler`  
  **Simulated output:**
```

The Print Spooler service was stopped successfully.
The Print Spooler service was started successfully.

```
- Attempted to print a test page; issue persisted.  
- Verified printer port and driver settings in Devices and Printers.

**Step 4: Establish a Plan of Action and Implement the Solution**  
- Reinstalled the printer driver from the manufacturer’s website.  
- Restarted the system.  
- Verified port configuration matched printer settings.

**Step 5: Verify Full System Functionality**  
- Printed a test page successfully.  
- User confirmed that normal printing operations were restored.

**Step 6: Document Findings, Actions, and Outcomes**  
- Root Cause: Stuck Print Spooler and outdated printer driver  
- Resolution Time: ~15 minutes  
- Action Taken: Restarted spooler, reinstalled driver, verified port configuration  
- Outcome: Printer fully operational
```

---
