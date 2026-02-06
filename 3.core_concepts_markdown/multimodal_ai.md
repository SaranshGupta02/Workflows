---
name: Multimodal AI Content Generator
description: Automates content creation for Multimodal AI concepts including Tutorials, Use Case Demos, and Visual Showcases.
---

# Multimodal AI Content Generator

Generate **immersive educational content** for Multimodal AI topics (Vision, Audio, Video) when the user provides a topic.

**Supported Topics:**
- Computer Vision (Object Detection, OCR, Segmentation)
- Audio Processing (STT, TTS, Audio Generation)
- Video Processing (Analysis, Generation)
- Multimodal LLMs (GPT-4o, Gemini 1.5 Pro, Claude 3.5 Sonnet)

⚠️ **MANDATORY RULE**  
ALWAYS perform a **web search** to:
- Check for the absolute latest model versions (this field moves fast)
- Verify file size limits and supported formats
- Find new libraries for media handling (e.g., `moviepy`, `pydub` alternatives)

---

## Input Format

User provides a **Target Topic** or **Modality**.

---

## Output: 3 Deliverables

### 1. Multimodal Tutorial (`01_[Topic]_Tutorial.md`)
### 2. Use Case Demo Script (`02_[Topic]_Demo.py`)
### 3. Visual Showcase Guide (`03_[Topic]_Visuals.md`)

---

## FILE 1: Multimodal Tutorial

**File Name:** `01_[Topic]_Tutorial.md`

**Structure:**
```markdown
# Multimodal Magic: [Topic]

## 👁️/👂/🎬 What is [Topic]?
Brief intro to the modality.

## 🤖 The Models
- **Model A**: Specs and strengths.
- **Model B**: Specs and strengths.

## 🛠️ Key Techniques
- **Prompting for Images**: "Describe vs Analyze"
- **Audio Pipelines**: Handling sampling rates.
- **Video Context**: Handling frames vs duration.

## 💻 Sample Code Snippet
Small snippet showing how to send an image/audio to an API.
```python
# Quick example
response = model.generate_content([prompt, image_file])
```
```

---

## FILE 2: Use Case Demo Script

**File Name:** `02_[Topic]_Demo.py`

**Purpose:**
A standalone Python script or small Streamlit app demonstrating a "WOW" factor use case.

**Ideas:**
- **Vision**: "Fridge Content Analyzer" (Upload photo -> Get recipes)
- **Audio**: "Podcast Summarizer" (Upload mp3 -> Get text summary)
- **Video**: "Highlight Extractor" (Upload video -> Get key timestamps)

**Requirements:**
- **Simple Dependencies**: minimal `requirements.txt`.
- **Clear Output**: Print results to console or display in UI clearly.
- **Asset Handling**: Include a check for a sample file or allow user upload.

---

## FILE 3: Visual Showcase Guide

**File Name:** `03_[Topic]_Visuals.md`

**Purpose:**
Since we can't generate the media files directly, this file provides **Exact Prompts** and **Input Examples** for the user to try.

**Structure:**
```markdown
# Visual Showcase: [Topic] Experiments

## 🧪 Experiment 1: [Name]
**Goal**: Test reasoning capabilities on complex charts.

**Input Image**: [Description of image to find/use]
**Prompt**:
> "Analyze this chart trend and predict the next 3 months..."

**Expected Output**:
[Description of what a good model should say]

---

## 🧪 Experiment 2: [Name]
**Goal**: Test creative generation.

**Input**: [Description]
**Prompt**:
> "..."
```

---

## Search Requirements

Before generating, search for:
1.  "Best multimodal models for [Topic] 2024/2025"
2.  "[Topic] python library recommendations"
3.  "Creative use cases for [Topic]"
