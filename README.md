**Personal AI**

A hyper-functional, completely free, sleek, web‑based personal AI interface powered by [Ollama](https://ollama.ai/) and Node.js. It leverages Turndown for HTML-to-Markdown conversion, supports Deep Research modes, and offers advanced settings to customize models and behaviors.

---

## 📚 Table of Contents
- [Features](#-features)
- [Requirements](#-requirements)
- [Installation](#-installation)
- [Usage](#-usage)
- [Advanced Settings](#-advanced-settings)
- [License](#-license)

---

## ⚠️ Disclaimers

This AI may generate inaccurate or misleading information. Do **not** rely on it for critical tasks or decisions. While efforts have been made to reduce hallucinations, always verify output independently.
<br><br>
Additionally, a lot of memory, RAM, and CPU may be used due to the size of AI models, and you need a lot of RAM and CPU based on the models you are using. Using too big models or using many concurrent processes will take a lot of time, and it may even bug due to timeout errors, so beware.
---

## 🚀 Features

- **HTML-to-Markdown**: Uses [Turndown](https://github.com/domchristie/turndown) (via Cheerio) to extract and convert web content to Markdown.
- **Ollama Models**: Integrates with Ollama to run local LLMs like `qwen2.5vl:3b` and `deepseek-r1:1.5b`.
- **Deep Research Modes**: Multiple research depths and breadths settings for fine-grained control.
- **Customizable AI Settings**:
  - System prompts
  - Primary and auxiliary models
  - Temperature sliders
  - WebSocket concurrency limits
- **Responsive UI**: Built with Tailwind CSS for a polished, mobile‑friendly experience.
- **Different Modes**:
  - Normal - Quick and easy responses
  - Deep Think - For complex tasks
  - Search - If up-to-date information is needed
  - Search + Deep Think - If complex thinking is required while searching
  - Deep Research Lite - Comprehensive searching using AI and <strong>COMPLETELY UNPAID</strong> APIs with <strong>NO API KEYS REQUIRED</strong> and <strong>ABSOLUTELY NO USAGE LIMITS</strong>.
  - Heavy Duty Deep Research - An even more comprehensive search just like Deep Research Lite, but requiring complex thinking and higher depth research. 
  - Auto - Automatically chooses a mode for you based on the prompt. However, may be <strong>UNSTABLE</strong>.
- **Location Support**: For AI Searches regarding location, such as restaurants near you or how the weather is like.
- **No Tracking**: All of the AI's used here are completely local, meaning that there is absolutely no tracking (except for maybe google searches, as it is a network request; maybe your ISP can see what the AI searched up but doesn't know it was an AI). 

---

## 📋 Requirements

- **Node.js**: Latest LTS version (>=18.x).
- **Ollama**: Installed and configured on your machine.
  - Pull the recommended models:
    ```bash
    ollama pull qwen2.5vl:3b
    ollama pull deepseek-r1:1.5b
    ```

---

## 🛠️ Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/personal-ai.git
   cd personal-ai
   ```
2. **Install dependencies**:
   ```bash
   npm install
   ```
3. **Configure Ollama**:
   - Ensure Ollama is running and models are available.
   - In the **Advanced Settings** modal (Settings ⚙️), verify that `qwen2.5vl:3b` and `deepseek-r1:1.5b` appear in the model lists.

---

## 🚀 Usage

1. **Start the server**:
   ```bash
   npm start
   ```
2. **Open your browser** and navigate to `http://localhost:3000`.
3. **Interact** with your Personal AI:
   - Select a mode (e.g., Normal, Deep Think, Search, Deep Research Lite, Heavy Duty Deep Research).
   - Type messages in the input area and hit **Send**.
   - View AI responses in the chat window.

---

## ⚙️ Advanced Settings

In the **Settings** modal, you can fine-tune:

- **Custom System Prompt**: Shape the AI’s behavior.
- **Primary / Auxiliary Model**:
  - Select from local Ollama models (e.g., `qwen2.5vl:3b`, `deepseek-r1:1.5b`, or pull new ones).
  - Adjust **Temperature** (0.0–2.0) for creativity control.
- **Deep Research Lite**:
  - **Depth** (1–5): How thoroughly to research.
  - **Breadth** (1–5): How many sources to consult.
- **WebSocket Concurrency**: Limit simultaneous model requests.
- **Pull New Model**:
  - Enter an Ollama model name (e.g., `llama3:latest`) and click **Pull**.

---

## 📄 License

MIT © 2025 Shayaan Hooda
