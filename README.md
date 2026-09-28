# 🤖 Python AI Research Agent

A simple AI research assistant built with **Python, LangChain, Anthropic Claude, DuckDuckGo, Wikipedia, and Pydantic**.

The agent accepts a research topic, uses available tools to gather information, generates a structured response, and can save the research output to a text file.

## ✨ Features

- 🤖 AI-powered research assistant using Anthropic Claude
- 🔎 Web search using DuckDuckGo
- 📚 Wikipedia search
- 🧩 LangChain tool calling / agent workflow
- 📋 Structured output using Pydantic
- 💾 Save research results to a text file
- 🐍 Simple Python project suitable for learning AI agents

## 🛠️ Tech Stack

- Python
- LangChain
- Anthropic Claude
- Pydantic
- DuckDuckGo Search
- Wikipedia
- python-dotenv

## 📁 Project Structure

```text
PythonAIAgentFromScratch/
│
├── main.py              # Main AI research agent
├── tools.py             # Search, Wikipedia and save tools
├── requirements.txt     # Python dependencies
├── sample.env           # Example environment variables
├── .env                 # Your private API keys (DO NOT upload)
├── .gitignore           # Files ignored by Git
└── README.md            # Project documentation
```

## 🔑 API Key Setup

This project requires an **Anthropic API key** because the application uses Claude.

### 1. Create a `.env` file

Create a file named `.env` in the project root:

```env
ANTHROPIC_API_KEY=your_anthropic_api_key_here
OPENAI_API_KEY=
```

### 2. Use your own API key

**Use your own Anthropic API key. Do not use or share someone else's API key.**

You can create an API key from the Anthropic Console:

https://console.anthropic.com/

> ⚠️ Never commit your `.env` file or expose your API key on GitHub.

The `sample.env` file can be committed because it contains only placeholders.

## 🚀 Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/PythonAIAgentFromScratch.git
cd PythonAIAgentFromScratch
```

### 2. Create a virtual environment

Windows:

```bash
python -m venv venv
venv\Scripts\activate
```

macOS/Linux:

```bash
python -m venv venv
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure your API key

Create `.env` and add your own Anthropic API key:

```env
ANTHROPIC_API_KEY=your_anthropic_api_key_here
```

## ▶️ Run the Project

```bash
python main.py
```

The application will ask:

```text
What can i help you research?
```

Enter a topic, for example:

```text
What is Generative AI?
```

The agent can use its configured tools to search for information and return a structured research response.

## 📤 Output Format

The application uses Pydantic to structure the response into:

```text
Topic
Summary
Sources
Tools Used
```

## 🔐 Security

Never upload your real API key to GitHub.

Your `.gitignore` should contain:

```gitignore
.env
.venv/
venv/
__pycache__/
*.pyc
research_output.txt
```

If an API key is accidentally pushed to GitHub, revoke/rotate the key immediately and replace it with a new one.

## 📚 Learning Goals

This project demonstrates basic concepts used when building AI agents with Python and LangChain:

- LLM integration
- Tool calling
- Agent execution
- Web search tools
- Structured output
- Pydantic models
- Environment variables
- Saving AI-generated results

## 🚧 Future Improvements

- Add conversation memory
- Add more research tools
- Add a Streamlit web interface
- Add PDF/document research
- Add RAG with a vector database
- Improve source handling and citations
- Add error handling and logging

## 👨‍💻 Author

**Sagar Fadatare**

GitHub: https://github.com/sagarfadatare

LinkedIn: https://www.linkedin.com/in/sagar-fadatare/
