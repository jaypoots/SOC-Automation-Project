# VM Setup

**VMs to create:** Windows 10, Splunk, Kali, n8n instance

### Actions
Created four virtual machines.  
![Image](../docs/snapshots/vm-setup.png)

Connected to the `coob-splunk` VM on my local machine with:
```bash
ssh username@ipaddress
```

Then updated its packages with:
```bash
sudo apt-get update && sudo apt-get upgrade -y
```
