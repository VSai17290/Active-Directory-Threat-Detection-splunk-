# Project Scenario

## Scenario Overview

This project implements **Active Directory security monitoring and threat detection using Splunk** in a simulated enterprise network. The goal is to create a centralized SIEM that collects and analyzes security events from multiple Windows systems joined to a domain.

## Infrastructure Setup

- **Host A (main system)** runs three VMs:
  - Kali Linux – attacker machine for penetration testing and simulated AD attacks. 
  - Windows Server – Active Directory Domain Controller for BESTIU.LOCAL.
  - Ubuntu – Splunk Enterprise server for log collection and analysis. 
- **Hosts B, C, D** are Windows 10 endpoints with Splunk Universal Forwarder and Sysmon, forwarding logs to the Splunk server.

## Project Objectives

- Implement AD security policies for users, groups, and access control. 
- Collect Windows event logs and Sysmon telemetry using Splunk Universal Forwarder.
- Detect incidents using Splunk searches, dashboards, and alerts. 
- Simulate attacks from Kali Linux and analyze resulting logs. 
- Practice forensic-style analysis using detailed event data. 
