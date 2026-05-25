# carbon-aware-re-ai
A requirements engineering framework and lightweight PoC for analyzing trade-offs between AI model performance and carbon efficiency.
---

## 📌 Overview

As AI models grow in complexity, their energy consumption and carbon footprint increase dramatically. This project introduces a Requirements Engineering (RE) framework that treats **carbon efficiency as a first-class concern** early in the development lifecycle. 

This repository provides a lightweight Python script to demonstrate how the controllable variables (such as model configuration, batch size, and training parameters) can be measured and logged in a Google Colab / local environment to analyze performance-sustainability trade-offs.

> ⚠️ **Note on Code Version**: The code provided in this repository is a **lightweight, baseline testing version (PoC)** designed to demonstrate the basic workflow of data ingestion, preprocessing, and custom CNN training with duration logging. The full-scale combinatorial experiments ($2 \times 2 \times 2$ grid with EfficientNet-B0/B2) described in Section V of the paper were conducted in a dedicated distributed environment with hardware-level energy meters.

---

## 📊 Framework Workflow

Our proposed RE framework consists of 6 steps to achieve a "good-enough" AI configuration:
1. **Define Quality Requirements** (e.g., target accuracy $\ge$ 95%)
2. **Identify Controllable Variables** (e.g., epochs, batch size, model depth)
3. **Specify Constraints** (e.g., GPU availability, PUE)
4. **Define Carbon-Aware Computational Requirements** (e.g., REQ-3: Max 10 kWh/epoch/GB)
5. **Select Sustainability Indicators** (e.g., Energy/epoch, Time)
6. **Analyze Sustainability Deliverables & Trade-offs**

---

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- TensorFlow 2.x
- Google Colab or Local GPU environment
