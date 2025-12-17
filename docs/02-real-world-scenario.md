# Real-World Scenario

## BESTIU.LOCAL Enterprise Simulation

The lab models a small enterprise network for **Bharatiya Engineering Science and Technology Innovation University (BESTIU)** with a dedicated Active Directory Domain Controller and centralized logging via Splunk. 

The domain `BESTIU.LOCAL` includes organizational units for admins, employees, interns, computers, and HR, reflecting realistic user segmentation and policy requirements. 

## Network & System Architecture

- Total hosts: 6 (A–F), including:
  - Host A: Kali Linux, Windows Server (AD DC), Ubuntu (Splunk). 
  - Hosts B, C, D: Windows workstations joined to BESTIU.LOCAL.
- Each Windows workstation runs Splunk Universal Forwarder and Sysmon to forward security-relevant events to Splunk.

All VMs are placed in **Bridged network mode** so they receive IPs in the same subnet as the host and can communicate directly for authentication, DNS, log forwarding, and attack simulation. 
