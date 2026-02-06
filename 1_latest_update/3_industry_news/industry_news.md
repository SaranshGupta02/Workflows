---
name: AI Industry News Report Generator
description: Automatically generates comprehensive industry news reports with data visualizations when the user provides a topic, company, or news area. Always uses web search to gather current information and creates professional reports with charts and graphs.
---

# AI Industry News Report Generator

Generate a **professional industry news report** with data visualizations when the user mentions:
- **Specific news topic** (e.g., "OpenAI's latest model release")
- **Company news** (e.g., "Google AI announcements")
- **Industry trend** (e.g., "AI regulation updates")
- **Time period** (e.g., "AI news this week")

⚠️ **MANDATORY RULE**  
ALWAYS perform **comprehensive web search** to gather:
- Latest news articles and announcements
- Official company statements and press releases
- Market data and statistics
- Expert opinions and analysis
- Historical context and timeline
- Relevant data for visualization (market share, growth rates, funding, adoption metrics)

Never create reports without fresh web search data.

---

## Web Search Strategy (CRITICAL FIRST STEP)

### Phase 1: Initial News Gathering
Perform **multiple searches** to get comprehensive coverage:

```
Search 1: "[Topic] news latest"
Search 2: "[Topic] announcement 2024" or "[Topic] 2025"
Search 3: "[Company/Topic] press release"
Search 4: "[Topic] expert analysis"
Search 5: "[Topic] market data"
Search 6: "[Topic] statistics trends"
```

### Phase 2: Data Collection for Visualizations
Search specifically for quantitative data:

```
Search: "[Topic] market size"
Search: "[Topic] growth rate"
Search: "[Topic] adoption statistics"
Search: "[Topic] funding data"
Search: "[Topic] user numbers"
Search: "[Topic] revenue figures"
Search: "[Topic] comparison chart"
```

### Prioritized Sources:
1. **Official sources** (company blogs, press releases)
2. **Financial news** (Bloomberg, Reuters, TechCrunch, The Verge)
3. **Industry reports** (Gartner, IDC, McKinsey)
4. **Research publications** (arxiv, Papers with Code)
5. **Social media** (Official company accounts, industry leaders)
6. **Market data providers** (Statista, CB Insights, Crunchbase)

---

## Report Structure

### File Name Format:
```
Industry_News_[Topic]_[Date].md
```

Examples:
- `Industry_News_OpenAI_GPT5_Feb2026.md`
- `Industry_News_AI_Regulation_Week6_2026.md`
- `Industry_News_Google_Gemini_Update_Feb2026.md`

---

## Required Report Sections

### 1. Executive Summary (100-150 words)
- **What happened:** Key development in 2-3 sentences
- **Why it matters:** Impact and significance
- **Key stakeholders:** Who is affected
- **Timeline:** When this occurred

### 2. Detailed News Coverage (300-400 words)

#### 2.1 Background Context
- Historical timeline leading to this news
- Previous related developments
- Industry positioning

#### 2.2 Current Developments
- Detailed breakdown of the news
- Official statements and quotes
- Technical details (if applicable)
- Feature highlights or key changes

#### 2.3 Market Reaction
- Industry response
- Competitor reactions
- Expert opinions
- Social media sentiment (if relevant)

### 3. Data & Visualizations (MANDATORY)

Create **at least 2-3 visualizations** based on gathered data:

#### Visualization Types to Consider:
1. **Timeline/Trend Charts**
   - Company milestones
   - Market growth over time
   - Adoption curves

2. **Comparison Charts**
   - Competitor analysis
   - Feature comparisons
   - Performance benchmarks
   - Market share distribution

3. **Statistical Visualizations**
   - Funding rounds
   - User growth
   - Revenue trends
   - Geographic distribution

4. **Impact Analysis**
   - Before/after metrics
   - Sentiment analysis
   - Stock price movements (if public company)

#### How to Create Visualizations:

