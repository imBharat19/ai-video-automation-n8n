<div align="center">
  <h1>🤖 AI Video Automation with n8n</h1>
  <p><b>A fully automated, low-code pipeline: Google Drive → AI SEO → YouTube Upload</b></p>

  ![n8n](https://img.shields.io/badge/n8n-FF6D5A?style=for-the-badge&logo=n8n&logoColor=white)
  ![Docker](https://img.shields.io/badge/Docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
  ![Google Drive](https://img.shields.io/badge/Google%20Drive-4285F4?style=for-the-badge&logo=googledrive&logoColor=white)
  ![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white)
  ![AI Powered](https://img.shields.io/badge/AI-OpenAI%20%7C%20Gemini-412991?style=for-the-badge)
</div>

---

> **Supports ANY content category:** Motivation, Quotes, Lifestyle, AI, Education, Wealth, Health, and Trending Reels.

## 🤖 Overview

This project is a fully automated AI-powered video publishing pipeline built using **n8n + AI models**.

Drop videos into Google Drive — everything else happens automatically:

- Detect topic  
- Generate viral SEO title  
- Create optimized description  
- Generate keywords  
- Generate 125 hashtags  
- Upload directly to YouTube  

Supports ANY niche:

Motivation • Quotes • Lifestyle • AI • Education • Wealth • Health • Trending Reels • Shorts

---

## ✨ Features

- Auto video detection (Google Drive)  
- AI topic understanding  
- Viral SEO titles with emojis  
- 5-line optimized descriptions  
- 50 trending keywords  
- 125 hashtags (100 viral + 25 AI)  
- Binary video handling  
- Automatic YouTube upload  
- Secure credential handling  

---

## 🏗 Architecture

Google Drive
    ↓
Watch Folder (n8n)
    ↓
Download Video
    ↓
AI SEO Generator
    ↓
Code Node (Merge JSON + Binary)
    ↓
YouTube Upload

---


---

## 🖥 Tech Stack

- n8n  
- Google Drive API  
- YouTube Data API  
- Gemini / OpenAI / Ollama  
- Docker  
- JavaScript (Code Node)  

---

## 📂 Project Structure

ai-video-automation-n8n/
│
├── workflows/
│ └── youtube-ai-automation.json
│
├── prompts/
│ └── seo_prompt.txt
│
├── env/
│ └── .env.example
│
├── screenshots/
│ ├── workflow.png
│ ├── code-node.png
│ └── youtube-upload.png
│
└── README.md


---

## 🐳 Run n8n (Docker)

```bash
docker run -it --rm \
-p 5678:5678 \
-v ~/.n8n:/home/node/.n8n \
n8nio/n8n
```

Open browser:
http://localhost:5678

⚙ Setup Guide
1. Import Workflow

n8n → Import → workflows/youtube-ai-automation.json

2. Configure Credentials

Create credentials inside n8n:

Google Drive OAuth

YouTube OAuth

AI Provider API Key

Never hardcode credentials.

3. Environment Variables

Copy:

.env.example → .env

Fill your own keys.

4. Update AI Prompt

Edit:

prompts/seo_prompt.txt
5. Run Workflow

Drop any video into your Drive folder.

Automation begins instantly.

🔐 Security

No credentials stored in repo

.env ignored

OAuth handled by n8n

Binary files stored locally

Never commit:

API Keys

OAuth Tokens

Personal Emails

Drive IDs

🚧 Roadmap
Phase 2

Instagram upload

TikTok upload

Auto captions

Phase 3

AI thumbnails

Engagement analytics

A/B title testing

Phase 4

Multi-account support

Feedback learning loop

Vector memory

⚠ Disclaimer

Educational automation project only.
Follow YouTube platform policies.

⭐ Support

If this helped:

Star ⭐
Fork 🍴
Build your own AI content factory 🤖

👨‍💻 Author

Built by Bharat

SQL Server DBA → Cloud → AI Automation Engineer
