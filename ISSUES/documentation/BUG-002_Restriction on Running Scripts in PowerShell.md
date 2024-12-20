## Issue: Restriction on Running Scripts in PowerShell

### Description:
While attempting to execute a PowerShell script, we encountered the following error message:

This error was caused by PowerShell's default execution policy, which restricts the running of scripts on the system for security reasons.

### Resolution Steps:

1. **Check the Current Execution Policy:**
   To check the current execution policy, we ran the following command in PowerShell:
   ```powershell
   Get-ExecutionPolicy
2. **Change the Execution Policy for Current User:** We adjusted the execution policy to allow local scripts to run by setting the policy to RemoteSigned for the current user:
```powershell
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser

  

