# User Account Locked (Active Directory) Troubleshooting (CompTIA A+ 6-Step Process)

**Issue:** User unable to log in due to account lockout.

**Step 1: Identify the Problem**  
- User reports login failure with the error "Account is locked".  
- Verified user attempts and checked Active Directory status.

**Step 2: Establish a Theory of Probable Cause**  
- Multiple failed login attempts triggered account lockout policy  
- Possible unauthorized access attempt

**Step 3: Test the Theory**  
- Checked account status in Active Directory Users and Computers (ADUC).  
- Verified recent login attempts and lockout events.  
  **Simulated output:**
```

Account: jsmith
Status: Locked
Lockout Time: 10:15 AM
Failed Attempts: 5

```

**Step 4: Establish a Plan of Action and Implement the Solution**  
- Unlocked the account in Active Directory.  
- Reset user password and provided temporary credentials.  
- Advised user to log in and change the password immediately.

**Step 5: Verify Full System Functionality**  
- User successfully logged in with new password.  
- Confirmed access to all required network resources.

**Step 6: Document Findings, Actions, and Outcomes**  
- Root Cause: Multiple failed login attempts triggered account lockout  
- Resolution Time: ~5 minutes  
- Action Taken: Unlocked account, reset password, advised user on proper login  
- Outcome: Access restored and user able to work normally

---
