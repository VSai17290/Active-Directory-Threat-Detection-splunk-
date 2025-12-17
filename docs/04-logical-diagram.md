# Logical Diagram

The logical diagram represents how the domain, servers, and endpoints are organized.

## Components

- `BESTIU.LOCAL` domain with OUs for Admins, Employees, Interns, HR, and Computers.
- Windows Server acting as Domain Controller and DNS server.
- Windows 10 clients joined to the domain, assigned to the appropriate OU.
- Ubuntu Splunk server receiving forwarded logs from all Windows hosts.
- Kali Linux attacker outside the domain but on the same network segment.

Refer to `lab-diagrams/logical-diagram.png` for the visual representation.
