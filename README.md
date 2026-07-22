<h1 align="center">Adam Khald</h1>

<h3 align="center">AI & Data Science Engineer · Researcher in Explainable AI, Multi-Agent Systems & Autonomous Perception</h3>

<p align="center">
  <a href="https://www.linkedin.com/in/adam-khald-19634b261/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:ad.khald@edu.umi.ac.ma"><img src="https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white" /></a>
  <a href="https://scholar.google.com/citations?user=YOUR_SCHOLAR_ID"><img src="https://img.shields.io/badge/Google_Scholar-4285F4?style=flat-square&logo=google-scholar&logoColor=white" /></a>
  <a href="https://orcid.org/0009-0006-3709-847X"><img src="https://img.shields.io/badge/ORCID-A6CE39?style=flat-square&logo=orcid&logoColor=white" /></a>
  <a href="https://your-personal-site.com"><img src="https://img.shields.io/badge/Website-000000?style=flat-square&logo=todoist&logoColor=white" /></a>
</p>

---

## About Me

I am a final-year **AI & Data Science Engineering** student at **ENSAM Meknès, Université Moulay Ismaïl (Morocco)**, graduating June 2027. My work sits at the intersection of **explainable AI, multi-agent LLM systems, and autonomous perception** — with a common thread of making complex, multi-stage AI pipelines transparent and auditable rather than treating them as black boxes.

Alongside research, I have spent the last two years building and shipping production AI systems across fintech, healthcare imaging, and applied machine learning tooling, giving me hands-on experience with the practical failure modes that motivate my research questions.

- Currently completing a vehicle trajectory prediction study (PointNet + BiLSTM with attention) on nuScenes
- Background spans applied ML (computer vision, time-series, NLP) and production AI systems engineering across three internships and one independent AI agent platform
- Open to research collaborations and co-authorship

---

## Research Interests

<table>
<tr>
<td width="50%">

**Explainable AI (XAI)**
Causal and structural explanation methods for opaque, multi-stage AI pipelines.

**Multi-Agent Systems**
Coordination, failure modes, and interpretability of hierarchical LLM-based agent architectures.

</td>
<td width="50%">

**Autonomous Systems & Perception**
Trajectory prediction and spatiotemporal modeling for autonomous vehicles.

**Deep Learning**
Architectures combining geometric representations (point clouds) with sequential modeling for structured prediction tasks.

</td>
</tr>
</table>

---

## Research Publications

<table>
<tr>
<td width="100%">

### Hierarchical Explanation Graph (HEG): Causal Explainability for Hierarchical LLM Multi-Agent Pipelines

<a href="https://doi.org/10.5281/zenodo.21009192"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.21009192.svg" /></a>

**Abstract / Contribution:**
HEG introduces a causal explainability framework for hierarchical, multi-agent LLM pipelines — systems where multiple orchestrators, planners, and executors interact across layers, making failure attribution notoriously difficult. A dual-orchestrator architecture executes the pipeline normally while a parallel orchestrator perturbs each layer's intermediate state and measures the resulting shift in the final output via cosine divergence, producing an experimentally grounded causal weight per layer. Across 7 tasks and 42 perturbation experiments, the framework detects systematic **confabulation** — self-explanations that are causally disconnected from the layer's actual influence on the output — most notably in the final evaluator layer, which explains its output with full confidence despite having near-zero measured causal contribution.

This work is positioned at the intersection of **interpretability research** and **practical multi-agent system reliability**, providing a diagnostic tool for auditing complex agentic AI systems rather than trusting their self-reports.

