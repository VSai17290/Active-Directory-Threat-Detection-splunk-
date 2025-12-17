# Active Directory Domain Setup

## AD DS Installation

On the Windows Server VM: 

1. Open **Server Manager → Manage → Add Roles and Features**.
2. Choose a role-based installation and add **Active Directory Domain Services (AD DS)**. 
3. Complete the wizard, then promote the server to a Domain Controller. 

## Creating the Domain

1. In Server Manager, click the flag notification and select **Promote this server to a domain controller**. 
2. Choose **Add a new forest**.
3. Enter `BESTIU.LOCAL` as the root domain name, set a DSRM password, and complete the wizard. 
4. After reboot, log on using the domain credentials to confirm the promotion succeeded. 
