# AI Agents Lab

A hands-on repository tracking my learning journey, implementations, and experiments through the **AI Agents Masterclass**.

---

## 🗺️ Learning Roadmap

### Core Masterclass

| # | Module | Status | Focus / Description |
|---|---|:---:|---|
| 01 | [**1-first-agent**](./1-first-agent/) | ✅ Completed | First AI Agent with OpenAI Function Calling & Asana REST API Integration |
| 02 | **02-langchain-agent** | ⏳ Planned | LangChain Agent Abstractions & Tool Calling |
| 03 | **03-agent-ui** | ⏳ Planned | Interactive Chat UI with Streamlit |
| 04 | **04-task-management-agent** | ⏳ Planned | Multi-tool Task Management Agent |
| 05 | **05-rag-agent** | ⏳ Planned | Retrieval-Augmented Generation (RAG) with Vector Databases |
| 06 | **06-rag-task-agent** | ⏳ Planned | Hybrid RAG + Task Automation Agent |
| 07 | **07-langgraph-agent** | ⏳ Planned | Cyclic Graphs, State Machines & LangGraph Orchestration |
| 08 | **08-n8n-asana-agent** | ⏳ Planned | Low-Code Agent Workflows with n8n & Asana |
| 09 | **09-n8n-rag-agent** | ⏳ Planned | Low-Code RAG Workflows with n8n |
| 10 | **10-deploy-ai-agent-langserve** | ⏳ Planned | Production Agent Deployment with FastAPI & LangServe |

### Advanced & Supplemental Topics
- [ ] **pydantic-ai**: Type-safe Agents with PydanticAI
- [ ] **local-swarm-agent**: Multi-Agent Swarm Orchestration with Local LLMs
- [ ] **sql-ai-agent**: Natural Language to SQL Agents
- [ ] **cost-saving-ai-router**: Smart Routing between Cheap & Heavy LLMs
- [ ] **local-llm-tool-calling**: Function Calling with Local Models (Ollama / Llama 3)
- [ ] **llm-agent-evaluation-framework**: Evaluating & Benchmarking Agent Performance

---

## 🚀 Quickstart

### 1. Prerequisites
- Python 3.10+
- Git

### 2. Running a Module
Each folder is self-contained with its own dependencies and configuration:

```powershell
# 1. Navigate to the desired module
cd 1-first-agent

# 2. Set up virtual environment
python -m venv venv
.\venv\Scripts\activate      # On Linux/macOS: source venv/bin/activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Configure environment variables
Copy-Item .env.example .env  # On Linux/macOS: cp .env.example .env
# Edit .env and supply your credentials

# 5. Run the agent
python agents.py
```

For module-specific walkthroughs, see each subfolder's `README.md` (e.g. [1-first-agent/README.md](./1-first-agent/README.md)).

---

## 🔧 Common Setup Notes

- **HTTPX Version Compatibility**: For older OpenAI client versions (`openai==1.10.0`), ensure `httpx<0.28.0` is installed to prevent `TypeError: Client.__init__() got an unexpected keyword argument 'proxies'`.
- **Alternative LLM Providers**: All agents support the `OPENAI_BASE_URL` environment variable, enabling seamless switching to free/low-cost providers like **Groq**, **Google Gemini (OpenAI endpoint)**, or local models via **Ollama**.

---

*Based on Cole Medin's AI Agents Masterclass.*
