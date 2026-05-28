# Math_Agent – Advanced Math Solver

[![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97-Live%20Demo-blue)](https://huggingface.co/spaces/kishor0101/MathWizard)
[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**MathWizard** is an AI‑powered mathematics tutor that solves equations, derivatives, integrals, and more – with **step‑by‑step explanations** and beautifully formatted **LaTeX** answers. Built with LangGraph, Groq LLM, Tavily search, and SymPy.

---

## Features

- **Step‑by‑Step Solutions** – Like Google Gemini / AI Studio, but runs on your own agent.
- **Adjustable Difficulty** – Ask for `easy`, `medium`, `hard`, or `very hard` explanations.
- **Equation Solver** – Handles linear, polynomial, exponential, logarithmic, and trigonometric equations.
- **Web Search** – Fetches additional math concepts or formulas (Tavily integration).
- **Friendly Bilingual Tutor** – Mixes English and simple Hindi to keep explanations engaging.
- **LaTeX Rendering** – Final answer always boxed: `\boxed{answer}`.
- **Interactive Chat** – Built with Gradio; full conversation history and copy buttons.

---

##  Tech Stack

| Technology | Purpose |
|------------|---------|
| **Python 3.11** | Core language |
| **LangGraph** | Multi‑agent workflow orchestration |
| **Groq (LLaMA 3.3 70B)** | Large language model for natural language reasoning |
| **SymPy** | Symbolic mathematics engine |
| **Tavily** | Web search tool (optional) |
| **Gradio** | Interactive chat UI |
| **Matplotlib** | (Future) Graph plotting |

---

## Installation (Local)

1. **Clone the repository**
   ```bash
   git clone https://github.com/kishor0101/Math_Agent.git
   cd Math_Agent

   Create a virtual environment (recommended)

2. python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

3. Install dependencies

pip install -r requirements.txt

4. Set up API keys
You need a Groq API key and (optional) a Tavily API key.
On Hugging Face Spaces, add them as Secrets (GROQ_API_KEY, TAVILY_API_KEY).
For local testing, set environment variables:

export GROQ_API_KEY="your-groq-key"
export TAVILY_API_KEY="your-tavily-key"

5. Run the app

python Math_Agent.py

Deployment on Hugging Face Spaces

1. Create a new Space → Docker SDK.

2. Push the repository (including Dockerfile, app.py, requirements.txt).

3. Add Secrets in Settings → Repository Secrets:

GROQ_API_KEY

TAVILY_API_KEY (optional)

4. The Space will automatically build and run.

Note: The Dockerfile uses a non‑root user, exposes port 7860, and installs all Python dependencies.

Contributing
Contributions, issues, and feature requests are welcome!
Feel free to open an issue or pull request.

License
Distributed under the MIT License. See LICENSE for more information.

Acknowledgements
Groq for lightning‑fast LLM inference

LangChain / LangGraph for agent orchestration

SymPy for symbolic mathematics

Tavily for web search

Gradio for the chat interface

Contact
Kishor – GitHub
Project Link: https://github.com/kishor0101/Math_Agent




