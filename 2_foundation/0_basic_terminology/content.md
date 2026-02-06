---
name: GenAI Fundamentals Content Generator
description: Creates educational content about GenAI terminology and concepts in 3 formats - YouTube script, viral tweet, and interactive notebook (when applicable)
---

# GenAI Fundamentals Content Generator

Generate **comprehensive educational content** for GenAI terminology and concepts when the user provides a topic (e.g., "tokens", "LLM", "embeddings", "prompt engineering", etc.).

⚠️ **MANDATORY RULE**  
ALWAYS perform a **web search** to:
- Verify current definitions and best practices
- Find real-world examples and use cases
- Check latest statistics and benchmarks
- Identify common misconceptions

---

## Input Format

User provides a **GenAI topic** such as:
- Tokens
- Large Language Models (LLMs)
- Embeddings
- Fine-tuning
- Prompt Engineering
- Temperature
- Context Window
- RAG (Retrieval Augmented Generation)
- Vector Databases
- Transformers
- etc.

---

## Output: 3 Deliverables

### 1. YouTube Video Script (`01_YouTube_[Topic].md`)
### 2. Viral Tweet Thread (`02_Tweet_[Topic].md`)
### 3. Interactive Notebook (`03_[Topic]_Interactive.ipynb`) - ONLY if hands-on demonstration is possible

---

## FILE 1: YouTube Video Script

**File Name:** `01_YouTube_[Topic].md`

**Structure:**
```markdown
# [Topic] - Complete Guide for Beginners

## 📌 Video Metadata
- **Duration:** 8-12 minutes
- **Target Audience:** Complete beginners to GenAI
- **Learning Outcome:** Clear understanding of [topic] with practical examples

---

## 🎬 HOOK (0:00-0:30)
[Attention-grabbing opening]
- Start with a relatable problem or surprising fact
- Example: "Ever wondered why ChatGPT sometimes cuts off mid-sentence? It's all about TOKENS..."

---

## 📚 INTRODUCTION (0:30-1:30)
[Set the stage]
- What is [topic]?
- Why does it matter?
- Real-world analogy (make it relatable)

---

## 🔍 DEEP DIVE (1:30-7:00)

### Part 1: The Basics
[Core concept explanation]
- Break down complex ideas into simple terms
- Use analogies and metaphors
- Include visual cue suggestions: [VISUAL: Show diagram of...]

### Part 2: How It Works
[Technical but accessible explanation]
- Step-by-step breakdown
- Real examples from popular AI tools

### Part 3: Common Misconceptions
[Address confusion]
- Myth vs Reality
- What people get wrong

### Part 4: Practical Implications
[Why it matters to users]
- How it affects AI performance
- Cost implications (if relevant)
- Best practices

---

## 💡 REAL-WORLD EXAMPLES (7:00-9:00)
[Concrete demonstrations]
- Example 1: [Specific scenario]
- Example 2: [Another scenario]
- Show before/after or comparison

---

## 🎯 KEY TAKEAWAYS (9:00-10:00)
[Summary bullets]
- 3-5 key points to remember
- Actionable tips

---

## 📢 CALL TO ACTION (10:00-end)
- Encourage experimentation
- Link to notebook (if applicable)
- Subscribe for more GenAI fundamentals

---

## 📝 VISUAL SUGGESTIONS
[List all suggested graphics/animations]
- Timestamp: Visual description
- Timestamp: Visual description

---

## 🔗 RESOURCES TO MENTION
- Official documentation links
- Tools to try
- Further reading
```

---

## FILE 2: Viral Tweet Thread

**File Name:** `02_Tweet_[Topic].md`

