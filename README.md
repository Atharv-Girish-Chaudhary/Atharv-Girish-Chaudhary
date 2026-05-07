<p align="center">
  <strong>ML Engineer / GenAI Engineer track</strong>
  <br/>
  <i>I build with ML and transformers. What pulls me in: how models learn and understand like humans.</i>
</p>

---

### About

MS AI student at Northeastern's Silicon Valley campus (GPA 3.833, graduating May 2027). My work spans deep learning, generative models, RL, and CV — most projects involve modifying an architecture, designing a custom reward, or shaping a non-standard loss rather than training off-the-shelf.

- **GenAI Intern at Tavant Technologies** (Summer 2026) — LangChain, LangGraph, RAG pipelines
- **BE in AI & ML, University of Mumbai** (2021–2025)
- **Compute:** Northeastern HPC (H200, SLURM), Colab Pro

**Relevant coursework** — Foundations of AI, Program Design Paradigm, Algorithms, Reinforcement Learning, Deep Learning (Fall 2026), Computer Vision (Fall 2026).

---

### Tech Stack

**Languages** — Python, C, C++, Java, SQL
**ML / Deep Learning** — PyTorch, TensorFlow, Hugging Face Transformers, Scikit-learn, OpenCV
**GenAI & Agents** — Claude API, MCP, FastAPI, ChromaDB
**Data & Infra** — NumPy, Pandas, CUDA, SLURM/HPC, Docker, Git, Jupyter

---

### Featured Projects

**[RL Beat Generation — PPO Agent with Transformer Discriminator](https://github.com/Atharv-Girish-Chaudhary/rl-beat-generation)** · *May 2026*
Trained a PPO agent that beat the random baseline by **~9.5× rule reward** (0.96 vs 0.10) on a 4×16 drum-beat composition task, with autoregressive 3-head action factoring. Pre-trained a 2-layer / 4-head transformer beat discriminator on Groove MIDI to **95.1% validation accuracy**, integrated as a learned reward in a hybrid α·rules + β·discriminator scheme. Extended to an 8×16 grid in Phase 2.
`PyTorch · PPO · Transformers · Gymnasium`

**[SpeakEmbed-T — Transformer-Based Speaker Encoder](https://github.com/Atharv-Girish-Chaudhary/SpeakEmbed-T)** · *May 2025*
Hybrid Transformer + GE2E loss architecture that cut Equal Error Rate to **6.44% on LibriSpeech — 11.3% lower than the LSTM baseline**. Audio preprocessing pipeline (resampling, peak normalization, VAD) runs at **310ms CPU inference**.
`PyTorch · HuggingFace Transformers · LibriSpeech`

**[NL2ECF-SRCNN — Modified SRCNN for Super-Resolution](https://github.com/Atharv-Girish-Chaudhary/NL2ECF-SRCNN-with-VW-Blending-and-KS-Refinement)** · *May 2024*
Modified SRCNN with non-linear luminance enhancement and LeakyReLU activations: **+13.3 PSNR / +0.32 SSIM** over baseline. Vibrancy-Weighted Blending + Kernel Sharpening postprocessing yields **50% better perceived sharpness** at 54–84ms per image on CPU.
`TensorFlow · OpenCV · Python`

**[Ordinal vs Nominal Sentiment Classification](https://github.com/Atharv-Girish-Chaudhary/ordinal-sentiment-classification)** · *Dec 2025*
Compared four classifiers (Multinomial NB, Logistic Regression, Ridge Regression, Ordinal Logistic) on **49,960 Amazon Electronics reviews** (TF-IDF, 5K unigrams + bigrams). Ridge Regression cut severe error rate (predictions ≥3 classes off) **from 34.8% to 18.1% — a 48% reduction** — trading ~16 points of exact-match accuracy for distance-aware error reduction critical for ordinal targets.
`Scikit-learn · mord · TF-IDF`

More: [Genetic Optimization Framework](https://github.com/Atharv-Girish-Chaudhary/Genetic-Optimisation-Framework-for-Pixel-Precise-Image-Reconstruction) · [OCR + Excel Visualization Dashboard](https://github.com/Atharv-Girish-Chaudhary/Optical-Character-Recognition-and-Excel-Visualisation-Dashboard)

---

### Achievements

**1st Place — Northeastern University "From Prototype to Product" AI Hackathon**
Pitched and built an agentic system using Claude API, MCP, FastAPI, and ChromaDB.

---

### Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/atharv-girish-chaudhary-529848378/)
[![LeetCode](https://img.shields.io/badge/LeetCode-FFA116?style=flat&logo=leetcode&logoColor=white)](https://leetcode.com/u/2TEPA8efOq/)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:chaudharyatharvgirish@gmail.com)