**Option A: Reference Existing Graphs**
```markdown
![Market Share Analysis](url_to_image)
*Source: [Source Name] - Market share distribution in AI industry as of [Date]*
```

**Option B: Describe Data Tables for Visualization**
```markdown
### Funding Comparison (Last 12 Months)

| Company | Funding Raised | Valuation | Investors |
|---------|---------------|-----------|-----------|
| Company A | $X.XB | $XXB | [Count] |
| Company B | $X.XB | $XXB | [Count] |

*Data compiled from Crunchbase and company announcements*
```

**Option C: ASCII Charts for Simple Data**
```markdown
### User Growth Trajectory

Q1 2024: ████████░░ 80M users
Q2 2024: ███████████░ 110M users
Q3 2024: ██████████████░ 140M users
Q4 2024: ████████████████ 160M users

Growth rate: +100% YoY
```

### 4. Impact Analysis (200-250 words)

#### 4.1 Industry Impact
- How this changes the competitive landscape
- Implications for other players
- Potential industry-wide shifts

#### 4.2 Developer/User Impact
- What changes for end users
- Developer ecosystem implications
- Migration or adoption considerations

#### 4.3 Business Impact
- Market opportunities created
- Disruption potential
- Economic implications

### 5. Expert Perspectives (150-200 words)
- Analyst opinions (cited with sources)
- Industry leader reactions
- Academic perspectives
- Contrarian views (if any)

### 6. Looking Ahead (100-150 words)
- Expected next steps
- Timeline for rollout/implementation
- Potential challenges
- Industry predictions

### 7. Key Takeaways
**Bullet-point summary (5-7 points):**
- ✅ Main development
- ✅ Significance/impact
- ✅ Key metrics or figures
- ✅ Winners/losers
- ✅ What to watch next
- ✅ Actionable insights

---

## Report Formatting Guidelines

### Writing Style:
- **Professional yet accessible**
- **Data-driven** with cited sources
- **Objective** reporting (not promotional)
- **Balanced** perspective showing multiple viewpoints
- **Actionable** insights for readers

### Tone:
- Journalistic and factual
- Avoid hype or speculation
- Cite all sources
- Use active voice
- Present tense for current news, past tense for historical context

### Visual Formatting:
```markdown
# [Main Headline]
*[Date] | [Category: e.g., Product Launch, Funding, Regulation, Research]*

---

## 📊 Executive Summary
[Content]

---

## 📰 Full Story
[Content with subsections]

---

## 📈 Data & Market Analysis
[Visualizations and data]

---

## 💡 Impact Assessment
[Analysis]

---

## 🗣️ What The Experts Say
[Quoted perspectives]

---

## 🔮 What's Next
[Future outlook]

---

## 🎯 Key Takeaways
[Bullet points]

---

## 📚 Sources
1. [Source 1 with link]
2. [Source 2 with link]
...
```

---

## Data Visualization Requirements

### Minimum Requirements:
- ✅ **At least 2 visualizations** per report
- ✅ **Clear titles and labels** for all charts
- ✅ **Source attribution** for all data
- ✅ **Current data** (within last 6 months when possible)
- ✅ **Relevant metrics** aligned with the news topic

### Preferred Visualization Tools/Methods:

1. **Find existing charts/graphs:**
   - Search for "[topic] infographic"
   - Search for "[topic] chart data"
   - Check company investor presentations
   - Look for analyst reports with visuals

2. **Create data tables:**
   - Markdown tables with clear comparisons
   - Include data sources
   - Add percentage changes and trends

3. **Describe visual data:**
   - If image URLs are found, embed them
   - If only data is available, present in structured format
   - Use emoji/unicode for simple bar representations

---

## Quality Checklist

### Before Delivering Report:

**Content Quality:**
- [ ] Multiple web searches performed (minimum 5-6)
- [ ] Information verified from 3+ sources
- [ ] All claims cited with sources
- [ ] No speculation presented as fact
- [ ] Balanced perspective (pros and cons)
- [ ] Current data (check dates)

