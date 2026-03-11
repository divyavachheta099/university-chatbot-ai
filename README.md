# 🎓 UniBot — AI University Chatbot

An intelligent student support chatbot for **Crestwood University**, powered by the **Claude AI API** and built with **Vue.js**. Students can ask questions about admissions, deadlines, courses, tuition, and housing — and get instant, accurate AI-generated responses.

---

## ✨ Features

- 🤖 **Real AI responses** — powered by Claude (Anthropic) with full conversation memory
- 📋 **Covers 6 key topics** — Admissions, Deadlines, Courses, Tuition, Housing, Contact
- 💬 **Suggested follow-ups** — smart chips guide students to the next question
- ⚡ **Zero backend required** — runs entirely in the browser as a single HTML file
- 🎨 **Polished UI** — built with Vue 3 Composition API, animated typing indicator, responsive design
- 🌐 **Easy to customize** — just edit the system prompt with your university's real data

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend Framework | Vue.js 3 (Composition API) |
| AI Engine | Claude API by Anthropic |
| Styling | Pure CSS with CSS variables |
| Build Tool | Zero-build — single `.html` file |
| Deployment | GitHub Pages |

---

## 📂 Project Structure

```
university-chatbot-ai/
├── index.html        # Complete Vue.js app (UI + AI logic)
├── screenshot.png    # App preview image
└── README.md         # This file
```

---

## ⚙️ How to Run Locally

**No installation or build step required.**

1. Clone the repository:
   ```bash
   git clone https://github.com/divyavachheta099/university-chatbot-ai.git
   cd university-chatbot-ai
   ```

2. Open `index.html` directly in your browser — that's it!

> ⚠️ The Claude API is called directly from the browser. For production use, proxy API calls through a backend to protect your API key.

---

## 🧠 How the AI Works

The chatbot uses a **system prompt** to give Claude context about the university. Every user message — along with the full conversation history — is sent to the Claude API, which returns a contextual, accurate response.

```
User message
    ↓
Full conversation history
    ↓
Claude API (claude-sonnet-4)
    ↓
Formatted response displayed in chat
```

The system prompt includes university-specific data: GPA requirements, tuition rates, deadlines, program names, and contact info. This is the only section you need to edit to adapt the bot to a different institution.

---

## 🎨 Customizing for Your University

Open `index.html` and update the `SYSTEM_PROMPT` constant at the top:

```javascript
const SYSTEM_PROMPT = `You are UniBot, a friendly AI assistant for YOUR UNIVERSITY NAME.
Answer questions about:
- Admission Requirements: ...
- Deadlines: ...
- Tuition: ...
...`;
```

Change the university name, requirements, deadlines, and contact details — the chatbot instantly reflects your real data.

---

## 📚 What I Learned

- Integrating a **large language model API** into a frontend application
- Managing **conversation history** for multi-turn AI chat
- Building reactive UIs with **Vue 3 Composition API** (`ref`, `computed`, `nextTick`)
- Crafting effective **system prompts** to constrain and guide AI behaviour
- Designing accessible, responsive chat interfaces with **pure CSS animations**

---

## 🗺️ Future Improvements

- [ ] Add a **Flask/Node.js backend** to secure the API key
- [ ] Add **multilingual support** (French/English)
- [ ] Implement **user authentication** for personalized response

---

## 👤 Author

**Divya Vachheta**
- GitHub: https://github.com/divyavachheta099
- LinkedIn: https://www.linkedin.com/in/divya-vachheta-39b48717a/
- Email: divyajvachheta@gmail.com

---



> Built as part of a software development portfolio — demonstrating AI integration, Vue.js frontend development, and conversational UX design.
