# 🤖 Agentic-AI

A hands-on learning repository for building **Agentic AI** systems using [LangChain](https://www.langchain.com/). This project covers LangChain fundamentals, multi-provider model integration, tool use, and agent workflows — with practical Jupyter notebooks and Python scripts.

---

## 📁 Project Structure

```
Agentic-AI/
├── updatedLangchain/
│   ├── 1-langchainIntro.ipynb       # LangChain core concepts & chains
│   ├── 2-modelIntegration.ipynb     # Multi-provider LLM integration
│   └── 3-tools.ipynb                # Tool use & function calling
├── practiceLangchain/               # Scratch/practice notebooks
├── main.py                          # Project entry point
├── pyproject.toml                   # Project metadata & dependencies (uv)
├── requirements.txt                 # Pip-compatible requirements
├── .env                             # API keys (not committed)
├── .python-version                  # Python version pin
└── uv.lock                          # Locked dependency graph
```

---

## 🚀 Getting Started

### Prerequisites

- Python **3.13+**
- [`uv`](https://docs.astral.sh/uv/) *(recommended)* **or** `pip`

### 1. Clone the repository

```bash
git clone https://github.com/Sross123/Agentic-AI.git
cd Agentic-AI
```

### 2. Set up the environment

**Using `uv` (recommended):**
```bash
uv sync
```

**Using `pip`:**
```bash
python -m venv .venv
.venv\Scripts\activate        # Windows
# source .venv/bin/activate   # macOS / Linux
pip install -r requirements.txt
```

### 3. Configure API keys

Copy the example and fill in your keys:

```bash
cp .env.example .env
```

```env
# .env
OPENAI_API_KEY=your_openai_key
GROQ_API_KEY=your_groq_key
GOOGLE_API_KEY=your_google_gemini_key
```

### 4. Run notebooks

```bash
uv run jupyter lab
# or
jupyter lab
```

---

## 📚 Notebooks

| Notebook | Description |
|---|---|
| [`1-langchainIntro.ipynb`](updatedLangchain/1-langchainIntro.ipynb) | LangChain core — chains, prompts, output parsers |
| [`2-modelIntegration.ipynb`](updatedLangchain/2-modelIntegration.ipynb) | Integrating OpenAI, Groq, Gemini & Ollama |
| [`3-tools.ipynb`](updatedLangchain/3-tools.ipynb) | Tool use, function calling & agents |

---

## 🔌 Supported LLM Providers

| Provider | Package | Model Examples |
|---|---|---|
| **OpenAI** | `langchain-openai` | `gpt-4o`, `gpt-4-turbo` |
| **Google Gemini** | `langchain-google-genai` | `gemini-2.0-flash`, `gemini-1.5-pro` |
| **Groq** | `langchain-groq` | `llama-3.3-70b`, `mixtral-8x7b` |
| **Ollama** | `langchain-ollama` | `llama3`, `mistral` *(local)* |

---

## 🛠️ Tech Stack

- **[LangChain](https://python.langchain.com/)** — LLM application framework
- **[LangChain Community](https://github.com/langchain-ai/langchain)** — Community integrations
- **[Python Dotenv](https://pypi.org/project/python-dotenv/)** — Environment variable management
- **[uv](https://docs.astral.sh/uv/)** — Fast Python package manager
- **[Jupyter](https://jupyter.org/)** — Interactive notebooks

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the project
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
