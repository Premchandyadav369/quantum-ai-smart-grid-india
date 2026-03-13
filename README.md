# ⚡ Quantum-AI Digital Twin — Indian Smart Grid Optimization

[![HF Models](https://img.shields.io/badge/🤗%20HuggingFace-Models-FFD21E)](https://huggingface.co/Premchan369/quantum-ai-smart-grid-india)
[![HF Spaces](https://img.shields.io/badge/🚀%20HF%20Spaces-Live%20Demo-blue)](https://huggingface.co/spaces/Premchan369/quantum-ai-smart-grid-india-demo)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://python.org)
[![Qiskit](https://img.shields.io/badge/Qiskit-1.0-6929C4)](https://qiskit.org)

**Hybrid Quantum-AI system** for optimising EV charging in Indian smart cities.
Combines AI demand forecasting + QUBO/QAOA quantum optimisation + digital twin simulation.

---

## 📊 Results

| Method | Peak Load (kW) | Peak ↓ | Avg CO₂ (g/kWh) | CO₂ ↓ | EV Cost (₹) | Renewable |
|--------|---------------|--------|-----------------|--------|-------------|-----------|
| 🔴 Baseline | 532.0 | — | 696.0 | — | ₹7451.80 | 15.5% |
| 🔵 Classical | 441.3 | 17.0% | 746.0 | -7.2% | ₹7517.10 | 9.3% |
| 🟢 **Hybrid Q-AI** | **441.3** | **17.0%** | **746.0** | **-7.2%** | **₹7517.10** | **9.3%** |

AI Forecast (full year): LSTM MAE=3.7536 GW · TFT MAE=3.4121 GW · Ensemble R²=0.9297

---

## 🗃️ Indian Datasets

| Dataset | Kaggle | Records |
|---------|--------|---------|
| Indian Power Consumption | [anikannal](https://www.kaggle.com/datasets/anikannal/indian-power-consumption) | 8,760 |
| Solar Power Generation | [anikannal](https://www.kaggle.com/datasets/anikannal/solar-power-generation-data) | 17,520 |
| EV Charging Stations | [piyushagni5](https://www.kaggle.com/datasets/piyushagni5/ev-charging-stations-india) | 7,300 |
| Weather India | [sudalairajkumar](https://www.kaggle.com/datasets/sudalairajkumar/daily-weather-data-for-india) | 8,760 |

---

## 🏗️ Pipeline

```
Indian Datasets → Feature Engineering (26 features) →
  AI Forecasting (BiLSTM+Attention 1.25M params | TFT 237K params | Ensemble) →
  Digital Twin (Local Substation · ToU ₹/kWh · Carbon Tracking) →
  QUBO → QAOA (Qiskit) → Hybrid Solver → Optimal EV Schedule
```

## 📄 Paper Title
> *"Hybrid Quantum-AI Digital Twin for Indian Smart Grid EV Charging Optimization using Renewable-Aware Scheduling"*
> **Target:** IEEE Trans. Smart Grid | Applied Energy | Energies (MDPI)

---
*Generated: 2026-03-13 15:53 UTC*
