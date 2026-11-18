<!-- Profile README · Mohammad Adib Watfa · animated SVGs in /assets are generated, not hand-edited · colors: #06090F bg · #2ED8FF cyan · #8C7CFF violet (matches the portfolio site) -->

<div align="center">

<a href="https://adibwatfa341-alt.github.io/Adib_CV/"><img width="100%" src="assets/header.svg" alt="Mohammad Adib Watfa · AI Engineer · Generative AI, Vision-Language Models, Document AI, RAG · open to remote AI engineering roles"/></a>

<p>
  <a href="https://www.linkedin.com/in/mohammad-adib-watfa"><img src="https://img.shields.io/badge/LinkedIn-mohammad--adib--watfa-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=06090F" alt="LinkedIn"/></a>
  <a href="mailto:adebwatefa754@gmail.com"><img src="https://img.shields.io/badge/Email-adebwatefa754%40gmail.com-2ED8FF?style=for-the-badge&logo=gmail&logoColor=white&labelColor=06090F" alt="Email"/></a>
  <a href="https://adibwatfa341-alt.github.io/Adib_CV/"><img src="https://img.shields.io/badge/Portfolio-Live_site-8C7CFF?style=for-the-badge&logo=githubpages&logoColor=white&labelColor=06090F" alt="Portfolio"/></a>
  <a href="https://adibwatfa341-alt.github.io/Adib_CV/Mohammad-Adib-Watfa-CV.pdf"><img src="https://img.shields.io/badge/CV-Download_PDF-34D399?style=for-the-badge&logo=readthedocs&logoColor=white&labelColor=06090F" alt="Download CV"/></a>
</p>

<img width="100%" src="assets/terminal.svg" alt="$ whoami → AI Engineer @ Metamas · $ cat focus.txt → Generative AI · VLMs · Document AI · RAG · 780+ tests passing · open to remote roles, can start immediately"/>

<img width="100%" src="assets/metrics.svg" alt="94% data-extraction accuracy in production · ~70 s per 14-page order · 16 of 20 defects found with 0 of 30 false alarms · 780+ automated tests"/>

</div>

### ⚡ Recruiter quick scan

<div align="center">

| 🎯 Role | 🧑‍💻 Experience | 🛠️ Core stack | 🌍 Location |
|:---:|:---:|:---:|:---:|
| AI Engineer<br/><sub>GenAI · VLMs · Document AI · RAG</sub> | **AI Engineer at Metamas**<br/><sub>Apr 2025 → now</sub> | Python · FastAPI · Celery · Redis<br/><sub>Gemini · Qwen3-VL · PyTorch · SAM 3</sub> | Aleppo, Syria · UTC+3<br/><sub>🟢 Open to remote roles</sub> |

<sub><b>Keywords:</b> AI Engineer · Machine Learning · Generative AI · Vision-Language Models · Document AI · RAG · Computer Vision · Anomaly Detection · LLM Evaluation · FastAPI · Celery · Redis · PyTorch · MCP</sub>

</div>

---

### 👋 About me

I turn **research models into tested Python services** that keep working in production, not only in a demo.

- 🏭 **Now:** AI Engineer at **Metamas**. Founder or lead of 3 AI services and an assessment platform, including a document-extraction service **in production for Saudi Electricity Company (SEC)**.
- 📏 **How I ship:** I measure model behaviour on labelled test sets before shipping; 780+ automated tests cover my services.
- 🧱 **Background:** Python backend engineering, so I treat an AI feature as a full product: async workers, validated outputs, retries, monitoring, tests and deployment.
- 🎤 Speaker at Metamas “Build Without Limits”, University of Aleppo (Oct 2026): turning a research paper into a product.
- 🌍 Aleppo, Syria (UTC+3) · Arabic (native), English (upper-intermediate) · **open to remote roles**

