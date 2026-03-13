# ⚡ Quantum-AI Digital Twin — Indian Smart Grid Optimization

[![HF Models](https://img.shields.io/badge/🤗%20HuggingFace-Models-FFD21E)](https://huggingface.co/Premchan369/quantum-ai-smart-grid-india)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://python.org)
[![Qiskit](https://img.shields.io/badge/Qiskit-1.0-6929C4)](https://qiskit.org)

**Hybrid Quantum-AI system** for optimising EV charging in Indian smart cities.
Combines AI demand forecasting + QUBO/QAOA quantum optimisation + digital twin simulation.

---

## 📊 Results

| Method | Peak Load (kW) | Peak ↓ | Avg CO₂ (g/kWh) | CO₂ ↓ | EV Cost (₹) | Renewable |
|--------|---------------|--------|-----------------|--------|-------------|-----------|
| 🔴 Baseline | 207872.1 | — | 819.8 | — | ₹4224.75 | 0.0% |
| 🔵 Classical | 207872.1 | 0.0% | 819.8 | -0.0% | ₹6159.90 | 0.0% |
| 🟢 **Hybrid Q-AI** | **207872.1** | **0.0%** | **819.8** | **-0.0%** | **₹6159.90** | **0.0%** |

AI Forecast: BiLSTM+Attention MAE=3.4427 GW  |  TFT MAE=3.2439 GW  |  Ensemble R²=0.9276

---

## 🗃️ Indian Datasets

| Dataset | Kaggle Link |
|---------|------------|
| Indian Power Consumption | [anikannal/indian-power-consumption](https://www.kaggle.com/datasets/anikannal/indian-power-consumption) |
| Solar Power Generation | [anikannal/solar-power-generation-data](https://www.kaggle.com/datasets/anikannal/solar-power-generation-data) |
| EV Charging Stations | [piyushagni5/ev-charging-stations-india](https://www.kaggle.com/datasets/piyushagni5/ev-charging-stations-india) |
| Weather India | [sudalairajkumar/daily-weather-data-for-india](https://www.kaggle.com/datasets/sudalairajkumar/daily-weather-data-for-india) |

---

## 🏗️ Pipeline

```
Indian Datasets → Feature Engineering → AI Forecasting (BiLSTM+Attention | TF-Transformer | Ensemble)
    → Digital Twin (Indian Grid Simulation + ToU Pricing + Carbon Tracking)
    → QUBO Formulation → QAOA (Qiskit) → Hybrid Quantum-Classical Solver
    → Optimal EV Charging Schedule → Grid / Carbon / Cost Analysis
```

## 📄 Suggested Paper Title
> *"Hybrid Quantum-AI Digital Twin for Indian Smart Grid EV Charging Optimization using Renewable-Aware Scheduling"*

Target: **IEEE Transactions on Smart Grid | Applied Energy | Energies (MDPI)**

---
*Auto-generated: 2026-03-13 15:31 UTC*
