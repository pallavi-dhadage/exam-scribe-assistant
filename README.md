# 📝 Exam Scribe Assistant

**Offline web app that helps human scribes assist blind and deaf students during exams.**  
Reduces scribe fatigue, speeds up dictation, and makes question/answer exchange clearer.

![Mockup of Blind Mode and Deaf Mode](https://via.placeholder.com/800x400?text=Screenshot+of+Blind+and+Deaf+Mode)  
*(Replace with your own screenshot after building the project)*

---

## 🎯 Problem Statement

Students who are **blind** or **deaf** often require a human scribe during exams (a common reasonable accommodation).  
Scribes currently:
- Type answers manually while listening to a blind student → slow, error‑prone.
- Communicate written questions to a deaf student → inconsistent, no large‑text support.

**Exam Scribe Assistant** solves this with two dedicated modes:

- **👁️ Blind Mode** – Scribe types/pastes the question → app reads it aloud. Student speaks their answer → app converts speech to text automatically.
- **👂 Deaf Mode** – Scribe types a question → app displays it in huge text. Scribe types the student’s written/signed answer.

All data stays **offline** and **on the device** – respects exam privacy and works without internet.

---

## ✨ Features

| Feature | Blind Mode | Deaf Mode |
|---------|------------|------------|
| Text‑to‑Speech (reads questions) | ✅ | ❌ |
| Speech‑to‑Text (dictates answers) | ✅ | ❌ |
| Large‑text question display | ❌ | ✅ |
| Manual answer typing | ❌ (voice only) | ✅ |
| Export answers to `.txt` file | ✅ | ✅ |
| Works completely offline | ✅ (Chrome/Edge) | ✅ |
| No data leaves your computer | ✅ | ✅ |

---

## 🖥️ Tech Stack

- **HTML5 / CSS3 / JavaScript** (vanilla, no build step)
- **Web Speech API** – speech synthesis (TTS) and speech recognition (STT)
- **LocalStorage / IndexedDB** – optional for session persistence
- **PWA manifest + service worker** – for offline caching (optional, see future)

Works best in **Google Chrome** or **Microsoft Edge** (speech recognition requires these browsers).

---

## 🚀 Getting Started

### 1. Download the repository

```bash
git clone https://github.com/your-username/exam-scribe-assistant.git
cd exam-scribe-assistant
