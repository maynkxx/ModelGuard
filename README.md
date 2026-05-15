# ModelGuard 🛡️

<p align="center">
  <b>LLM Safety, Red-Teaming & Capability Evaluation Framework</b>
</p>

<p align="center">
  Evaluate, benchmark, and compare Large Language Models across safety and capability dimensions using automated red-team pipelines and interactive analytics dashboards.
</p>

---

## 🚀 Overview

ModelGuard is a comprehensive evaluation framework designed to benchmark Large Language Models (LLMs) on:

- 🔐 Safety robustness
- 🎯 Capability performance
- ⚠️ Jailbreak resistance
- 📊 Hallucination analysis
- 🤖 LLM-as-a-Judge scoring
- 📈 Interactive evaluation dashboards

The framework combines:
- capability benchmarks
- adversarial attack datasets
- automated judging pipelines
- metric aggregation
- Streamlit-based visualization

to provide end-to-end LLM evaluation workflows.

---

## 🧠 Evaluation Pipeline

```text
Capability Benchmarks + Red-Team Attack Sets
                    ↓
               Target LLM(s)
                    ↓
           LLM-as-a-Judge Layer
                    ↓
      Safety Metrics | Capability Metrics
                    ↓
     Interactive Analytics Dashboard
```

---

# ✨ Features

- Multi-model evaluation support
- Automated red-team attack testing
- LLM-as-a-judge evaluation layer
- Capability benchmarking pipelines
- Safety metric computation
- Hallucination tracking
- Interactive Streamlit dashboard
- Model comparison analytics
- Config-driven architecture
- Mock evaluation support for testing

---

# 📊 Supported Benchmarks

| Category | Benchmarks |
|----------|-------------|
| Capability | TruthfulQA, GSM8K, MMLU, HellaSwag |
| Safety | HarmBench, AdvBench |
| Jailbreaks | DAN, Dev Mode, Base64 prompts |

---

# 🏗️ Architecture

## Four-Layer Evaluation System

### Layer 1 — Inputs
- Capability benchmark datasets
- Adversarial attack datasets
- Jailbreak prompts/templates

### Layer 2 — Target LLMs
Supports configurable evaluation across:
- GPT-4o
- Claude Sonnet
- Mistral-7B
- Llama-3

### Layer 3 — LLM-as-a-Judge
Automated scoring for:
- Harmfulness
- Truthfulness
- Refusal quality

### Layer 4 — Metrics & Analytics

| Safety Metrics | Capability Metrics |
|----------------|-------------------|
| Attack Success Rate (ASR) | Accuracy |
| Refusal Rate | BLEU |
| False Positive Rate | BERTScore |
| Per-category ASR | Hallucination Rate |

--

# 🖥️ Dashboard Modules

| Module | Description |
|--------|-------------|
| Observe | Live evaluation monitoring |
| Run Evaluation | Launch evaluation runs |
| Safety Analysis | ASR and jailbreak analytics |
| Capability Analysis | Benchmark performance tracking |
| Model Comparison | Multi-model score comparison |

---

# 📁 Project Structure

```text
ModelGuard/
├── config/
│   ├── models.yaml
│   ├── benchmarks.yaml
│   └── attack_sets.yaml
│
├── data/
│   ├── capability_benchmarks/
│   ├── attack_sets/
│   └── results/
│
├── safeeval/
│   ├── models/
│   ├── benchmarks/
│   ├── attacks/
│   ├── judge/
│   ├── metrics/
│   └── pipeline.py
│
├── dashboard/
│   ├── app.py
│   ├── charts/
│   └── data_loader.py
│
├── scripts/
│   └── run_eval.py
│
└── tests/
    └── test_pipeline.py
```

---

# ⚡ Quick Start

## 1. Clone Repository

```bash
git clone https://github.com/maynkxx/ModelGuard.git
cd ModelGuard
```

---

## 2. Create Virtual Environment

```bash
python3 -m venv venv
source venv/bin/activate
```

---

## 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 4. Configure API Keys (Optional)

```bash
export OPENAI_API_KEY=your_key
export ANTHROPIC_API_KEY=your_key
```

Demo mode works without API keys.

---

## 5. Launch Streamlit Dashboard

```bash
streamlit run dashboard/app.py
```

---

## 6. Run CLI Evaluation

```bash
python scripts/run_eval.py \
    --models gpt-4o \
    --models claude-sonnet \
    --num-bench 20 \
    --num-attack 20
```

---

# 🧪 Running Tests

```bash
pytest tests/ -v
```

All tests use mock responses and mock judge scores.

---

# 📌 Future Improvements

- Additional red-team attack datasets
- Latency benchmarking support
- PDF evaluation report export
- Distributed benchmark execution
- Cost estimation dashboard
- Real-time evaluation monitoring

---

# 🤝 Contributing

Contributions, feature requests, and improvements are welcome.

Feel free to fork the repository and submit pull requests.

---

# 📄 License

This project is intended for research and educational purposes.

---

# 👨‍💻 Author

**Mayank Choudhary**

AI/ML • LLM Systems • RAG • AI Safety • Evaluation Frameworks