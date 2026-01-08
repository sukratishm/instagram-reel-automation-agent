# Instagram Reel Automation

Automate faceless Instagram Reels end-to-end using **n8n** + **Blotato**.

This repo contains an **n8n workflow JSON** you can import, configure with environment variables, and run on a schedule to:
- generate reel content (script/caption),
- send it to Blotato for video creation,
- publish to Instagram.

> No faces were harmed in the making of this automation 😄

---

## What’s inside

- `workflow/instagram-reel-automation.n8n.json` — the n8n workflow (sanitized: no secrets)
- `.env.example` — environment variables you need to set in n8n
- `.gitignore` — keeps secrets out of Git history

---

## Requirements

- n8n (self-hosted or cloud)
- Blotato account + API key
- Instagram account connected in Blotato
- Any extra credentials referenced by your n8n nodes (e.g., OpenAI) configured in n8n

---

## Setup

### 1) Import the workflow into n8n
In n8n:
1. **Workflows** → **Import from File**
2. Select: `workflow/instagram-reel-automation.n8n.json`

### 2) Set environment variables (important)
This workflow expects these variables:

- `BLOTATO_API_KEY`
- `BLOTATO_INSTAGRAM_ID`

Create them in your n8n environment (recommended) or your hosting environment.

Use `.env.example` as a template.

### 3) Configure n8n credentials
If any nodes use external services (e.g., OpenAI, Google, etc.), configure their credentials inside n8n.

### 4) Activate
Turn the workflow **Active** and let it cook.

---

## Security note (please read)
✅ This workflow file is **sanitized** and does **not** include your real API key.  
Never commit real secrets to GitHub.

---

## License
MIT — do whatever you want, just don’t blame the workflow if your Reels become too powerful.
