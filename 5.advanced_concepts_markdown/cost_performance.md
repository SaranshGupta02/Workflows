---
name: Cost & Performance Optimization Content Generator
description: Automates content creation for LLM Optimization including Token Management and Caching Strategies.
---

# Cost & Performance Optimization Content Generator

Generate **optimization guides** for scaling LLM applications efficiently.

**Supported Topics:**
- Token Optimization (Prompt compression)
- Caching Strategies (Semantic Cache, Redis)
- Rate Limiting & Batching
- Model Routing (Using cheaper models for simple tasks)

⚠️ **MANDATORY RULE**  
ALWAYS perform a **web search** to:
- Find current API pricing for OpenAI/Anthropic/Gemini
- Check for new "Prompt Caching" features (e.g., Anthropic's Beta headers)
- Verify latency benchmarks for model routers

---

## Input Format

User provides a **Optimization Target**.

---

## Output: 2 Deliverables

### 1. Optimization Guide (`01_[Target]_Guide.md`)
### 2. Benchmark Notebook (`02_[Target]_Benchmark.ipynb`)

---

## FILE 1: Optimization Guide

**File Name:** `01_[Target]_Guide.md`

**Structure:**
```markdown
# Reducing Costs: [Target] Strategy

## 💰 The Math
"If you have 1k users doing 10 queries/day..."
Show the cost calculation BEFORE and AFTER optimization.

## 🛠️ Implementation
- **Technique 1**: Semantic Caching
  - Code snippet using `gptcache` or Redis.
- **Technique 2**: Prompt Compression
  - Removing stop words, summarizing context.

## 📉 Routing Logic
"If query is simple -> Use gpt-4o-mini"
"If query is complex -> Use gpt-4o"
Code snippet for the router.
```

---

## FILE 2: Benchmark Notebook

**File Name:** `02_[Target]_Benchmark.ipynb`

**Header:**
```markdown
<img src="https://drive.google.com/uc?export=view&id=1wYSMgJtARFdvTt5g7E20mE4NmwUFUuog" width="200">

## [Target] Optimization Benchmark
*Measuring Latency & Cost Savings*

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/[NOTEBOOK_ID])
```

**Structure:**
1.  **Metric Setup**: Define functions to measure Time and Cost.
2.  **Experiment**: Run 100 requests with and without the optimization.
3.  **Visualization**: Bar chart showing 50% cost reduction / 2x speedup.

---

## Search Requirements

Before generating, search for:
1.  "LLM semantic cache python"
2.  "OpenAI batch API guide"
3.  "Anthropic prompt caching tutorial"
