# Splunk Universal Forwarder on Windows

## Purpose

The Splunk Universal Forwarder (UF) is used to send Windows event logs and Sysmon logs from endpoints to the Splunk server, using minimal resources. 

## Steps

1. Configure the Windows 10 VM with a static IP on the same subnet as the Splunk server. 
2. Access Splunk Web at `http://<splunk-ip>:8000` to confirm the server is reachable. 
3. Download the **Splunk Universal Forwarder for Windows (64-bit, .msi)** from the Splunk site. 
4. During installation:
   - Choose “An on-premises Splunk Enterprise instance”. 
   - Set the receiving server to the Splunk server IP (e.g., `192.168.10.10`). 
5. After installation, ensure the Splunk Forwarder service is running under the Local System account. 
