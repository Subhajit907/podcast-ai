# 🎙️ AI Podcast Generator

Transform any web article or blog post into an engaging, two-speaker podcast using **Minimax M2.1** and **Minimax Speech 2.6**.

AI Podcast Generator turns written content into natural, conversational audio—making it easy to listen to articles instead of reading them.

---

## 🚀 Overview

**AI Podcast Generator** is an intelligent tool that converts online content into high-quality podcast dialogues.
Simply provide a URL, and the system will:

* Scrape and extract clean, readable content from any webpage
* Generate an engaging, two-host podcast script with a natural conversational flow
* Convert the script into high-quality audio using multi-speaker text-to-speech
* Merge all audio segments into a single, ready-to-listen podcast file

From URL to podcast—in minutes.

---

## 🧰 Tech Stack

* **Minimax M2.1** – Intelligent script generation and dialogue creation
* **Minimax Speech 2.6** – Natural-sounding, multi-voice text-to-speech
* **Firecrawl** – Robust web scraping and content extraction
* **Streamlit** – Interactive and user-friendly web interface

---

## 🧠 How It Works

1. **Content Extraction**
   Firecrawl scrapes the provided URL and extracts clean, structured text.

2. **Script Generation**
   Minimax M2.1 analyzes the content and transforms it into an engaging podcast conversation between two hosts.

3. **Audio Synthesis**
   Each dialogue segment is converted into speech using Minimax’s advanced text-to-speech models.

4. **Audio Merging**
   All generated audio segments are seamlessly combined into a single podcast file.

5. **Delivery**
   Users can listen to, download, and share their AI-generated podcast.

---

## ⚙️ Installation & Setup

### Prerequisites

* **Python 3.12+**

---

### 1️⃣ Install Dependencies

First, install `uv` and set up the environment.

**MacOS / Linux**

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

**Windows**

```bash
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

Create and set up the project:

```bash
uv init ai-podcast-generator
cd ai-podcast-generator

uv venv
source .venv/bin/activate   # MacOS/Linux
.venv\Scripts\activate      # Windows

uv sync
```

---

### 2️⃣ Configure Environment Variables

Create a `.env` file using `.env.example` as a reference and add your API keys:

```env
MINIMAX_API_KEY=<YOUR_MINIMAX_API_KEY>
FIRECRAWL_API_KEY=<YOUR_FIRECRAWL_API_KEY>
OPENROUTER_API_KEY=<YOUR_OPENROUTER_API_KEY>
```

---

### 3️⃣ Obtain API Keys

* **Minimax**: [https://platform.minimax.io](https://platform.minimax.io)
* **Firecrawl**: [https://firecrawl.dev](https://firecrawl.dev)
* **OpenRouter**: [https://openrouter.ai](https://openrouter.ai)

You can also enter these keys directly from the app’s sidebar when running the application.

---

## ▶️ Usage

### Run the Web Application

```bash
streamlit run app.py
```

The app will be available at:
👉 `http://localhost:8501`

---

### Using the Application

1. **Enter API Keys**
   Add your Firecrawl, OpenRouter, and Minimax API keys in the left sidebar.

2. **Provide a URL**
   Paste the link to any article or blog post you want to convert.

3. **Generate Podcast**
   Click **Generate Podcast** and let the system do the rest.

4. **Listen & Download**
   Play the generated podcast directly in the app or download it for later.

---

## 🤝 Contributing

Contributions are welcome!
Feel free to fork the repository, make improvements, and submit a pull request.

