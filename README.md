#  Cold Mail Bot

> Paste a LinkedIn post URL → AI writes a personalized cold email → Sends it from your own Gmail automatically.

[![Live Demo](https://img.shields.io/badge/Live-Demo-brightgreen?style=for-the-badge)](https://cold-mail-frontend.vercel.app)
[![Frontend](https://img.shields.io/badge/Frontend-React-blue?style=for-the-badge&logo=react)](https://github.com/ShouryaGoel007/cold-mail-frontend)
[![Backend](https://img.shields.io/badge/Backend-Flask-black?style=for-the-badge&logo=flask)](https://github.com/ShouryaGoel007/cold-mail-backend)

---

##  What it does

1. You paste a **LinkedIn post URL** from an HR
2. AI reads the post and writes a **personalized cold email**
3. Email gets sent from **your own Gmail** with your resume attached
4. All in under 30 seconds

---

##  Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | React, Vercel |
| Backend | Python, Flask, Render |
| AI | Groq (LLaMA 3.3 70B) |
| Email | Gmail API (OAuth 2.0) |
| Email Finding | Hunter.io API |

---

##  Repositories

| Repo | Description |
|------|-------------|
| [cold-mail-frontend](https://github.com/ShouryaGoel007/cold-mail-frontend) | React website — user interface |
| [cold-mail-backend](https://github.com/ShouryaGoel007/cold-mail-backend) | Flask API — scraping, AI, email sending |

---

##  How to Use

1. Open [cold-mail-frontend.vercel.app](https://cold-mail-frontend.vercel.app)
2. Click **Connect Gmail** and sign in with your Google account
3. Paste a LinkedIn post URL from any HR
4. Fill in HR name and company domain
5. Click **Generate Email**
6. Review and edit the AI-written email
7. Click **Send Email** — done!

---

##  How to Run Locally

### Backend
\`\`\`bash
git clone https://github.com/ShouryaGoel007/cold-mail-backend
cd cold-mail-backend
pip install -r requirements.txt
python app.py
\`\`\`

### Frontend
\`\`\`bash
git clone https://github.com/ShouryaGoel007/cold-mail-frontend
cd cold-mail-frontend
npm install
npm start
\`\`\`

### Environment Variables (Backend)
\`\`\`
GROQ_API_KEY=your_groq_key
HUNTER_API_KEY=your_hunter_key
LINKEDIN_COOKIES={"li_at":"...","JSESSIONID":"..."}
CREDENTIALS_JSON=your_google_oauth_json
REDIRECT_URI=your_backend_url/oauth2callback
FRONTEND_URL=your_frontend_url
SECRET_KEY=any_random_string
ADMIN_PASSWORD=your_admin_password
\`\`\`

---

##  Features

-  **Per-user Gmail** — every user sends from their own Gmail
-  **AI-powered emails** — LLaMA 3.3 70B writes personalized emails
-  **Auto email detection** — finds HR email from post or Hunter.io
-  **Resume attachment** — PDF resume attached automatically
-  **Profile saved** — your profile saved in browser, never retype
-  **Edit before send** — preview and edit email before sending

---


⭐ Star this repo if you found it useful!
