# Networking – Bridge Mode

## Why Bridge Mode

Bridge networking is chosen so each VM receives an IP address from the same network as the host, creating a realistic corporate-like environment. 

Bridge mode enables:

- Direct communication between Splunk server, AD Domain Controller, Windows clients, and Kali Linux. 
- Proper DNS resolution and authentication for domain-joined machines. 
- Log forwarding from Universal Forwarders to Splunk without NAT complications. 

## Key Benefits

- Each VM has its own IP, simplifying troubleshooting with tools like ping and Wireshark. 
- Kali can reach other systems as an attacker would in a real network. 
- Splunk can receive data from multiple hosts across the subnet. 
