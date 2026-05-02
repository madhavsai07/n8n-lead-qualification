# 🚀 AI Lead Qualification Automation (n8n)

An AI-powered lead qualification system that automatically classifies incoming leads into **HOT, WARM, and COLD** using LLM analysis (Gemini/OpenAI) and rule-based decision logic.

---

## 🎯 Overview

Businesses often waste time manually filtering leads, resulting in slow response times and missed high-value opportunities.
This project automates lead qualification, enabling faster and smarter prioritization.

---

## ⚙️ Workflow Preview

### 🔹 Full Workflow

![Workflow](screenshots/workflow.png)

### 🔹 AI Output Parsing

![Parse Node](screenshots/parse-node.png)

### 🔹 Lead Classification Logic

![IF Logic](screenshots/if-logic.png)

---

## 🧠 How It Works

1. Lead data is captured via form submission
2. AI analyzes:
   - Intent
   - Budget
   - Urgency
   - Maturity

3. Structured JSON output is generated
4. Rule-based logic classifies leads:

- 🔥 **HOT** → High score + high urgency + strong confidence
- ❄️ **COLD** → Low score OR low budget OR unclear intent
- 🌤 **WARM** → Everything else

---

## ✨ Features

- AI-powered lead scoring
- Intent and urgency detection
- Automated classification (HOT / WARM / COLD)
- Multi-branch workflow routing
- Real-time processing
- Gmail alerts for high-priority leads
- Google Sheets integration for tracking

---

## 📤 Output

- 🔥 HOT → Instant notification + Sheet entry
- 🌤 WARM → Nurture pipeline
- ❄️ COLD → Low-priority storage

---

## 🛠 Tech Stack

- **n8n** – Workflow automation
- **Gemini / OpenAI API** – AI analysis
- **Google Sheets** – Data storage
- **Gmail API** – Notifications

---

## 🔐 Environment Setup

1. Copy `.env.example` → `.env`
2. Add required API keys
3. Configure credentials in n8n:
   - Google Sheets OAuth
   - Gmail OAuth
   - Gemini/OpenAI API

⚠️ Do not commit `.env` to GitHub

---

## 📦 Project Structure

```
N8N-Lead-Qualification/
│──screenshots/
│   ├── workflow.png
│   └── excel sheet.png
│── workflow/
│   └── ai-lead-qualification.json
│── README.md
│── .env.example
```

---

## 🚀 How to Use

1. Import workflow into n8n
2. Add required credentials
3. Connect Google Sheets
4. Execute workflow

---

## 🔮 Future Improvements

- CRM integration (HubSpot / Salesforce)
- Automated follow-ups
- Lead analytics dashboard
- Dynamic scoring model

---

## 👤 Author

**Madhav Sai Chinthaginjala**
