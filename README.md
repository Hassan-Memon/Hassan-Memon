<div align="center">

# Hassan Memon

### AI platform engineer for LLM agents, retrieval, voice and evaluation, who can also judge the answers

I build production AI systems end to end: LangGraph agents as microservices, retrieval on PostgreSQL and pgvector, voice intake, and the dashboards people use to supervise them. I also hold an advanced qualification in Islamic jurisprudence (Ifta' and Fiqh) with native Arabic and Urdu. That pairing is rare: I can build an Arabic or Islamic-finance AI system *and* tell whether what it says is right.

📍 Karachi, Pakistan · 🌍 Open to remote roles worldwide and to relocation (Gulf) · ✉️ [hassan.ghaddai@live.com](mailto:hassan.ghaddai@live.com) · [LinkedIn](https://www.linkedin.com/in/hassan-memon-a109b3257/)

</div>

---

## 🚀 Live products

Four products, each open source, tested in CI and running on free tiers.

| Product | What it does | Try it | Built with |
|---|---|---|---|
| [**AgentMesh**](https://github.com/Hassan-Memon/agentmesh) | An open, self-hostable platform for running AI agents in production. LangGraph agents run as separate services behind a gRPC contract, report every step over an event bus, and pause for a human to approve risky actions. | [Live demo](https://agentmesh.hassan-memon.workers.dev) | Python, LangGraph, gRPC, RabbitMQ or Kafka, Nest.js, Next.js, Socket.IO, Prisma, PostgreSQL + pgvector |
| [**IntakeAgent**](https://github.com/Hassan-Memon/intakeagent) | Voice-first intake for clinics and law firms. The agent listens, asks the follow-up questions a coordinator would, and produces a FHIR R4 record or a Clio matter that a person approves. Patient data stays on local models. | [Live demo](https://intakeagent.hassan-memon.workers.dev) | FastAPI, WebSockets, Whisper, LangGraph, FHIR R4, Clio API, Next.js, PostgreSQL + pgvector |
| [**OpenInfer**](https://github.com/Hassan-Memon/openinfer) | One model, any hardware. An OpenAI-compatible server that runs models on CPU, Apple Metal, CUDA, ROCm or an NPU, and routes each request local or cloud by privacy, latency and cost. Private requests never reach the cloud. | [Router playground](https://openinfer.hassan-memon.workers.dev) | Python, FastAPI, llama.cpp, Ollama, vLLM, Groq and Gemini, Prometheus, Docker |
| [**TrueRate**](https://github.com/Hassan-Memon/truerate) | One honest exchange rate. Asks 4 independent market feeds and 108 central banks at once, then shows the consensus, the spread between sources and a trust score, with every publisher named. English and Urdu. | [Live site](https://truerate.hassan-memon.workers.dev) | Node.js 22 on Cloudflare Workers, zero runtime dependencies, zero API keys |

**How they fit together:** OpenInfer is the model layer, AgentMesh orchestrates agents on top of it, and IntakeAgent is a product built from both. The AgentMesh demo and the IntakeAgent demo run their backend inside your browser, so anyone can click through a full run without an account. The real stacks start with one `docker compose up`.

<details>
<summary><b>What each repository shows about how I work</b></summary>

- **Contracts first.** AgentMesh's gateway and agents share one protobuf contract. OpenInfer adopts the OpenAI wire format, so every existing SDK is already a client.
- **Humans in the loop as real state.** Approval pauses are checkpointed in Postgres and survive a restart, rather than living in a waiting process.
- **Privacy by policy.** OpenInfer's `private` tag and IntakeAgent's redaction step keep patient data on local models, and the rule lives in a config file an auditor can read.
- **Honest status.** Every README says what has been verified and what has not. AgentMesh, IntakeAgent and OpenInfer each have a changelog, architecture decision records and a teaching track in `docs/learn/`.
- **Runs with no keys.** Each project has a demo mode and offline tests, so a reviewer can run it in two minutes.

</details>

---

## 🧭 More projects

| Project | What it does | Stack |
|---|---|---|
| [**TranslateBook AI**](https://github.com/Hassan-Memon/ai-book-translator) | Translates whole scanned books between Urdu and Arabic with a scholar in the loop: structure-aware chunking, a verify-and-retry agent per chunk, terminology decided once and applied everywhere, crash-safe jobs | Python, FastAPI, LangGraph, PostgreSQL + PGVector, React |
| [**Hadith research, offline**](https://github.com/Hassan-Memon/hadith-search-offline-apps) | The full tehqeqatehadees.com collection on the reader's own device: Urdu/Arabic full-text search in the browser (SQLite + FTS5 in a Web Worker), hourly incremental sync through GitHub Actions, one installable PWA for every platform | TypeScript, SQLite/FTS5, PWA, GitHub Actions |
| **SarfBench** *(in progress)* | A bilingual benchmark that tests LLMs on Islamic rulings for currency exchange, gold, fees and loans under two frameworks (AAOIFI and Hanafi), with deterministic scoring and a scholar-review tool. I am verifying every case myself before the repository goes public | Python, FastAPI, pydantic, Ollama / OpenAI / Claude / Gemini adapters |

---

## 🛠 What I have shipped at work

- **Senior Software Engineer, EL Technologies (Doha, remote), 2024 to 2025.** Architected a multi-agent system (LangGraph, LangChain, FastAPI) with query, impact-analysis and document-writing agents; webhook-driven human-in-the-loop review; ingestion and semantic search over large PDF/CSV/XLS sets on PostgreSQL + PGVector; LangSmith tracing; Docker and Azure Container Apps CI/CD.
- **Software Engineer, Techwards (Karachi), 2023 to 2024.** Voice-to-voice conversation with OpenAI Whisper and TTS on the Chatwards chatbot platform, function calling, and the backend of a production Django RAG platform.
- **Software Engineer, Techwards, 2020 to 2022.** Led a full-text search engine over a large classical Arabic corpus (Django REST Framework, React, Elasticsearch) that still serves 100 to 150 readers a day in Arabic and Urdu.
- **Open source.** Documentation fixes merged into [LangChain](https://github.com/langchain-ai/langchain/pull/25285) and [LangGraph](https://github.com/langchain-ai/langgraph/pull/1392).

## 🧰 Stack

- **LLM systems:** LangGraph · LangChain · multi-agent workflows · human-in-the-loop · RAG · tool calling · context-window management · evaluation and benchmark design · LangSmith · Whisper / TTS · llama.cpp · Ollama · vLLM
- **Backend and services:** Python · FastAPI · Django / DRF · Node.js · Nest.js · gRPC and protobuf · RabbitMQ · Kafka / Redpanda · WebSockets and Socket.IO · OAuth2
- **Frontend:** Next.js (App Router) · React · TypeScript · Tailwind CSS
- **Data:** PostgreSQL · pgvector · Prisma · SQLModel · MongoDB · Redis · Elasticsearch · OCR and document pipelines
- **Healthcare and legal integration:** FHIR R4 · Clio API · PHI redaction · HIPAA technical safeguards mapping
- **Cloud and delivery:** Docker and Compose · Cloudflare Workers · Azure Container Apps · GitHub Actions · Prometheus · supply-chain hygiene (SHA-pinned actions, secret scanning)
- **Domain:** Islamic commercial law (fiqh al-mu'amalat) · Islamic banking and Takaful rulings · Urdu–Arabic scholarly translation
- **Languages:** Arabic (native) · Urdu (native) · English (professional)

---

<div align="center">

**Hiring for agentic AI platforms, healthcare or legal AI, Arabic or Islamic-finance AI, or LLM evaluation?**
I reply to every serious message: [hassan.ghaddai@live.com](mailto:hassan.ghaddai@live.com) · [LinkedIn](https://www.linkedin.com/in/hassan-memon-a109b3257/)

</div>
