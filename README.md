# 🚀 Polyglot Studio

A high-performance, web-based code editor with a focus on realtime visualization and multi-language support.

## ⚡ Core Features
* **Monaco Editor:** Desktop-grade coding with IntelliSense.
* **Ping-Pong Sync:** Instant, realtime updates to detached preview tabs via `BroadcastChannel`.
* **Multi-Tab UI:** Fluid file management with persistent state.
* **Smart Outline:** Automatic symbol and selector mapping for fast navigation.
* **Integrated Shell:** Realtime backend terminal feedback.

## 🛠️ Setup
1. **Backend:** Run your Node.js server on `port 3001`.
2. **Frontend:** Serve `index.html` via a local web server.
3. **Sync:** Open a "Live Preview" and click the detach icon to test realtime broadcasting.

## 📡 Sync Protocol
- **Sender:** `syncChannel.postMessage` triggers on every keystroke.
- **Receiver:** `channel.onmessage` replaces the preview DOM instantly without reloading.



## 📝 License
MIT
