---
name: AI Benchmark & Research Content Generator
description: Automatically creates comprehensive, beginner-friendly content for any AI benchmark or research paper when the user provides the benchmark/research name.
---

# AI Benchmark & Research Content Generator

Generate a **detailed yet easy-to-understand content piece** (200-300 words) for any AI benchmark or research when the user mentions:
- **Benchmark name** (e.g., MMLU, HumanEval, GSM8K, GPQA)
- **Research paper title** or **arxiv ID**

⚠️ **MANDATORY RULE**  
ALWAYS perform a **web search** to gather:
- Official benchmark description
- What it measures
- Key metrics and evaluation criteria
- Notable model performances
- Historical context and importance
- Any associated graphs, charts, or visual data
- Real-world implications

Never assume information—always verify through web search first.

---

## Content Generation Guidelines

### Target Audience
- **Beginners** with basic AI knowledge
- Non-technical stakeholders
- Students and learners
- AI practitioners seeking quick summaries

### Writing Style
- **Clear and conversational** (avoid jargon)
- Use **analogies and examples** when explaining complex concepts
- Break down technical terms
- Include **practical implications**
- Make it **engaging and scannable**

---

## Required Content Structure

### 1. Introduction (40-60 words)
- What is this benchmark/research?
- Why does it matter?
- Quick context setting

### 2. What It Measures (60-80 words)
- Core evaluation criteria
- Test methodology
- Specific capabilities assessed
- How scores are calculated

### 3. Key Findings & Performance (60-80 words)
- Notable model performances
- State-of-the-art results
- Trends and patterns
- Comparative analysis

### 4. Real-World Impact (40-60 words)
- Why this matters in practice
- Industry applications
- Limitations to consider
- Future implications

---

## Visual Elements (MANDATORY)

### Include When Available:
1. **Performance comparison graphs**
   - Bar charts showing model rankings
   - Line graphs showing progress over time
   - Scatter plots for capability mapping

2. **Score distributions**
   - Histogram of results
   - Percentile breakdowns

3. **Benchmark composition**
   - Pie charts showing task categories
   - Sample question types

### Format for Including Images:
```markdown
![Benchmark Name - Description](image_url)
*Figure caption explaining what the graph shows*
```

⚠️ **If graphs are found during web search:**
- Include image URLs directly in content
- Add descriptive captions
- Reference the graph in the text

---

## Web Search Strategy

### Primary Sources to Search:
1. **Official benchmark papers** (arxiv.org, papers with code)
2. **Leaderboards** (huggingface.co, paperswithcode.com)
3. **Model provider blogs** (OpenAI, Anthropic, Google, etc.)
4. **Academic publications** (Google Scholar)
5. **Benchmark documentation** (GitHub repos, official sites)

### Search Queries to Use:
- "[Benchmark Name] explained"
- "[Benchmark Name] leaderboard"
- "[Benchmark Name] results comparison"
- "[Benchmark Name] what does it test"
- "[Benchmark Name] sota results"
- "[Benchmark Name] visualization graph"

---

## Content Requirements

### Must Include:
- ✅ **Word count:** 200-300 words (excluding image captions)
- ✅ **Readability:** 8th-grade reading level
- ✅ **Technical accuracy:** Verified through web search
- ✅ **Current data:** Latest available scores and rankings
- ✅ **Visual elements:** At least 1 graph/chart if available
- ✅ **Practical context:** Real-world relevance explained

### Should Avoid:
- ❌ Dense academic language
- ❌ Unexplained acronyms
- ❌ Outdated information
- ❌ Overly technical formulas (unless crucial)
- ❌ Speculation without data

---

## Example Content Format

```markdown
# [Benchmark/Research Name]

## Overview
[40-60 word introduction explaining what this is and why it matters]

## What It Evaluates
[60-80 words describing the evaluation methodology and what capabilities are tested]

![Performance Graph](url_to_graph)
*Caption describing the visualization and key takeaways*

## Current State-of-the-Art
[60-80 words covering latest results, top performers, and trends]

## Why This Matters
[40-60 words explaining real-world applications and implications]

---

**Key Metrics:**
- Metric 1: Description
- Metric 2: Description
- Metric 3: Description

**Top Performers (as of [date]):**
1. Model A - Score
2. Model B - Score
3. Model C - Score

**Learn More:** [Official Source Link]
```

---

## Special Cases

### For Research Papers:
- Extract key contributions
- Explain methodology in simple terms
- Highlight novel findings
- Show before/after comparisons

### For Multi-Task Benchmarks:
- Break down by task category
- Show performance across different dimensions
- Explain weighting methodology

### For Domain-Specific Benchmarks:
- Provide domain context
- Explain why domain expertise matters
- Show cross-domain comparison

---

## Quality Checklist

Before delivering content, verify:

- [ ] Web search completed with multiple sources
- [ ] Information is current (check publication/update dates)
- [ ] Technical accuracy verified
- [ ] Word count within 200-300 range
- [ ] At least 1 visual element included (if available)
- [ ] Beginner-friendly language used
- [ ] Real-world implications explained
- [ ] All acronyms defined on first use
- [ ] Sources cited or linked
- [ ] Content is scannable with clear sections

---

## Output Format

Deliver content as a **markdown (.md) file** with:
- Clear hierarchical headings
- Proper formatting for readability
- Embedded images with captions
- Bullet points for key metrics
- Links to sources

### File Naming Convention:
```
[Benchmark_Name]_Explained.md
```

Examples:
- `MMLU_Explained.md`
- `HumanEval_Explained.md`
- `GPQA_Explained.md`

---

## Edge Cases

### If Benchmark Is Very New:
- Note limited data availability
- Focus on methodology and intended use
- Compare to similar existing benchmarks

### If Benchmark Is Deprecated:
- Explain historical importance
- Note current alternatives
- Provide context for why it was replaced

### If Information Is Limited:
- Be transparent about knowledge gaps
- Synthesize from related sources
- Suggest where to find more information

---

## Example Workflow

1. **User Input:** "Generate content for MMLU benchmark"

2. **Your Actions:**
   - Search: "MMLU benchmark explained"
   - Search: "MMLU leaderboard 2024"
   - Search: "MMLU benchmark visualization"
   - Search: "what does MMLU test"

3. **Content Creation:**
   - Synthesize findings
   - Write in beginner-friendly language
   - Include performance graph if found
   - Add practical context

4. **Delivery:**
   - Save as `MMLU_Explained.md`
   - Verify word count and quality checklist
   - Present to user

---

## Best Practices

### Do:
✅ Use active voice
✅ Include specific numbers and metrics
✅ Explain "so what?" implications
✅ Use analogies for complex concepts
✅ Update content with latest data
✅ Cross-reference multiple sources

### Don't:
❌ Copy-paste from sources verbatim
❌ Use undefined technical jargon
❌ Present opinions as facts
❌ Ignore recent developments
❌ Overcomplicate explanations

---

## Additional Notes

- **Performance Data:** Always include the date when citing scores (models improve rapidly)
- **Context Matters:** Explain limitations and what the benchmark doesn't measure
- **Fairness:** Present multiple perspectives when there's debate about benchmark validity
- **Updates:** Note if this is an evolving benchmark with planned changes

---

*Maintained by: @BuildFastWithAI*
*Content Generator Version: 1.0*
