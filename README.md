# ⚡ Polyglot Studio: Neural Core IDE

**Polyglot Studio** is a lightweight, ultra-responsive web-based code editor featuring multi-tab support, live previewing, and a high-contrast futuristic aesthetic. It is engineered for developers who need a fast, zero-install environment for web experimentation and script testing.

![Polyglot Studio Banner](link-to-your-icon.png)

## 🌟 Key Features

### 🧠 Monaco-Powered Intelligence
Utilizes the same core engine as VS Code, providing features like:
* **IntelliSense & Autocomplete:** Context-aware code suggestions.
* **Syntax Highlighting:** Support for JavaScript, HTML, CSS, Python, and more.
* **Multi-Cursor Editing:** Edit multiple lines at once for rapid refactoring.

### 🏓 Real-Time Sync (The Ping-Pong Technique)
Experience zero-latency updates with our custom synchronization engine:
* **The Ping:** Every keystroke in the editor broadcasts a payload via the `BroadcastChannel` API.
* **The Pong:** Internal iframes and detached pop-out windows listen for these pings and update their DOM content instantly without a full page reload.

### 📂 Advanced Workspace Management
* **Multi-Tab Architecture:** Open and switch between dozens of files while maintaining scroll position and undo history.
* **Dynamic Explorer:** A nested file tree that reflects your backend structure in real-time.
* **Symbol Outline:** An automatic scanner that parses your code for IDs, classes, and selectors for quick jumping.

### 🖥️ Integrated System Vitals
* **Live Preview:** Toggle a side-by-side view of your rendered web projects.
* **Backend Terminal:** Integrated shell feedback from the Node.js server to debug scripts and view console logs.
* **Visual Feedback:** A "Sync Dot" in the status bar blinks on every update, confirming your connection is live.



## 🛠️ Installation & Setup

### 1. Backend Configuration
Polyglot Studio requires a Node.js backend to handle file operations.
```bash
cd backend
npm install
node server.js
