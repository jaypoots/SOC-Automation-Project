# SOC-Automation-Project

## Overview
This project demonstrates an automated **Security Operations Center workflow** using platforms like **Splunk**, **n8n**, **ChatGPT**, and **Slack**.

Goal:
> Create a Windows 10 virtual machine that would send telemetry to Splunk, then configure alerts in Splunk, forward them to n8n via webhook, process the alerts through ChatGPT, and automatically post the summarized results into a Slack channel.

All of the setup steps were documented live in a Discord and then formatted into all these Github notes for clarity and shareability.

### Components
| Component| Purpose |
| **Windows 10 VM** | Generates telemetry and failed login attempts |
| **Splunk VM** | Acts as the SIEM — indexes logs, creates alerts |
| **n8n VM** | Automation workflow engine (Docker container) |
| **OpenAI GPT-4.1-mini** | Interprets and summarizes alerts |
| **Slack** | Endpoint for delivering processed alerts |

### Process Flow
1. Windows VM sends logs to Splunk via Universal Forwarder.
2. Splunk then triggers an alert on failed RDP attempts.
3. The alert is sent to n8n via webhook.
4. n8n runs the alert data through ChatGPT.
5. ChatGPT summarizes and classifies the alert.
6. n8n then posts the structured result in a Slack channel called '#alerts'.
