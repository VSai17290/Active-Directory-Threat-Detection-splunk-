# Sysmon Setup

## Why Sysmon

Sysmon (System Monitor) provides detailed Windows telemetry such as process creation, network connections, and file changes, which is critical for threat detection and forensics. 

## Installation & Configuration

1. Download Sysmon from the Microsoft Sysinternals website and extract the files. 
2. Download a tuned Sysmon configuration, such as **Olaf Hartong’s modular config** (`sysmonconfig.xml`). 
3. Open PowerShell as Administrator and navigate to the Sysmon directory.
4. Install Sysmon with a configuration:  
   `.\Sysmon64.exe -i ..\sysmonconfig.xml` 
5. Accept the license agreement. Sysmon will start as a Windows service and generate events in the `Microsoft-Windows-Sysmon/Operational` channel. 

The Splunk Universal Forwarder is then configured via `inputs.conf` to collect these Sysmon events. 
