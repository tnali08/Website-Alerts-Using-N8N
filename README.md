# Website-Alerts-Using-N8N
This project contains an N8N workflow that monitors a  website sends an SMS alert using N8N, if the site is down or returns an error status.
- Checks website status (Cron trigger)
- Sends an alert via N8N if the site is down
- Logs status with timestamp
- Easy to configure for multiple websites

Tech Stack
- N8N (Low-code automation)
- HTTP Request Node
- IF Node (Conditional logic)
- N8N Node (SMS) Open AI Chat Model
- Cron Node

Workflow Overview
Cron Trigger Executes every hour.
HTTP Request Checks the availability of a website.
IF NodeCompares response status code.
N8N Trigger Node Sends an alert if the site is down.
Setup Instructions
Import the Workflow
1. Open [N8N Editor UI](https://n8n.io/)
2. Click on the top-right menu → `Import`
3. Upload `uptime-monitor-workflow.json` from this repo
2. Configure N8N Credentials
- In your N8N instance, go to `Credentials` → Triggers
- Enter your **Account SID**, **Auth Token**, and **From phone number**
 Edit Website URL
- Open the HTTP Request node and replace site URL.
 Add Your Phone Number
- In the N8N node, update the field with your verified number

Author
Tejaswi N

