---
name: LLM Evaluation Content Generator
description: Automates content creation for LLM Evaluation including Comparison Guides and Setup Tutorials.
---

# LLM Evaluation Content Generator

Generate **QA and Evaluation content** for LLM systems.

**Supported Topics:**
- Eval Frameworks (LangSmith, DeepEval, Ragas, TruLens)
- LLM-as-a-Judge patterns
- Custom Metrics (Faithfulness, Relevance, Toxicity)
- A/B Testing Prompts

⚠️ **MANDATORY RULE**  
ALWAYS perform a **web search** to:
- Check for the latest integration guides for [Eval Tool]
- Find standard datasets for benchmarking (if applicable)
- Verify how to define custom metrics in the target tool

---

## Input Format

User provides a **Eval Tool** or **Metric Strategy**.

---

## Output: 2 Deliverables

### 1. Evaluation Setup Tutorial (`01_Setting_Up_[Tool].md`)
### 2. Metric Definition Guide (`02_Defining_Metrics.md`)

---

## FILE 1: Evaluation Setup Tutorial

**File Name:** `01_Setting_Up_[Tool].md`

**Structure:**
```markdown
# Evaluating RAG with [Tool]

## 🎯 Why Measure?
"You can't improve what you don't measure."

## 🔌 Integration
How to wrap your LLM calls to trace them.
```python
# Code snippet showing the tracer/wrapper
with tracer.trace("My RAG Pipeline"):
    result = chain.invoke(query)
```

## 📊 Running a Dataset
How to run a batch of 50 questions and get a score.

## 📈 Dashboard Walkthrough
Screenshots/Description of interpreting the results.
```

---

## FILE 2: Metric Definition Guide

**File Name:** `02_Defining_Metrics.md`

**Structure:**
```markdown
# Custom LLM Metrics

## ⚖️ LLM-as-a-Judge Prompt
The exact prompt used to grade the output.
> "You are a strict teacher. Grade this answer 1-5 based on..."

## 📐 Faithfulness vs. Relevance
- **Faithfulness**: Did it hallucinate?
- **Relevance**: Did it answer the user?

## 🚫 Detecting Regressions
How to set up CI/CD to fail if score drops below X.
```

---

## Search Requirements

Before generating, search for:
1.  "[Tool] quickstart python"
2.  "RAG evaluation metrics guide"
3.  "LLM as a judge prompt templates"
