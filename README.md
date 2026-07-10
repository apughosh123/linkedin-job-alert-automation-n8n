# 🚀 LinkedIn Job Alert Automation using n8n

> Automate LinkedIn job scraping using **n8n**, **Apify API**, and **Google Sheets** with an AI-powered hiring summary.

---

## 📌 Project Overview

This workflow automates the process of collecting LinkedIn job postings.

Instead of manually searching LinkedIn every day, the workflow:

- Accepts search parameters via Webhook
- Starts the Apify LinkedIn Jobs Scraper
- Waits for the scraping process to finish
- Retrieves the latest job dataset
- Stores the results in Google Sheets
- Generates an AI hiring summary

---

## ✨ Features

- ✅ Webhook Trigger
- ✅ Dynamic Job Search
- ✅ Apify API Integration
- ✅ Actor Status Polling
- ✅ Google Sheets Integration
- ✅ AI Hiring Summary
- ✅ Error Handling
- ✅ Fully Automated Workflow

---

## 🛠 Tech Stack

- n8n
- Apify API
- Google Sheets
- HTTP Request
- AI Agent
- Webhooks

---

## 🔄 Workflow

```text
Webhook
      │
      ▼
HTTP Request
(Start Apify Actor)
      │
      ▼
Wait
      │
      ▼
HTTP Request
(Check Status)
      │
      ▼
IF (Succeeded?)
      │
      ▼
HTTP Request
(Get Dataset)
      │
      ▼
Google Sheets
      │
      ▼
AI Summary
      │
      ▼
Respond to Webhook
```

---

## 📥 Sample Webhook Payload

```json
{
  "jobTitle": "Python Developer",
  "location": "Remote",
  "limit": 20
}
```

---

## 📊 Google Sheet Output

The workflow stores:

- Job Title
- Company Name
- Location
- Posted Time
- Job URL
- Company URL

---

## 🤖 AI Summary

The AI Agent generates a short summary highlighting:

- Most common hiring companies
- Most common locations
- Hiring trends

---

## 📷 Screenshots

### Workflow

> Upload `workflow.png` inside the **screenshots** folder.

### Google Sheets Output

> Upload `google-sheet.png` inside the **screenshots** folder.

### AI Summary

> Upload `ai-summary.png` inside the **screenshots** folder.

---

## 📁 Repository Structure

```
linkedin-job-alert-automation-n8n
│
├── workflow/
│   └── linkedin-job-alert-automation.json
│
├── screenshots/
│   ├── workflow.png
│   ├── google-sheet.png
│   └── ai-summary.png
│
├── README.md
└── LICENSE
```

---

## 👨‍💻 Author

**Apu Ghosh**

AI Automation Specialist • n8n Developer
