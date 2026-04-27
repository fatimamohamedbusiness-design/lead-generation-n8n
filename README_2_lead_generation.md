# 2. Lead Generation — Auto-Capture to Google Sheets + Email Alert
### n8n + Google Sheets + Gmail/SMTP

## What It Does
Every time a new lead fills a contact form or sends a message, this workflow automatically:
- Saves their info to a Google Sheet (name, email, phone, source, timestamp)
- Sends an instant email notification to the business owner
- Tags the lead as "New" for follow-up

**Use cases:** Clinics, gyms, real estate, online stores, freelancers

## Workflow
```
Webhook (form submission) → Format Lead Data → Google Sheets (save lead) → Send Email Alert → Respond OK
```

## Data Captured
| Field | Source |
|-------|--------|
| Full Name | Form input |
| Email | Form input |
| Phone | Form input |
| Service Interested In | Form input |
| Source / Channel | Auto-detected |
| Date & Time | Auto-generated |
| Status | "New Lead" |

## Setup
1. Import `workflow.json` into n8n
2. Connect your Gmail or SMTP credentials
3. Connect Google Sheets — set your lead tracker sheet ID
4. Embed the webhook URL in your contact form
5. Activate

## Tools
- [n8n](https://n8n.io) · Google Sheets · Gmail API

---
Built by **Fatma Mohamed** — Business Automation Specialist | [LinkedIn](https://linkedin.com/in/fatmamohamed-remot)
