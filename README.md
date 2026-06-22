# Hi, I'm Roshan Kumar

Full-stack engineer focused on building production-ready systems — workflow automation, AI-powered applications, and data pipelines that handle real-world messiness reliably.

Currently based in Bengaluru. Open to roles at the intersection of AI and systems engineering.

---

## Stack

**Languages** &nbsp;·&nbsp; Java · Python · JavaScript  
**Frontend** &nbsp;·&nbsp; React · TypeScript · Tailwind CSS · ReactFlow · TanStack Query · Recharts  
**Backend** &nbsp;·&nbsp; Node.js · FastAPI · Flask  
**Databases** &nbsp;·&nbsp; PostgreSQL · MongoDB · Redis  
**AI / ML** &nbsp;·&nbsp; LangChain · LLMs · scikit-learn · MediaPipe · BiLSTM  
**Infra** &nbsp;·&nbsp; Docker · AWS · Vercel · Render · Neon  

---

## Projects

### AI Spend Observability System &nbsp;·&nbsp; [Live](https://ai-usage-ledger.vercel.app/)
> Multi-vendor AI usage tracking — one trustworthy number for cost, usage, and identity across tools

The hard part of this system isn't the dashboard — it's making messy, inconsistent, late-arriving data from multiple vendors converge into something you can act on without silent failures.

- **Canonical event schema** — every vendor (ChatGPT, Copilot, Cursor) maps into one `AIUsageEvent` shape; adding a new vendor is one new parser file, nothing else changes
- **Deterministic deduplication** — hashed `dedup_key` per event; same event delivered twice is recognized and skipped, never double-counted
- **Late-cost backfill** — billing lag treated as a patch on the existing row, not a new duplicate event
- **Drift detection** — baseline key-paths recorded per vendor on first ingest; any silent field rename or removal raises `DRIFT_DETECTED` instead of quietly writing zeros
- **Proof-based identity resolution** — the same human appears under different IDs across tools; identities are only linked when there's an explicit recorded proof type, never a fuzzy guess
- **Snapshot regression harness** — pytest snapshots ensure fixing one vendor's parser can't silently break another's output

`FastAPI` `PostgreSQL` `React` `TypeScript` `TanStack Query` `Recharts` `Neon` `Render` `Vercel`

---

### Workflow Automation Platform &nbsp;·&nbsp; [Live](https://vectorshift-tau.vercel.app/)
> Visual AI pipeline editor with drag-and-drop node canvas and real-time DAG validation

- Node-based execution pipeline built with React Flow — dynamic, composable, stateful
- FastAPI backend with DFS cycle detection (3-state node tracking) to validate directed acyclic graphs
- Returns node count, edge count, and DAG status on every save
- Workflow persistence, import/export, and execution metadata via REST APIs

`React` `ReactFlow` `FastAPI` `Tailwind CSS`

---

### Soni &nbsp;·&nbsp; [soni.app](https://soni.app)
> Voice-activated AI assistant with context-aware responses and personalized auth

- LangChain-powered NLP backend handling weather, Wikipedia, calendar, and web automation via LLM tool calls
- Passcode-based authentication with PostgreSQL session management — scoped, persistent, secure
- Google Cloud Text-to-Speech integration for natural audio output

`Flask` `LangChain` `PostgreSQL` `Google Cloud TTS`

---

### Cloner &nbsp;·&nbsp; [cloner.live](https://cloner.live)
> End-to-end pipeline that converts any live website into clean HTML or React + Tailwind

- HTML and CSS semantic analysis preserves layout, content, and design while stripping hydration scripts and trackers
- Outputs a complete, ready-to-run project with merged components and minimal hallucination
- Handles both static HTML export and full React component output

---

### ISL Translator — Indian Sign Language
> Multimodal AI pipeline for real-time gesture-to-Hindi translation

- BiLSTM + MediaPipe for dynamic gesture recognition from video input
- LLM-based language generation converts gesture predictions into natural Hindi sentences
- Modular architecture with clean separation between vision, prediction, and generation — designed for API deployment

`Python` `BiLSTM` `MediaPipe` `LLMs`

---

## Experience

**Associate Software Engineer** &nbsp;·&nbsp; Mphasis &nbsp;·&nbsp; Mar 2026 – May 2026  
Built Python data pipelines for enterprise analytics — ingestion, cleaning, feature engineering, and a scikit-learn predictive model on top. Automated the full end-to-end flow, cutting analysis time from hours to minutes.

**Software Developer** &nbsp;·&nbsp; Shubham Engineering &nbsp;·&nbsp; May 2025 – Aug 2025  
Built and deployed the company's production website. Managed digital compliance workflows for ESIC and PF documentation.

---

## Education

**MCA** &nbsp;·&nbsp; Presidency University, Bengaluru &nbsp;·&nbsp; 2024 – 2026 &nbsp;·&nbsp; CGPA 8.9  
**BCA** &nbsp;·&nbsp; Amity University, Ranchi &nbsp;·&nbsp; 2021 – 2024 &nbsp;·&nbsp; CGPA 7.65

---

## Certifications

AWS SimuLearn: Cloud Practitioner &nbsp;·&nbsp; AWS Training & Certification  
Java Certified &nbsp;·&nbsp; HackerRank

---

## Contact

[roshanhere03@gmail.com](mailto:roshanhere03@gmail.com) &nbsp;·&nbsp; [LinkedIn](https://www.linkedin.com/in/roshan-kumar-6398bb227/) &nbsp;·&nbsp; [GitHub](https://github.com/roshankumar1204) &nbsp;·&nbsp; +91 73688 27906