<table>
<tr>
<td width="46%"><a href="https://adibwatfa341-alt.github.io/Adib_CV/"><img src="https://adibwatfa341-alt.github.io/Adib_CV/og.jpg" alt="Portfolio preview"/></a></td>
<td>

### 🌐 Live portfolio

**[adibwatfa341-alt.github.io/Adib_CV](https://adibwatfa341-alt.github.io/Adib_CV/)**

The interactive version of this page:

- 🧭 animated diagrams of the 4 systems; click any part to read what it does
- 🎚️ a calibration lab you can drag yourself
- 🧠 my second brain as a live, draggable graph
- 📄 one-page CV to download

</td>
</tr>
</table>

---

### 🚀 Featured work

<sub>Built at Metamas. The code is private; the descriptions and numbers are mine. The diagrams are live: data moves through them. Expand a project for details.</sub>

<img width="100%" src="assets/docai-flow.svg" alt="Document AI pipeline: Client ERP → FastAPI → Redis → Celery worker → PyMuPDF → OpenCV router (0 LLM calls) → Gemini VLM (JSON schema) → normalize + rules → typed JSON back to the ERP"/>

<details>
<summary><b>📄 Enterprise Document Intelligence & Data Extraction</b> · founder of the service · <b>in production</b></summary>
<br/>

Turns scanned work-order PDFs of up to **72 pages** into typed JSON inside the client's ERP. I founded and built version 1; it grew into a 4-engineer platform **in production** at **94% data-extraction accuracy**.

`FastAPI` `Celery` `Redis` `Gemini VLM` `OpenCV` `PyMuPDF` `Pydantic` `Flower` `Docker`

- ⏱️ A 14-page, 52-field order in **about 70 seconds**, against an estimated 15+ minutes of manual entry
- 📚 Spec-driven extraction catalog grown from **1 to 15 work-order types** (15 of the platform's 31)
- 🧭 OpenCV header-template routing of **100% of pages with zero LLM calls**; skips the 15 to 29 map and attachment pages
- 🔁 Exponential-backoff retries, per-page progress streaming and Flower monitoring
- 🧾 Constrained **JSON-schema** outputs, deterministic normalization and cross-field validation rules

</details>

<img width="100%" src="assets/inspection-flow.svg" alt="Tool inspection pipeline: field photo → FastAPI + Celery → SAM 3 → AnomalyCLIP → calibration → shape checks → Qwen3-VL-8B judge → verdict; one worksite photo, 26 tools: 12 fit, 6 inspect, 4 remove, 4 retake"/>

<details>
<summary><b>🔍 Zero-Shot Tool Inspection & Anomaly Detection</b> · AnomalyCLIP + SAM 3 + Qwen3-VL on NVIDIA DGX</summary>
<br/>

Turned the **AnomalyCLIP** research model (ICLR 2024) into a FastAPI service in **3 days**, then into an inspection product that gives every tool in a field photo a verdict: fit, inspect, remove or retake.

`PyTorch` `AnomalyCLIP` `SAM 3` `Qwen3-VL` `FastAPI` `Celery` `React` `TypeScript` `PostgreSQL` `Docker`

- 🎯 Robust calibration (median + k·MAD): **16 of 20 defects found with 0 of 30 false alarms**, against 3 of 20 at the textbook k = 3
- ✂️ **SAM 3** scores each part separately: about **13x** more model coverage on a 20 px defect
- 📐 Outline-based shape checks catch bent or broken tools that a texture model cannot see
- ⚖️ Local **Qwen3-VL-8B** judge with rules per tool type, checked on a supervisor-labelled exam set and stability-tested over **1,950+ runs**
- 🔌 React/TypeScript UI in Arabic and English, public `/api/v1` with API keys for the Odoo team, Docker Compose on **NVIDIA DGX Spark**

<img width="100%" src="https://adibwatfa341-alt.github.io/Adib_CV/assets/anomaly-run.jpg" alt="The live service on a worksite photo: every tool segmented, heat-mapped and scored"/>

</details>

<img width="100%" src="assets/calibration.svg" alt="Calibration case study: k=1 finds 19 of 20 defects with 8 false alarms; k=2 (shipped) finds 16 of 20 with 0; k=3 finds 3 of 20 with 0"/>

<details>
<summary><b>🎚️ Why a fixed 0.5 threshold failed, and what replaced it</b> · anomaly detection · statistics</summary>
<br/>

**Problem:** after cropping parts out of a multi-object frame, a frame of perfectly good parts scored **0.89**, "defective" under any fixed 0.5 rule.

**Approach:** score 20+ known-good parts per part type through the same crop policy, and set the threshold at `median + k · 1.4826 · MAD`. That bound stays stable even if one bad part slips into the "good" set. Every profile is stamped with a hash of the crop policy, so thresholds are never compared across policies.

**Result (30 good + 20 defective parts):**

| k | Recall | False alarms |
|:---:|:---:|:---:|
| 1.0 | 19/20 | 8/30 |
| **2.0** | **16/20** | **0/30** |
| 3.0 | 3/20 | 0/30 |

The textbook k = 3 looked safe but caught only 15% of defects; k = 2 caught 80% with no false alarms.

</details>

<details>
<summary><b>📝 Talent Assessment Platform</b> · used to screen 200 university students</summary>
<br/>

Arabic (RTL) online assessment, scored automatically across 5 traits.

`FastAPI` `React` `SQLite` `Docker` `Nginx`

- ✅ Auto-scores **28 of 30** questions across 5 traits (93% less manual grading)
- ⏱️ Server-signed 30-minute timer, answer shuffling and duplicate checks
- 📤 Excel export in the original scoring template, plus automatic backups

</details>

<details>
<summary><b>🔎 RAG Application</b> · personal project · <a href="https://github.com/adibwatfa341-alt/mini-rag">mini-rag</a></summary>
<br/>

End-to-end retrieval-augmented generation with local models.

`FastAPI` `Qdrant` `PGVector` `PostgreSQL` `SQLAlchemy` `Alembic` `Ollama`

- 📥 Document ingestion, chunking and embeddings
- 🧲 Semantic retrieval with **Qdrant**
- 💬 Grounded answers with local models through **Ollama**

</details>

<details>
<summary><b>🧾 Multimodal AI PDF-to-Markdown Service</b> · Gemma · Arabic & English</summary>
<br/>

Converts PDF pages into clean Markdown with a multimodal LLM, through background jobs.

`FastAPI` `Celery` `Redis` `PyMuPDF` `Gemma` `Google GenAI`

- 🚦 Redis rate limiter (atomic Lua script) that keeps **every worker** under a 10 requests/minute quota
- 🔁 Exponential-backoff retries with jitter, per-page progress and task-status APIs
- 🔌 Pluggable LLM provider interface and 20 tests

</details>

---

### 🤖 How I build with AI

<img width="100%" src="assets/workflow.svg" alt="Workflow: Spec → Context (Obsidian second brain) → Map (Graphify) → Build (Claude Code + my skills) → Verify (pytest + labelled sets)"/>

<details>
<summary><b>What the agents do, and what stays mine</b></summary>
<br/>

`Claude Code` `Agent Skills & Plugins` `MCP Connectors` `Obsidian second brain` `Graphify`

| Stage | What AI agents do | What stays mine |
|---|---|---|
| Explore | Read the codebase, trace data flow, map impact | Decide the design and the trade-offs |
| Build | Scaffold routes, models, tests and docs | Domain logic and boundaries |
| Review | Propose fixes and refactors | Review every diff |
| Test | Generate test cases and diagnostic scripts | Decide what "correct" means |

</details>

---

### 🔬 More engineering notes

<details>
<summary><b>🚦 One rate limit, many workers</b> · Redis · Lua · Celery</summary>
<br/>

**Problem:** the model API allows a fixed number of requests per minute, but several Celery workers process pages in parallel. Per-worker limits still exceed the shared quota.

**Approach:** one shared slot counter in Redis, reserved through an **atomic Lua script**, so every worker waits for its own slot. Temporary failures retry with exponential backoff and jitter instead of failing the whole document.

</details>

<details>
<summary><b>🖥️ Deploying PyTorch on an ARM64 GPU box</b> · NVIDIA DGX Spark · Docker</summary>
<br/>

**Problem:** the common CUDA base images have no ARM64 build, so a full Docker image failed with `exec format error`.

**Approach:** a hybrid setup. Postgres and Redis run in containers (multi-arch), while the model runs on the machine's native, GPU-enabled PyTorch. A setup script checks the architecture, GPU access, port conflicts and cached weights, then prints the exact commands for the mode that works.

</details>

---

### 🧰 Tech stack

<div align="center">

<img src="https://skillicons.dev/icons?i=python,fastapi,pytorch,opencv,redis,postgres,mongodb,docker,nginx,django,react,ts,linux,git,githubactions&theme=dark&perline=15" alt="Python, FastAPI, PyTorch, OpenCV, Redis, PostgreSQL, MongoDB, Docker, Nginx, Django, React, TypeScript, Linux, Git, GitHub Actions"/>

</div>

<details>
<summary><b>See the full stack by area</b></summary>
<br/>

| Area | Tools |
|---|---|
| **AI & LLMs** | Machine learning, deep learning, Generative AI, vision-language models (Qwen3-VL, Gemini, Gemma), RAG, semantic/vector search, structured outputs, prompt engineering, model & LLM evaluation, local inference, Hugging Face, Ollama |
| **Computer Vision** | PyTorch, CLIP / ViT, AnomalyCLIP, SAM 3, OpenCV, image segmentation, OCR |
| **Documents** | PyMuPDF, PDF processing, page classification, PDF-to-Markdown |
| **Backend** | Python, FastAPI, Django REST Framework, Pydantic, SQLAlchemy, Alembic |
| **Async & Data** | Celery, Redis, Flower, PostgreSQL, PGVector, Qdrant, MongoDB, SQLite |
| **DevOps** | Docker, Docker Compose, Nginx, Linux, GitLab, GitHub Actions, NVIDIA DGX Spark |
| **Testing** | pytest, unit and API tests, test doubles |
| **AI-native tools** | Claude Code, agent skills & plugins, MCP connectors, Obsidian, Graphify, n8n |

</details>

---

### 🎓 Education & speaking

<div align="center">

| 🎓 **B.Sc. Computer Systems Engineering** · Cordoba Private University · 2020 – 2025 | 🎤 **Speaker** · Metamas “Build Without Limits”, University of Aleppo · Oct 2026 |
|:---:|:---:|

</div>

### 💭 How I think

```python
class Adib(AIEngineer):
    mission = "Build AI that keeps working after the demo ends."

    principles = [
        "A model is a feature; the product is everything around it.",
        "Validate every output. Retry every transient failure.",
        "Measure before you trust a threshold.",
        "AI agents speed me up. Judgment stays human.",
    ]

    def on_new_problem(self) -> str:
        return "Let's ship it, and test it."
```

---

<div align="center">

### 🤝 Let's connect

Open to **remote AI engineering roles**: Generative AI, vision-language models, Document AI and RAG · can start immediately

<a href="https://www.linkedin.com/in/mohammad-adib-watfa"><img src="https://img.shields.io/badge/Connect_on_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
<a href="mailto:adebwatefa754@gmail.com"><img src="https://img.shields.io/badge/Send_an_email-0E7490?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
<a href="https://adibwatfa341-alt.github.io/Adib_CV/"><img src="https://img.shields.io/badge/Visit_portfolio-6D5DF5?style=for-the-badge&logo=githubpages&logoColor=white" alt="Portfolio"/></a>

<img width="100%" src="assets/footer.svg" alt=""/>

</div>