**DOI:** [10.5281/zenodo.21009192](https://doi.org/10.5281/zenodo.21009192)
**Affiliation:** ENSAM Meknès
**Status:** Published on Zenodo; arXiv submission in preparation

</td>
</tr>
</table>

<details>
<summary><b>In progress: Vehicle Trajectory Prediction (PointNet + BiLSTM with Attention, nuScenes)</b></summary>
<br>

A trajectory prediction model combining point-cloud feature extraction (PointNet) with a BiLSTM-Attention sequence model, benchmarked on the nuScenes dataset. Builds on prior CARLA-simulation-based autonomous vehicle work. Full research pipeline set up (EDA, baseline benchmarking, model implementation, ablations, writeup). Manuscript in preparation.

</details>

---

## Featured Projects

<table>
<tr>
<td width="50%">

### 🔹 Hierarchical Explanation Graph (HEG)
Causal explainability framework for hierarchical multi-agent LLM pipelines, detecting confabulated self-explanations via controlled perturbation experiments.
`Tech: Python, GPT-4o, dual-orchestrator architecture` · `Status: Published (Zenodo), arXiv in prep`

</td>
<td width="50%">

### 🔹 Ciffeer
AI agent SaaS platform designed and built solo (Corarea). Multi-layer planning architecture (Orchestrator → Planner → Mid-Level Planner → Analyser → Executor → Evaluator), 100+ tools across 15 categories, semantic memory via pgvector.
`Tech: Go, Python/FastAPI, Next.js, Supabase/pgvector, GCP Cloud Run` · `Status: Live in production`

</td>
</tr>
<tr>
<td width="50%">

### 🔹 COLFI Back-Office Platform & LLM Monitoring Agent
React + FastAPI back-office platform for corporate action processing and treasury funding allocation. Built an LLM monitoring agent on top of the existing multi-agent orchestration system for financial model drift detection (PPCA-based) and governed alerting.
`Tech: React, FastAPI, PostgreSQL, OpenAI API, multi-agent orchestration` · `Status: Private repository`

</td>
<td width="50%">

### 🔹 ColFi Collateral Finance Management DApp
Decentralized collateral/asset management platform for financial institutions. Hyperledger Fabric chaincode for asset state transitions and audit trails, Next.js frontend, Fabric network hosted on Amazon EC2.
`Tech: Hyperledger Fabric, Next.js/TypeScript, AWS EC2, AWS Amplify` · `Status: Public repository`
[Repository](https://github.com/Adamkhald/colfi-internship-dapp)

</td>
</tr>
<tr>
<td width="50%">

### 🔹 Insight-Ray
AI-powered chest X-ray analysis system detecting 14 thoracic abnormality classes with YOLOv8, fine-tuned on VinBigData (18,000+ images), with Gemini-generated natural-language explanations of findings. Research/educational tool, not for clinical use.
`Tech: YOLOv8/Ultralytics, Flask, Tkinter, Gemini API` · `Status: Public repository`
[Repository](https://github.com/Adamkhald/InsightRay)

</td>
<td width="50%">

### 🔹 Dalil AI
Offline-first desktop research platform unifying scikit-learn, PyTorch, TensorFlow, MediaPipe, and Stable-Baselines3/Gymnasium behind one GUI — classical ML, deep learning, computer vision, and RL, all local, no cloud dependency.
`Tech: Python, PyTorch, TensorFlow, scikit-learn, MediaPipe` · `Status: Public repository`
[Repository](https://github.com/Adamkhald/dalil_ai) · [Website](https://adamkhald.github.io/dalil_ai/)

</td>
</tr>
<tr>
<td width="50%">

### 🔹 Breiman CART
Pure Python, from-scratch reimplementation of the original CART algorithm (Breiman, Friedman, Olshen & Stone, 1984), with cost-complexity pruning, native categorical feature handling, and full tree inspection.
`Tech: Python` · `Status: Published on PyPI`
[PyPI](https://pypi.org/project/breiman-cart/) · [Repository](https://github.com/Adamkhald/breiman-cart)

</td>
<td width="50%">

</td>
</tr>
</table>

---

## Industry & Applied Experience

**COLFI** — London-based fintech · *DApp Developer Intern, Summer 2025*
Built the Hyperledger Fabric-based collateral management DApp described above.

**COLFI** — London-based fintech · *Second internship*
Contributed the LLM-based financial model monitoring agent described above, built on the platform's existing multi-agent orchestration system.

**OCP MEA** — Integrated Mine, MEA washing facility · *Internship*
Proposed a machine-learning-based soft sensor for pulp density estimation, scoped and delivered over a three-week engagement.

---

## Awards & Recognition

- **1st Prize, Innov'am 2024** — Autonomous TGV bogie inspection robot
- **3rd Prize, Innovathon 2024**

---

## Technical Skills

<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white" />
  <img src="https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white" />
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" />
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white" />
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" />
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" />
  <img src="https://img.shields.io/badge/Google_Cloud-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white" />
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white" />
  <img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white" />
</p>

**Languages:** English, French, Arabic, German (B2, self-studied)

---

## Currently Learning

<details>
<summary>Expand</summary>
<br>

- Advanced causal inference methods for AI interpretability
- Geometric deep learning for 3D perception
- Formal approaches to multi-agent system verification

</details>

---

## Connect with Me

<p align="left">
  <a href="https://www.linkedin.com/in/adam-khald-19634b261/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:ad.khald@edu.umi.ac.ma"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://scholar.google.com/citations?user=YOUR_SCHOLAR_ID"><img src="https://img.shields.io/badge/Google_Scholar-4285F4?style=for-the-badge&logo=google-scholar&logoColor=white" /></a>
  <a href="https://orcid.org/0009-0006-3709-847X"><img src="https://img.shields.io/badge/ORCID-A6CE39?style=for-the-badge&logo=orcid&logoColor=white" /></a>
  <a href="https://your-personal-site.com"><img src="https://img.shields.io/badge/Website-000000?style=for-the-badge&logo=todoist&logoColor=white" /></a>
</p>

---

<p align="center">
<i>"The purpose of research is not to eliminate uncertainty, but to make it legible enough to act on."</i>
</p>
