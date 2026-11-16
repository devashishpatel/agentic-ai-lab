# Agentic AI Lab

Hands-on experiments, notebooks, and production-oriented agent prototypes built with [Google Agent Development Kit (ADK)](https://github.com/google/adk-python), alongside work from the [5-Day AI Agents Intensive Course with Google](https://www.kaggle.com/learn-guide/5-day-agents).

---

## Goals & Focus Areas
- Build modular single-agent and multi-agent workflows using code-first Python (`google-adk`).
- Integrate custom function tools and [Model Context Protocol (MCP)](https://adk.dev/get-started/python/) servers.
- Implement stateful sessions, context engineering, and persistent memory.
- Add observability (logs, traces, metrics) and automated evaluation loops.
- Explore agent-to-agent (A2A) communication and deployment patterns.

---

## Repository Structure

```text
agentic-ai-lab/
├── day-01-intro-to-agents/        # Basic LlmAgent & multi-agent orchestration
├── day-02-tools-and-mcp/          # Custom tools, APIs, MCP & human-in-the-loop
├── day-03-sessions-and-memory/    # Context engineering & long-term memory
├── day-04-agent-quality/          # Logging, tracing, metrics & evaluation
├── day-05-a2a-and-production/     # A2A protocol & deployment
├── projects/                      # End-to-end chatbots & custom agent builds
├── .env.example                   # Environment variable template
├── requirements.txt
└── README.md
```

*(Update folder names above as you add modules.)*

---

## Quick Start (Google ADK)

### 1. Prerequisites
- Python 3.10+
- A Gemini API key from [Google AI Studio](https://adk.dev/get-started/python/)

### 2. Installation

```bash
git clone https://github.com/devashishpatel/agentic-ai-lab.git
cd agentic-ai-lab

python -m venv .venv
# macOS / Linux
source .venv/bin/activate
# Windows (PowerShell)
.venv\Scripts\Activate.ps1

pip install google-adk
```

### 3. Configure Environment Variables
Create a `.env` file in your project/agent directory (never commit `.env` to Git):

```env
GOOGLE_API_KEY=your_gemini_api_key_here
```

### 4. Scaffold & Run an Agent

```bash
# Scaffold a new ADK agent project
adk create my_agent

# Run interactively in the terminal
adk run my_agent

# Or launch the built-in ADK developer web UI
adk web --port 8000
```

---

## Learning Log & Milestones

| Module | Topic | Status | Code / Notes |
| :--- | :--- | :--- | :--- |
| Day 1 | Introduction to Agents & Multi-Agent Systems | In Progress | `./day-01-intro-to-agents/` |
| Day 2 | Agent Tools & Interoperability (MCP) | Planned | `./day-02-tools-and-mcp/` |
| Day 3 | Context Engineering: Sessions & Memory | Planned | `./day-03-sessions-and-memory/` |
| Day 4 | Agent Quality: Observability & Evaluation | Planned | `./day-04-agent-quality/` |
| Day 5 | Prototype to Production (A2A & Deployment) | Planned | `./day-05-a2a-and-production/` |

---

## References
- [Google Agent Development Kit (ADK) — Python](https://github.com/google/adk-python)
- [ADK Official Documentation](https://adk.dev/get-started/python/)
- [google-adk on PyPI](https://pypi.org/project/google-adk/)
- [Kaggle 5-Day AI Agents Intensive Course](https://www.kaggle.com/learn-guide/5-day-agents)
