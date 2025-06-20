﻿# 🧠 Agya AI - Your Hindi/English Voice Assistant

**Agya AI** is a smart, bilingual (Hindi + English) voice assistant developed in Python. It listens to your commands, speaks back in Hindi, answers using Google's Gemini API, opens websites, plays YouTube videos, and tells the time — all with voice interaction.

---

## 🚀 Features

### 🗣️ Voice Wake-Up
- Activates when you say: `hey agya`, `agya`, `are you there`, `hello`, etc.
- Once active, listens for further commands.

### 🧏 Speech Recognition
- Uses Google Speech-to-Text to understand spoken input.
- Robust error handling for unclear or failed input.

### 🔊 Text-to-Speech (TTS)
- Uses Microsoft Edge TTS (`edge-tts`) with `hi-IN-SwaraNeural` voice.
- Fluent Hindi/English voice output.

### 🌐 Web and Media Control
- `open <site>` → Opens websites (e.g., `open linkedin` opens `https://www.linkedin.com`)
- `play <video>` → Plays YouTube videos based on the query

### 🕒 Time Feature
- Asks: `what time is it?` or `time` → Replies with the current time.

### 🤖 AI-Powered Responses (Gemini API)
- For all other queries, Agya fetches smart answers from the **Gemini AI API** (Google).
- Replies in conversational Hindi.



---

## 📦 Tech Stack

| Module               | Purpose                           |
|----------------------|-----------------------------------|
| `edge-tts`           | Text-to-speech (Hindi)            |
| `speech_recognition` | Converts speech to text           |
| `requests`           | Interacts with Gemini API         |
| `playsound`          | Plays generated mp3 output        |
| `asyncio`            | Handles asynchronous TTS          |
| `tempfile` + `os`    | Temporary audio file management   |
| `.env`               | Stores API key securely           |

---

## 🛠️ Setup Instructions

### 1. Clone the Repo
```bash
git clone https://github.com/yourusername/agya-ai.git
cd agya-ai


# CREATE A VIRTUAL ENVIRONMENT  recommended
python -m venv .venv
.\.venv\Scripts\activate  # For Windows
