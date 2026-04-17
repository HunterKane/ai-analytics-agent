# AI Analytics Agent

AI-powered analytics system that transforms natural language questions into data-driven insights using agentic LLM workflows, SQL tool integration, and context-aware reasoning.

---

## 🧠 Overview

This project implements a production-style AI system that enables users to query structured data using natural language.

Instead of manually writing SQL or building dashboards, users can ask questions like:

> “Why did revenue drop last week?”

The system interprets the request, retrieves relevant data, performs analysis, and returns structured insights with explanations.

---

## 🎯 Problem

Business stakeholders often struggle to extract insights due to:

* Dependence on SQL or data teams
* Slow, manual analysis workflows
* Lack of context (metric definitions, historical benchmarks)

This creates bottlenecks in decision-making.

---

## 🚀 Solution

This project introduces an **AI Analytics Agent** that:

1. Interprets natural language queries
2. Plans multi-step analytical workflows
3. Executes SQL queries on structured data
4. Applies business context (metrics, definitions)
5. Validates outputs and retries when needed
6. Returns clear, data-backed insights with confidence scores

---

## 🏗️ Architecture

The system is designed as a modular agentic pipeline:

* **Agent Loop** – Controls reasoning and execution flow
* **Planner** – Breaks down complex questions into steps
* **Tools Layer** – Executes actions (SQL queries, calculations, metrics lookup)
* **Context Manager (RAG)** – Injects relevant business knowledge
* **Multi-Agent System** – Distributes tasks across specialized agents
* **Validation Layer** – Ensures reliability via checks and retries

---

## 💻 Example Usage

```python
query = "Why did revenue drop last week?"

response = agent.run(query)

print(response)
```

### Example Output

```json
{
  "insight": "Revenue decreased by 15% due to a 20% drop in traffic.",
  "root_cause": "Reduced user sessions from paid channels.",
  "confidence": 0.87
}
```

---

## 🧪 Features

* Agentic reasoning loop (plan → execute → evaluate → retry)
* Multi-agent orchestration (coordinator + specialized agents)
* SQL tool integration for real data querying
* Context-aware retrieval (RAG for business metrics)
* Structured outputs for consistency and reliability
* Validation and retry mechanisms to reduce hallucinations

---

## 📊 Dataset

Synthetic e-commerce dataset including:

* User sessions
* Transactions
* Revenue metrics
* Traffic sources

---

## 📁 Project Structure

```
ai-analytics-agent/
│
├── core/              # Agent loop, planner, execution logic
├── agents/            # Coordinator + specialized agents
├── tools/             # SQL, metrics, calculation tools
├── hooks/             # Validation and control logic
├── evaluation/        # Test cases and evaluation scripts
├── config/            # Prompt templates and agent rules
├── data/              # Database and metrics definitions
├── week-modules/      # Weekly implementations (learning progression)
├── final-project/     # Integrated system
```

---

## 📚 Weekly Modules

This project is built progressively across 10 modules:

* Week 1: Agentic loops
* Week 2: Multi-agent orchestration
* Week 3: Hooks & workflows
* Week 4: Tool design
* Week 5: Configuration
* Week 6: Planning & iteration
* Week 7: Prompt engineering
* Week 8: Validation systems
* Week 9: Context management
* Week 10: Advanced context & provenance

---

## 📈 Results

* Reduced time-to-insight through automation
* Improved reliability with validation loops
* Demonstrated scalable architecture for AI-powered analytics

---

## 🔧 Setup

```bash
pip install -r requirements.txt
```

---

## 🧭 Future Improvements

* Real-time data integration
* Dashboard UI for interaction
* Advanced evaluation metrics
* Integration with production data pipelines

---

## 💼 Resume Impact

This project demonstrates:

* Agentic LLM system design
* Multi-agent orchestration
* Tool-based reasoning (SQL integration)
* Context-aware AI workflows
* Production-style reliability patterns

---

## 📜 License

MIT License

