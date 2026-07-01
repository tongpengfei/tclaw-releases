# tclaw — Your Local Private AI Assistant · [中文](README.md)

> Your AI. Your data. Your call. Yes I Can, Yes I do.

tclaw is a **ready-to-use** local private AI assistant. Just download, unzip, and run — all it takes is a few minutes to configure your API Key and you're good to go.

tclaw itself is **completely free**. Your only cost is the AI model service you choose, and many providers offer free credits to get started at zero cost.

All your conversations and files stay on your own computer — no cloud account, no data uploads, everything belongs to you.

**Supported model services**:
- 🔥 **Volcengine (Doubao)** — By ByteDance, fast access in China, great for beginners
- ☁️ **Alibaba Cloud Bailian (Qwen)** — By Alibaba Cloud, free credits available
- 🧠 **Zhipu AI (GLM)** — Free credits available
- 🌊 **DeepSeek** — Excellent value, strong reasoning
- 🌙 **Moonshot (Kimi)** — Great for long-context tasks
- 🤖 **Claude (Anthropic)** — Strong all-around capability
- ⚙️ **Custom provider** — Any service compatible with the OpenAI protocol

---

## Showcase

### Demo Video

https://github.com/tongpengfei/tclaw-releases/raw/main/docs/showcase/tclaw_showcase_01.mp4

### Screenshots

| CLI Launch | Xiaohongshu Content Generation |
|---|---|
| ![CLI](https://github.com/tongpengfei/tclaw-releases/raw/main/docs/screenshots/tclaw01_cli01.png) | ![Xiaohongshu](https://github.com/tongpengfei/tclaw-releases/raw/main/docs/screenshots/tclaw02_xhs01.png) |

| Stock Analysis | File Browser |
|---|---|
| ![Stock](https://github.com/tongpengfei/tclaw-releases/raw/main/docs/screenshots/tclaw03_stock01.png) | ![File Browser](https://github.com/tongpengfei/tclaw-releases/raw/main/docs/screenshots/tclaw04_file_browser01.png) |

| Debug Logs | Apps |
|---|---|
| ![Logs](https://github.com/tongpengfei/tclaw-releases/raw/main/docs/screenshots/tclaw05_log01.png) | ![Apps](https://github.com/tongpengfei/tclaw-releases/raw/main/docs/screenshots/tclaw06_apps01.png) |

| Code Dev 1 | Code Dev 2 |
|---|---|
| ![Code1](https://github.com/tongpengfei/tclaw-releases/raw/main/docs/screenshots/tclaw07_code01.png) | ![Code2](https://github.com/tongpengfei/tclaw-releases/raw/main/docs/screenshots/tclaw08_code02.png) |

---

## What can it do?

### 📋 Research & Summarize
Paste an article, report, or conversation and let AI extract key points, restructure content, or translate it — without copying and pasting to a web AI tool every time.

### 📊 Analyze Documents & Data
Upload CSV, Excel, PDF, or text files. Ask questions, get analysis reports, or let AI surface the key data you need.

### 🛠️ Build Your Own Productivity Tools (Apps)
Create custom AI workflows — just describe what you want: auto-format meeting notes, batch rename files, generate weekly reports, and more.

### 🌐 Generate Web Prototypes
Describe the page you have in mind and AI generates a previewable HTML prototype — great for validating ideas or communicating requirements.

### 📁 Manage Local Files
Built-in file browser lets you browse, preview, and organize local files, with AI assistance for batch document processing.

### 💬 Chat via Feishu / WeChat
Send messages to your AI directly from Feishu or WeChat — ask questions, look things up, or handle tasks on the go, without opening the desktop app.

---

## Features

- **Fully local**: Conversations stay on your machine, never passing through any third-party server
- **Multi-model support**: Compatible with OpenAI and Anthropic protocols — any service implementing either protocol can be connected
- **Lightweight**: Single executable, unzip and run, no Python / Node / other dependencies required. CLI ~8 MB, GUI ~10 MB
- **Cross-platform**: macOS, Windows, and Linux versions available

---

## Installation

### macOS (GUI recommended)
1. Download `tclaw-darwin-arm64-gui.dmg` (Apple Silicon) or `tclaw-darwin-amd64-gui.dmg` (Intel)
2. Open the DMG and drag `tclaw.app` into your **Applications** folder
3. Double-click to launch

> **Note**: If macOS says the app is "damaged" or "cannot be verified", run this in Terminal:
> ```
> xattr -cr /Applications/tclaw.app
> ```
> Then try opening again. This is a standard macOS restriction for apps without Apple notarization.

### Windows (GUI)
1. Download `tclaw-windows-amd64-gui.zip` and unzip
2. Double-click `tclaw.exe`
3. If a security warning appears, click **More info → Run anyway**

### CLI (all platforms)
Download the ZIP for your platform, unzip, then:
1. Copy `config.json.example` to `config.json` and fill in your API Key
2. Run `./tclaw` and open `http://localhost:PORT` in your browser

---

## Quick Start

### Step 1: Configure your API Key
Open Settings (gear icon, bottom left), select your model provider, and enter your API Key.  
A setup wizard will guide you on first launch.

### Step 2: Start a conversation
Click「+」in the top left to create a new session and start asking questions.

### Step 3: Upload files
Click the 📎 button next to the input box to upload documents, images, or code files.

### Step 4: Use Apps
Click the Apps icon on the left sidebar to explore built-in tools or create your own workflow.

---

## Share Your Ideas

What work scenarios do you most want tclaw to help with? Feel free to open an [Issue](../../issues) — your feedback directly shapes what gets built next.

---

## Feedback & Support

Found a bug or have a suggestion? Please open an [Issue](../../issues) and I'll keep improving tclaw.
