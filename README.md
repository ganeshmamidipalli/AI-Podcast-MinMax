
# 🎙️ AI Podcast Generator

Turn any web article into a two-host podcast conversation — powered by MiniMax M2.1 and MiniMax Speech 2.6.

## What It Does

Drop in a URL. Get back a podcast.

This tool takes written content and transforms it into natural, engaging audio dialogue between two AI hosts. No editing required.

**The Pipeline:**
1. **Scrape** → Firecrawl extracts clean content from any webpage
2. **Script** → MiniMax-M2.1 generates a conversational podcast script
3. **Speak** → MiniMax Speech 2.6 synthesizes multi-voice audio
4. **Merge** → All segments combine into a single podcast file

## Tech Stack

| Component | Purpose |
|-----------|---------|
| [MiniMax-M2.1](https://www.minimax.io/) | Script generation & dialogue creation |
| [MiniMax Speech 2.6](https://www.minimax.io/) | Text-to-speech synthesis |
| [Firecrawl](https://firecrawl.dev) | Web scraping & content extraction |
| [Streamlit](https://streamlit.io) | Web interface |

## Getting Started

### Prerequisites
- Python 3.12+

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ganeshmamidipalli/AI-Podcast-MinMax.git
   cd AI-Podcast-MinMax
   ```

2. **Set up the environment:**

   Install `uv` (fast Python package manager):
   ```bash
   # MacOS/Linux
   curl -LsSf https://astral.sh/uv/install.sh | sh

   # Windows
   powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
   ```

   Create and activate virtual environment:
   ```bash
   uv venv
   source .venv/bin/activate  # MacOS/Linux
   .venv\Scripts\activate     # Windows

   uv sync
   ```

3. **Configure API keys:**

   Create a `.env` file (see `.env.example`):
   ```env
   MINIMAX_API_KEY=<your_key>
   FIRECRAWL_API_KEY=<your_key>
   OPENROUTER_API_KEY=<your_key>
   ```

   **Get your keys:**
   - MiniMax → [platform.minimax.io](https://platform.minimax.io)
   - Firecrawl → [firecrawl.dev](https://firecrawl.dev)
   - OpenRouter → [openrouter.ai](https://openrouter.ai)

### Run the App

```bash
streamlit run app.py
```

Open `http://localhost:8501` in your browser.

### How to Use

1. Enter your API keys in the sidebar
2. Paste the URL of any article or blog post
3. Click **Generate Podcast**
4. Listen or download your podcast

## Why MiniMax-M2.1?

Open-source model delivering impressive benchmarks:
- **72.5%** on SWE-Multilingual
- **88.6%** on VIBE-bench

Claude-level performance at a fraction of the cost.

## Contributing

Contributions welcome! Fork the repo and submit a PR.

## Connect

Built by [Ganesh Mamidipalli](https://ganeshmamidipalli.com)

