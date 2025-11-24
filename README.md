
---

# 🌿 Murf AI Voice Agents Challenge – Day 3: Health & Wellness Companion

This repository contains my submission for **Day 3** of the **Murf AI Voice Agents Challenge**, featuring a fully functional **Health & Wellness Voice Companion** with JSON-based persistence and contextual memory.

---

## 🎯 Challenge Objective

### **Day 3 Goal**

Build a wellness voice companion that performs daily check-ins using natural voice interaction and saves all user data in JSON format.

### **Core Requirements**

* Well-defined system prompt for a supportive wellness companion
* Voice-based daily conversations
* Collect daily mood, energy, goals, and concerns
* Persist all check-ins in a `.json` file
* Reference previous logs in future sessions

---

## ✨ What I Built

### ✅ **Wellness Voice Companion**

A supportive, non-medical wellness agent that:

* Conducts structured daily check-ins
* Provides simple, actionable tips
* Saves each check-in to `wellness_log.json`
* Loads and references past logs naturally

### ✅ **Daily Check-In Flow**

* Mood assessment
* Energy level check
* Stress/concern inquiry
* Collection of 1–3 daily intentions
* Additional notes support
* Summary + confirmation
* Auto-saved JSON record

### ✅ **Function Tools Implemented**

| Function             | Purpose                  |
| -------------------- | ------------------------ |
| `set_mood()`         | Record user mood         |
| `set_energy()`       | Capture energy level     |
| `set_stress()`       | Store stress/concerns    |
| `add_objective()`    | Add daily goals          |
| `add_note()`         | Add optional reflections |
| `complete_checkin()` | Save all data to JSON    |

---

## ⚙️ Technical Achievements (Day 3)

* Set up complete development environment (Python 3.11, Node.js, pnpm, uv)
* Integrated **Murf Falcon TTS**
* Linked **Google Gemini** for reasoning
* Integrated **Deepgram STT**
* Fully connected backend + frontend + LiveKit
* Built JSON-based persistence layer
* Held real-time voice conversations with agent
* Pushed complete code to GitHub

---

## ☕ Day 2 Recap – Coffee Shop Barista Agent (Completed)

### ✔ Highlights

* “**Brew**” — friendly barista persona
* Order state management system
* JSON order logging
* Clarifying questions before finalizing order

### ✔ Tools Implemented

* `set_drink_type()`
* `set_size()`
* `set_milk()`
* `add_extra()`
* `set_customer_name()`
* `complete_order()`

### ✔ Advanced Challenge Completed

* Real-time beverage visualization (HTML/CSS/JS)
* Dynamic cup size
* Animation for filling drink
* Toppings rendering
* Live order summary
* Smooth UI with Starbucks-styled theme

---

## 📁 Repository Structure

```
ten-days-of-voice-agents-2025/
├── backend/          # LiveKit Agents backend (Python)
├── frontend/         # Next.js UI for voice interaction
├── challenges/       # Daily task documentation
└── README.md         # Project documentation
```

---

## 🧠 Backend (Python)

Built using **LiveKit Agents** + **Murf Falcon TTS**.

**Features:**

* Streaming TTS
* Speaker turn detection
* Noise/background cancellation
* Function calling
* LLM-driven dialog
* JSON persistence
* Docker support
* Integrated evaluation test suite

---

## 🎨 Frontend (React/Next.js)

Based on LiveKit's **agent-starter-react** template.

**Features:**

* Live voice interaction
* Microphone & camera streaming
* Real-time audio visualization
* Data channel integration
* Light/dark themes
* Custom UI branding
* Barista-inspired beverage visualization (Day 2)

---

## 🚀 Quick Start

### **1. Prerequisites**

* Python 3.11 or 3.12
* uv package manager
* Node.js 18+ with pnpm
* LiveKit Server binary

---

### **2. Clone Repository**

```bash
https://github.com/vikasyadav097/AI-Voice-Agents-Challenge-Day-3-Health-Wellness-Voice-Companion- 
```

---

### **3. Backend Setup**

```bash
cd backend
uv sync --python 3.11
```

Create `.env.local`:

```
LIVEKIT_URL=ws://127.0.0.1:7880
LIVEKIT_API_KEY=devkey
LIVEKIT_API_SECRET=secret
MURF_API_KEY=<your-murf-api-key>
GOOGLE_API_KEY=<your-google-api-key>
DEEPGRAM_API_KEY=<your-deepgram-api-key>
```

Download required models:

```bash
uv run python src/agent.py download-files
```

---

### **4. Frontend Setup**

```bash
cd ../frontend
pnpm install
```

Add `.env.local`:

```
LIVEKIT_API_KEY=devkey
LIVEKIT_API_SECRET=secret
LIVEKIT_URL=ws://127.0.0.1:7880
```

---

### **5. Run LiveKit Server**

```bash
.\livekit-server.exe --dev   # Windows
# ./livekit-server --dev     # Mac/Linux
```

---

### **6. Run Backend**

```bash
cd backend
.venv\Scripts\Activate.ps1
python src/agent.py dev
```

---

### **7. Run Frontend**

```bash
cd frontend
pnpm dev
```

Open: **[http://localhost:3000](http://localhost:3000)**

---

## 📑 Data Structure

Each check-in entry includes:

* Timestamp
* Mood
* Energy level
* Stress notes
* Daily objectives
* Additional reflections
* Auto-generated summary

Saved in:

```
backend/wellness_log.json
```

---

## 📅 Challenge Progress

| Day      | Status         |
| -------- | -------------- |
| Day 1    | ✅ Completed    |
| Day 2    | ✅ Completed    |
| Day 3    | ✅ Completed    |
| Day 4–10 | 🔜 Coming soon |
                                                                                            |

---

## 🛠 Tech Stack

**Backend:** Python, LiveKit Agents, Murf Falcon TTS, Google Gemini, Deepgram STT
**Frontend:** Next.js 15, React 19, Tailwind, TypeScript, Framer Motion
**Communication:** LiveKit Server
**Package Managers:** uv (Python), pnpm (Node.js)

---

## 📚 Resources

* Murf Falcon API
* LiveKit Agents
* Deepgram STT
* Gemini developer docs

---

## 📄 License

Based on MIT-licensed starter templates provided by LiveKit.

---

## 🙌 Final Note

This project is part of the **10 Days of AI Voice Agents Challenge** by Murf.ai.
The goal: build, learn, innovate, and push the limits of voice AI.

---



Just tell me!
