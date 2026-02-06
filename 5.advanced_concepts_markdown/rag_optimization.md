---
name: RAG Optimization Content Generator
description: Automates content creation for Advanced RAG concepts including Notebooks and Deep Dive Guides.
---

# RAG Optimization Content Generator

Generate **advanced technical content** for RAG optimization when the user provides a topic.

**Supported Topics:**
- Hybrid Search (Dense + Sparse)
- Reranking (Cohere, Cross-Encoders)
- Query Expansion (Multi-query, Step-back)
- Metadata Filtering
- Context Compression
- Multi-Vector Retrieval

⚠️ **MANDATORY RULE**  
ALWAYS perform a **web search** to:
- Find the latest "SOTA" (State of the Art) techniques
- Check benchmarks for Rerankers (e.g., MTEB Leaderboard)
- Verify library support in `langchain` / `llama-index`

---

## Input Format

User provides a **Optimization Technique**.

---

## Output: 2 Deliverables

### 1. Deep Dive Notebook (`01_Advanced_[Topic]_RAG.ipynb`)
### 2. Concept Deep Dive (`02_[Topic]_DeepDive.md`)

---

## FILE 1: Deep Dive Notebook

**File Name:** `01_Advanced_[Topic]_RAG.ipynb`

**Header:**
```markdown
<img src="https://drive.google.com/uc?export=view&id=1wYSMgJtARFdvTt5g7E20mE4NmwUFUuog" width="200">

## Advanced RAG: [Topic]
*Performance Optimization Series*

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/[NOTEBOOK_ID])
```

**Structure:**
1.  **Baseline**: Set up a "naive" RAG pipeline first.
2.  **Implementation**: Implement the [Topic] (e.g., add a Reranker).
3.  **Comparison**: Run the same tricky queries on Baseline vs Optimized.
4.  **Metrics**: Measure partial improvement (Did the correct chunk appear higher?).

**Code Style:**
- Precise visualization of "Rank" changes.
- Use `pandas` to show side-by-side retrieved contexts.

---

## FILE 2: Concept Deep Dive

**File Name:** `02_[Topic]_DeepDive.md`

**Structure:**
```markdown
# Mastering [Topic] for RAG

## 🔬 The Science
Why does this work? (e.g., "Cross-encoders attend to the interaction between query and document...")

## 📉 When to use it?
- **Scenario A**: High recall needed.
- **Scenario B**: Noisy data.

## 🛑 Cost/Latency Trade-offs
- "Reranking adds X ms latency..."
- "Query expansion increases LLM costs by Y%..."

## 🔗 Reference Architecture
[Mermaid Diagram of the advanced flow]
```

---

## Search Requirements

Before generating, search for:
1.  "[Topic] benchmark results 2024"
2.  "Optimizing RAG with [Topic]"
3.  "[Topic] latency vs accuracy trade-off"
