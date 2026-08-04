# 🤖 V1 Action Autonomy: Support Router Agent

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![OpenAI](https://img.shields.io/badge/Model-GPT--4o--mini-green.svg)](https://platform.openai.com/)
[![Observability](https://img.shields.io/badge/Tracing-Arize%20Phoenix-orange.svg)](https://arize.com/phoenix/)

An intelligent customer support routing agent built to classify incoming customer inquiries and route them to appropriate internal departments with structured reasoning and observability.

---

## 📌 Overview

This project demonstrates Level 1 (Action Autonomy) in the AI Autonomy Ladder. The router receives unstructured customer messages, evaluates intent, and outputs structured routing decisions to streamline support operations.

### Key Features
* 🏷️ 7-Department Classification: Routes to BILLING, RETURNS, TECHNICAL_SUPPORT, ORDER_STATUS, PRODUCT_INQUIRY, ACCOUNT_MANAGEMENT, and ESCALATION.
* 🔒 Structured JSON Output: Utilizes gpt-4o-mini with low temperature (0.1) and strict JSON formatting.
* 🧪 Mock API Engine: Includes a robust MockOpenAI client to facilitate offline testing and evaluation without incurring API costs or rate-limit issues (429).
* 📊 Observability & Tracing: Integrated with Arize Phoenix (OpenTelemetry) to trace LLM reasoning, monitor latency, and analyze failure patterns.
* 📈 Benchmarking & Iteration: Evaluated on a 30-case benchmark dataset to track prompt iterations and accuracy metrics.

---

## 🛠️ Tech Stack

* Language: Python 3.10+
* LLM Engine: OpenAI API (gpt-4o-mini)
* Observability: Arize Phoenix, OpenTelemetry
* Data Processing: Pandas, Dataclasses, Enums
* Environment: Google Colab / Jupyter Notebook

🔗 **Live Demo:** https://merry-sable-0193c0.netlify.app
---

## 🚀 Getting Started

### Prerequisites

Clone the repository and install required packages:

```bash
pip install openai pandas python-dotenv arize-phoenix openinference-instrumentation-openai
