<div align="center">

# Hi, I'm Rohan 👋

<img src="https://media.tenor.com/Bpbu2-YNL6cAAAAM/hacker-pupper-dog.gif" width="160" alt="Hacker pupper typing" />

**AI/ML Engineer · MS in Data Analytics Engineering @ Northeastern University (4.0 GPA)**

I build LLM systems end to end: agents, RAG, model distillation, and the evals and MLOps around them.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/rohan-reddy-kolla)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:monu4959@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF6B35?style=for-the-badge&logo=firefoxbrowser&logoColor=white)](https://monu4959.github.io/Personal-Portfolio/)

</div>

---

- 💼 **AI/ML Intern @ CREWASIS:** building custom AI agents for global consumer brands and pharmaceutical clients, from problem statement to production
- 🔬 **Currently:** reinforcement learning (GRPO) on the distilled text-to-SQL model behind HuskySwap
- 🎯 **Open to:** full-time AI/ML roles starting **April 2027**
- 📫 **Reach me:** [monu4959@gmail.com](mailto:monu4959@gmail.com)

---

## 🚀 Featured Projects

### 🛒 [HuskySwap](https://github.com/monu4959/Huskyswap) · Marketplace + Text-to-SQL Agent

`Next.js` `TypeScript` `Supabase Postgres` `pgvector` `vLLM` `Qwen3-4B` `LoRA` `Airflow` `GitHub Actions`

A Northeastern-only buy/sell/rent marketplace with **200+ users** and live chat, with access and business rules enforced through Postgres row-level security. On top of it sits an AI agent that answers plain-English questions about marketplace data.

- **Distillation:** gpt-oss-120b → Qwen3-4B with two-stage LoRA. Held-out accuracy **56.4% → 75.9%**, answering **2× faster** with **54% fewer tokens** than the base model
- **Safety:** asks for clarification instead of guessing, and refuses destructive SQL, PII extraction and prompt injection (refusals **25% → 93%**)
- **Experiments:** 6,600+ graded runs on H200 GPUs showed an 8B student gave no gain over 4B (75.8% vs 75.9%), so the bottleneck is data, not model size
- **MLOps:** 318-question execution-based test set, model registry, automated promotion gate, canary routing with teacher fallback, Airflow pipelines and CI/CD

### ♿ [TransitWise Boston](https://github.com/monu4959/Boston__Transit_MBTA) · Step-Free Trip Planner for Wheelchair Users

`Python` `FastAPI` `OpenTripPlanner` `GTFS-Realtime` `Snowflake` `Claude API` `MCP` `Docker`

An elevator outage can make an MBTA trip impossible, and riders usually find out on arrival. TransitWise plans door-to-door step-free trips and checks every leg against live elevator and service alerts before the rider leaves.

- Found a step-free option for **all 300** random test trips and rerouted **every** trip hit by a live outage (5%)
- Fixed a routing bug that dropped wheelchair transfers network-wide; returns up to **6 trip choices** in **0.27 s** median
- Claude explanations with RAG over MBTA accessibility policy (embeddings in Snowflake), guarded by citation and claim checks
- Exposed as an **MCP server** with 5 tools so assistants like Claude Desktop can plan trips; 90+ offline tests run in CI

### 🛡️ ModCascade · Two-Tier Content Moderation

`DeBERTa-v3` `LangGraph` `vLLM` `Qwen3-4B` `Qdrant` `MLflow` `FastAPI` `Docker`

A moderation cascade over 1.53M Quora and Jigsaw posts: a DeBERTa-v3 classifier resolves 88% of posts, and a policy-citing LLM agent handles the rest.

- **61% recall at 80% precision**, vs 57% for the agent alone, at **8× lower cost**
- Reported a failed pre-registered test alongside the results

### 👥 [HR Intelligence Platform](https://github.com/asvkashyap/hr-analytics-chatbot) · Agentic RAG + Knowledge Graph *(team capstone)*

`LangGraph` `Neo4j` `ChromaDB` `BM25 hybrid search` `FastAPI` `React` `LangSmith`

A RAG chatbot that answers people-analytics questions over employee-recognition data, combining vector search with a Neo4j knowledge graph of employees, awards and skills.

- Built an LLM taxonomy and annotation pipeline that structures raw recognition messages for the agent
- Validated an LLM-as-a-judge grader against human labels; fixing the failures it surfaced raised answer accuracy **69% → 92%**

---

## 🧪 More Projects

| Project | What it does | Result |
|---|---|---|
| **CLIP + GPT-2 Image Captioning** | CLIP encoder paired with a GPT-2 decoder, LoRA fine-tuned on COCO | CIDEr **0.7668**, beats pretrained BLIP |
| **Movie Recommender** | Five LangGraph agents over 8,807 Netflix titles, fusing pgvector and full-text search with RRF | Follow-ups in **<2 s** vs ~10 s · LLM-judge relevance **4.45/5** |
| **[Protein Function Prediction](https://github.com/monu4959/protein_function_classifier)** | Custom PyTorch CNN classifying 270K+ UniProt sequences into 7 enzyme classes, served via FastAPI | **96.09%** accuracy · **1,000+** seqs/min |
| **Restaurant Recommender** | NeuMF, transformer and hybrid recommenders over 100K+ restaurants and millions of reviews | Precision@10 **+40%** over baseline |

<details>
<summary><b>Earlier work</b></summary>
<br/>

| Project | Highlights |
|---|---|
| **[RAG for SEC Filings](https://github.com/monu4959/RAG)** | RAG over 50K+ SEC filings with LangGraph, ChromaDB and GPT-4o, deployed on AWS ECS |
| **Prompt Engineering Eval Platform** | LLM benchmarking across GPT-4 and open-source models over 500+ tasks with MLflow; 27% lower hallucination rate |
| **Neural Architecture Search** | ANN design with PSO, Differential Evolution and Genetic Algorithms; 25% accuracy gain with 40% fewer parameters |
| **Malware Analysis** | CNN-LSTM over API call sequences (98.91%) and classical ML baselines (99.4%) |
| **Wearable Stress Detector** | Affective-state classification from ECG, EDA and respiration using time-series and permutation-entropy features |
| **Reinforcement Learning** | Deep Q-Networks and policy optimization for control and navigation tasks |

</details>

---

## ⚙️ Tech Stack

| Area | Tools |
|---|---|
| **Languages** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) |
| **ML / Deep Learning** | ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) ![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white) ![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black) ![LoRA](https://img.shields.io/badge/LoRA_fine--tuning-6E40C9?style=flat-square) |
| **LLMs & Agents** | ![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white) ![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white) ![vLLM](https://img.shields.io/badge/vLLM-30A2FF?style=flat-square) ![Claude](https://img.shields.io/badge/Claude_API-D97757?style=flat-square&logo=anthropic&logoColor=white) ![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white) ![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white) ![MCP](https://img.shields.io/badge/MCP-333333?style=flat-square) |
| **Data** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![pgvector](https://img.shields.io/badge/pgvector-336791?style=flat-square) ![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white) ![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white) ![Neo4j](https://img.shields.io/badge/Neo4j-4581C3?style=flat-square&logo=neo4j&logoColor=white) ![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6446?style=flat-square) ![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=flat-square) ![Airflow](https://img.shields.io/badge/Airflow-017CEE?style=flat-square&logo=apacheairflow&logoColor=white) |
| **MLOps & Infra** | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white) ![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white) ![Slurm HPC](https://img.shields.io/badge/Slurm_HPC-555555?style=flat-square) |
| **Web** | ![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white) ![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black) |

---

<div align="center">

*"Building AI systems that reason, retrieve, and generalize — one deployment at a time."*

</div>
