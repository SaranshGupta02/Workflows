---
name: AI Agents Basics Content Generator
description: Automates content creation for AI Agents concepts including Notebooks, Documentation, and Demo Apps.
---

# AI Agents Basics Content Generator

Generate **hands-on educational content** for AI Agents topics when the user provides a topic.

**Supported Topics:**
- Agent Loops (ReAct, Plan-and-Solve)
- Tool Calling / Function Calling
- Planning & Reasoning
- Memory Systems (Short-term vs Long-term)
- Frameworks (LangChain, CrewAI, AutoGen, Agno)

⚠️ **MANDATORY RULE**  
ALWAYS perform a **web search** to:
- Verify latest API syntax for libraries like `langchain-core` or `crewai`
- Find recent examples of agent patterns
- Check for new "Agentic" models or capabilities

---

## Input Format

User provides a **Target Topic** or **Agent Pattern**.

---

## Output: 3 Deliverables

### 1. Agentic Notebook (`01_[Topic]_Agent_Logic.ipynb`)
### 2. Documentation Explainer (`02_[Topic]_Explained.md`)
### 3. Demo App Interface (`03_[Topic]_Agent_App.py` - Optional)

---

## FILE 1: Agentic Notebook

**File Name:** `01_[Topic]_Agent_Logic.ipynb`

**Header:**
```markdown
<img src="https://drive.google.com/uc?export=view&id=1wYSMgJtARFdvTt5g7E20mE4NmwUFUuog" width="200">

## AI Agents: [Topic] Workshop
*Building Intelligent Systems*

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/[NOTEBOOK_ID])
```

**Structure:**
1.  **Objective**: What kind of agent are we building? (e.g., "Research Agent").
2.  **Tools Setup**: Defining functions the agent can use (Search, Calculator, etc.).
3.  **The Brain (LLM)**: Initializing the model (OpenAI/Anthropic/Gemini).
4.  **The Loop**: Implementing the [Topic] (e.g., The ReAct loop logic).
5.  **Execution**: Running the agent on test tasks.
6.  **Inspection**: Printing the "Thought Process" (intermediate steps).

**Code Style:**
- Use `pydantic` for structured tool definitions.
- Show raw prompt/completion logs if possible to demystify the "magic".

---

## FILE 2: Documentation Explainer

**File Name:** `02_[Topic]_Explained.md`

**Structure:**
```markdown
# Understanding [Topic] in AI Agents

## 🎬 The Analogy
Explain the concept using a human role (e.g., "A Project Manager" or "A Librarian").

## 🧠 The Architecture
Visualize the flow:
`Observation -> Thought -> Action -> Result`

## 💻 Tech Stack Options
- **LangChain**: Good for...
- **CrewAI**: Good for...
- **Scratch**: Good for learning...

## 🚧 Common Challenges
- Infinite loops
- Hallucinated tool calls
- Context window overflow

## 📚 Further Reading
- [Paper Link]
- [Documentation Link]
```

---

## FILE 3: Demo App Interface

**File Name:** `03_[Topic]_Agent_App.py`

**Purpose:**
A clean interface to interact with the agent defined in the notebook.

**Requirements:**
- **Streamlit** based.
- **Chat Interface**: Use `st.chat_message` to show the conversation.
- **Sidebar**:
  - API Keys
  - Agent Configuration (e.g., "Max Iterations", "Temperature")
  - Branding Block (Standard HTML)
- **"Thinking" Indicator**: Show a spinner or expander while the agent is processing.

```python
with st.status("Agent is thinking...", expanded=True) as status:
    st.write("Searching web...")
    st.write("Reading content...")
    status.update(label="Complete!", state="complete", expanded=False)
```

---

## Search Requirements

Before generating, search for:
1.  "[Topic] agent implementation python"
2.  "Latest changes in [Framework] 2024/2025"
3.  "State of the art [Topic] agents"
