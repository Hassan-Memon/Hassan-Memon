<div align="center">

# Hassan Memon

### AI engineer for LLM agents, retrieval and evaluation — who can also judge the answers

I build production Python and LLM systems (LangGraph, FastAPI, PostgreSQL/PGVector, voice AI) and hold an advanced qualification in Islamic jurisprudence (Ifta' and Fiqh) with native Arabic and Urdu. That pairing is rare: I can build an Arabic or Islamic-finance AI system *and* tell whether what it says is right.

📍 Karachi, Pakistan · 🌍 Open to remote roles worldwide and to relocation (Gulf) · ✉️ [hassan.ghaddai@live.com](mailto:hassan.ghaddai@live.com) · [LinkedIn](https://www.linkedin.com/in/hassan-memon-a109b3257/)

</div>

---

## 💱 Featured: TrueRate — one honest exchange rate, with every source shown

<div align="center">

**[truerate.truerate-app.workers.dev](https://truerate.truerate-app.workers.dev)** — live, free, no sign-up

[![CI](https://github.com/Hassan-Memon/truerate/actions/workflows/ci.yml/badge.svg)](https://github.com/Hassan-Memon/truerate/actions/workflows/ci.yml)
[![Deploy](https://github.com/Hassan-Memon/truerate/actions/workflows/deploy.yml/badge.svg)](https://github.com/Hassan-Memon/truerate/actions/workflows/deploy.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-22c55e)](https://github.com/Hassan-Memon/truerate/blob/master/LICENSE)

</div>

Every website shows a different dollar rate, and none of them tells you **who decided it, how, and when**. TrueRate asks **4 independent market feeds and 108 central banks** at the same moment, then shows the consensus, the spread between sources, the official central-bank view and a trust score — with every publisher named.

| What makes it different | How it is built |
|---|---|
| Shows the *disagreement* between sources instead of hiding it behind one number | Zero runtime dependencies: plain Node.js 22 on Cloudflare Workers, no build step |
| Central-bank rates next to market rates, with the gap measured | Zero API keys and zero hosting cost — every upstream is free and public |
| A research write-up on [who actually sets exchange rates](https://github.com/Hassan-Memon/truerate/blob/master/docs/research.md), traced to primary sources | 67 offline tests, CI on Node 22 and 24, deploy on merge with SHA-pinned actions |
| Honest about its own weak point: the consensus is only as good as its sources, so each one is graded | Security headers on every response; the full posture is [documented with verification commands](https://github.com/Hassan-Memon/truerate/blob/master/docs/security.md) |

**→ [Read the code](https://github.com/Hassan-Memon/truerate)** · Next on the roadmap: the State Bank of Pakistan rate ladder (interbank → bank → open market), so a person can see exactly where their money goes. Built with Claude Code as the coding assistant.

---

## 🧭 More projects

| Project | What it does | Stack |
|---|---|---|
| [**TranslateBook AI**](https://github.com/Hassan-Memon/ai-book-translator) | Translates whole scanned books between Urdu and Arabic with a scholar in the loop: structure-aware chunking, a verify-and-retry agent per chunk, terminology decided once and applied everywhere, crash-safe jobs | Python, FastAPI, LangGraph, PostgreSQL + PGVector, React |
| [**Hadith research, offline**](https://github.com/Hassan-Memon/hadith-search-offline-apps) | The full tehqeqatehadees.com collection on the reader's own device: Urdu/Arabic full-text search in the browser (SQLite + FTS5 in a Web Worker), hourly incremental sync through GitHub Actions, one installable PWA for every platform | TypeScript, SQLite/FTS5, PWA, GitHub Actions |
| **SarfBench** *(in progress)* | A bilingual benchmark that tests LLMs on Islamic rulings for currency exchange, gold, fees and loans under two frameworks (AAOIFI and Hanafi), with deterministic scoring and a scholar-review tool. I am verifying every case myself before the repository goes public | Python, FastAPI, pydantic, Ollama / OpenAI / Claude / Gemini adapters |

---

## 🛠 What I have shipped at work

- **Senior Software Engineer, EL Technologies (Doha, remote), 2024–2025** — architected a multi-agent system (LangGraph, LangChain, FastAPI) with query, impact-analysis and document-writing agents; webhook-driven human-in-the-loop review; ingestion and semantic search over large PDF/CSV/XLS sets on PostgreSQL + PGVector; LangSmith tracing; Docker and Azure Container Apps CI/CD.
- **Software Engineer, Techwards (Karachi), 2023–2024** — voice-to-voice conversation with OpenAI Whisper and TTS on the Chatwards chatbot platform, function calling, and the backend of a production Django RAG platform.
- **Software Engineer, Techwards, 2020–2022** — led a full-text search engine over a large classical Arabic corpus (Django REST Framework, React, Elasticsearch) that still serves 100–150 readers a day in Arabic and Urdu.
- **Open source** — documentation fixes merged into [LangChain](https://github.com/langchain-ai/langchain/pull/25285) and [LangGraph](https://github.com/langchain-ai/langgraph/pull/1392).

## 🧰 Stack

**LLM systems:** LangGraph · LangChain · multi-agent workflows · RAG · tool calling · evaluation and benchmark design · LangSmith · Whisper / TTS
**Backend and data:** Python · FastAPI · Django / DRF · Node.js · PostgreSQL · PGVector · Elasticsearch · OCR and document pipelines
**Cloud and delivery:** Docker · Azure Container Apps · Cloudflare Workers · GitHub Actions · supply-chain hygiene (SHA-pinned actions, secret scanning)
**Domain:** Islamic commercial law (fiqh al-mu'amalat) · Islamic banking and Takaful rulings · Urdu–Arabic scholarly translation
**Languages:** Arabic (native) · Urdu (native) · English (professional)

---

<div align="center">

**Hiring for Arabic or Islamic-finance AI, LLM evaluation, or agentic backends?**
I reply to every serious message: [hassan.ghaddai@live.com](mailto:hassan.ghaddai@live.com) · [LinkedIn](https://www.linkedin.com/in/hassan-memon-a109b3257/)

![Hassan's GitHub stats](https://github-readme-stats.vercel.app/api?username=Hassan-Memon&show_icons=true&theme=default)

</div>
