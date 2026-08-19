# TERMINUS COMMAND CENTER (v7.4)

A high-performance, single-file real-time operations dashboard built for emergency dispatchers, team coordination, and low-latency collaboration. It features instant cross-browser synchronization via MQTT, custom themes, a micro pixel canvas with drag-to-draw capabilities, text-to-speech alerts, and secure burner messages.

---

## ✨ Key Features

* **Real-Time Sync:** Instant cross-browser communication powered by HiveMQ MQTT via WebSockets (`wss://`).
* **Micro Pixel Canvas:** A 16x16 interactive pixel grid featuring continuous drag-to-draw support, eraser functionality, and live synchronization across all connected operators.
* **Active Matrix Nodes (Radar):** Live presence tracking and operational status indicators for all connected nodes.
* **Subsystem Dispatch Feed:** Color-coded priority tiers (`Normal`, `Urgent`, `Critical`), real-time search filtering, and local transcript export.
* **Self-Destructing Burner Messages:** Optional 60-second self-destruct mode for sensitive logs.
* **Voice Dispatcher (TTS):** Built-in browser-based text-to-speech audio alerts for high-priority dispatches.
* **Dynamic Theme Engine:** Instantly switch visual skins (`cyberpunk`, `matrix`, `retro`, `void`).

---

## 🚀 Quick Start

Because this application is self-contained into a single file, deployment is instant:

1. Download or copy the **`index.html`** file.
2. Push the file to the root directory of a public GitHub repository.
3. Enable **GitHub Pages** in your repository settings (set the branch to `main` and folder to `/ (root)`).
4. Access your live web app directly via the provided GitHub Pages URL, or double-click the file locally to run it in any modern browser.

---

## ⌨️ Command & Shortcut Reference

### Slash Commands

Type these directly into the message input bar and press **Enter**:

* `/theme <name>` — Switch UI visual skin (`cyberpunk`, `matrix`, `retro`, `void`).
* `/clear` — Clear the feed view locally and broadcast a clear event to all nodes.
* `/del last` — Delete the most recent message.
* `/wipe` — Erase all chat history across connected clients.
* `/export` — Download the active log transcript as a text file.

### Keyboard Shortcuts

* **`Ctrl + K`** — Focus the feed search/filter bar.
* **`Alt + U`** — Focus the message input and tag the payload as urgent.
* **`Escape`** — Close active modals or unfocus input fields.
