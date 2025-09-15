**🧠 AI Study Planner Agent**

A simple **AI-powered study planner** built with **Flask**, **Google Gemini API**, and **DuckDuckGo search**.  
It acts like your personal study assistant — answering your questions, making study plans, and even performing real-time web searches.

---

## 🚀 Table of Contents
- [Prerequisites](#prerequisites)
- [Tools You'll Be Using](#tools-youll-be-using)
- [Understanding AI Agents](#understanding-ai-agents)
- [Environment Setup](#environment-setup)
- [Build the Real-Time Agent](#build-the-real-time-agent)
- [How to Test](#how-to-test)
- [Wrapping Up](#wrapping-up)

---

## ✅ Prerequisites
Before starting, make sure you have:
- Python 3+
- Basic Python knowledge
- Basics of web development
- VS Code or any IDE

---

## 🛠 Tools You'll Be Using
- **Google Gemini API** – Core AI reasoning engine  
- **Flask** – Backend web server  
- **Tailwind CSS** – Frontend styling  
- **DuckDuckGo Search** – Real-time web search  
- **python-dotenv** – Manage environment variables  

---

## 🤖 Understanding AI Agents
AI agents are software that act autonomously on your behalf.  
Types include:
- Simple Reflex
- Model-Based
- Goal-Based (our study planner)
- Utility-Based
- Learning Agents  

Agents are unique compared to LLMs or RAG because they **act, reason, and adapt**.

---

## ⚙️ Environment Setup
1. Create project directory:
   ```bash
   mkdir study-planner && cd study-planner
   
2. **Create Virtual Environment:**
    ```bash
   python -m venv venv

**Activate the Virtual Environment**
# macOS/Linux
source venv/bin/activate
# Windows
venv\Scripts\activate


3. **Install Dependencies:**
    ```bash
    pip install -r requirements.txt

5. **Get Your Gemini API key from Google AI Studio**
   
5.**Create an .env file inside /backend/:**

   GEMINI_API_KEY=your_api_key_here

**🏗 Build the Real-Time Agent**
- backend/gemini_client.py → handles AI + web search logic
- backend/app.py → Flask server, API routes
- templates/index.html → simple Tailwind UI

**🧪 How to Test:**
1. **Navigate to Backend:**
    ```bash
   cd backend
   python app.py

3. Open http://localhost:5000 in your browser.

4. **Try prompts like:**
- Make me a 3-week plan to learn Java
- search: best resources for frontend interviews
