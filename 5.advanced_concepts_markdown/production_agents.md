---
name: Production Agents Content Generator
description: Automates content creation for Production-Grade Agents including Multi-Agent Architectures and Project Tutorials.
---

# Production Agents Content Generator

Generate **deployment-ready agent architectures** when the user provides a framework or pattern.

**Supported Topics:**
- Multi-Agent Systems (Supervisor-Worker, Hierarchical)
- Frameworks (LangGraph, AutoGen, CrewAI Enterprise)
- Human-in-the-loop patterns
- State Management & Persistence

⚠️ **MANDATORY RULE**  
ALWAYS perform a **web search** to:
- Find "production" examples (not just toy demos)
- Check how to handle state persistence (Postgres, Redis) in the target framework
- Verify recommended patterns for "Human-in-the-loop"

---

## Input Format

User provides a **Framework** and **Architecture Pattern**.

---

## Output: 2 Deliverables

### 1. Full Project Tutorial (`01_[Framework]_Project.md`)
### 2. Architecture Diagram (`02_[Framework]_Arch.mermaid`)

---

## FILE 1: Full Project Tutorial

**File Name:** `01_[Framework]_Project.md`

**Structure:**
```markdown
# Building a Production [Framework] Agent

## 🏗️ The Scenario
"We are building a Customer Support Team that..."
- Triage Agent (Router)
- Refund Agent (Tool user)
- QA Manager (Reviewer)

## 🗄️ State Management
How we save state so the agent doesn't forget context on refresh.
```python
# Code snippet for checkpointing
checkpointer = PostgresSaver(conn)
```

## 🕵️ Human-in-the-Loop
Adding a breakpoint where a human must approve an action.

## 🚀 Deployment
Dockerizing and serving this agent via API (FastAPI/LangServe).
```

---

## FILE 2: Architecture Diagram

**File Name:** `02_[Framework]_Arch.mermaid`

**Requirement:**
Complex interactions visualization.

**Structure:**
```mermaid
sequenceDiagram
    participant User
    participant Router
    participant Researcher
    participant Editor
    participant Database

    User->>Router: "Write a blog post about X"
    Router->>Researcher: Delegate task
    Researcher->>Database: Fetch implementation_plan
    Researcher->>Router: Return Draft
    Router->>Editor: Request Review
    Editor-->>User: Request Approval (Human Interface)
```

---

## Search Requirements

Before generating, search for:
1.  "Deploying [Framework] to production"
2.  "[Framework] state persistence guide"
3.  "Multi-agent patterns [Framework] 2025"
