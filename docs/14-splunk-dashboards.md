# Splunk Dashboards

## Login Monitoring Dashboard

A Splunk dashboard is created to monitor failed login attempts across the domain. 

Panels include:

- **Top Failed Login Attempts**:
  ```
  index=endpoint EventCode=4625
  | stats count by Account_Name, Workstation_Name, host
  | sort - count
  ```
  
- **Login Failures Over Time**:  
  ```
  index=endpoint EventCode=4625
  | timechart span=1h count by host
  ```

These panels help identify possible brute-force activity or misconfigurations in authentication.
