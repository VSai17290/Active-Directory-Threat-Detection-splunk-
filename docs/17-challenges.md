# Challenges Faced

## Active Directory Complexity

Designing the OU structure and configuring domain roles and policies required careful planning and testing to avoid misconfigurations. 

## Network Connectivity

Ensuring that all VMs could communicate across the bridged network, join the domain, and forward logs to Splunk involved IP planning and troubleshooting. 

## Simulated Attacks

Setting up realistic but safe attack scenarios from Kali Linux demanded a balance between meaningful telemetry and maintaining a controlled lab environment. 

## Data Onboarding

Correctly forwarding Security, System, Application, and Sysmon logs to the `endpoint` index and validating them in Splunk took several iterations. 
