# Domain Structure

The Active Directory domain is named **BESTIU.LOCAL**. 

## Logical Structure

- Root domain: `BESTIU.LOCAL` 
- Top-level OUs:
  - `Users`
  - `Computers` 

Under `Users`, sub-OUs are created to represent roles:

- `Admins`
- `Employees`
- `Interns`
- `HR` (for HR_Manager-type accounts)

This structure allows applying different Group Policy Objects (GPOs) to each group, enforcing appropriate security controls and restrictions per role. [file:1]
