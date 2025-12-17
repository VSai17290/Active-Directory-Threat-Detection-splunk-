# Splunk Server on Ubuntu

## Static IP Configuration

On the Ubuntu VM, a static IP is configured (e.g., `192.168.10.10`) using netplan: 

- Edit `/etc/netplan/00-installer-config.yaml`.
- Set a static address, gateway, and DNS.
- Apply the configuration with `sudo netplan apply` and verify with `ip a`. 

## Splunk Enterprise Installation

- Download the Splunk Enterprise `.deb` installer on the host and share it into the Ubuntu VM using VirtualBox shared folders. 
- Install required VirtualBox guest utilities and mount the shared folder.
- Install Splunk with `sudo dpkg -i splunk-<version>-linux-2.6-amd64.deb`. 
- Switch to the `splunk` user and start Splunk from `/opt/splunk/bin` using `./splunk start`, then create the admin credentials. 
- Enable Splunk to start on boot with `sudo ./splunk enable boot-start -user splunk`. 
