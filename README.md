# CS-594 — Provenance & Explanation

Course project for **CS-594 (Provenance and Explanation)**, applied to our ICRA 2025 paper:

> **Sensory Glove-Based Surgical Robot User Interface**  
> Borgioli, L., Oh, K-H., Valle, V., Ducas, A., Halloum, M., Mendoza Medina, D. F., Sharifi, A., López, P. A., Cassiani, J., Žefran, M., *et al.* (ICRA 2025)

---

## 🔎 Overview

This repository explores **explainability and provenance** for a sensory glove interface controlling a surgical robot.  
The project focuses on:
- Capturing **data provenance** (what inputs led to which actions)
- Generating human-readable **explanations** of control decisions
- Lightweight **reproducibility hooks** (configs, seeds, logs)

> The aim is to make human–robot interaction auditable and interpretable without slowing down the control loop.

---

## 🗂 Repository Layout

- `notebooks/` — exploration, analysis, and reports  
- `src/` — core logic (instrumentation, explanation, provenance)  
- `configs/` — YAML configs for experiments  
- `data/` — (optional) small toy datasets or CSV logs  
- `scripts/` — helper scripts for running experiments and exporting reports  

> Exact paths may vary based on your setup—feel free to adapt.

---

## 🚀 Quick Start

```bash
# 1) Create an environment
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate

# 2) Install dependencies
pip install -r requirements.txt

# 3) Run a demo (example)
python scripts/run_demo.py --config configs/default.yaml

# 4) Generate an explanation report
python scripts/export_explanations.py --runs runs/latest --out reports/explanations.md
