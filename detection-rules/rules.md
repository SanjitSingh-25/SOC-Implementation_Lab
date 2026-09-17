# Detection Rules

## Rule 1 — Multiple Failed Logons

- **Event ID:** 4625
- **Condition:** 5 or more failed logons within 5 minutes
- **Alert:** Multiple Failed Login Attempts
- **Initial Severity:** Medium
- **Investigation:** Check account, timestamp, logon type, workstation/source information, and nearby successful logons.

## Rule 2 — PowerShell Process Creation

- **Event ID:** 4688
- **Condition:** New process is `powershell.exe` or `pwsh.exe`
- **Alert:** PowerShell Process Creation
- **Initial Severity:** Medium
- **Investigation:** Check user, process path, parent process, timestamp, and surrounding activity.

> These rules identify activity for review. They do not automatically prove malicious behavior.
