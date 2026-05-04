# SellerIQ — Amazon Intelligence Platform
Before you get started please watch ## Demo Video at https://youtu.be/XlG1FPez2f8


Paste any Amazon product URL and get a full intelligence report:

- **Market Size** — how big is this market?
- **AI Visibility** — do OpenRouter / Groq / Gemini recommend you?
- **Review Analytics** — what do buyers actually want? Fake review detector.
- **Rufus Readiness** — how does Amazon's AI answer shopper questions about your product?
- **Competitor Spy** — where do you rank vs top players?
- **Fix It For Me** — AI-generated bullet rewrites for every gap found
- **Roast Mode** — Gen Z mode with brutal honest advice

---

## Setup

### 1. Get your API keys

| Key | Where |
|-----|-------|
| OpenRouter | https://openrouter.ai |
| Groq | https://console.groq.com |
| Gemini | https://aistudio.google.com |
| ScraperAPI | https://scraperapi.com |

### 2. Set environment variables on Railway

In Railway dashboard > Variables, add:

```
OPENROUTER_API_KEY=your_key
GROQ_API_KEY=your_key
GEMINI_API_KEY=your_key
SCRAPER_API_KEY=your_key
```

### 3. Deploy to Railway

1. Push this repo to GitHub
2. Go to railway.app > New Project > Deploy from GitHub
3. Select this repo
4. Add the environment variables above
5. Deploy — Railway auto-detects Python and uses the Procfile

### 4. Local development

```bash
pip install -r requirements.txt
export OPENROUTER_API_KEY=...
export GROQ_API_KEY=...
export GEMINI_API_KEY=...
export SCRAPER_API_KEY=...
python app.py
```

Open http://localhost:5000

---

## Tech Stack

- **Backend**: Python / Flask
- **Frontend**: Vanilla HTML/CSS/JS (Report Card aesthetic)
- **APIs**: OpenRouter (GPT-4o-mini), Groq (LLaMA 3), Gemini 1.5 Flash, ScraperAPI
- **Deploy**: Railway (free tier)

---

Built for Pixii.ai Founding Engineer application.
