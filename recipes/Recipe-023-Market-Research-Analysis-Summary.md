# Market Research Analysis and Summary

**Recipe #23: From Raw Research to Actionable Insights**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 10 minutes (first time) / 5 minutes (repeat) | 4-8 hours per report | Intermediate | Strategy, Marketing, Product, Sales, Executives |

---

## The Problem

You have access to market research—industry reports, analyst publications, trend data, survey results—but transforming this into insights your organization can act on is time-consuming. Reports are often hundreds of pages, full of data that may or may not be relevant to your situation. You need the "so what?" not just the "what." By the time you've processed one report, three more have arrived.

**Pain Points:**
- Reports are too long and generic
- Hard to extract what matters for YOUR business
- Data without implications
- Multiple conflicting sources
- No time to read everything
- Research sits unused after purchase

---

## The Outcome

Synthesized market insights tailored to your business context with clear implications and recommended actions. Transform lengthy reports into actionable intelligence that drives decisions. Get value from research investments by actually using the findings.

**What You'll Have When Done:**
- Concise summary of key market findings
- Implications specific to your business
- Trend analysis with forecasts
- Opportunity and threat identification
- Recommended actions
- Data-supported decision making

---

## When to Use This Recipe

**Good Fit:**
- Processing new market research reports
- Annual market review and planning
- Entering new markets or segments
- Validating business assumptions
- Investor/board market briefings
- Competitive and market intelligence

