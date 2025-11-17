2️⃣ Organizational Units & Users Setup

Goal: Create department-based OUs and add domain users in mydomain.local.

Steps Taken:
# Create Organizational Units
New-ADOrganizationalUnit -Name "IT"
New-ADOrganizationalUnit -Name "HR"
New-ADOrganizationalUnit -Name "Finance"
New-ADOrganizationalUnit -Name "Managers"
New-ADOrganizationalUnit -Name "Workstations"

# Create Users inside OUs
New-ADUser -Name "Alice IT" -Enabled $true `
-AccountPassword (Read-Host -AsSecureString) `
-Path "OU=IT,DC=mydomain,DC=local"

New-ADUser -Name "Bob HR" -Enabled $true `
-AccountPassword (Read-Host -AsSecureString) `
-Path "OU=HR,DC=mydomain,DC=local"

Notes:

OUs were created to organize users and apply GPOs per department.

Basic test users were created to validate login and policy deployment.

Passwords set through PowerShell (secure string).


![OU](../screenshots/ou.jpeg)
![Users](../screenshots/users.jpeg)

All actions completed in Server Core using PowerShell only.
