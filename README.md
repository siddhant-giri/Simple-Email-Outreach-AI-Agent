
# Simple Email Outreach AI Agent (n8n Template)

🚀 **Automate your email outreach easily using this n8n-powered AI Agent!**  
This workflow helps you automatically generate and send personalized emails based on user inputs and AI-powered text generation.

---

## ✨ Features
- Automatically generate personalized outreach emails
- Send emails via your SMTP or Gmail account
- Customize email tone, style, and audience
- Modular and easy to adapt for different use cases
- Lightweight, no coding required

---

## 📦 What You Need
- **n8n** (self-hosted or cloud version)
- **Email Account** (SMTP or Gmail credentials set up in n8n)
- **Google Sheets Access** (For storing outreach data such as recipient emails, names, etc.)
- **OpenAI Access** OpenAI API Key if you're using AI for text generation

---

## ⚙️ Setup Instructions

1. **Import the Workflow**
   - Download this repository or copy the JSON file.
   - Open your n8n editor.
   - Click the three dots `...` next to **Workflows** ➔ **Import from File** ➔ Select the `.json` file.

2. **Configure Environment Variables**
   - Set up your credentials in n8n:
     - Email (SMTP / Gmail) node
     - (Optional) OpenAI Credentials node
   
3. **Connect to Google Sheets**
   - Ensure you have **Google Sheets access** set up in n8n.
   - Create a new sheet to store recipient details like name and email.
   - Update the Google Sheets node with the relevant sheet ID and range.
   
4. **Customize Templates**
   - Edit the content of the email generation node to match your outreach style (e.g., casual, formal, sales-focused).

5. **Test the Workflow**
   - Run it manually or trigger it using a webhook, cron, or another method.

6. **Go Live!**
   - Activate the workflow once you're happy with the results.

---

## 🛠️ Workflow Structure
- **Trigger Node** (Webhook / Schedule)
- **Google Sheets Node** (Fetch recipient data)
- **AI Node** (Generate email text)
- **Email Send Node** (SMTP / Gmail)
- **Success/Failure Check**

---

## 📌 Notes
- Keep your API Keys secure using environment variables.
- Ensure your SMTP provider allows automated emails to avoid account blocks.
- You can extend this workflow by integrating CRM tools, lead sheets, or LinkedIn outreach.

---

## 📬 Example Use Cases
- Cold email outreach for startups
- Sales drip campaigns
- Job application outreach
- Partnership collaboration requests

---

## 🧡 Credits
Created using [n8n.io](https://n8n.io) — the powerful open-source automation tool.
