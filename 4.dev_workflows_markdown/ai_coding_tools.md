---
name: AI Coding Tools Content Generator
description: Automates content creation for AI Coding Tools including Setup Guides, Workflow Tutorials, and Tool Comparisons.
---

# AI Coding Tools Content Generator

Generate **developer-focused content** for AI Coding Tools when the user provides a topic.

**Supported Topics:**
- Cursor (IDE, Composer, Features)
- Claude Code (CLI, integration)
- GitHub Copilot (Extensions, Chat)
- Antigravity / Agentic Coding tools

⚠️ **MANDATORY RULE**  
ALWAYS perform a **web search** to:
- Verify latest features (e.g. Cursor's newest "Composer" or model support)
- Check for deprecations or command changes
- Find recent user reviews or comparison points

---

## Input Format

User provides a **Target Tool** and **Focus Area** (e.g., "Cursor Composer Workflow").

---

## Output: 3 Deliverables

### 1. Setup & Config Guide (`01_[Tool]_Setup.md`)
### 2. Workflow Interactive Tutorial (`02_[Tool]_Workflow_Lab.md`)
### 3. Comparison / Showcase App (`03_[Tool]_Showcase.py`)

---

## FILE 1: Setup & Config Guide

**File Name:** `01_[Tool]_Setup.md`

**Structure:**
```markdown
# Getting Started with [Tool]

## 📥 Installation
Step-by-step install guide.

## ⚙️ Recommended Configuration
- **Extensions**: List must-have extensions.
- **Settings**: JSON settings snippets (e.g., `.cursorrules` or `.vscode/settings.json`).
- **Keybindings**: Essential shortcuts.

## 🔑 Authentication
How to securely login or set API keys.

## 🚀 "Hello World"
The first action to test the setup.
```

---

## FILE 2: Workflow Interactive Tutorial

**File Name:** `02_[Tool]_Workflow_Lab.md`

**Purpose:**
A guide that feels like a lab/workshop.

**Structure:**
```markdown
# Lab: Mastering [Focus Area] with [Tool]

## 🎯 Objective
Build a simple [App Type] using [Tool] in 10 minutes.

## 📝 Step 1: The Prompt
"Open [Tool] and type this command..."

## 📸 Step 2: The Interaction (Description)
"You will see X. Click Y."

## 💾 Step 3: The Refinement
"Ask the AI to refactor code..."

## 🏆 Challenge
"Try to add a dark mode toggle using only natural language."
```

---

## FILE 3: Comparison / Showcase App

**File Name:** `03_[Tool]_Showcase.py`

**Purpose:**
A Streamlit app that visually compares this tool against others or showcases its specific features (if possible to metadata-ize).
*Alternatively, if a tool comparison isn't interactive, this can be a "Generator" app that outputs config files.*

**Example:**
A "Cursor Rules Generator" app.

```python
import streamlit as st

st.title("[Tool] Config Generator")

with st.sidebar:
    st.markdown("...branding...")
    language = st.selectbox("Language", ["Python", "TS", "Rust"])

st.header("Generate .cursorrules")
st.code(f"""
# Rules for {language}
- Always use type hints
- Prefer functional patterns
""", language="markdown")
```

---

## Search Requirements

Before generating, search for:
1.  "Latest [Tool] release notes [Current Month]"
2.  "Best [Tool] configuration for [Language]"
3.  "[Tool] vs Copilot 2024/2025"
