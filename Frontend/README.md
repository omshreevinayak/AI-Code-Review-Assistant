# ⚡ AI Code Review Assistant – Gemini-powered Dev Helper

This project is a full-stack AI-powered code reviewer that helps developers understand and troubleshoot programming concepts. Built with a clean Node.js + Express backend integrated with Google’s Gemini API, and a fast, responsive React frontend using Vite.

---

## 🔧 Frontend Tech Stack

📁 Path: `code-review-main/Frontend`

- **Framework**: React.js (`App.jsx`, `main.jsx`, `vite.config.js`)
- **Build Tool**: Vite
- **Styling**: CSS (`App.css`, `index.css`)
- **Linting**: ESLint (`eslint.config.js`)

---

## 🛠️ Backend Tech Stack

📁 Path: `code-review-main/BackEnd`

- **Runtime**: Node.js
- **Framework**: Express.js (`app.js`, `server.js`)
- **Architecture**: MVC pattern with folders:
  - `controllers/` → route logic
  - `routes/` → API endpoints
  - `services/` → Gemini integration

- **Functionality**:
  - Accepts developer prompts via POST (e.g., "Explain closures in JavaScript")
  - Forwards prompts to Google’s **Gemini 2.5 Flash** model via `@google/genai`
  - Returns structured, conversational, and detailed AI-powered responses

---

## 🚀 Setup Instructions

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/code-review-main
   cd code-review-main

2. Create a .env file in BackEnd/:
   GOOGLE_GEMINI_API_KEY=your_api_key_here

3. Install dependencies:
    cd BackEnd
    npm install  
    npm start or npx nodemon