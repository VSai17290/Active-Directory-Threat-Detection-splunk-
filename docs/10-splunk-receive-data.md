# Splunk Configured to Receive Data

## Index Creation

In Splunk Web:

1. Go to **Settings → Indexes**.
2. Create a new index named `endpoint` to store Windows and Sysmon logs. 

## Verifying Ingestion

1. Open **Search & Reporting**.
2. Run `index=endpoint` to confirm events are arriving from Windows hosts. 
3. Ensure you see Security, System, Application, and Sysmon events if configured. 

With the index created and Universal Forwarders configured, the Splunk server is now receiving endpoint telemetry. 