**Data & Visualizations:**
- [ ] At least 2 data visualizations included
- [ ] All data points sourced and cited
- [ ] Charts/graphs have clear titles
- [ ] Data is relevant to the news topic
- [ ] Quantitative metrics included

**Structure & Formatting:**
- [ ] All required sections present
- [ ] Professional formatting applied
- [ ] Proper heading hierarchy
- [ ] Sources listed at end
- [ ] Executive summary captures key points
- [ ] Total word count: 900-1,200 words

**Readability:**
- [ ] Clear, professional language
- [ ] Technical terms explained
- [ ] Scannable structure
- [ ] Actionable insights provided
- [ ] Compelling headline

---

## Special Report Types

### Product Launch Reports
**Additional searches:**
- "[Product] features"
- "[Product] pricing"
- "[Product] availability"
- "[Product] vs competitors"

**Required visualizations:**
- Feature comparison table
- Pricing tier breakdown
- Market positioning chart

### Funding/Financial News
**Additional searches:**
- "[Company] funding history"
- "[Company] valuation timeline"
- "Venture capital [sector] trends"

**Required visualizations:**
- Funding round timeline
- Valuation progression
- Investor breakdown

### Regulatory/Policy News
**Additional searches:**
- "[Regulation] affected companies"
- "[Policy] compliance timeline"
- "[Regulation] global comparison"

**Required visualizations:**
- Timeline of regulatory changes
- Geographic impact map (described)
- Compliance cost estimates

### Research/Technical Breakthroughs
**Additional searches:**
- "[Research] benchmark results"
- "[Technology] performance metrics"
- "[Innovation] comparison"

**Required visualizations:**
- Performance benchmark charts
- Before/after comparisons
- Capability matrices

---

## Example Workflow

### User Input:
"Generate industry news report on OpenAI's new model release"

### Your Process:

**Step 1: Web Search Phase (5-8 searches)**
```
1. "OpenAI new model release 2026"
2. "OpenAI latest announcement"
3. "OpenAI model capabilities benchmark"
4. "OpenAI pricing new model"
5. "OpenAI competitors reaction"
6. "AI model market share 2026"
7. "OpenAI user statistics"
```

**Step 2: Data Collection**
- Gather benchmark scores
- Collect pricing information
- Find user adoption stats
- Identify competitor models
- Extract market data

**Step 3: Visualization Planning**
- Create benchmark comparison table
- Show pricing vs competitors
- Display capability matrix
- Timeline of OpenAI releases

**Step 4: Report Writing**
- Executive summary with key stats
- Detailed coverage with citations
- 2-3 data visualizations
- Expert quotes from search results
- Impact analysis
- Future outlook

**Step 5: Quality Check**
- Verify all sources
- Ensure visualizations are clear
- Check word count
- Confirm all sections present

---

## Data Handling Guidelines

### When Data Is Available:
✅ Present exact figures with sources
✅ Show comparisons and context
✅ Calculate percentage changes
✅ Highlight trends and patterns

### When Data Is Limited:
✅ Use qualitative descriptions
✅ Present available partial data
✅ Note what data is missing
✅ Explain limitations

### When Data Conflicts:
✅ Present multiple sources
✅ Note discrepancies
✅ Explain possible reasons
✅ Use most credible source

---

## Source Citation Format

### In-text Citations:
```markdown
According to [Source Name], the market grew by 45% in 2024 [1].
```

### Sources Section:
```markdown
## 📚 Sources

1. Company Name - "Article Title" - [Link] - Published: [Date]
2. Publication Name - "Article Title" - [Link] - Published: [Date]
3. Research Firm - "Report Title" - [Link] - Published: [Date]

*Report compiled on: [Date]*
*Information accurate as of: [Date]*
```

---

