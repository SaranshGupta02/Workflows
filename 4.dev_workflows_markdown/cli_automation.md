---
name: CLI & Terminal Automation Content Generator
description: Automates content creation for CLI tools and Terminal scripts including Demos and Productivity Tips.
---

# CLI & Terminal Automation Content Generator

Generate **developer-productivity content** for CLI/Terminal topics when the user provides a tool name.

**Supported Topics:**
- Claude CLI
- Gemini CLI
- Shell Scripting (Bash/PowerShell)
- Terminal Automation tools (e.g., gh cli, jq)

⚠️ **MANDATORY RULE**  
ALWAYS perform a **web search** to:
- Check for latest CLI flags and commands
- Verify cross-platform compatibility (Mac/Linux/Windows)
- Find cool "one-liners" that impress developers

---

## Input Format

User provides a **Target Tool** or **Workflow**.

---

## Output: 3 Deliverables

### 1. Cheat Sheet (`01_[Tool]_Cheatsheet.md`)
### 2. Magic Script Demo (`02_[Tool]_Magic_Script.sh`)
### 3. Video Script (Short) (`03_[Tool]_Short_Video.md`)

---

## FILE 1: Cheat Sheet

**File Name:** `01_[Tool]_Cheatsheet.md`

**Structure:**
```markdown
# [Tool] Power User Cheat Sheet

## 🚀 Basic Commands
| Command | Does |
|---------|------|
| `tool run` | ... |

## 🧙‍♂️ Advanced Flags
- `--json`: Output as JSON for piping.
- `--filter`: ...

## 💡 Top 3 Use Cases
1. **Log Analysis**: `tool logs | grep error`
2. **Auto-PR**: `tool pr create --fill`
```

---

## FILE 2: Magic Script Demo

**File Name:** `02_[Tool]_Magic_Script.sh` (or `.ps1`)

**Purpose:**
A copy-pasteable script that does something useful immediately.

**Structure:**
```bash
#!/bin/bash

# [Tool] Magic Automator
# Purpose: [Explain purpose]

echo "Starting automation..."

# 1. Fetch data
[tool] fetch > data.json

# 2. Process
[tool] process --input data.json

echo "Done!"
```

---

## FILE 3: Video Script (Short)

**File Name:** `03_[Tool]_Short_Video.md`

**Purpose:**
Script for a 60-second vertical video (TikTok/Reels/Shorts).

**Structure:**
```markdown
# 📱 60s Magic: [Tool]

## 🎬 Scene 1: The Problem (0-10s)
*Visual: Developer struggling with manual terminal task.*
"Stop doing X manually in the terminal!"

## 🎬 Scene 2: The Solution (10-40s)
*Visual: Screen recording of [Tool] running.*
"Use [Tool]. Just type `[Command]` and watch it fly."

## 🎬 Scene 3: The Result (40-60s)
"It generated the whole file in seconds. Link in bio."
```

---

## Search Requirements

Before generating, search for:
1.  "[Tool] cool tricks 2024"
2.  "[Tool] automation scripts github"
3.  "Most useful [Tool] commands"
