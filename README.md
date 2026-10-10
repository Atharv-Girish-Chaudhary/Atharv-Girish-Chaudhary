# Atharv Girish Chaudhary

**ML Engineer / GenAI Engineer track**\
*Building generative and RL systems. What pulls me in: how models learn and fail in interesting ways.*

---

## About

MS AI student at Northeastern's Silicon Valley campus (graduating May 2027), after a BE in AI & ML from the University of Mumbai (2021 to 2025). My work spans deep learning, generative models, RL, agentic LLM systems, and CV. Most projects involve modifying an architecture, designing a custom reward, shaping a non-standard loss, or building the evaluation and observability layer around a system, rather than training off-the-shelf.

Completed coursework: Reinforcement Learning, Foundations of Artificial Intelligence, Algorithms, and Program Design Paradigms.

---

## Experience

**GenAI Intern, Tavant Technologies** · *May 2026 to July 2026*\
Built an evaluator for multi-agent LLM pipelines: the supervisory evaluation layer most agent stacks skip.

- Scored agent hops with five deterministic checks (routing, retrieval, tool calls) plus three LLM-as-a-Judge scorers (per-hop faithfulness grounded in that hop's own source, answer relevance, route appropriateness), emitting structured per-hop verdicts. The deterministic context-precision and tool-call scores match RAGAS's own implementations on every test case.
- Built deterministic failure attribution that walks per-agent verdicts in execution order to name the first agent whose own verdict failed, paired with retrieval and tool-call checks for the faults that leave every verdict passing (the wrong retrieved chunk, tool, or argument). Exercised on 7 fault-injection scenarios in a LangGraph pipeline.
- Architected it to score saved, OpenTelemetry-compatible trace files (decoupled from the pipeline, not an in-graph node) for offline replay, so the same scorers ran unchanged on a Pydantic AI app's native OpenTelemetry traces through one added adapter. Built spec-first in thin, independently shippable slices against Amazon Bedrock models.
- Added an online mode that tails live traces to score unlabeled traffic reference-free, plus a drift job (PSI and embedding-centroid distance) covering routing, retrieved context, input queries, and output quality.

---

## Currently

- Open to ML Engineer and GenAI Engineer roles (graduating May 2027)
- Finishing model-verdict, a multi-model prompt-comparison app with a blind LLM judge (live at [model-verdict.omnideckai.com](https://model-verdict.omnideckai.com))
- Taking Deep Learning and Computer Vision for my MS this fall

---

## Tech Stack

**ML / Deep Learning**
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat&logo=huggingface&logoColor=black)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat&logo=opencv&logoColor=white)
![Gymnasium](https://img.shields.io/badge/Gymnasium-2E2E2E?style=flat&logoColor=white)

**GenAI & Agents**
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat&logo=langgraph&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat&logo=langchain&logoColor=white)
![Anthropic](https://img.shields.io/badge/Claude%20API-D97757?style=flat&logo=anthropic&logoColor=white)
![Claude Code](https://img.shields.io/badge/Claude%20Code-D97757?style=flat&logo=claude&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini%20API-8E75B2?style=flat&logo=googlegemini&logoColor=white)
![NVIDIA](https://img.shields.io/badge/NVIDIA%20API-76B900?style=flat&logo=nvidia&logoColor=white)
![Amazon Bedrock](https://img.shields.io/badge/Amazon%20Bedrock-232F3E?style=flat&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=flat&logoColor=white)
![RAGAS](https://img.shields.io/badge/RAGAS-2E2E2E?style=flat&logoColor=white)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-425CC7?style=flat&logo=opentelemetry&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6B35?style=flat&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white)
![OpenRouter](https://img.shields.io/badge/OpenRouter-94A3B8?style=flat&logo=openrouter&logoColor=white)

**Languages**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat&logo=c&logoColor=black)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

**Data & Infra**
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat&logoColor=white)
![Server-Sent Events](https://img.shields.io/badge/Server--Sent%20Events-FF6C37?style=flat&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat&logo=pytest&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat&logo=githubactions&logoColor=white)
![CUDA](https://img.shields.io/badge/CUDA-76B900?style=flat&logo=nvidia&logoColor=white)
![SLURM](https://img.shields.io/badge/SLURM-2C3E50?style=flat&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![AWS Lightsail](https://img.shields.io/badge/AWS%20Lightsail-232F3E?style=flat&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)

---

## Featured Projects

**[model-verdict: Multi-Model Prompt-Comparison App](https://model-verdict.omnideckai.com)** · *May 2026 to present* · *source private*\
Sends one prompt to 2 to 4 models chosen from a 9-model catalog, routed through OpenRouter, and streams their answers side by side in real time over Server-Sent Events. You pick a favorite, and a blind LLM-as-a-Judge picks its own winner from the shuffled answers, with its confidence, the winner's strengths, and what each other answer did better. The core value is the disagreement case: where the judge's blind pick diverges from yours. Per-response latency and token counts, a zero-cost mock mode for development and CI, and a spec-first build. Dockerized and hosted on AWS Lightsail; GitHub Actions runs lint and tests with a 95% coverage gate, and a version tag publishes the image to GitHub's container registry once they pass.\
`FastAPI · Python · JavaScript · SSE · OpenRouter · Docker · AWS Lightsail · GitHub Actions`

**[DevFlow: Engineering Lifecycle Intelligence Platform](https://github.com/Atharv-Girish-Chaudhary/devflow)** · *March 2026*\
**1st Place, Northeastern "From Prototype to Product" AI Hackathon** (3-person team). Agentic system that captures engineering knowledge before team members leave and surfaces it when new ones onboard, differentiated from code-intelligence tools by targeting the why behind architectural decisions, not just the what. Design and architecture are published (story, docs, architecture diagram); the agentic implementation is the next build stage.\
Planned stack: `Claude API · LangGraph · FastAPI · ChromaDB · Multi-Agent`

**[RL Beat Generation: PPO Agent with Transformer Discriminator](https://github.com/Atharv-Girish-Chaudhary/rl-beat-generation)** · *May 2026*\
3-person team project; my part: the PPO training loop, the discriminator, and the Phase 2 expansion. Trained a PPO agent that beat the random baseline by **+130% rule reward** (0.96 vs 0.42) on a 4×16 drum-beat composition task, with autoregressive 3-head action factoring. Pre-trained a 2-layer, 4-head transformer beat discriminator on Groove MIDI, integrated as a learned reward in a hybrid α·rules + β·discriminator scheme. Extended to an 8×16 grid in Phase 2.\
`PyTorch · PPO · Transformers · Gymnasium`

**[SpeakEmbed-T: Transformer-Based Speaker Encoder](https://github.com/Atharv-Girish-Chaudhary/SpeakEmbed-T)** · *May 2025*\
Built jointly with Keegan Dsouza. Replaced the usual LSTM speaker encoder with a Transformer trained on LibriSpeech with GE2E loss, mapping speech to 256-dimensional speaker embeddings used for voice cloning. Audio preprocessing with resampling, loudness normalization, and WebRTC voice activity detection.\
`PyTorch · LibriSpeech · Streamlit`

**[NL2ECF-SRCNN: Modified SRCNN for Super-Resolution](https://github.com/Atharv-Girish-Chaudhary/NL2ECF-SRCNN-with-VW-Blending-and-KS-Refinement)** · *May 2024*\
Built jointly with Keegan Dsouza. Modified SRCNN with LeakyReLU activations that sharpens blurry, low-resolution images by predicting their luminance (Y) channel, followed by Vibrancy-Weighted Blending and Kernel Sharpening post-processing.\
`TensorFlow · OpenCV · Python`

**More projects**

- [CodeCorrect](https://github.com/Atharv-Girish-Chaudhary/CodeCorrect): spell checker for mistyped code, built on four edit-distance methods. CS 5800 team project with Sandeep Vijayarao and Scott Biggs; my part: the tabulated and space-optimized methods, the benchmarking notebook and plots, the Streamlit demo, 5 of the 6 test files, and CI.
- [Ordinal Sentiment Classification](https://github.com/Atharv-Girish-Chaudhary/ordinal-sentiment-classification): predicts 1 to 5 star ratings for Amazon reviews, comparing standard classifiers with ones that treat the stars as ordered. On 9,992 held-out reviews, Ridge regression cut the share of mistakes that were off by two or more stars from between 35% and 44% to 18%, at a cost of about 16 accuracy points. CS 5100 team project with Kien Nguyen and Zijie Liu; my part: preprocessing, TF-IDF features, the Ridge model, and the visualizations.
- [Genetic Image Reconstruction](https://github.com/Atharv-Girish-Chaudhary/Genetic-Optimisation-Framework-for-Pixel-Precise-Image-Reconstruction): genetic algorithm that rebuilds an image pixel by pixel, with no gradients or neural network. Built jointly with Keegan Dsouza.
- [OCR Table Extraction](https://github.com/Atharv-Girish-Chaudhary/Optical-Character-Recognition-and-Excel-Visualisation-Dashboard): desktop app that finds table cells in scanned PDFs and images with OpenCV and reads them with Tesseract. Solo project.

---

## Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logoColor=white)](https://www.linkedin.com/in/atharv-girish-chaudhary/)
[![LeetCode](https://img.shields.io/badge/LeetCode-FFA116?style=flat&logo=leetcode&logoColor=white)](https://leetcode.com/u/2TEPA8efOq/)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:chaudhary.at@northeastern.edu)
