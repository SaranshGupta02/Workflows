---
name: SDLC with AI Content Generator
description: Automates content creation for SDLC phases including Planning, Coding, Debugging, and Review.
---

# SDLC with AI Content Generator

Generate **workflow-centric content** optimization Software Development Life Cycle phases with AI.

**Supported Topics:**
- Requirement Drafting (AI Planning)
- Code Generation Strategies
- AI-Assisted Debugging
- Test Generation (Unit/Integration)
- Code Review (AI Reviewers)

⚠️ **MANDATORY RULE**  
ALWAYS perform a **web search** to:
- Find methodologies like "Test Driven Development with AI"
- Check for tools integrating specifically into CI/CD
- Verify best practices for "Human-in-the-loop" reviews

---

## Input Format

User provides a **SDLC Phase** (e.g., "Debugging", "Testing").

---

## Output: 2 Deliverables

### 1. Workflow Tutorial (`01_AI_[Phase]_Workflow.md`)
### 2. Prompt Template Library (`02_[Phase]_Prompts.md`)

---

## FILE 1: Workflow Tutorial

**File Name:** `01_AI_[Phase]_Workflow.md`

**Structure:**
```markdown
# Modern [Phase] with AI

## 🔄 The Old Way vs The AI Way
Comparison table showing time/effort savings.

## 🛠️ The Process
1. **Input**: What you give the AI (Logs, Code, Requirements).
2. **Action**: The prompt/tool to use.
3. **Refinement**: How to check the output.

## ⚠️ Gotchas
- "AI will hallucinate edge cases..."
- "Don't paste secrets..."

## 📸 Demo Flow
Screenshots/Text description of a real execution.
```

---

## FILE 2: Prompt Template Library

**File Name:** `02_[Phase]_Prompts.md`

**Purpose:**
A collection of copy-paste prompts for this specific phase.

**Structure:**
```markdown
# AI Prompts for [Phase]

## 🌟 The "Super [Phase]" Prompt
> "Act as a senior QA engineer. Analyze this code for edge cases..."

## 🐛 The "Fix It" Prompt
> "Explain this error stack trace and suggest 3 potential fixes..."

## 🧪 The "Test Gen" Prompt
> "Write pytest cases for this function, covering happy path and null inputs..."
```

---

## Search Requirements

Before generating, search for:
1.  "AI for [Phase] best practices"
2.  "Prompt engineering for [Phase]"
3.  "Case studies AI in [Phase]"
