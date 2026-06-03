# 📖 Dyslexia AI Reading Assistant

An AI-powered reading tool designed to help people with dyslexia read, understand, and interact with documents more easily. Upload a PDF or DOCX, get a simplified version powered by Claude AI, and listen along with word-by-word text-to-speech highlighting.

---

## 📸 Screenshots

> _Add your screenshots here. Replace the placeholder paths below with your actual image files._

| Home Screen | Reading View | AI Assistance |
|---|---|---|
| ![Home Screen](screenshots/home.png) | ![Reading View](screenshots/reading.png) | ![AI Assistance](screenshots/ai.png) |

> **Figma Design:** [View UI Design on Figma](#) ← _paste your Figma link here_

---

## ✨ Features

- **📄 Document Upload** — Drag and drop or browse for PDF and DOCX files (up to 10MB)
- **🤖 AI Simplification** — Automatically rewrites document text into simpler language using Claude AI
- **🔊 Text-to-Speech** — Word-by-word playback with live highlighting so readers can follow along
- **🎛️ Reading Controls** — Adjustable playback speed (0.5x–2x), font size, and font family
- **🔖 Bookmarks** — Save and search your reading positions across documents
- **🧠 AI Assistance Panel** — Dedicated tools to Simplify, Summarise, Define Terms, or extract Key Points from any text
- **⚙️ Settings** — Customise font, font size, TTS voice preference, speed, volume, and simplification level
- **💾 Persistent Storage** — Documents, bookmarks, and settings are saved across sessions

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | Vanilla HTML, CSS, JavaScript (single-file app) |
| AI Engine | [Anthropic Claude API](https://www.anthropic.com/) (`claude-sonnet-4-20250514`) |
| DOCX Parsing | [Mammoth.js](https://github.com/mwilliamson/mammoth.js) (client-side) |
| PDF Extraction | Anthropic API document blocks (base64) |
| Storage | `window.storage` API (persistent key-value) |
| TTS | Web Speech API (browser-native) |

---

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge, Safari)
- An [Anthropic API key](https://console.anthropic.com/)

### Running Locally

This project is a **single HTML file** — no build tools or installs required.

1. Clone the repository:
   ```bash
   git clone https://github.com/BiniyamAFirde/dyslexia_reading_assistant.git
   cd dyslexia_reading_assistant
   ```

2. Open `dyslexia_reading_assistant.html` directly in your browser:
   ```bash
   open dyslexia_reading_assistant.html   # macOS
   ```
   Or just double-click the file in Finder.

> **Note:** The Anthropic API key is handled by the environment this app is embedded in (e.g. Claude.ai Artifacts). If running standalone, you may need to add your own API key to the fetch headers in the script section.

---

## 📁 Project Structure

```
dyslexia_reading_assistant/
├── dyslexia_reading_assistant.html   # Main application (self-contained)
├── screenshots/                      # Add your screenshots here
│   ├── home.png
│   ├── reading.png
│   └── ai.png
└── README.md
```

---

## 🖥️ How to Use

1. **Upload a Document** — Click "Upload Document" on the home screen and select a PDF or DOCX file
2. **AI Simplification** — The app automatically extracts and simplifies the text using Claude AI
3. **Read Along** — Press ▶ to start TTS playback; each word highlights as it is spoken
4. **Adjust Settings** — Use the ⚙️ icon to change font, size, and audio preferences
5. **AI Assistance** — Tap 🤖 from any screen to Simplify, Summarise, Define Terms, or pull Key Points from text
6. **Bookmarks** — Tap 🔖 while reading to save your position; access all bookmarks from the home screen

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you'd like to change.

---

## 📄 License

[MIT](LICENSE)

---

## 👤 Author

**Biniyam A. Firde**
- GitHub: [@BiniyamAFirde](https://github.com/BiniyamAFirde)
