# Project Takeaways

### Takeaways
- Learned how to deploy and interconnect multiple virtual machines (Windows, Splunk, n8n).
- Understood how log forwarding and indexing work between a Windows endpoint and Splunk.
- Gained experience configuring Docker Compose and handling Linux permissions.
- Implemented end-to-end automation using n8n, OpenAI, and Slack integrations.
- Strengthened troubleshooting skills by debugging network, permission, and webhook issues.

Overall, this project helped me connect SIEM tools, automation platforms, and AI services into one cohesive security workflow.

---

### Lessons Learned

- **VM networking**: Ensuring proper connectivity between VMs was tricky, but with the IPs being static and noting them down, it made it easier.
- **Docker permissions**: n8n’s file ownership issues taught me to check container user mappings early.
- **Automation chaining**: Connecting Splunk to n8n to OpenAI to Slack showed just how many moving parts there are in SOC automation.

---

### Results
- Fully functional end-to-end automation pipeline  
- Validated alert forwarding, webhook integration, and Slack delivery  
- Built scalable foundation for further automation (ticketing, enrichment, etc.)

---

### Future Improvements
- The possibility of adding other nodes for further enrichment.
- Use kali as a threat actor of some sort. For this I resorted to inputting the wrong login info, but theres potential for other incidents.
- Still unsure how, but maybe integrate AWS to help with the automation or data storage?