**Structure:**
```markdown
# Viral Tweet Thread: [Topic] Explained

## 🧵 Thread Structure (8-12 tweets)

---

**Tweet 1 - HOOK** 🎣
[Attention-grabbing opener with emoji]
- Use a surprising statistic or bold claim
- Include relevant emoji
- Max 280 characters
- End with "A thread 🧵"

Example:
"You're wasting 50% of your AI budget because you don't understand TOKENS.

Here's what every AI user needs to know (and the tools don't tell you):

A thread 🧵"

---

**Tweet 2 - THE PROBLEM**
[Identify the pain point]
- What confusion exists?
- What's the cost of not understanding?

---

**Tweet 3-4 - SIMPLE EXPLANATION**
[Break down the concept]
- Use simple language
- Include an analogy
- One idea per tweet

---

**Tweet 5-6 - HOW IT WORKS**
[Technical details made simple]
- Visual descriptions (since we can't embed images)
- Step-by-step if needed

---

**Tweet 7-8 - PRACTICAL EXAMPLES**
[Real-world scenarios]
- Concrete numbers
- Before/after comparisons
- Tool-specific tips

---

**Tweet 9 - COMMON MISTAKES**
[What to avoid]
- Quick list format
- Save people money/time

---

**Tweet 10 - PRO TIPS**
[Advanced insights]
- Lesser-known facts
- Optimization tricks

---

**Tweet 11 - TAKEAWAY**
[Summary with impact]
- Memorable one-liner
- Actionable insight

---

**Tweet 12 - CTA**
[Call to action]
- Retweet if valuable
- Follow for more
- Link to notebook (if applicable)
- Tag @BuildFastWithAI

---

## 📊 ENGAGEMENT ELEMENTS
- Emojis to use: [List relevant emojis]
- Hashtags: #GenAI #AI #MachineLearning #[TopicSpecific]
- Best posting time: [Suggestion based on tech audience]

## 🎨 VISUAL SUGGESTIONS (for manual creation)
- Thread unroller friendly format
- Consider creating infographic from tweets 3-8
```

---

## FILE 3: Interactive Notebook (Conditional)

**File Name:** `03_[Topic]_Interactive.ipynb`

**Create ONLY if the topic allows hands-on demonstration**, such as:
- ✅ Tokens (tokenization examples)
- ✅ Embeddings (similarity calculations)
- ✅ Temperature (generation variations)
- ✅ Prompt Engineering (A/B testing)
- ❌ General LLM concepts (too abstract)

---

### Notebook Header (REQUIRED)
```markdown
<img src="https://drive.google.com/uc?export=view&id=1wYSMgJtARFdvTt5g7E20mE4NmwUFUuog" width="200">

[![Gen AI Experiments](https://img.shields.io/badge/Gen%20AI%20Experiments-GenAI%20Bootcamp-blue?style=for-the-badge&logo=artificial-intelligence)](https://github.com/buildfastwithai/gen-ai-experiments)
[![Gen AI Experiments GitHub](https://img.shields.io/github/stars/buildfastwithai/gen-ai-experiments?style=for-the-badge&logo=github&color=gold)](http://github.com/buildfastwithai/gen-ai-experiments)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/[NOTEBOOK_ID])

## Understanding [Topic] - Interactive Guide

**Learning Objectives:**
- Understand what [topic] is
- See it in action with real examples
- Learn best practices
- Experiment yourself

👉 [Master GenAI Fundamentals](https://www.buildfastwithai.com/genai-course)
```

---

### Notebook Structure

| Section | Purpose |
|---------|---------|
| **1. What is [Topic]?** | Text explanation with diagrams |
| **2. Setup** | Install dependencies, imports |
| **3. Basic Example** | Simplest demonstration |
| **4. Interactive Experimentation** | User can modify and see results |
| **5. Real-World Scenarios** | Practical applications |
| **6. Comparison** | Show variations/alternatives |
| **7. Best Practices** | Tips and tricks |
| **8. Cost/Performance** | Metrics when relevant |
| **9. Try It Yourself** | Exercises with solutions |

---

### Implementation Rules

