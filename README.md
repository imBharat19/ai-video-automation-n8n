# ai-video-automation-n8n

🤖 AI Video Automation with n8n

Fully automated AI-powered video pipeline:

Google Drive → AI SEO → YouTube Upload

Supports ANY content category:
Motivation, Quotes, Lifestyle, AI, Education, Wealth, Health, Trending Reels.

🚀 Features

Auto detect video topic

Viral SEO title generation

5-line optimized description

50 keywords

125 hashtags (100 + 25 AI)

Binary video handling

Direct YouTube upload

Fully no-code/low-code

🧠 Architecture
Google Drive
   ↓
Watch Folder
   ↓
Download File
   ↓
AI SEO Generator
   ↓
Code Node (Merge Binary + SEO)
   ↓
YouTube Upload
🛠 Requirements

Docker

n8n

Google Drive API

YouTube Data API

OpenAI / Gemini / Ollama

🐳 Run n8n
docker run -it --rm \
-p 5678:5678 \
-v ~/.n8n:/home/node/.n8n \
n8nio/n8n
⚙ Setup

Import workflow from workflows/

Add credentials inside n8n UI

Configure Drive folder

Paste AI prompt

Run workflow

🔐 Security

No credentials stored in repo

Uses environment variables

.env ignored

OAuth handled inside n8n

Binary data kept local

NEVER commit:

API keys

OAuth tokens

Personal emails

Drive IDs

📁 Folder Guide
Folder	Purpose
workflows	n8n automation
prompts	AI SEO prompt
screenshots	UI reference
env	env examples
docs	diagrams
🚧 Roadmap

Instagram upload

TikTok upload

Auto captions

Thumbnail generation

Language detection

Scheduler

Analytics feedback loop

⚠ Disclaimer

Educational project only.
Respect platform policies.

🔐 EXTRA SECURITY (Highly Recommended)

Inside n8n:

Settings → Security

Enable:

✅ Basic Auth
✅ HTTPS (if public)
✅ Disable executions list
✅ Strong admin password
