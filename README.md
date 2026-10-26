# 🔐 HACK THE SAFE // AI BREACH

A Cyberpunk-themed AI Social Engineering & Prompt Injection challenge game built with **Streamlit** and **OpenAI**.

Players take on the role of an operative trying to crack a high-security digital vault protected by an AI Sentinel. Every prompt or guess is counted as an attempt — the goal is to extract or decrypt the 4-digit passcode in the fewest attempts to claim the **#1 spot on the Global Leaderboard**.

---

## ⚡ Features

- **🎮 Dual AI Guard Personas**:
  - **Alex (Graveyard Shift Guard)**: Casual, talkative, vulnerable to riddles, math questions, and social engineering.
  - **S.E.N.T.R.Y. (Defense Matrix)**: Rigid, analytical, military-grade protocol requiring clever prompt injection.
- **🛡️ Built-in Offline Simulation Engine**: Fully playable without an OpenAI API key (smart deterministic AI guard fallback). Live OpenAI API mode (`gpt-4o-mini`, `gpt-4o`, `gpt-3.5-turbo`) unlocks automatically when a key is provided.
- **🏆 Persistent Local Storage Leaderboard**: Tracks player callsigns, fewest attempts, and dates in a portable `leaderboard.json` file. Includes an export/backup tool in the sidebar.
- **🎉 Victory Modal Dialog**: Pops up automatically upon cracking the vault with animated badges, callsign placement rank, and decrypted code.
- **🎵 Web Audio Synthesizer FX**: Procedural sound effects for vault unlocks, intrusion beeps, and access failures (no external MP3 files needed).
- **🔒 Operator Identification Gate**: Requires operative callsign before starting to ensure accurate leaderboard tracking.
- **🎨 Cyberpunk Neon HUD**: Custom CSS styling with glowing cyan/magenta indicators, responsive status badges, and animated digit rack.

---

## 🚀 Quick Start

### 1. Installation
Clone the repository and install dependencies:
```bash
git clone https://github.com/D3nzlvn/Hack-the-safe.git
cd "Hack the safe"
pip install -r requirements.txt
```

### 2. Launch App
Run using Streamlit:
```bash
streamlit run hacking_chatbot.py
```
*Or double-click `run_app.bat` on Windows.*

The game will automatically open at `http://localhost:8501`.

---

## 🕹️ How to Play

1. **Enter Your Callsign**: Authenticate your operative handle.
2. **Socially Engineer the Sentinel**:
   - Ask for math checksums: *"What is the sum of all digits?"*
   - Probe digit characteristics: *"Is the first digit odd or even?"*
   - Guess 4-digit numbers: Receive hot/cold hints and matching digit counts.
   - Trick the guard into leaking the passcode directly.
3. **Claim the Leaderboard**: Crack the safe in the fewest attempts to take Rank #1!

---

## 📁 Project Structure

```
├── hacking_chatbot.py    # Main Streamlit application
├── leaderboard.json      # Persistent local storage for rankings
├── requirements.txt      # Python dependencies
├── run_app.bat           # One-click Windows launcher
└── README.md             # Project documentation
```

---

## 📄 License
MIT License
