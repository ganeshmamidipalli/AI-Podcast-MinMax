I built an AI podcasting studio that turns any website into a podcast.
The entire stack is open-source.
Here's how it works:

You provide a website URL
Firecrawl scrapes the content
MiniMax-M2.1 refines it and generates a podcast script
MiniMax Speech 2.6 converts it into a multi-speaker podcast

From URL to podcast in minutes.
Why MiniMax-M2.1?
It's the new open-source model making waves right now:
→ 72.5% on SWE-Multilingual
→ 88.6% on VIBE-bench
Performance that rivals closed-source alternatives at a fraction of the cost.
Tech Stack:

MiniMax M2.1 — script generation
MiniMax Speech 2.6 — text-to-speech
Firecrawl — web scraping

Check out the code: https://github.com/patchy631/ai-engineering-hub/tree/main/ai-podcast-generator
Open-source keeps pushing the boundaries of what's possible.

Want me to adjust the tone (more casual/more technical), shorten it, or add any specific details about your implementation?thsi my repo name https://github.com/ganeshmamidipalli/AI-Podcast-MinMax# AI Podcast Generator
Transform any web article or blog post into an engaging podcast between two speakers using [Minimax](https://www.minimax.io/) M2.1 and [Minimax](https://www.minimax.io/) Speech 2.6's state of the art capabilities.
## Overview
AI Podcast Generator is an intelligent tool that converts written content into natural-sounding podcast dialogues. Simply provide a URL, and the system will:
- Scrape and extract clean content from any webpage
- Generate an engaging two-host podcast script with natural conversation flow
- Converts the text script into audio segments for the podcast
- Merge all segments into a complete, ready-to-listen podcast
### Tech Stack
- **Minimax-M2.1** for intelligent script generation and dialogue conversion
- **Minimax Speech 2.6** for natural-sounding text-to-speech with multiple voice options
- **Firecrawl** for robust web scraping and content extraction
- **Streamlit** for an intuitive and interactive web interface
## How It Works
1. **Content Extraction**: Firecrawl scrapes the provided URL and extracts clean, structured content
2. **Script Generation**: Minimax-M2.1 analyzes the content and creates an engaging podcast dialogue between two hosts
4. **Audio Synthesis**: Each dialogue segment is converted to speech using Minimax's advanced TTS models
5. **Merging**: All audio segments are seamlessly combined into a single podcast file
6. **Delivery**: Users can listen to, download, and share their AI-generated podcast
## Installation & Setup
**Prerequisites**: Python 3.12+**Install dependencies:**
 First, install uv and set up the environment:
 bash
 # MacOS/Linux
 curl -LsSf https://astral.sh/uv/install.sh | sh
 # Windows
 powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
 
 Install dependencies:
 bash
 # Create a new directory for our project
 uv init ai-podcast-generator
 cd ai-podcast-generator
 # Create virtual environment and activate it
 uv venv
 source .venv/bin/activate  # MacOS/Linux
 .venv\Scripts\activate     # Windows
 # Install dependencies
 uv sync
 **Set up environment variables:**
Create a .env file with your API keys as specified in .env.example file:
env
MINIMAX_API_KEY=<YOUR_MINIMAX_API_KEY>
FIRECRAWL_API_KEY=<YOUR_FIRECRAWL_API_KEY>
OPENROUTER_API_KEY=<YOUR_OPENROUTER_API_KEY>
**Get your API keys:**
**Minimax**: [platform.minimax.io](https://platform.minimax.io)**Firecrawl**: [firecrawl.dev](https://firecrawl.dev)**OpenRouter**: [openrouter.ai](https://openrouter.ai)
You can enter these keys directly in the app's sidebar when you run it.
## Usage
### Running the Web Application
bash
streamlit run app.py

The app will open at http://localhost:8501
### Using the Application**Enter API Keys**: Input your Firecrawl, OpenRouter, and Minimax API keys in the left sidebar**Provide URL**: Enter the URL of the article or blog post you want to convert**Generate**: Click "Generate Podcast" and watch the magic happen**Listen & Download**: Once complete, listen to your podcast or download it for later
## 📬 Stay Updated with Our Newsletter!
**Get a FREE Data Science eBook** 📖 with 150+ essential lessons in Data Science when you subscribe to our newsletter! Stay in the loop with the latest tutorials, insights, and exclusive resources. [Subscribe now!](https://join.dailydoseofds.com)
[![Daily Dose of Data Science Newsletter](https://github.com/patchy631/ai-engineering/blob/main/resources/join_ddods.png)](https://join.dailydoseofds.com)
---
## Contribution
Contributions are welcome! Please fork the repository and submit a pull request with your improvements.chnage this reaadme file and same but differenlyShow more5:01 PMOrchestrated personalized README redesign maintaining original structure.The user wants me to rewrite the README file for their forked repository. They want it to be similar but different - essentially making it their own version while keeping the same structure and information. Let me create a fresh, clean README that reflects Ganesh's ownership of this project.Here's a refreshed README for your repo:

🎙️ AI Podcast Generator
Turn any web article into a two-host podcast conversation — powered by MiniMax M2.1 and MiniMax Speech 2.6.
What It Does
Drop in a URL. Get back a podcast.
This tool takes written content and transforms it into natural, engaging audio dialogue between two AI hosts. No editing required.
The Pipeline:

Scrape → Firecrawl extracts clean content from any webpage
Script → MiniMax-M2.1 generates a conversational podcast script
Speak → MiniMax Speech 2.6 synthesizes multi-voice audio
Merge → All segments combine into a single podcast file

Tech Stack
ComponentPurposeMiniMax-M2.1Script generation & dialogue creationMiniMax Speech 2.6Text-to-speech synthesisFirecrawlWeb scraping & content extractionStreamlitWeb interface
Getting Started
Prerequisites

Python 3.12+

Installation

Clone the repository:

bash   git clone https://github.com/ganeshmamidipalli/AI-Podcast-MinMax.git
   cd AI-Podcast-MinMax

Set up the environment:
Install uv (fast Python package manager):

bash   # MacOS/Linux
   curl -LsSf https://astral.sh/uv/install.sh | sh

   # Windows
   powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
Create and activate virtual environment:
bash   uv venv
   source .venv/bin/activate  # MacOS/Linux
   .venv\Scripts\activate     # Windows

   uv sync

Configure API keys:
Create a .env file (see .env.example):

env   MINIMAX_API_KEY=<your_key>
   FIRECRAWL_API_KEY=<your_key>
   OPENROUTER_API_KEY=<your_key>
Get your keys:

MiniMax → platform.minimax.io
Firecrawl → firecrawl.dev
OpenRouter → openrouter.ai

Run the App
bashstreamlit run app.py
Open http://localhost:8501 in your browser.
How to Use

Enter your API keys in the sidebar
Paste the URL of any article or blog post
Click Generate Podcast
Listen or download your podcast

Why MiniMax-M2.1?
Open-source model delivering impressive benchmarks:

72.5% on SWE-Multilingual
88.6% on VIBE-bench

Claude-level performance at a fraction of the cost.
Contributing
Contributions welcome! Fork the repo and submit a PR.
Connect
Built by Ganesh Mamidipalli
