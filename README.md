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

## 🚀 Features

* **🧠 Auto-Detect Video Topic:** Understands context before generating metadata.
* **🔥 Viral SEO Title Generation:** Optimized hooks for maximum click-through rates.
* **📝 Smart Descriptions:** 5-line, highly optimized video descriptions.
* **🔑 Keyword & Hashtag Engine:** Generates 50 tags + 125 hashtags (100 standard + 25 AI-tailored).
* **⚙️ Binary Video Handling:** Efficiently processes large video files.
* **📺 Direct YouTube Upload:** No manual intervention required.
* **🛠️ Fully No-Code/Low-Code:** Easy to maintain and customize.

---

## 🧠 Architecture



```mermaid
graph LR
    A[Google Drive] -->|Watch Folder| B(Download File)
    B --> C{AI SEO Generator}
    C -->|Generate Metadata| D[Code Node]
    B -->|Binary Data| D
    D -->|Merge Binary + SEO| E[YouTube Upload]
    E --> F((Live Video!))
    
    style A fill:#4285F4,stroke:#fff,stroke-width:2px,color:#fff
    style E fill:#FF0000,stroke:#fff,stroke-width:2px,color:#fff
    style C fill:#412991,stroke:#fff,stroke-width:2px,color:#fff
