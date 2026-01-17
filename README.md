# 🎬 Faceless Video Automation with Memory System

Create and publish faceless Instagram videos automatically using AI with a built-in memory system that **prevents repeated topics** and **learns from your best-performing hooks**.

Powered by **n8n + OpenAI + Blotato + Google Sheets**.

---

## 🚀 What This System Does

✅ Generates 50 unique video ideas daily (GPT-powered)  
✅ Randomly selects 1 idea (while avoiding past topics)  
✅ Writes a full 25-second script + caption  
✅ Creates a faceless video via Blotato  
✅ Publishes the video to Instagram automatically  
✅ Logs everything into Google Sheets for tracking  

---

## 🧠 Why This Is Different (Memory System)

Most AI content systems generate random scripts with no context.

This one **remembers everything you’ve posted** and improves over time by:
✅ tracking used topics automatically  
✅ studying your best-performing hooks  
✅ reusing winning hook formats while generating fresh topics  

Result: **less repetition, stronger hooks, better growth.**

---

## 📦 Included Files

Faceless_Video_Workflow_CLEAN.json

Faceless_Video_Tracker_Template.csv ✅ (Upload this to Google Sheets)


---

## ⚡ Quick Start Setup (10 Minutes)

### 1) Create Your Google Sheet
1. Open Google Drive → **New → Google Sheets**
2. Go to **File → Import**
3. Upload:  
   ✅ `sheets/Faceless_Video_Tracker_Template.csv`
4. This sheet becomes your **Reel Log** tracker.

---

### 2) Import Workflow into n8n
1. Open n8n
2. Workflows → **Import from file**
3. Import:
   ✅ `workflows/Faceless_Video_Workflow_CLEAN.json`

---

### 3) Add Credentials in n8n
✅ Google Sheets OAuth2 Credential  
✅ OpenAI API Credential  

---

### 4) Configure Placeholders
Open the workflow and replace these values:

#### In ALL Google Sheets nodes:
- `YOUR_SPREADSHEET_ID`

#### In “Prepare Video” node:
- `YOUR_BLOTATO_API_KEY`

#### In “Prepare for Publish” node:
- `YOUR_BLOTATO_API_KEY`
- `YOUR_INSTAGRAM_ACCOUNT_ID`

---

### 5) Run Your First Test
✅ Add at least 3 hooks into the **Best Hooks** tab in your Google Sheet  
✅ Click **Execute Workflow** in n8n  
✅ Confirm a new row appears in your sheet  

---

## 🧩 Customization Options

You can easily change:

✅ Posting schedule (Schedule Trigger node)  
✅ Video style (cinematic / modern / vintage)  
✅ Voice (ElevenLabs voiceId)  
✅ Hook formats + script rules (AI Agent prompt)  

---

## 🐛 Troubleshooting

### Google Sheets errors
✅ Spreadsheet ID wrong OR Google credential not connected

### AI repeats topics
✅ Make sure your sheet has past rows in Reel Log  
✅ Confirm "Topic" column exists and is populated

### Video fails to generate
✅ Blotato credits missing or API key invalid

### Instagram publish fails
✅ Account ID wrong OR Instagram account not connected in Blotato

---

## 🔐 Security Notes

This repo contains **NO API keys** and **NO personal IDs**.

Never commit:
- OpenAI keys
- Blotato keys
- Instagram IDs
- Spreadsheet IDs

---

## 📄 License
MIT — free for personal + commercial use.

---

## ✅ You’re Ready

Once configured, this system becomes a self-improving content machine that:
✅ posts daily  
✅ remembers what worked  
✅ avoids repeats  
✅ improves hooks automatically  

Happy automating 🚀


