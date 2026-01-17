# 🛠️ Setup Instructions

Follow these steps carefully. Total setup time: ~30 minutes.

---

## 1. Upload Google Sheet

1. Upload `Faceless_Video_Tracker_Template.xlsx` to Google Drive
2. Open with Google Sheets
3. Copy Spreadsheet ID from the URL

---

## 2. Import Workflows into n8n

- Import files from `/workflows`
- Enable credentials later

---

## 3. Add Credentials

### Google Sheets
- OAuth2 credential
- Name: Google Sheets - Faceless Videos

### OpenAI
- Paste your OpenAI API key
- Name: OpenAI - GPT

---

## 4. Configure Workflow Placeholders

Replace everywhere you see:

- `YOUR_SPREADSHEET_ID`
- `YOUR_BLOTATO_API_KEY`
- `YOUR_INSTAGRAM_ACCOUNT_ID`

---

## 5. First Run Checklist

- At least 3 hooks in “Best Hooks” sheet
- Blotato account has credits
- Instagram account is Business/Creator

---

## 6. Activate Schedules

- Main workflow: daily posting
- Analytics workflow (optional): daily metrics

---

You're live 🚀
