# Group Policy Configuration

## Admins GPO

- Enable Remote Desktop for admins. 
- Disable UAC for the built-in administrator account (for lab-only unrestricted access). 
- Allow unrestricted PowerShell script execution for administrative tasks. 

## Employees GPO

- Keep Microsoft Defender Antivirus enabled. 
- Prohibit user software installations via Windows Installer. 
- Restrict access to the Command Prompt to reduce misuse. 

## Interns GPO

- Block access to Control Panel and PC settings. 
- Disable Command Prompt and restrict PowerShell scripts. 
- Deny access to removable storage devices via removable storage policies. 

## Computers GPO

- Enforce firewall protection for all network connections. 
- Disable the Guest account. 
- Enforce password policies: minimum length, history, and maximum age. 

## HR Manager GPO

- Enable detailed auditing for logon events, process creation, and network connections to an HR workstation, reflecting increased phishing risk for HR. 
