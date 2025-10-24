# Splunk Alert Integration with n8n
 
### Actions:
Created alert in Splunk to ensure n8n webhook can catch it.  

---

Generated failed attempts by trying to RDP into Windows machine.  

Before failed attempts:  
![Image](../docs/snapshots/before-failed-attempts.PNG)  

After failed attempts:  
![Image](../docs/snapshots/After-failed-attempts.PNG)  

---

Filtered down to only certain fields.  
![Image](../docs/snapshots/splunk-filter.PNG)

---

Created Splunk alert with n8n Webhook to catch the alert.  
![Image](../docs/snapshots/Alert.PNG)

---

n8n instance successfully caught Splunk alert.  
![Image](../docs/snapshots/n8n-listen.PNG)