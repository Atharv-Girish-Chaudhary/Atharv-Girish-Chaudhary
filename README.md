# Atharv Girish Chaudhary

**ML Engineer / GenAI Engineer track**\
*Building generative and RL systems. What pulls me in: how models learn and fail in interesting ways.*

---

## About

MS AI student at Northeastern's Silicon Valley campus (graduating May 2027), after a BE in AI & ML from the University of Mumbai (2021 to 2025). My work spans deep learning, generative models, RL, agentic LLM systems, and CV. Most projects involve modifying an architecture, designing a custom reward, shaping a non-standard loss, or building the evaluation and observability layer around a system, rather than training off-the-shelf.

---

## Experience

**GenAI Intern, Tavant Technologies** · *May 2026 to July 2026*
Built an offline evaluator for multi-agent LLM pipelines: the supervisory evaluation layer most agent stacks skip.

- Scored each agent hop with six deterministic checks (routing, retrieval, tool calls) plus three LLM-as-a-Judge scorers (per-hop faithfulness grounded in that hop's own source, answer relevance, route appropriateness), cross-validated against RAGAS and emitting structured per-hop verdicts.
- Built deterministic failure attribution that walks per-agent verdicts in execution order to pinpoint the first agent responsible for a multi-hop pipeline failure.
- Architected it to score off saved, OpenTelemetry-compatible trace files (decoupled from the pipeline, not an in-graph node) for offline replay, built spec-first in thin, independently shippable slices against Amazon Bedrock models.
- Added an online mode that tails live traces to score unlabeled traffic reference-free, with drift detection (PSI and embedding-centroid distance) across routing, retrieved context, input queries, and output quality.

---

## Currently

- Interviewing for ML Engineer and GenAI Engineer roles
- Building LLM Router: a multi-provider prompt-comparison app with a neutral LLM judge (live demo deploy next)

---

## Tech Stack

**ML / Deep Learning**
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat&logo=huggingface&logoColor=black)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat&logo=opencv&logoColor=white)

**GenAI & Agents**
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat&logo=langgraph&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat&logo=langchain&logoColor=white)
![Anthropic](https://img.shields.io/badge/Claude%20API-D97757?style=flat&logo=anthropic&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini%20API-8E75B2?style=flat&logo=googlegemini&logoColor=white)
![NVIDIA](https://img.shields.io/badge/NVIDIA%20API-76B900?style=flat&logo=nvidia&logoColor=white)
![Amazon Bedrock](https://img.shields.io/badge/Amazon%20Bedrock-232F3E?style=flat&logo=amazonaws&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=flat&logoColor=white)
![RAGAS](https://img.shields.io/badge/RAGAS-2E2E2E?style=flat&logoColor=white)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-425CC7?style=flat&logo=opentelemetry&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6B35?style=flat&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)

**Languages**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat&logo=c&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=flat&logo=cplusplus&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat&logo=mysql&logoColor=white)

**Data & Infra**
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Server-Sent Events](https://img.shields.io/badge/Server--Sent%20Events-FF6C37?style=flat&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat&logo=pytest&logoColor=white)
![CUDA](https://img.shields.io/badge/CUDA-76B900?style=flat&logo=nvidia&logoColor=white)
![SLURM](https://img.shields.io/badge/SLURM-2C3E50?style=flat&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)

---

## Featured Projects

**[LLM Router: Multi-Provider Prompt-Comparison App](https://github.com/Atharv-Girish-Chaudhary/llm-router)** · *June 2026 to present*
Fans a single prompt out to Anthropic, NVIDIA, and Google Gemini concurrently and streams their responses side by side in real time over Server-Sent Events. A neutral LLM-as-a-Judge (Llama 3.3 70B, a non-contestant) then scores the responses with bias-randomized ordering and picks a winner. The core value is the disagreement case: where the judge's blind pick diverges from the user's. Provider-agnostic adapter interface with a mock-to-real flag, a per-response latency and token panel, a committed SPEC.md, a no-network pytest suite, and MIT license.
`FastAPI · Python · JavaScript · SSE · Anthropic / NVIDIA / Gemini APIs`

**[DevFlow: Engineering Lifecycle Intelligence Platform](https://github.com/Atharv-Girish-Chaudhary/devflow)** · *March 2026*
**1st Place, Northeastern "From Prototype to Product" AI Hackathon** (3-person team). Agentic system that captures engineering knowledge before team members leave and surfaces it when new ones onboard, differentiated from code-intelligence tools by targeting the why behind architectural decisions, not just the what. Design and architecture are published (story, docs, architecture diagram); the agentic implementation is the next build stage.
`Claude API · LangGraph · FastAPI · ChromaDB · Multi-Agent`

**[RL Beat Generation: PPO Agent with Transformer Discriminator](https://github.com/Atharv-Girish-Chaudhary/rl-beat-generation)** · *May 2026*
Trained a PPO agent that beat the random baseline by **+130% rule reward** (0.96 vs 0.42) on a 4×16 drum-beat composition task, with autoregressive 3-head action factoring. Pre-trained a 2-layer, 4-head transformer beat discriminator on Groove MIDI to **95.1% validation accuracy**, integrated as a learned reward in a hybrid α·rules + β·discriminator scheme. Extended to an 8×16 grid in Phase 2.
`PyTorch · PPO · Transformers · Gymnasium`

**[SpeakEmbed-T: Transformer-Based Speaker Encoder](https://github.com/Atharv-Girish-Chaudhary/SpeakEmbed-T)** · *May 2025*
Hybrid Transformer + GE2E loss architecture that cut Equal Error Rate to **6.44% on LibriSpeech** (11.3% lower than the LSTM baseline). Audio preprocessing pipeline (resampling, peak normalization, VAD) runs at **310ms CPU inference**.
`PyTorch · HuggingFace Transformers · LibriSpeech`

**[NL2ECF-SRCNN: Modified SRCNN for Super-Resolution](https://github.com/Atharv-Girish-Chaudhary/NL2ECF-SRCNN-with-VW-Blending-and-KS-Refinement)** · *May 2024*
Modified SRCNN with non-linear luminance enhancement and LeakyReLU activations: **+13.3 PSNR, +0.32 SSIM** over baseline. Vibrancy-Weighted Blending and Kernel Sharpening postprocessing yields **50% better perceived sharpness** at 54 to 84ms per image on CPU.
`TensorFlow · OpenCV · Python`

**More:** [Genetic Optimization](https://github.com/Atharv-Girish-Chaudhary/Genetic-Optimisation-Framework-for-Pixel-Precise-Image-Reconstruction) · [OCR + Excel Dashboard](https://github.com/Atharv-Girish-Chaudhary/Optical-Character-Recognition-and-Excel-Visualisation-Dashboard) · [Ordinal Sentiment Classification](https://github.com/Atharv-Girish-Chaudhary/ordinal-sentiment-classification) · [CodeCorrect](https://github.com/Atharv-Girish-Chaudhary/CodeCorrect)

---

## Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/atharv-girish-chaudhary-529848378/)
[![LeetCode](https://img.shields.io/badge/LeetCode-FFA116?style=flat&logo=leetcode&logoColor=white)](https://leetcode.com/u/2TEPA8efOq/)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:chaudhary.at@northeastern.edu)
[![Resume](https://img.shields.io/badge/Resume-2E2E2E?style=flat&logo=adobeacrobatreader&logoColor=white)](https://github.com/Atharv-Girish-Chaudhary/Atharv-Girish-Chaudhary/blob/main/Atharv_Chaudhary_Resume.pdf)