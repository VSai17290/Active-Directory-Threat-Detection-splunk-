# Splunk Alerts

## Excessive Failed Logins Alert

An alert is configured to notify when an account experiences many failed login attempts in a short period. 

### Search
```
index=endpoint Code=4625
| stats count by host, Account_Name
| where count > 5
```

### Alert Settings

- Schedule: Run every 5 minutes.
- Trigger: If the search returns any results (number of results > 0). 
- Action: Send an email, run a script, or trigger a webhook for further automation. 

This alert helps detect potential brute-force attacks or compromised credentials. 


