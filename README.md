# Arquam Rahman

AI/ML & Embedded Software Engineer in Kobe, Japan @ RSG (Mitsubishi Heavy Industries Group).

I build production AI for environments where the cloud isn't an option — offline RAG pipelines, on-premise LLM serving, and real-time computer vision deployed to air-gapped enterprise and edge hardware. IIT Delhi, 2024.

## What I work on

**Offline agentic-RAG document-intelligence platform** — Deployed on air-gapped enterprise Windows machines. Hybrid retrieval (BM25 + Qdrant, fused via RRF with a reranking stage), local LLM serving on vLLM (Gemma), full Japanese-language support. Shipped as a self-contained, machine-licensed Windows executable.
*Proprietary — source private.*

**Automated vehicle-inspection system (C++)** — Multi-threaded capture fusing multiple Basler cameras and TOF lasers over PLC/TCP-IP at 20 FPS; deployed on-site across distributed PCs in Singapore.
*Proprietary — source private.*

## Public projects

**[agent-conductor](https://github.com/arquam07/agent-conductor)** — Kubernetes platform for long-running agentic jobs. FastAPI takes job submissions, a Redis queue decouples them from a pool of LangGraph agent workers, and results land in Postgres. KEDA scales workers from 1 to 10 on queue depth, so capacity follows the backlog.

<img src="https://github.com/arquam07/agent-conductor/raw/main/agent-conductor-demo.gif" alt="agent-conductor: worker pods scale up as the job queue drains" width="700">

**[vlmdoc](https://github.com/arquam07/vlmdoc)** — Offline document parsing with a local vision-language model (Ollama or vLLM). Renders each page to an image, transcribes it to Markdown, and chunks it for RAG — built for tables and complex Japanese/English layouts that text-layer extractors mangle. Python package with tests and CI.

**[whisper-v3-benchmark](https://github.com/arquam07/whisper-v3-benchmark)** — How much VRAM does batched Whisper large-v3 actually need? Measured batch sizes 1–16 on an RTX 6000-class GPU over 125 minutes of real audio. Finding: batch 16 used 32 GiB and was 24% *slower* than batch 8; batch 4 got within 5% of the best speed on 10 GiB.

**[bill-analyzer](https://github.com/arquam07/bill-analyzer)** — Full-stack expense app: photograph a receipt, get structured line items, split bills with friends, see spending analytics. Two-stage Gemini 2.5 Flash pipeline on Vertex AI (multimodal extraction, then item-name normalization) with deterministic tax reconciliation for multilingual receipts. FastAPI + async SQLAlchemy, Postgres (Neon), Google OAuth + password auth, React, deployed on Cloud Run and Firebase Hosting.

**[KikuNote](https://github.com/arquam07/KikuNote)** — Turns real Japanese conversations into a personal vocabulary list. Batch transcription with Google Chirp, deterministic JLPT-level tagging via fugashi/MeCab and dictionary lookup, Gemini reserved for summaries, and SM-2 spaced repetition that shows each word in the sentence where you actually heard it.

## Tech

Python · C/C++ · FastAPI · PyTorch · vLLM · Ollama · Hugging Face Transformers · LangGraph · Qdrant · Postgres · Redis · Docker · Kubernetes · KEDA · GCP (Vertex AI, Cloud Run) · OpenCV · YOLO / SAM · Jetson / Raspberry Pi

## Reach me

[LinkedIn](https://linkedin.com/in/arquamrahman) · arquamrahman7@gmail.com · Kobe, Japan
