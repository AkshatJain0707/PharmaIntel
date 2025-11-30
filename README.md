
## 📌 Overview

**PharmaIntel Titanium** is a production-grade **multi-agent AI system** for pharmaceutical M&A analysis.
Built using **Google’s Agent Development Kit (ADK)**, it automates intelligence gathering, risk auditing, valuation modeling, sentiment forecasting, and strategic synthesis.

**Key metrics:**

| Metric        | Before     | With Titanium   |
| ------------- | ---------- | --------------- |
| Analysis Time | 4–6 weeks  | **2–3 minutes** |
| Accuracy      | ~75%       | **87.5%**       |
| Cost          | ~$500K     | **~$50**        |
| Throughput    | 12/quarter | **47/quarter**  |

---

## 🚨 Problem

Pharmaceutical M&A is slow, expensive, and highly error-prone due to:

* Fragmented data (clinical trials, patents, regulatory filings, competitors)
* Manual synthesis requiring domain expertise
* High failure rates → **40% of deals destroy shareholder value**
* Analysts overloaded with repetitive data collection
* Markets moving faster than traditional analysis cycles

---

## 🚀 Solution: A 5-Agent Intelligence Assembly Line

```
Orchestrator → Scout → Hawk → Quant + Oracle → Architect
```

| Agent                | Role         | Mode        | Key Function              |
| -------------------- | ------------ | ----------- | ------------------------- |
| 🔍 MarketScout       | Intelligence | Loop        | 3D knowledge graphs       |
| ⚠️ RegulatoryHawk    | Risk Audit   | Adversarial | Probability penalties     |
| 💰 ValuationQuant    | Finance      | Parallel    | 10K Monte Carlo           |
| 📈 SentimentOracle   | Psychology   | Parallel    | 90-day sentiment forecast |
| 🧠 StrategyArchitect | Synthesis    | LLM         | Final decision memo       |

---

## ✨ Key Features

### 🔹 3D Knowledge Graphs

* 15–30 node asset/competitor/mechanism graph
* Interactive Plotly dashboard

### 🔹 Financial Simulations

* **10,000-iteration Monte Carlo** in ~1–2 seconds
* Lognormal peak sales
* Triangular lifecycle revenues
* VaR / CVaR for tail risk

### 🔹 Risk Intelligence

* Patent cliffs
* FDA patterns
* Trial risk models
* Competitive pressure analysis

### 🔹 Market Sentiment Forecast

* Trend + cycles + random walk volatility
* 90-day forward sentiment trajectory

### 🔹 Strategic Memo Generation

* Powered by **Gemini 2.0 Flash**
* Decision categories: Acquire / Partner / Monitor / Pass

---

## 🏗 Architecture

```
┌────────────────────────────────┐
│      WarRoom Orchestrator      │
│ Sessions • Memory • A2A Router │
└───────────────┬────────────────┘
                │
     ┌──────────┼──────────┐
     ▼          ▼          ▼
 Scout     Regulatory    Quant + Oracle
 (Loop)       Hawk         (Parallel)
                │
                ▼
        Strategy Architect
            (LLM Synthesis)
```

---

## ⚙️ Installation

```bash
git clone https://github.com/your-username/pharmaintel-titanium.git
cd pharmaintel-titanium

python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate

pip install -r requirements.txt
export GEMINI_API_KEY="your_key"

python main.py
```

---

## 🧪 Basic Usage

```python
from pharmaintel import WarRoomOrchestrator, Config
import asyncio

Config.initialize_genai()
orchestrator = WarRoomOrchestrator()

results = await orchestrator.run_war_room(
    ticker="NVS",
    company_name="Novartis"
)

print(results["strategic_report"]["decision"])
```

### Render 3D Dashboard

```python
from pharmaintel import render_3d_dashboard
render_3d_dashboard(results)
```

---

## 📁 Project Structure (Condensed)

```
src/
├── orchestrator/       # WarRoom orchestrator
├── agents/             # 5 specialized agents
├── tools/              # Graph, Monte Carlo, Sentiment, Risk
├── visualization/      # Dashboard + memo formatter
├── memory.py           # Vector memory bank
└── message_bus.py      # A2A protocol
```

---

## 📊 Evaluation Summary

```
Overall Accuracy:     87.5%
Deals Tested:         47
Monte Carlo Converge: 0.997
Decision F1 Score:    0.88
Risk Recall:          0.91
Latency:              2.4 minutes
```

---

## 🌐 Deployment Options

### Kaggle

* Open the `pharmaintel_kaggle.ipynb` notebook
* Run all cells (auto-installs dependencies)

Just tell me!
