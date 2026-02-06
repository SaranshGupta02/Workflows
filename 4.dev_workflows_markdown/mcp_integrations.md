---
name: Integrations & MCPs Content Generator
description: Automates content creation for MCP Servers, GitHub Actions, and Bot Integrations.
---

# Integrations & MCPs Content Generator

Generate **technical integration content** for connecting AI with external tools (MCP, GitHub, Slack, DBs).

**Supported Topics:**
- Model Context Protocol (MCP) Servers
- GitHub Actions & Automation
- Slack/Discord Bots
- Database Integrations (Postgres with AI)

⚠️ **MANDATORY RULE**  
ALWAYS perform a **web search** to:
- **CRITICAL**: Search for the official "Model Context Protocol" spec updates.
- Verify latest API endpoints for Slack/GitHub/Discord.
- Check security best practices for webhooks and bots.

---

## Input Format

User provides a **Integration Target** (e.g., "Postgres MCP", "GitHub Action PR Reviewer").

---

## Output: 3 Deliverables

### 1. Integration Cookbook (`01_[Target]_Cookbook.md`)
### 2. Server/Bot Code (`02_[Target]_Code.py` or `.ts`)
### 3. Usage Guide (`03_[Target]_Usage.md`)

---

## FILE 1: Integration Cookbook

**File Name:** `01_[Target]_Cookbook.md`

**Structure:**
```markdown
# Building a [Target] Integration

## 🎯 Goal
Connect AI to [Target] to allow [Capability].

## 🏗️ Architecture
- **Protocol**: MCP / Webhook / REST API
- **Auth**: OAuth / API Key
- **Flow**: User -> AI -> [Target]

## 📋 Prerequisites
- [Target] Account
- Python/Node.js installed
- ngrok (if local webhook testing)
```

---

## FILE 2: Server/Bot Code

**File Name:** `02_[Target]_Code.py`

**Purpose:**
The actual server code (MCP server or Bot backend).

**Example (MCP):**
```python
# Simple MCP Server for [Target]
from mcp.server import Server
import requests

app = Server("[Target] Connector")

@app.tool()
def fetch_data(query: str):
    """Fetches data from [Target]"""
    # implementation
    pass

if __name__ == "__main__":
    app.run()
```

---

## FILE 3: Usage Guide

**File Name:** `03_[Target]_Usage.md`

**Structure:**
```markdown
# How to use the [Target] Integration

## 🔌 Connection
How to configure the client (e.g., Claude Desktop or Cursor) to use this MCP server.
```json
{
  "mcpServers": {
    "my-server": {
      "command": "python",
      "args": ["server.py"]
    }
  }
}
```

## 🗣️ Commands
- "Ask Claude to fetch the latest PRs..."
- "Ask Claude to query the database..."

## 🐞 Troubleshooting
- Common connection errors.
```

---

## Search Requirements

Before generating, search for:
1.  "Model Context Protocol python sdk"
2.  "[Target] API documentation"
3.  "Building AI agents with [Target]"
