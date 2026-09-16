<div align="center">

# Hi, I'm Abdoulaye Sow 👋
### AI Product Manager · Founder · Hands-On Systems Builder

[![Anthropic Certified](https://img.shields.io/badge/Anthropic-Certified_Foundations_Associate-6B4FBB?style=for-the-badge&logo=anthropic&logoColor=white)](https://www.anthropic.com)
[![Claude Code Architect](https://img.shields.io/badge/Claude_Code-Skills_%7C_MCP_Architect-D97706?style=for-the-badge&logo=anthropic&logoColor=white)](https://anthropic.com)
[![Scrum.org PSPO II](https://img.shields.io/badge/Scrum.org-PSPO_II_%7C_PAL--EBM-005B94?style=for-the-badge&logo=scrumalliance&logoColor=white)](https://scrum.org)
[![arXiv Research](https://img.shields.io/badge/arXiv-2310.15612_NLP-B31B1B?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2310.15612)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/abdoulaye-sow-44861633)

<br/>

**I build AI products and put them in front of real users myself.**  
*13+ years in software engineering and product leadership, turning loose hypotheses into live, production-grade systems.*

<br/>

[🧠 Claude & Agents](#-the-core-superpower-claude-agentic-engineering--mcp) • [⚡ Overview](#-what-i-bring-to-the-table) • [🏗️ Architectures](#️-featured-system-architectures) • [🌟 Public Repos](#-featured-open-source-repositories) • [🧰 Tech Stack](#-technical-arsenal) • [📜 Credentials](#-certifications--credentials) • [📬 Contact](#-get-in-touch)

</div>

---

### 🔭 Currently Focused On
* 🧠 **Local AI & Air-Gapped Inference:** Architecting private on-metal agentic workflows with **Ollama (`qwen2.5-coder`) accelerated on NVIDIA RTX 3060 GPUs**.
* 🎙️ **Voice Telephony & Latency:** Real-time telephony state machines, Whisper speech-to-text audio pipelines, and conversational scoring.
* 💬 **Ask me about:** 0→1 AI product incubation, Model Context Protocol (MCP) servers, WhatsApp conversational agents, and low-resource multilingual NLP.

---

### ⚡ What I Bring to the Table

- 🚀 **Founder Mentality (0→1 Execution):** Founded Improve So and Friasoft. Built **Pulse** from a loose problem to a live B2B SaaS subscription product with 5 paying clients.
- 🛠️ **Build Agents, Not Just Specs:** I don't stop at PRDs. I prototype and deploy hands-on using **Claude Code, the Anthropic SDK, and Model Context Protocol (MCP) servers**.
- 🏢 **Enterprise Global Scale:** AI Delivery & Platform Lead across a global footprint of **40,000+ retail locations**, shipping 5 production AI agents on Atlassian MCP servers and cutting manual testing by 70%.
- 🧠 **On-Metal Local AI & Hardware:** Architect of high-performance local AI and VLM stacks on **NVIDIA GeForce RTX 5080 (16GB) and RTX 3060 GPUs** using Ollama for air-gapped privacy and cross-continental edge compute.
- 🔬 **Published ML Researcher:** Author of [*Machine Translation for Nko: Tools, Corpora and Baseline Results*](https://arxiv.org/abs/2310.15612) (arXiv:2310.15612), advancing NLP for low-resource West African languages.

---

### 🧠 The Core Superpower: Claude Agentic Engineering & MCP

> *"Most engineers use LLMs as basic autocomplete. I harness Claude as a full multi-agent engineering department."*

I specialize deeply in the **Anthropic Claude Ecosystem**—moving beyond naive chat prompts into architecting closed-loop, deterministic multi-agent systems with **Claude Code, the Anthropic SDK, Model Context Protocol (MCP), and custom Skills & Hooks**:

```mermaid
flowchart TD
    subgraph Core["Agent Brain (Claude Code / Anthropic SDK)"]
        Agent["Claude Autonomous Agent<br/>(Planner / Builder / Critic)"]
    end

    subgraph SkillsLayer["Modular Skills (.claude/skills)"]
        S1["Domain Skills<br/>(Task-Specific Workflows)"]
        S2["Closed-Loop Learning<br/>(Generate ➔ Reflect ➔ Refine)"]
    end

    subgraph HooksLayer["Deterministic Hooks & Guardrails"]
        H1["PreToolUse Hook<br/>(Protected File & Credential Guard)"]
        H2["PostExecution Gate<br/>(Automated Pytest & Linter Evals)"]
    end

    subgraph MCPLayer["Model Context Protocol (MCP) Integration"]
        M1["Atlassian MCP Server<br/>(Jira / Confluence Automation)"]
        M2["Local Edge MCP Server<br/>(SQLite WAL / Local Filesystem)"]
        M3["Custom API MCP Server<br/>(WhatsApp / Telecom Gateways)"]
    end

    Agent <--> SkillsLayer
    Agent <--> HooksLayer
    Agent <--> MCPLayer
```

#### How I Architect with Claude:
* 🧩 **Modular Skills (`SKILL.md`):** Authoring domain-specific, on-demand capability packages that agents invoke dynamically based on intent, enabling complex multi-step workflows without token bloat.
* 🛡️ **Deterministic Hooks & Validation Gates:** Combining probabilistic LLM reasoning with strict programmatic guardrails (PreToolUse security filters, automated test suites, and schema validators) so agents never commit broken code or leak credentials.
* 🔌 **Model Context Protocol (MCP) Servers:** Engineering custom MCP servers that expose real-world systems (Atlassian Jira, SQLite databases, hardware sensors, and telecom APIs) directly into Claude's tool-calling space.
* 🔄 **Closed-Loop Self-Improvement:** Building self-refining agent trajectories where agents mine past execution logs and failures to iteratively refine their own skill definitions.

---

### 🏗️ Featured System Architectures

#### 🩺 Bip'AI — Wearable Health Sentinel *(HealthTech & Biometrics)*
> An AI-powered health sentinel that turns consumer smartwatches into proactive vitals monitoring for families and the diaspora.

```mermaid
flowchart LR
    subgraph Wearable["Wearable Layer"]
        W["Samsung Galaxy Watch<br/>(Heart Rate / Vitals)"] -->|Health Connect API| App["Android Companion<br/>(Kotlin / Compose)"]
    end

    subgraph Backend["Cloud Backend (Railway)"]
        App -->|Async REST / JSON| API["FastAPI Service<br/>(Python 3.11)"]
        API --> DB[("TimescaleDB<br/>(PostgreSQL 16)")]
        API --> Agent["Claude 3.5 Sonnet<br/>(Anthropic SDK Anomaly Detection)"]
    end

    subgraph Alerts["Omnichannel Alerting"]
        Agent -->|Critical Event| WA["WhatsApp Business API<br/>(Meta Cloud API + Twilio)"]
        Agent -.->|Fallback| SMS["Carrier SMS<br/>(NimbusMS Gateway)"]
    end
```

<details>
<summary><b>🔍 Click to view Bip'AI Architecture & Engineering Details</b></summary>
<br/>

* **Biometric Ingestion:** Captures high-frequency time-series heart rate and vital telemetry from Galaxy Watch sensors using Android Health Connect.
* **Storage & Aggregation:** Ingests readings into PostgreSQL 16 with **TimescaleDB hypertables** for rolling window analysis and time-series aggregation.
* **LLM Health Interpretation:** Anthropic Python SDK prompts analyze multi-hour vital trends to distinguish false spikes from true cardiovascular anomalies.
* **Resilient Multi-Provider Routing:** Automated fallback: Meta Cloud API $\to$ Twilio WhatsApp $\to$ NimbusMS SMS for guaranteed delivery in low-connectivity markets.
</details>

---

#### 🎙️ O'Takos Voice Hub — Conversational Telephony Intelligence *(Voice AI / Retail)*
> Offline-first call analytics engine capturing retail dining orders and enforcing greeting compliance standards in real time.

```mermaid
flowchart LR
    subgraph Counter["Counter Ingestion"]
        Phone["Samsung Counter Phone<br/>(Auto Call Recording)"] -->|Silent .m4a Sync| Daemon["Sync Daemon"]
    end

    subgraph Engine["Local Processing Hub"]
        Daemon --> Hub["FastAPI Voice Server"]
        Hub --> Slicer["Audio Slicer<br/>(First 30s Window)"]
        Slicer --> Whisper["Whisper STT<br/>(French Transcription)"]
        Whisper --> NLP["Greeting Compliance<br/>Evaluator"]
        NLP --> Store[("SQLite WAL<br/>Metrics & SLAs")]
    end

    subgraph UI["Management"]
        Store --> SSE["Server-Sent Events"]
        SSE --> Dash["Live Manager Dashboard"]
    end
```

<details>
<summary><b>🔍 Click to view Voice Hub Telephony State Machine Details</b></summary>
<br/>

* **Telephony State Machine:** Explicit event lifecycle management (`RINGING` $\to$ `ANSWERED` / `MISSED` $\to$ `ENDED`) to calculate ring latency ($T_{\text{answered}} - T_{\text{ringing}}$) and alert on 15s SLA breaches.
* **Speech-to-Text & French Evaluation:** Automated transcription using OpenAI Whisper, scoring salutations, brand mentions, and courteous phrasing with strict privacy number masking (`+224 621 ** ** 56`).
* **Offline-First Resilience:** Operates locally on SQLite WAL mode with real-time UI updates via Server-Sent Events (SSE).
</details>

---

#### 🔒 Hermes — Air-Gapped Local AI Stack *(On-Metal Privacy & Hardware)*
> 100% private, zero-data-leakage autonomous assistant and second brain running on local NVIDIA hardware.

```mermaid
flowchart LR
    subgraph Client["Control Interface"]
        User["User / Admin"] -->|Encrypted Commands| TG["Telegram Bot<br/>(Allowlisted Chat ID)"]
    end

    subgraph Host["HP Envy (Loopback 127.0.0.1)"]
        TG --> Bot["Orchestrator Daemon"]
        Bot --> DB[("SQLite WAL<br/>Snapshots & Ledgers")]
        Bot --> RAG["Local Vector Store<br/>(ChromaDB / FAISS)"]
        Bot --> LocalLLM["Ollama v0.32.14<br/>(qwen2.5-coder:7b)"]
    end

    subgraph Hardware["Hardware Acceleration"]
        LocalLLM --> GPU["NVIDIA GeForce RTX 3060<br/>(6GB VRAM Budget Tuning)"]
    end
```

<details>
<summary><b>🔍 Click to view Hermes On-Metal Hardware & Security Architecture</b></summary>
<br/>

* **Hardware & VRAM Allocation:** Engineered to run 100% locally on an **NVIDIA GeForce RTX 3060 Laptop GPU (6GB VRAM)** using Ollama v0.32.14 serving `qwen2.5-coder:7b`, carefully tuned to maximize context window while staying within the 6GB hardware boundary.
* **Air-Gapped Privacy & Zero Leakage:** Enforces a strict loopback security baseline (`127.0.0.1:11434`). Sensitive documents, personal finances, and proprietary logs never leave the machine or touch third-party cloud APIs.
* **Local RAG & Second Brain:** Ingests unstructured Markdown notes and SQLite databases into local vector embeddings (**ChromaDB / FAISS**) for semantic retrieval and context-aware Q&A.
* **Telegram Control Plane:** Secure, rate-limited, allowlisted Telegram bot as the sole interaction interface, driving operational modules:
  * 🎯 **Career Copilot:** Parses job application logs, computes follow-up deadlines, and runs stateful mock interview sessions.
  * 💰 **Financial Ledger:** Natural language expense logging and fund tracking.
</details>

---

### 🌟 Featured Open-Source Repositories (Public Code)

Directly explore and clone my public codebases:

| Repository | Tech Stack | Highlights |
| :--- | :--- | :--- |
| 🏷️ **[`deal-buddy-ai-powered-app-0012-2026`](https://github.com/abdoulayesow/deal-buddy-ai-powered-app-0012-2026)** | Claude AI · TypeScript | AI-powered deal finder and price intelligence assistant. |
| 📊 **[`digital-ledger-for-small-store-0011-2026`](https://github.com/abdoulayesow/digital-ledger-for-small-store-0011-2026)** | TypeScript · Claude Code | Offline-first digital bookkeeping ledger designed for small merchants. |
| 💬 **[`whatsapp-notifier-utility-008-2026`](https://github.com/abdoulayesow/whatsapp-notifier-utility-008-2026)** | TypeScript · Vitest | Resilient notification utility and dispatch worker for messaging workflows. |
| 🚗 **[`ride-app-guinea-project-007-2025`](https://github.com/abdoulayesow/ride-app-guinea-project-007-2025)** | Full-Stack | Ride-hailing application designed for emerging market operational realities. |
| 🧠 **[`learn-ai-skill-with-anthropic`](https://github.com/abdoulayesow/learn-ai-skill-with-anthropic)** | Anthropic SDK · Python | Hands-on patterns for tool use, prompt chaining, and Claude Skills. |
| 🧪 **[`ai-antigravity-testing-and-learning`](https://github.com/abdoulayesow/ai-antigravity-testing-and-learning)** | Python · Pytest | Multi-agent orchestration and automated tool testing harness. |
| 📑 **[`slide-dev-experiment-003-2026`](https://github.com/abdoulayesow/slide-dev-experiment-003-2026)** | Slidev · HTML | Automated interactive presentation generator for PSM I training courses. |

---

### 🧰 Technical Arsenal

<div align="center">

#### AI, Models & Agent Frameworks
![Claude](https://img.shields.io/badge/Anthropic_Claude_3.5-D97706?style=for-the-badge&logo=anthropic&logoColor=white)
![MCP](https://img.shields.io/badge/Model_Context_Protocol_(MCP)-10B981?style=for-the-badge&logo=codeforces&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama_(Local_LLMs)-000000?style=for-the-badge&logo=ollama&logoColor=white)
![Whisper](https://img.shields.io/badge/OpenAI_Whisper_STT-412991?style=for-the-badge&logo=openai&logoColor=white)
![HuggingFace](https://img.shields.io/badge/Hugging_Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![NVIDIA](https://img.shields.io/badge/NVIDIA_RTX_GPU_Compute-76B900?style=for-the-badge&logo=nvidia&logoColor=white)

#### Languages & Backends
![Python](https://img.shields.io/badge/Python_3.11+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js_14-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin_(Android)-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)
![Bash](https://img.shields.io/badge/Bash_Scripting-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)

#### Databases & Cloud Platforms
![PostgreSQL](https://img.shields.io/badge/PostgreSQL_16-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![TimescaleDB](https://img.shields.io/badge/TimescaleDB-FDB515?style=for-the-badge&logo=timescale&logoColor=black)
![SQLite](https://img.shields.io/badge/SQLite_WAL-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![Railway](https://img.shields.io/badge/Railway_Cloud-0B0D0E?style=for-the-badge&logo=railway&logoColor=white)

#### Messaging, Hardware & Telephony
![WhatsApp](https://img.shields.io/badge/WhatsApp_Business_API-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)
![Twilio](https://img.shields.io/badge/Twilio_Messaging-F22F46?style=for-the-badge&logo=twilio&logoColor=white)
![Telegram](https://img.shields.io/badge/Telegram_Bot_API-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)
![GalaxyWatch](https://img.shields.io/badge/Health_Connect_API-000000?style=for-the-badge&logo=samsung&logoColor=white)

</div>

---

### 📊 GitHub Activity & Metrics

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=abdoulayesow&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" height="175" alt="Abdoulaye Sow GitHub Stats" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=abdoulayesow&layout=compact&theme=tokyonight&hide_border=true" height="175" alt="Top Languages" />

<br/>

<img src="https://streak-stats.demolab.com/?user=abdoulayesow&theme=tokyonight&hide_border=true" alt="GitHub Streak" />

</div>

---

### 📜 Certifications & Credentials

* 🏅 **Anthropic Foundations Associate** (2026)
* 🏅 **Scrum Product Owner AI Essentials** (2026)
* 🏅 **PSPO II** — Professional Scrum Product Owner II (2025)
* 🏅 **PAL-EBM** — Professional Agile Leadership, Evidence-Based Management (2024)
* 🏅 **SAFe SPC6 AI Empowered** — Scaled Agile Program Consultant (2018 / 2026)
* 🎓 **Master of Engineering, Industrial & Computer Engineering** — *Polytech' Marseille, France* (2013)

---

### 📬 Get in Touch

* 💼 **LinkedIn:** [linkedin.com/in/abdoulaye-sow-44861633](https://linkedin.com/in/abdoulaye-sow-44861633)
* 📧 **Email:** [abdoulaye.sow.co@gmail.com](mailto:abdoulaye.sow.co@gmail.com)
* 🌐 **Location:** Houston, TX area · *Open to Relocation (Austin, SF, Seattle, NYC) & Remote*

---
<div align="center">
  <sub>Built with high-agency hands-on execution. Always shipping.</sub>
</div>
