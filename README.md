<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,60:161b22,100:0d1117&height=130&section=header" width="100%"/>

<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=22&duration=3000&pause=1000&color=58A6FF&center=true&vCenter=true&width=720&lines=Hi%2C+I'm+Sanket+%F0%9F%91%8B;Applied+AI+Engineer;LLM+%E2%80%A2+RAG+%E2%80%A2+Evals+%E2%80%A2+Prod+Infra;I+learn+it.+I+build+it.+I+ship+it.)](https://git.io/typing-svg)

</div>

---

## 🧠 About Me

- 🧑‍💻  **Currently:** Software Engineer @ SAZ Tech | Research Assistant @ UB
- 💼 **Background:** 2+ years building LLM pipelines, RAG systems & eval frameworks | Anthropic Claude API, OpenAI, LangChain, FastAPI, AWS
- 🚀 **Actively seeking:** Full-time SWE / Applied AI Engineer roles | open to relocate
- ⚡ **Off the clock:** Playing basketball, watching NBA, hitting the gym, gaming, or exploring a new city and a good series

---

## 🛠️ Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-0d1117?style=flat-square&logo=python&logoColor=3776AB)
![TypeScript](https://img.shields.io/badge/TypeScript-0d1117?style=flat-square&logo=typescript&logoColor=3178C6)
![SQL](https://img.shields.io/badge/SQL-0d1117?style=flat-square&logo=postgresql&logoColor=336791)

**Generative AI & LLMs**

![Anthropic Claude](https://img.shields.io/badge/Anthropic_Claude_API-0d1117?style=flat-square&logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI_API-0d1117?style=flat-square&logo=openai&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-0d1117?style=flat-square&logo=python&logoColor=1C3C3C)
![LangGraph](https://img.shields.io/badge/LangGraph-0d1117?style=flat-square&logo=graphql&logoColor=E10098)
![RAG](https://img.shields.io/badge/RAG-0d1117?style=flat-square&logo=databricks&logoColor=FF3621)
![Pydantic](https://img.shields.io/badge/Pydantic-0d1117?style=flat-square&logo=pydantic&logoColor=E92063)
![Prompt Engineering](https://img.shields.io/badge/Prompt_Engineering-0d1117?style=flat-square&logo=openai&logoColor=58A6FF)
![MCP](https://img.shields.io/badge/MCP-0d1117?style=flat-square&logo=anthropic&logoColor=D4A574)

**Vector & Retrieval**

![pgvector](https://img.shields.io/badge/pgvector-0d1117?style=flat-square&logo=postgresql&logoColor=336791)
![FAISS](https://img.shields.io/badge/FAISS-0d1117?style=flat-square&logo=meta&logoColor=0668E1)
![Voyage AI](https://img.shields.io/badge/Voyage_AI_Embeddings-0d1117?style=flat-square&logo=openai&logoColor=white)

**Evaluation**

![LangSmith](https://img.shields.io/badge/LangSmith-0d1117?style=flat-square&logo=python&logoColor=1C3C3C)
![LLM-as-Judge](https://img.shields.io/badge/LLM--as--Judge-0d1117?style=flat-square&logo=scales&logoColor=58A6FF)
![Golden Test Sets](https://img.shields.io/badge/Golden_Test_Sets-0d1117?style=flat-square&logo=checkmarx&logoColor=00B050)

**Backend & Infrastructure**

![FastAPI](https://img.shields.io/badge/FastAPI-0d1117?style=flat-square&logo=fastapi&logoColor=009688)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-0d1117?style=flat-square&logo=postgresql&logoColor=336791)
![Redis](https://img.shields.io/badge/Redis-0d1117?style=flat-square&logo=redis&logoColor=DC382D)
![MongoDB](https://img.shields.io/badge/MongoDB-0d1117?style=flat-square&logo=mongodb&logoColor=47A248)
![Amazon S3](https://img.shields.io/badge/Amazon_S3-0d1117?style=flat-square&logo=amazons3&logoColor=569A31)

**Cloud & DevOps**

![AWS](https://img.shields.io/badge/AWS-0d1117?style=flat-square&logo=amazonwebservices&logoColor=FF9900)
![Docker](https://img.shields.io/badge/Docker-0d1117?style=flat-square&logo=docker&logoColor=2496ED)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-0d1117?style=flat-square&logo=githubactions&logoColor=2088FF)

**ML & Research**

![PyTorch](https://img.shields.io/badge/PyTorch-0d1117?style=flat-square&logo=pytorch&logoColor=EE4C2C)
![Hugging Face](https://img.shields.io/badge/Hugging_Face-0d1117?style=flat-square&logo=huggingface&logoColor=FFD21E)
![QLoRA](https://img.shields.io/badge/QLoRA-0d1117?style=flat-square&logo=pytorch&logoColor=EE4C2C)
![RLHF](https://img.shields.io/badge/RLHF-0d1117?style=flat-square&logo=openai&logoColor=white)

---

## 🚀 Featured Projects

### [🔍 ApplyTrak – LLM-Powered Job-Match Pipeline](https://github.com/sank3t9/applytrak)

`Anthropic Claude API` `Voyage AI` `pgvector` `LangSmith` `FastAPI` `Docker`

A production multi-model orchestration pipeline that automates job discovery, deduplication, and relevance ranking at scale.

| Layer | Implementation |
|-------|----------------|
| **Multi-model pipeline** | Claude Haiku extracts structured JDs via Pydantic tool-use; Claude Sonnet scores relevance against a candidate profile |
| **Semantic deduplication** | Voyage AI embeddings + pgvector suppress reposts before scoring ever runs |
| **Eval harness** | LLM-as-Judge on 30 hand-labeled JDs → **0.94 mean parse accuracy** · **0.80 reasoning quality** |
| **Regression gates** | GitHub Actions wires eval runs on every push — no silent regressions |
| **Cost optimization** | Anthropic prompt caching on the score-stage prefix → **~76% reduction** in input token cost |

---

### [📞 VoxProbe – Evaluation Harness for Voice AI Agents](https://github.com/sank3t9/voxprobe)

`FastAPI` `OpenAI API` `GPT-4o-mini` `Vapi` `MongoDB`

A production-grade eval framework for voice AI agents — surfacing behavioral failures that unit tests simply can't catch.

| Layer | Implementation |
|-------|----------------|
| **LLM-driven testing** | GPT-4o-mini runs 12 prompt-engineered personas via real outbound phone calls against target agents |
| **Bug detection** | 9 behavioral detectors (hold loops, failed escalations, identity-verification loops) → **6 of 8 prod bugs flagged** |
| **Async backend** | FastAPI + Pydantic with webhook handling, background transcript polling & MongoDB persistence |
| **Observability** | React/Tailwind dashboard for call control, transcript review & bug triage |

---

### [🤖 Accio AI – Multi-Domain Conversational RAG Agent](https://github.com/sank3t9/Accio_AI)

`Qwen3-4B` `QLoRA` `RLHF` `FAISS` `LangChain` `Hugging Face`

End-to-end fine-tuning + retrieval pipeline for a multi-domain conversational agent, built from the ground up.

| Layer | Implementation |
|-------|----------------|
| **Fine-tuning** | QLoRA-SFT on 25,200+ instruction samples (OASST, Dolly, Orca Math) → **78% token accuracy**, **56% loss reduction** |
| **Retrieval** | FAISS + Flash Attention 2 grounds responses against a PDF-derived knowledge base to reduce hallucinations |
| **RLHF loop** | Reward model training + PPO fine-tuning on A/B preference data collected from live user feedback |

---

## 📊 GitHub Stats

<div align="center">
  <img src="http://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=sank3t9&theme=github_dark" width="100%"/>
</div>
<div align="center">
  <img src="http://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=sank3t9&theme=github_dark" height="180"/>
  &nbsp;&nbsp;
  <img src="http://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=sank3t9&theme=github_dark" height="180"/>
  &nbsp;&nbsp;
  <img src="http://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=sank3t9&theme=github_dark&utcOffset=-4" height="180"/>
</div>
<div align="center">
  <img src="https://raw.githubusercontent.com/sank3t9/sank3t9/output/github-contribution-grid-snake-dark.svg" alt="contribution snake animation" />
</div>

---

## 🏆 Certification

<div align="center">

![AWS ML Associate](https://img.shields.io/badge/AWS_Certified_ML_Engineer-Associate-FF9900?style=for-the-badge&logo=amazonwebservices&logoColor=white&labelColor=0d1117)

</div>

---

## 📬 Let's Connect

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0d1117?style=for-the-badge&logo=linkedin&logoColor=0A66C2)](https://linkedin.com/in/sanketshigaonkar)
[![Portfolio](https://img.shields.io/badge/Portfolio-0d1117?style=for-the-badge&logo=vercel&logoColor=white)](https://sanketshigaonkar.vercel.app)
[![Email](https://img.shields.io/badge/Email-0d1117?style=for-the-badge&logo=gmail&logoColor=EA4335)](mailto:sankets0930@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-0d1117?style=for-the-badge&logo=github&logoColor=white)](https://github.com/sank3t9)

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,60:161b22,100:0d1117&height=100&section=footer" width="100%"/>