**Not a Good Fit:**
- Primary research (creating original research)
- Real-time market monitoring (too slow)
- Highly technical research requiring domain expertise
- When you need to verify data accuracy (Claude summarizes, doesn't audit)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have market research to analyze (PDFs, reports, data)
- [ ] You know your specific questions and needs
- [ ] You understand your current business context
- [ ] You have 1-2 hours for analysis and synthesis

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Reads and summarizes lengthy documents
- Extracts key data points and trends
- Identifies patterns across multiple sources
- Translates generic findings to your context
- Creates structured summaries
- Generates visualizable data

**Where Human Judgment Is Essential:**
- Validating data accuracy
- Understanding nuances research might miss
- Applying organizational context
- Making strategic decisions
- Knowing what research to trust
- Balancing research with intuition

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Industry reports | Gartner, Forrester, IDC reports | Market sizing, trends |
| Survey data | Customer surveys, market surveys | Customer insights |
| Analyst publications | Investment research, commentary | Expert perspectives |
| Trade publications | Industry news, trend pieces | Current developments |
| Your context | Business description, questions | Tailored analysis |

**Sample Input:**
```
Market Research Analysis Request

Our company: HealthTrack (employee wellness platform)
Market: Corporate wellness and benefits
Current position: 200 customers, $15M ARR, mid-market focused

Research to analyze:
1. [Gartner report on corporate wellness market - 85 pages]
2. [Willis Towers Watson benefits survey - 120 pages]
3. [Deloitte wellbeing report - 45 pages]
4. [McKinsey future of work article - 20 pages]

Questions we're trying to answer:
1. How big is the market and how fast is it growing?
2. What trends should we be paying attention to?
3. Where is buyer demand shifting?
4. What opportunities exist for us specifically?
5. What threats should concern us?
6. Should we expand beyond mid-market?
```

---

## Step-by-Step Implementation

### Step 1: Gather Your Research
**Time: 10-15 minutes**

Collect the research you want to analyze:
- Download or access the reports
- Note your specific questions
- Identify what decisions this analysis should inform
- Prioritize which sources matter most

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
cd ~/Documents/market-research
claude
```

---

### Step 3: Process Each Research Source
**Time: 10-15 minutes per source**

Start with individual source analysis:

**For each document, use this prompt:**

```
Please analyze this market research document.

DOCUMENT: [Name of report/source]
"""
[Paste document content or provide file path]
"""

OUR CONTEXT:
- Company: [Your company and what you do]
- Market: [Your market/segment]
- Current position: [Your size, focus, customers]

SPECIFIC QUESTIONS:
- [Question 1]
- [Question 2]
- [Question 3]

EXTRACT:
1. KEY FINDINGS
   - Top 5-7 most important findings
   - Supporting data for each

2. MARKET DATA
   - Market size (TAM, SAM, SOM if available)
   - Growth rates
   - Segmentation data
   - Geographic breakdown

3. TRENDS IDENTIFIED
   - Major trends with supporting evidence
   - Timeline expectations
   - Confidence level

4. IMPLICATIONS FOR US
   - What this means for our business specifically
   - Opportunities identified
   - Threats identified

5. DATA QUALITY NOTES
   - Methodology (if stated)
   - Potential biases or limitations
   - How recent is the data?
```

---

### Step 4: Synthesize Across Sources
**Time: 15-20 minutes**

After processing individual sources, synthesize:

**PRIMARY PROMPT: Market Research Synthesis**

```
Synthesize the market research I've shared into actionable insights.

OUR COMPANY CONTEXT:
- Company: [Name and description]
- Market: [Your market segment]
- Current position: [Size, focus, customers]
- Strategic questions: [What you're trying to decide]

RESEARCH SOURCES ANALYZED:
1. [Source 1 summary]
2. [Source 2 summary]
3. [Source 3 summary]
(Use the summaries from Step 3)

PLEASE PROVIDE:

1. EXECUTIVE SUMMARY
   - Key takeaways in 3-5 bullets
   - Overall market assessment
   - One-paragraph synthesis

2. MARKET OVERVIEW
   - Total market size and growth
   - Segmentation relevant to us
   - Geographic considerations
   - Where sources agree/disagree

3. TREND ANALYSIS
   | Trend | Evidence Level | Timeline | Impact on Us |

   For each major trend:
   - What's happening
   - How confident are we (multiple sources vs. single)
   - When will it matter
   - Implications for our business

4. OPPORTUNITY ASSESSMENT
   - Market opportunities identified
   - Size of opportunity
   - Our ability to capture
   - Required investments
   - Risk level

5. THREAT ASSESSMENT
   - Threats to our current business
   - Likelihood and timing
   - Potential impact
   - Mitigation options

6. COMPETITIVE DYNAMICS
   - What research says about competition
   - Market structure evolution
   - Our relative position

7. CUSTOMER INSIGHTS
   - Buyer behavior trends
   - Changing needs/preferences
   - Decision-making patterns
   - Segment-specific insights

8. STRATEGIC IMPLICATIONS
   - What this means for our strategy
   - Decisions we should consider
   - Questions we still need to answer
   - Recommended next steps

9. CONFIDENCE ASSESSMENT
   | Finding | # Sources | Consistency | Confidence |

   Flag where sources conflict or data is limited

10. APPENDIX: DATA TABLES
    - Key data points extracted
    - Source citations
```

---

### Step 5: Validate and Enrich
**Time: 15-20 minutes**

Review the synthesis:

**To validate findings:**
```
Some of these findings seem optimistic. What are the potential biases in these sources? What would make these projections wrong?
```

**To add current context:**
```
This research is from [date]. What's changed since then that might affect these conclusions? (Search for recent developments.)
```

**To go deeper on specifics:**
```
Go deeper on the enterprise segment opportunity. What specifically does the research say about enterprise buyers, and what would it take for us to compete?
```

**To challenge assumptions:**
```
The market sizing seems aggressive. Walk me through the methodology and identify where the estimates might be inflated.
```

---

### Step 6: Create Deliverables
**Time: 10 minutes**

```
Create these outputs:

1. MARKET BRIEF (2-3 pages)
   - Executive summary format
   - Key data points visualized
   - Clear recommendations

2. DATA TABLES
   - Market sizing data
   - Growth projections
   - Segment breakdowns
   - Source citations

3. PRESENTATION SLIDES (8-10 slides)
   - Visual format for leadership briefing
   - Key charts and data points
   - Strategic implications highlighted

4. QUESTIONS FOR FURTHER RESEARCH
   - Gaps in current research
   - Areas needing primary research
   - Suggested next steps
```

---

## Example Output

Below is an abbreviated market research synthesis example:

---

> **MARKET RESEARCH SYNTHESIS: Corporate Wellness Market**
> **Prepared for: HealthTrack | October 2024**
>
> ---
>
> **EXECUTIVE SUMMARY**
>
> The corporate wellness market is experiencing significant transformation driven by post-pandemic workforce changes, mental health prioritization, and technology integration. Key findings:
>
> - **Market size:** $65B globally, growing 7-9% annually (varies by segment)
> - **Fastest growth:** Mental health (+15%), integrated platforms (+12%)
> - **Buyer shift:** Moving from point solutions to integrated platforms
> - **Enterprise opportunity:** Larger employers investing significantly more
> - **Threat:** Traditional wellness (gym subsidies, biometrics) declining
>
> **Bottom line for HealthTrack:** The market is moving in your direction (integrated, tech-enabled), but the window to capture enterprise is narrowing as large platform players consolidate.
>
> ---
>
> **MARKET OVERVIEW**
>
> | Metric | Finding | Confidence |
> |--------|---------|------------|
> | Global market (2024) | $62-68B | High (3 sources agree) |
> | US market (2024) | $22-25B | High |
> | Growth rate | 7-9% CAGR | Medium (range varies) |
> | Enterprise segment | $12B, growing faster (11%) | Medium |
> | Mid-market segment | $6B, moderate growth (7%) | Medium |
>
> **Source Reconciliation:**
> - Gartner: Conservative ($62B, 7% growth)
> - Willis Towers Watson: Aggressive ($68B, 9% growth)
> - Deloitte: Middle ($65B, 8% growth)
>
> Differences largely due to segment definitions—Gartner excludes EAP, others include it.
>
> ---
>
> **TREND ANALYSIS**
>
> | Trend | Evidence | Timeline | Impact on HealthTrack |
> |-------|----------|----------|----------------------|
> | Mental health prioritization | All 4 sources | Now | ✅ High positive |
> | Platform consolidation | Gartner, McKinsey | 12-24 months | ⚠️ Opportunity and threat |
> | Personalization demand | All sources | Now | ✅ Product opportunity |
> | ROI scrutiny | WTW, Deloitte | Increasing | ⚠️ Need to prove value |
> | Integration requirements | All sources | Now | ✅ API strength matters |
>
> **Detailed Trend: Platform Consolidation**
>
> The market is rapidly moving from point solutions to integrated platforms. Buyers want:
> - Single vendor for multiple wellness dimensions
> - Integration with HRIS, benefits admin, and payroll
> - Unified reporting and analytics
>
> *What this means for HealthTrack:* You need to either expand platform capabilities or establish strong integration partnerships. Pure-play point solutions are losing to comprehensive platforms.
>
> ---
>
> **OPPORTUNITY ASSESSMENT**
>
> **Opportunity 1: Enterprise Expansion**
>
> | Dimension | Assessment |
> |-----------|------------|
> | Market size | $12B and growing fastest (11%) |
> | Our current position | Limited (<5% of revenue from enterprise) |
> | Barrier to entry | Sales motion, security requirements, implementation |
> | Investment required | $2-3M (enterprise sales team, compliance) |
> | Likelihood of success | Medium—need to move fast, market consolidating |
>
> *Recommendation:* Pursue with urgency—the enterprise window is closing as larger players consolidate.
>
> **Opportunity 2: Mental Health Deep Expansion**
>
> | Dimension | Assessment |
> |-----------|------------|
> | Market size | $8B segment, growing 15% |
> | Our current position | Basic capabilities |
> | Barrier to entry | Clinical expertise, content, regulations |
> | Investment required | $1-2M (content, partnerships) |
> | Likelihood of success | High—strong demand, underserved market |
>
> *Recommendation:* Priority investment—highest growth segment with strong product-market fit potential.
>
> ---
>
> **THREAT ASSESSMENT**
>
> **Threat 1: Platform Vendor Consolidation**
>
> - **What:** Large HR tech players (Workday, SAP) expanding into wellness
> - **Timeline:** Already happening—Workday launched wellness module in 2024
> - **Impact:** Could commoditize standalone wellness platforms
> - **Mitigation:** Specialize deeply or build unassailable integrations
> - **Severity:** 🔴 High
>
> **Threat 2: Point Solution Commoditization**
>
> - **What:** Basic wellness features becoming table stakes
> - **Timeline:** 12-24 months
> - **Impact:** Price pressure, reduced differentiation
> - **Mitigation:** Move up value chain to outcomes, not features
> - **Severity:** ⚠️ Medium
>
> ---
>
> **STRATEGIC IMPLICATIONS**
>
> Based on this research:
>
> 1. **Move upmarket with urgency.** The enterprise segment is most attractive, but the window is closing. Delay means competing against entrenched platform players.
>
> 2. **Invest in mental health.** This is the highest-growth segment with the most unmet need. Deep capability here creates differentiation.
>
> 3. **Build or buy integration.** The market demands integrated solutions. You need either platform breadth or unbeatable integration with major HR platforms.
>
> 4. **Prove ROI.** Buyer scrutiny is increasing. Invest in measurement and outcomes demonstration.
>
> **Recommended Next Steps:**
> 1. Conduct enterprise buyer research (our primary research gap)
> 2. Develop enterprise sales motion business case
> 3. Evaluate mental health partnership/acquisition options
> 4. Build integration roadmap for top 5 HR platforms

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Findings too generic | Research not connected to your context | Add: "Specifically for a company like ours that [description], what does this mean?" |
| Numbers don't make sense | Different definitions/methodologies | Ask: "What methodology did each source use? Reconcile the differences" |
| Missing key questions | Questions not specified | Be explicit: "I specifically need to know about [X]" |
| Research seems biased | Source limitations | Ask: "What are the potential biases in this source? Who funded it?" |
| Can't reconcile conflicting data | Sources genuinely disagree | Ask: "Where sources conflict, which is more credible and why?" |
| Implications too obvious | Not enough analysis | Ask: "Go deeper—what non-obvious implications does this have?" |

---

## Tips from Experience

1. **Question the research.** Reports have biases, methodological limitations, and aging data. Always ask "who produced this and why?"

2. **Context is everything.** Generic market data becomes valuable only when interpreted for your specific situation.

3. **Triangulate sources.** Single-source findings are hypotheses. Multi-source agreement is more reliable.

4. **Focus on decisions.** What decisions will this research inform? Keep that front and center.

5. **Note the gaps.** What did you NOT learn? That's your primary research agenda.

6. **Update your priors.** Research should change your thinking. If it just confirms what you believed, you either found the right research or you're not learning.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Complex reports are distilled to actionable insights
- [ ] Research informs actual decisions
- [ ] Stakeholders understand market dynamics
- [ ] Opportunities and threats are clearly identified
- [ ] Next steps are concrete and actionable

**Track over time:**
- Decisions influenced by research
- Time from research acquisition to insight delivery
- Stakeholder satisfaction with research synthesis
- Accuracy of research-based predictions (retrospective)

---

## Variations

### Quick Report Summary
For single report rapid processing:
```
Summarize this market research report for a busy executive.

Report: [Paste or attach]
Our company: [Brief description]

Provide:
1. 5 key findings (1 sentence each)
2. What it means for us (2-3 sentences)
3. Recommended action (1 sentence)
4. What to ignore (1-2 sentences)

Keep total summary under 300 words.
```

### Trend Watch
For monitoring market trends:
```
Based on recent market research and news, update me on trends in [market].

Our last review: [Date and key findings]
What we're watching: [Specific trends]

Search for recent developments and provide:
1. What's changed since our last review
2. New trends emerging
3. Trends accelerating or decelerating
4. Implications for our [specific area]
```

### Competitive Market Analysis
For market research focused on competition:
```
Analyze this market research with focus on competitive dynamics.

Research: [Paste or attach]
Our position: [Where we sit]
Key competitors: [List]

Focus on:
1. Market structure and concentration
2. How competition is evolving
3. Where competitors are winning/losing
4. White space opportunities
5. Competitive threats to our position
```

### Customer Segment Deep Dive
For segment-specific analysis:
```
Analyze this research focused on [specific segment].

Research: [Paste or attach]
Segment of interest: [Description]
Our current position in segment: [Description]

Extract:
1. Segment size and growth
2. Segment-specific needs and behaviors
3. How this segment differs from others
4. Our opportunity in this segment
5. What it would take to win
```

---

## Building Your Repeatable System

After several research cycles, establish your system:

1. **Create a research tracker** documenting what you have
2. **Build an insights library** of key findings
3. **Establish update cadence** for recurring topics
4. **Maintain source quality ratings** based on accuracy
5. **Connect research to strategy** through regular reviews

**Sample Setup:**
```
market-research/
├── sources/
│   ├── industry-reports/
│   ├── analyst-publications/
│   ├── surveys/
│   └── articles/
├── syntheses/
│   ├── 2024-Q4-market-review/
│   │   ├── synthesis.md
│   │   ├── presentation.pptx
│   │   └── data-tables.xlsx
│   └── archive/
├── templates/
│   ├── analysis-prompt.txt
│   └── synthesis-prompt.txt
└── tracking/
    ├── source-inventory.md
    └── insights-library.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**process multiple sources → extract key findings → synthesize patterns → derive implications → recommend actions**—applies broadly:

| Role | Application |
|------|-------------|
| **Strategy** | Market sizing, trend analysis |
| **Product** | Market requirements, opportunity sizing |
| **Marketing** | Customer insights, positioning |
| **Sales** | Market intelligence, territory planning |
| **Executives** | Board preparation, investor relations |
| **Consultants** | Client market research |

---

## Next Steps

1. **Gather your research:** Collect reports you've been meaning to read
2. **Prioritize by value:** Which reports matter most for current decisions?
3. **Run the analysis:** Start with your highest-priority source
4. **Build the habit:** Make research synthesis a regular practice

---

*Recipe #23 of 100 in the Claude Code Knowledge Worker Recipe Collection*
