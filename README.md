# 📚 ExamFocus

> A sleek, all-in-one exam preparation dashboard — built with pure HTML, CSS & JavaScript. No frameworks. No backend. Just open and go.

![ExamFocus Screenshot](https://img.shields.io/badge/Status-Active-22c55e?style=flat-square) ![Version](https://img.shields.io/badge/Version-1.0-f59e0b?style=flat-square) ![License](https://img.shields.io/badge/License-MIT-6366f1?style=flat-square) ![HTML](https://img.shields.io/badge/Built%20with-HTML%2FCSS%2FJS-f59e0b?style=flat-square)

---

## ✨ Features

### 🏠 Dashboard — Exam Tracker
- Add exams with **name**, **subject**, **date & time**, and **priority** (High / Medium / Low)
- Live **countdown timer** showing Days, Hours, Minutes, Seconds for each exam
- Color-coded **priority badges** (🔴 High, 🟡 Medium, 🟢 Low)
- Mark exams as done once the date passes ("Exam Over ✓")
- Delete any exam (also clears its linked notes and PDFs)

### 📄 Study Material — PDF Manager
- Upload one or more **PDF files** per exam
- Files are read and stored entirely **in your browser** (no server needed)
- Open any PDF in a new browser tab for quick review
- Delete individual PDFs per exam

### ⏱️ Pomodoro Timer
- Classic **25-minute study / 5-minute break** cycle
- Animated **SVG ring** that depletes in real-time
- **Play / Pause / Reset / Skip** controls
- Audio **beep alert** when a session ends (via Web Audio API)
- Daily stats: **Cycles completed** and **Minutes studied** (auto-resets each day)

### 📝 Quick Notes
- Per-exam **sticky-note style** cards
- Write formulas, key points, and reminders
- **Auto-saves** as you type — character count shown in footer
- Color-coded card borders matching exam priority

---

## 🚀 Getting Started

No installation. No build step. No dependencies.

1. **Clone the repository**
   ```bash
   git clone https://github.com/Pradipdas647000/Exam-Focus.git
   cd Exam-Focus
   ```

2. **Open the app**
   ```bash
   # Just double-click ExamFocus.html
   # — or open it directly in your browser:
   open ExamFocus.html          # macOS
   xdg-open ExamFocus.html      # Linux
   start ExamFocus.html         # Windows
   ```

That's it. The app runs entirely in your browser.

---

## 🗂️ Project Structure

```
Exam-Focus/
└── ExamFocus.html    # The entire app — HTML + CSS + JS in one file
```

---

## 💾 Data Storage

All data is persisted using the browser's **`localStorage`** API under the key `examfocus_v2`. This includes:

| Data | Where Stored |
|------|--------------|
| Exams (name, subject, date, priority) | `localStorage` |
| Quick Notes (per exam) | `localStorage` |
| Uploaded PDFs (as Base64) | `localStorage` |
| Pomodoro stats (cycles, minutes, date) | `localStorage` |

> **⚠️ Note:** `localStorage` has a ~5–10 MB limit per origin. If you upload many large PDFs, you may hit this limit. The app will alert you when storage is full.

---

## 🎨 Design Highlights

- **Dark theme** with a deep navy (`#0b0d17`) background
- **Amber accent** (`#f59e0b`) for interactive elements and timers
- **Syne** font for headings, **Inter** for body text (via Google Fonts)
- Fully **responsive** — collapses to icon-only sidebar on small screens
- Smooth CSS transitions on hover, focus, and timer ring animation

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Structure | HTML5 |
| Styling | Vanilla CSS (CSS Variables, Grid, Flexbox) |
| Logic | Vanilla JavaScript (ES6+) |
| Storage | Web Storage API (`localStorage`) |
| Audio | Web Audio API |
| Fonts | Google Fonts (Syne, Inter) |

---

## 📋 Roadmap / Ideas

- [ ] Export notes as PDF or plain text
- [ ] PWA support (offline + installable)
- [ ] Custom Pomodoro durations (configurable study/break times)
- [ ] Dark/Light theme toggle
- [ ] Exam progress tracking (syllabus checklist per exam)
- [ ] Cloud sync via Firebase or similar

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the **MIT License** — feel free to use, modify, and distribute it.

---

## 👤 Author

**Pradip Das**
- GitHub: [@Pradipdas647000](https://github.com/Pradipdas647000)
- Email: daspradip1157@gmail.com

---

<p align="center">Made with ❤️ to help students stay focused and ace their exams.</p>
