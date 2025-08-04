# 🤖 Autodesk AI Bot — AI-Powered Service Desk Automation

This project is an intelligent AI-powered **Service Desk Bot** that automates common IT support tasks like resetting passwords, unlocking accounts, and creating tickets — all with natural language understanding.

Built using **Flask**, **LLaMA 3**, and **Groq**, this system combines the power of LLMs with real-time automation logic to simulate a production-grade service desk assistant.

---

## 🚀 Features

- 🔍 **Intent Detection** — Detects support intents like:
  - `reset_password`
  - `unlock_account`
  - `create_ticket`
- ✅ **User Confirmation** — Asks for confirmation before taking action.
- 📧 **Real Email Integration** — Sends password reset emails using Gmail SMTP.
- 🧠 **LLM-Powered NLP** — Uses LLaMA 3 via Groq API for fast and accurate prompt handling.
- 🧩 **Modular Design** — Clean architecture with separate services for actions, GPT handling, and utilities.

---

## 🗂️ Project Structure

```bash
autodesk_ai_bot/
│
├── app.py                      # Main Flask application
├── .env                        # Environment variables (ignored in Git)
├── services/
│   ├── email_service.py        # Email sending logic
│   └── action_service.py       # Handles actions like reset/unlock
├── utils/
│   ├── gpt_utils.py            # GPT prompt management
│   └── intent_handler.py       # Intent parsing and confidence
├── templates/
│   └── index.html              # Basic web interface (if used)
└── README.md                   # This file
