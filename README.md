# Active Directory & Threat Detection using Splunk

This repository documents a full homelab project that simulates an enterprise environment with Active Directory, Windows endpoints, Sysmon, and Splunk for centralized logging and threat detection.

The lab is based on the domain **BESTIU.LOCAL** and shows how to collect Windows security telemetry, monitor it with Splunk dashboards, and generate alerts for suspicious activity such as failed logons and brute-force attempts.

## Lab Architecture

- **Domain**: BESTIU.LOCAL with OUs for Admins, Employees, Interns, Computers, and HR.
- **Splunk Server**: Ubuntu VM running Splunk Enterprise, receiving logs on a custom index `endpoint`.
- **Domain Controller**: Windows Server VM with AD DS, DNS, and Group Policies.
- **Endpoints**: Windows 10 VMs with Splunk Universal Forwarder and Sysmon installed. 
- **Attacker**: Kali Linux VM used to simulate attacks (e.g., brute force, AD abuse).

All VMs use **Bridged networking** so they receive IPs in the same subnet and can communicate like a small corporate network. 

## Repository Structure

- `docs/` – Step-by-step documentation for each stage (scenario, setup, configuration, conclusion). 
- `lab-diagrams/` – Diagrams for domain structure, logical design, and network architecture.
- `splunk/` – Splunk inputs configuration and example SPL searches for dashboards and alerts.
- `sysmon/` – Notes on Sysmon configuration and usage in the lab.

## Skills Demonstrated

- Designing an AD domain and OU structure with role-based Group Policy Objects. 
- Configuring Splunk Enterprise on Linux and Universal Forwarders on Windows.
- Using Sysmon for detailed process and network telemetry. 
- Building Splunk dashboards and alerts for failed logons and suspicious activity.
- Documenting homelab projects in a portfolio-friendly GitHub format.
