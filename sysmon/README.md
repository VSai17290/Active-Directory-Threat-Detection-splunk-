# Sysmon in This Lab

Sysmon is used on Windows endpoints to collect detailed process, network, and file activity that is not available in basic Windows logs. 

In this project:

- Sysmon is installed as a service using `Sysmon64.exe -i sysmonconfig.xml`. 
- A tuned configuration (based on Olaf Hartong’s modular config) is used to reduce noise and focus on security-relevant events. 
- Events are written to the `Microsoft-Windows-Sysmon/Operational` log and forwarded by Splunk Universal Forwarder into the `endpoint` index. 