- **Beginner-friendly code** with extensive comments
- **No API keys required** for basic examples (use mock data when possible)
- If API needed, use Colab secrets:
```python
  from google.colab import userdata
  api_key = userdata.get("OPENAI_API_KEY")  # or relevant key
```
- **Interactive widgets** where possible (sliders for temperature, dropdowns, etc.)
- **Visual outputs**: charts, tables, color-coded text
- **Side-by-side comparisons** to show differences
- Every code cell **must produce output**
- Total runtime: **under 5 minutes**

---

### Example Interactive Elements

**For Tokens:**
```python
# Interactive tokenizer
import ipywidgets as widgets
from IPython.display import display

text_input = widgets.Textarea(
    value='Hello, world!',
    description='Text:',
    layout=widgets.Layout(width='50%', height='100px')
)

def show_tokens(change):
    # Tokenization code here
    pass

text_input.observe(show_tokens, names='value')
display(text_input)
```

**For Temperature:**
```python
# Slider to adjust temperature
temperature_slider = widgets.FloatSlider(
    value=0.7,
    min=0.0,
    max=2.0,
    step=0.1,
    description='Temperature:'
)
```

---

## Quality Checklist

### YouTube Script
- [ ] Hook grabs attention in first 30 seconds
- [ ] Complex concepts broken into analogies
- [ ] 3-5 visual cue suggestions
- [ ] Addresses common misconceptions
- [ ] Includes real-world examples
- [ ] 8-12 minute duration
- [ ] Clear call-to-action

### Tweet Thread
- [ ] Hook tweet is compelling
- [ ] 8-12 tweets total
- [ ] One idea per tweet
- [ ] Includes emojis strategically
- [ ] Actionable insights
- [ ] No jargon without explanation
- [ ] CTA includes @BuildFastWithAI

### Interactive Notebook
- [ ] Runs in fresh Colab environment
- [ ] No hardcoded secrets
- [ ] Interactive elements work
- [ ] Clear visual outputs
- [ ] Under 5 minute runtime
- [ ] Exercises with solutions
- [ ] Proper branding header

---

## Content Guidelines

### Language & Tone
- **Conversational but authoritative**
- Explain like teaching a smart friend
- Avoid unnecessary jargon
- When using technical terms, define them immediately
- Use active voice

### Examples to Use
- ChatGPT, Claude, GPT-4, Gemini (popular models people know)
- Real pricing examples
- Actual token counts
- Common use cases (writing, coding, analysis)

### What to Avoid
- Overly academic language
- Assumptions about prior knowledge
- Outdated examples or statistics
- Controversial takes on AI safety (stay educational)

---

## Search Requirements

Before generating content, **web search** for:
1. **Latest definitions** - ensure accuracy
2. **Current best practices** - what's changed?
3. **Real-world statistics** - token costs, limits, etc.
4. **Common questions** - what confuses people?
5. **Tool updates** - latest features in ChatGPT, Claude, etc.

---

## Delivery Format

Create a folder structure:
```
[Topic]_Educational_Package/
├── 01_YouTube_[Topic].md
├── 02_Tweet_[Topic].md
└── 03_[Topic]_Interactive.ipynb (if applicable)
```

---

## Example Topics & Interactivity

| Topic | YouTube | Tweet | Notebook |
|-------|---------|-------|----------|
| Tokens | ✅ | ✅ | ✅ (tokenizer demo) |
| LLMs | ✅ | ✅ | ❌ (too abstract) |
| Embeddings | ✅ | ✅ | ✅ (similarity calc) |
| Temperature | ✅ | ✅ | ✅ (generation tests) |
| Context Window | ✅ | ✅ | ✅ (truncation demo) |
| Prompt Engineering | ✅ | ✅ | ✅ (A/B testing) |
| RAG | ✅ | ✅ | ✅ (simple pipeline) |
| Fine-tuning | ✅ | ✅ | ⚠️ (complex, maybe skip) |

---

*Maintained by: @BuildFastWithAI*
*Mission: Making GenAI accessible to everyone*