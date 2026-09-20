# Hi there, I'm Sooun Choi

**Electrical & Electronic Engineering Undergraduate @ Korea University**

I build LLM applications and AI agents, with focus on production-grade agent architectures, evaluation methodologies, and system reliability. I care about how good development environments and rigorous evaluation loops shape great AI products.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/csu0915)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/terrapin888)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:csw21c915@gmail.com)

![Profile Views](https://komarev.com/ghpvc/?username=terrapin888&color=blue&style=flat-square)

---

## Now

- Building an **AI Agent for SQL performance analysis** @ **SAP STAR Intern** (SQL Agent TF Team, July 2026 – Present)
- Contributing to the [langchain-ai](https://github.com/langchain-ai) ecosystem — docs, deepagents
- Exploring AI Agent orchestration, LLM observability, and evaluation harness design
- Preparing for graduation (Expected Feb 2027)

---

## Featured Projects

### [Credit-PT](https://github.com/terrapin888/credit-pt) — Credit Recovery AI Agent
*KOSCOM AI Agent Challenge 2025* | **2nd Prize**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-blueviolet?style=flat-square)
![XGBoost](https://img.shields.io/badge/XGBoost-FF6600?style=flat-square&logo=xgboost&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6F61?style=flat-square)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

- **Solo-developed** a personalized credit recovery AI agent for financially vulnerable individuals
- Designed an **MCP server with 9 tools** (auth, data collection, ML analysis, RAG-based planning, public-service matching) — deployed via Docker-based native Claude Desktop integration
- Combined LLM with an **XGBoost credit-score predictor** for quantitative accuracy and explainability (**MAE 15.74 / R² 0.8331**, 10 mydata-derived features)
- Chose **RAG over fine-tuning** given Colab-level GPU constraints — built a **KR-SBERT + ChromaDB** RAG system mapping 20 recovery strategies from public institutions to ML scenarios
- Introduced a **fallback chain (API → DB → user input)** stabilizing matching across **6,832 public financial products**

### [LANEIGE Ranking Insight Agent](https://github.com/terrapin888/amore_ai_agent)
*Amorepacific AI Innovation Challenge 2026*

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square)
![LangSmith](https://img.shields.io/badge/LangSmith-000000?style=flat-square)
![Claude API](https://img.shields.io/badge/Claude_API-191919?style=flat-square&logo=anthropic&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6F61?style=flat-square)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)

- **Led AI/backend implementation** in a 3-person team for a global beauty e-commerce ranking monitoring AI agent
- Chose **LangGraph-based ReAct Agent** over a fixed pipeline since tool invocation order varied per user query — dynamic dispatch across **9 domain-specific tools**
- Built a RAG system with **Claude API + ChromaDB + Sentence-Transformers (all-MiniLM-L6-v2)** for semantic product-context retrieval
- Instrumented **LangSmith** for agent execution tracing — monitored tool-call flow, token usage, failure cases to iteratively refine prompts and tool logic
- Combined 5 prompt-engineering techniques (CoT / Few-shot, etc.) for answer accuracy and format consistency

### [E.M.Pilot](https://github.com/jinsunghub/copilot_project) — On-Device AI Email Agent
*Qualcomm @ Edge AI Developer Hackathon* | **Top Prize (1st)**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Tauri](https://img.shields.io/badge/Tauri-FFC131?style=flat-square&logo=tauri&logoColor=black)
![QNN SDK](https://img.shields.io/badge/QNN_SDK-3253DC?style=flat-square&logo=qualcomm&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

- **Led a 5-engineer team as team lead & PM** for a Gmail-integrated on-device AI email agent
- Designed an **embedding-based intent classifier** using Nomic-Embed with two dispatch paths — auto-categorizing incoming emails to downstream handlers (Qwen2-7B, EasyOCR, YOLOv8) and routing chatbot commands
- Resolved on-device inference latency of **QNN-quantized models** by introducing a caching layer with a MySQL schema memoizing per-email AI outputs — **75% latency reduction** on repeated fetches
- Designed and implemented a scalable **Flask/MySQL backend** supporting Gmail session management, user personalization, and multi-model orchestration

### [BlogOPT](https://apps.apple.com/kr/app/%EB%B8%94%EB%A1%9C%EA%B7%B8%EC%98%B5%ED%8A%B8-n-%EB%B8%94%EB%A1%9C%EA%B7%B8-%EC%88%98%EC%9D%B5%ED%99%94/id6759182875) — AI-Powered Productivity Tool for Bloggers
*Solo-shipped to App Store & Google Play*

![React Native](https://img.shields.io/badge/React_Native-61DAFB?style=flat-square&logo=react&logoColor=black)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)

- Architected, built, and deployed **BlogOPT** to both App Store and Google Play — full end-to-end ownership from product strategy to production release
- Designed a **multi-LLM pipeline** (Gemini Flash, GPT-4o mini, Claude Haiku) automating end-to-end SEO evaluation and content generation
- Optimized database performance under scalable workloads by engineering automated query execution plan analysis and validating GIN indexing strategies

### GPU Scheduler for ML Inference
*Graduation Project* | Advisor: Prof. Jong Kook Kim, HPIC Lab

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Ray](https://img.shields.io/badge/Ray-028CF0?style=flat-square&logo=ray&logoColor=white)
![CUDA](https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white)

- Designed an **adaptive scheduler for heterogeneous GPU environments** using Ray Framework
- Achieved **31% cost reduction** while satisfying user-defined throughput and power constraints
- Built scheduler algorithms selecting optimal GPU combinations for AI inference (YOLO-based object detection workloads)

---

## Open Source Contributions

### [langchain-ai](https://github.com/langchain-ai) *(Sep 2026 – Present)*

- **[langchain-ai/docs #6005](https://github.com/langchain-ai/docs/pull/6005)** — Added SkillsMiddleware override examples showing how to customize agent `system_prompt`, lowering ramp-up cost for developers building production LangChain agents *(merged)*
- **[langchain-ai/deepagents #6316](https://github.com/langchain-ai/deepagents/pull/6316)** — Root-caused a silent data-corruption bug in deepagents' tool-result offload path and proposed the fix as **Co-Author**, restoring correctness of long-context tool outputs for LangGraph-based agents *(merged)*

---

## Experience

### SAP STAR Intern @ SAP — SQL Plan Mgmt Team (SQL Agent TF)
*Seoul, South Korea* | July 2026 – Present

- Developing an AI Agent for SQL performance analysis — owning end-to-end implementation across LangGraph agent architecture, A2A framework, evaluation flow, and skill-routing system
- Refactored analysis logic previously bundled in a single prompt into modular parts, introduced a dedicated routing module, and redefined execution order between main/sub LLMs — resolving context contamination and reducing token consumption by **33%**
- Designed an **A2A testing framework** for communication with upstream agents within SAP's AI Agent Joule, and optimized the **Human-in-the-Loop** workflow
- Integrated an **LLM-as-a-Judge** based validation flow for diverse SQL scenarios into the CI/CD pipeline

### AI Agent Verification & Evaluation @ Alignerr (Freelancer, Remote)
*multi-challenge-v2-feb-2026 project* | February 2026 – May 2026

- Evaluated **multi-turn conversation quality** of LLM agents through rubrics aligned with predefined evaluation axes
- Combined **manual evaluation with AI-assisted quality checks**, applying a **blind evaluation setup** (scenario context withheld from the LLM judge) to minimize bias
- **Promoted to Technical Reviewer**, auditing peer evaluations and providing feedback to ensure dataset integrity

### Research Intern @ ETRI — Super Computing System Lab
*Daejeon, South Korea* | July 2025 – August 2025

- Set up an **ADAS-oriented RISC-V board** (SiFive HiFive Unmatched RevB) by building Ubuntu, Linux kernel, and ROS2 on bare metal
- Built a **Linux 6.12 RT-patched kernel** with an optimized configuration — achieving **91.43% improvement** in ROS2 network responsiveness (real-time QoS) and **98.29% gain** under high network load
- Presented the optimization results at the **IEIE Fall Conference 2025**

### Undergraduate Intern @ Korea University — SMRL (SoC & Microprocessor Research Lab)
*Seoul, South Korea* | December 2024 – February 2025

- Advisor: Prof. Sung Woo Chung
- Studied hardware/software optimization techniques for system-level power and thermal efficiency
- Analyzed OS-level power management policies (DVFS, DTM)

---

## Education

**Korea University** | Seoul, South Korea
- B.S. in Electrical Engineering | March 2020 - February 2027 (Expected)
- GPA: 3.83 / 4.5

---

## Tech Stack

### Languages
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

### AI/ML Frameworks
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square)
![MCP](https://img.shields.io/badge/MCP-blueviolet?style=flat-square)

### Backend
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)

### Systems
![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![CI/CD](https://img.shields.io/badge/CI/CD-2088FF?style=flat-square&logo=githubactions&logoColor=white)

---

## Publication

- S. U. Choi, S. Y. Kim, "Performance Analysis of a Real-Time Kernel in a RISC-V Environment for SDR," IEIE, November 2025.

---

## Awards & Honors

- **Qualcomm @ Edge AI Developer Hackathon in Seoul** — Top Prize (1st Place)
- **KOSCOM AI Agent Challenge 2025** — 2nd Prize

---

<p align="center">
  <i>"Think deep, develop simple."</i>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/csu0915">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="https://github.com/terrapin888">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  </a>
  <a href="mailto:csw21c915@gmail.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
</p>
