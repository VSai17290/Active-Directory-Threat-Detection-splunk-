# Sysmon Notes

- Confirm Sysmon is running with `sc query sysmon64` or by checking the Event Viewer channel `Microsoft-Windows-Sysmon/Operational`. 
- When updating the configuration, run `Sysmon64.exe -c sysmonconfig.xml` to reload rules without reinstalling. 
- Use Sysmon event IDs (e.g., 1 for process creation, 3 for network connections) in Splunk searches to build more advanced detections. 