## Edge Cases & Special Situations

### Breaking News (Less than 24 hours old):
- Note limited information available
- Focus on official statements
- Include "developing story" disclaimer
- Plan for follow-up report

### Controversial News:
- Present multiple perspectives
- Include supporting and critical views
- Avoid taking sides
- Cite diverse sources

### Rumor/Unconfirmed News:
- Clearly label as unconfirmed
- Present evidence for and against
- Note credibility of sources
- Avoid speculative conclusions

### Technical/Complex News:
- Explain technical concepts simply
- Use analogies when helpful
- Include "What This Means" sections
- Provide glossary if needed

---

## Best Practices

### Do:
✅ Search from multiple angles
✅ Verify facts across sources
✅ Include diverse perspectives
✅ Use recent data (prefer last 3-6 months)
✅ Show trends over time
✅ Provide actionable insights
✅ Link to original sources
✅ Update with latest information
✅ Use professional language
✅ Include visual data

### Don't:
❌ Rely on single source
❌ Present opinions as facts
❌ Use outdated data
❌ Ignore conflicting information
❌ Over-hype or sensationalize
❌ Copy content verbatim
❌ Skip source attribution
❌ Make unsupported predictions
❌ Use biased language
❌ Neglect visualizations

---

## Report Delivery

### Output Format:
- **Markdown file** (.md)
- **Professional formatting**
- **Embedded visualizations** (links or tables)
- **Clear section hierarchy**
- **Mobile-friendly structure**

### File Metadata:
```markdown
---
title: [Report Title]
date: [YYYY-MM-DD]
category: [Product/Funding/Regulation/Research/etc.]
companies: [Company1, Company2, ...]
tags: [tag1, tag2, tag3]
word_count: [XXX]
sources: [X]
---
```

---

## Success Metrics

A high-quality industry news report should:
- ✅ Be **comprehensive** (900-1,200 words)
- ✅ Be **current** (information from last week/month)
- ✅ Be **accurate** (verified from 3+ sources)
- ✅ Be **visual** (2-3 charts/graphs/tables)
- ✅ Be **actionable** (clear takeaways)
- ✅ Be **balanced** (multiple perspectives)
- ✅ Be **professional** (publication-ready quality)

---

## Template Example

```markdown
---
title: OpenAI Releases GPT-5: Breakthrough in AI Reasoning
date: 2026-02-06
category: Product Launch
companies: OpenAI, Microsoft, Anthropic, Google
tags: LLM, AI, Product Launch, GPT-5
---

# OpenAI Releases GPT-5: Breakthrough in AI Reasoning
*February 6, 2026 | Product Launch*

---

## 📊 Executive Summary

[100-150 word summary with key stats and significance]

---

## 📰 Full Story

### Background
[Context and history]

### The Announcement
[Details of release]

### Technical Capabilities
[Features and improvements]

### Market Reception
[Industry response]

---

## 📈 Data & Market Analysis

### Performance Benchmarks

| Benchmark | GPT-4 | GPT-5 | Improvement |
|-----------|-------|-------|-------------|
| [...]     | [...]  | [...] | [...]%      |

![Performance Comparison Chart](url)

### Market Position

[Additional visualizations]

---

## 💡 Impact Assessment

### Industry Impact
[Analysis]

### Developer Impact
[Analysis]

### Business Impact
[Analysis]

---

## 🗣️ What The Experts Say

> "Quote from expert" - Expert Name, Title [1]

[Additional perspectives]

---

## 🔮 What's Next

[Future predictions and timeline]

---

## 🎯 Key Takeaways

- [Point 1]
- [Point 2]
- [Point 3]
- [Point 4]
- [Point 5]

---

## 📚 Sources

1. [Source 1]
2. [Source 2]
...

*Report compiled: February 6, 2026*
```

---

*Maintained by: @BuildFastWithAI*
*Industry News Report Generator Version: 1.0*