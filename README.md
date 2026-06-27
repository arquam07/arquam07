# Arquam Rahman

AI/ML & Embedded Software Engineer in Kobe, Japan (Mitsubishi Heavy Industries Group).

I build production AI for environments where the cloud isn't an option — offline RAG pipelines, on-premise LLM serving, and real-time computer vision deployed to air-gapped enterprise and edge hardware. IIT Delhi, 2024.

## What I work on

**Offline agentic-RAG document-intelligence platform** — Deployed on air-gapped enterprise Windows machines. Hybrid retrieval (BM25 + Qdrant, fused via RRF with a reranking stage), local LLM serving on vLLM (Gemma), full Japanese-language support. Shipped as a self-contained, machine-licensed Windows executable.
*Proprietary — source private.*

<!-- Named version, if your NDA allows it:
**RINA** — Offline agentic-RAG platform built at Ryoyu System Engineering (MHI Group)...
-->

**Automated vehicle-inspection system (C++)** — Multi-threaded capture fusing multiple Basler cameras and TOF lasers over PLC/TCP-IP at 20 FPS; deployed on-site across distributed PCs in Singapore.
*Proprietary — source private.*

## Public projects

**[bill-analyzer](https://github.com/arquam07/bill-analyzer)** — Full-stack expense app. FastAPI + async SQLAlchemy on Cloud Run, Cloud SQL (Postgres), OAuth2/JWT, Dockerized. AI receipt OCR via Vertex AI / Gemini (~98% across Japanese, German, English, Hindi).

**[KikuNote](https://github.com/arquam07/KikuNote)** — Turns real Japanese conversations into a personalized vocabulary list. Streaming transcription (Google Cloud Speech / Chirp), deterministic JLPT-level tagging via MeCab/fugashi + dictionary lookup, LLM reserved for summarization.

## Tech

Python · C/C++ · FastAPI · PyTorch · vLLM · Ollama · LangGraph · Qdrant · Docker · GCP (Cloud Run, Cloud SQL) · OpenCV · YOLO / SAM · Jetson / Raspberry Pi

## Reach me

[LinkedIn](https://linkedin.com/in/arquamrahman) · arquamrahman7@gmail.com · Kobe, Japan
