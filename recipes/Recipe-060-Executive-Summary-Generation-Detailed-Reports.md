# Executive Summary Generation from Detailed Reports

**Recipe #60: Distill Complex Reports into Actionable Summaries**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 2 minutes (first time) / 1 minute (repeat) | 30-60 minutes per summary | Beginner | Analysts, Managers, Chiefs of Staff, Anyone Presenting Up |

---

## The Problem

You have a 50-page report full of important information, but executives have 5 minutes. You understand the details, but struggle to extract what matters most. Every stakeholder wants the "bottom line" but defining that bottom line requires judgment. Reports get buried because the summary wasn't compelling enough to read. Good analysis goes to waste because it wasn't packaged for decision-makers.

**Pain Points:**
- Executives don't read long reports
- Hard to identify the 3-5 things that really matter
- Important nuance gets lost in oversimplification
- Time pressure forces rushed summaries
- Different stakeholders need different emphasis
- Critical recommendations buried on page 47
- "So what?" question unanswered

---

## The Outcome

Crisp, compelling executive summaries that convey the essential findings, implications, and recommendations from any detailed report. Summaries calibrated for executive attention spans that preserve necessary nuance while cutting through complexity.

**What You'll Have When Done:**
- One-page executive summary
- Key findings (3-5 bullet points)
- Implications for the business
- Recommended actions
- What to do with the detailed report
- Talking points for verbal briefing

---

## When to Use This Recipe

**Good Fit:**
- Research reports
- Analysis documents
- Consultant deliverables
- Industry reports
- Internal audit findings
- Project post-mortems
- Competitive analyses
- Any report >10 pages

**Not a Good Fit:**
- Already short documents
- Creative or narrative content
- Legal documents requiring full review
- Highly technical specifications needing expert interpretation

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have the detailed report to summarize
- [ ] You know who will receive the summary
- [ ] You understand what decisions the summary should inform
- [ ] You have 15-30 minutes for summary development

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Extracts key themes from long documents
- Identifies main findings and recommendations
- Structures summaries clearly
- Calibrates detail level to audience
- Maintains logical flow
- Highlights implications

**Where Human Judgment Is Essential:**
- Validating extracted findings
- Adding organizational context
- Emphasizing what matters most to this audience
- Catching misinterpretations
- Final tone and positioning
- Approval before distribution

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Full report | PDF, document, text | Content extraction |
| Audience | Who will read | Calibration |
| Purpose | What decision | Focus |
| Constraints | Length, format | Output shaping |
| Context | What they know | Emphasis |

**Sample Input:**
```
Executive Summary Request

REPORT: Q3 2024 Customer Churn Analysis
PAGES: 34 pages with appendices
AUTHOR: Customer Success Analytics Team

FULL REPORT CONTENT:
[Paste report or key sections]

SUMMARY OF SECTIONS:
1. Executive Summary (existing - 2 pages)
2. Methodology (3 pages)
3. Churn Metrics Overview (5 pages)
4. Segment Analysis (8 pages)
5. Root Cause Analysis (6 pages)
6. Predictive Model Findings (4 pages)
7. Recommendations (3 pages)
8. Appendices (3 pages)

KEY DATA POINTS FROM REPORT:
- Q3 churn rate: 4.2% (vs 3.8% Q2, 3.5% Q3 2023)
- Highest churn segment: SMB (<50 employees) at 8.1%
- Lowest churn segment: Enterprise (>500 employees) at 1.2%
- Top 3 churn reasons: Price (34%), Competitor switch (28%), Unmet needs (22%)
- Predictive model identifies at-risk accounts with 78% accuracy
- 127 accounts flagged high-risk for Q4
- Recommended interventions estimated to retain $2.3M ARR

KEY FINDINGS FROM REPORT:
1. Churn acceleration is concentrated in SMB segment
2. Price sensitivity increased 40% YoY following pricing changes
3. Competitor X capturing share with lower-cost alternative
4. Accounts with <3 integrations churn at 3x rate
5. CSM touch in past 30 days reduces churn by 60%
6. At-risk account model is production-ready

RECOMMENDATIONS FROM REPORT:
1. Launch SMB retention campaign (high priority)
2. Consider pricing tier for smallest customers
3. Prioritize CSM outreach based on risk model
4. Track integration adoption as health metric
5. Competitive response strategy for Competitor X

AUDIENCE: CEO and executive team
PURPOSE: Quarterly business review (5 minutes for this topic)
WHAT THEY KNOW: Aware churn increased; don't know details
WHAT THEY CARE ABOUT: Revenue impact, competitive position, what to do

CONSTRAINTS:
- Maximum 1 page
- Must include a recommendation
- Should enable decision-making without reading full report
```

---

## Step-by-Step Implementation

### Step 1: Gather Report Content
**Time: 5-10 minutes**

Either:
- Paste full report text
- Paste key sections (findings, recommendations)
- Provide structured summary of report content

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Executive Summary Prompt
**Time: 3-5 minutes for Claude to process**

---

**PRIMARY PROMPT: Executive Summary Generation**

```
Please create an executive summary of this detailed report.

REPORT TITLE: [Title]
REPORT LENGTH: [Pages]
REPORT PURPOSE: [What the report was meant to accomplish]

REPORT CONTENT:
[Paste full report or key sections]

KEY DATA POINTS:
[If extracted separately]

AUDIENCE: [Who will read this summary]
PURPOSE: [What decision or action should result]
PRIOR KNOWLEDGE: [What they already know]
KEY CONCERNS: [What they care most about]

CONSTRAINTS:
- Length: [One page / 500 words / etc.]
- Format: [Requirements]
- Must include: [Requirements]

CREATE:

1. ONE-PAGE EXECUTIVE SUMMARY

   **HEADLINE**
   [One sentence that captures the most important takeaway]

   **SITUATION**
   [2-3 sentences: Context and why this report was needed]

   **KEY FINDINGS**
   [3-5 bullet points, each with a "so what"]
   - Finding: [What the data shows]
     Implication: [Why it matters]

   **CRITICAL INSIGHT**
   [The one thing they must understand—not just data, but meaning]

   **RECOMMENDATION**
   [Clear action recommendation with expected outcome]
   - Action: [What to do]
   - Investment: [What it requires]
   - Expected Return: [What it delivers]

   **RISK IF NO ACTION**
   [What happens if this is ignored]

   **NEXT STEPS**
   [Immediate actions to take]

2. 30-SECOND VERBAL BRIEF
   [What to say if you have 30 seconds]

3. THREE QUESTIONS TO ANTICIPATE
   - Q: [Likely question]
   - A: [Prepared answer]

4. GUIDANCE ON FULL REPORT
   Who should read the full report: [Roles]
   Most important sections: [Sections]
   Skip if pressed for time: [Sections]

Write with confidence. Be direct about conclusions. Make recommendations clear.
```

---

### Step 4: Review and Validate
**Time: 5-10 minutes**

Check:
- Are findings accurately extracted?
- Is the emphasis correct for this audience?
- Do recommendations match the report?
- Is the critical insight truly critical?

---

### Step 5: Customize for Audience
**Time: 5 minutes**

```
Adjust the executive summary for these specifics:

AUDIENCE ADJUSTMENTS:
- They are particularly concerned about: [Topic]
- They may push back on: [Area]
- Don't emphasize: [Topic]
- Do emphasize: [Topic]

ORGANIZATIONAL CONTEXT:
- Related initiative: [What else is happening]
- Sensitive topic: [What to handle carefully]
- Preferred language: [Terms they use]

PRESENTATION CONTEXT:
- This will be presented [in writing / verbally / both]
- Time allotted: [Minutes]
- Follow-up expected: [Yes/No]
```

---

### Step 6: Generate Final Deliverable
**Time: 2 minutes**

```
Finalize the executive summary:

1. FINAL ONE-PAGER
   Polished executive summary ready for distribution

2. EMAIL VERSION
   Body text for email distribution with summary inline

3. SLIDE VERSION
   Content structured for single PowerPoint slide

4. TALKING POINTS
   Bullet points for verbal delivery
```

---

## Example Output

Below is an example executive summary:

---

> **EXECUTIVE SUMMARY**
>
> **Q3 2024 Customer Churn Analysis**
>
> ---
>
> ## Headline
>
> **Churn is accelerating in our SMB segment due to pricing sensitivity, threatening $2.3M in Q4 ARR—but a targeted retention campaign can reverse this trend.**
>
> ---
>
> ## Situation
>
> Q3 churn increased to 4.2%, up from 3.8% in Q2 and 3.5% a year ago. This acceleration warranted a deep analysis to understand drivers and identify intervention opportunities. The analysis reveals a concentrated problem with a clear solution path.
>
> ---
>
> ## Key Findings
>
> **1. SMB segment is driving the churn spike**
> - SMB churn hit 8.1% vs 1.2% for Enterprise
> - *Implication: Enterprise strategy is working; SMB needs different approach*
>
> **2. Price sensitivity has increased 40% year-over-year**
> - 34% of churners cite price as primary reason
> - *Implication: January pricing changes are having delayed impact*
>
> **3. Competitor X is successfully capturing our dissatisfied customers**
> - 28% of churners switched to Competitor X's lower-cost offering
> - *Implication: We're losing the value-conscious segment*
>
> **4. Product engagement predicts retention**
> - Accounts with <3 integrations churn at 3x the rate
> - *Implication: Adoption, not just purchase, determines stickiness*
>
> **5. CSM intervention works**
> - Accounts with CSM touch in past 30 days churn 60% less
> - *Implication: Proactive outreach is high-ROI*
>
> ---
>
> ## Critical Insight
>
> The churn problem is **concentrated and addressable**. It's not that all customers are leaving—it's that SMB customers who don't receive attention and who are price-sensitive are leaving. Our predictive model can identify these accounts with 78% accuracy. This is an execution problem, not a product problem.
>
> ---
>
> ## Recommendation
>
> **Launch a targeted SMB retention campaign in Q4.**
>
> | Element | Detail |
> |---------|--------|
> | **Action** | Deploy CSM outreach to 127 high-risk accounts identified by model |
> | **Investment** | 1 dedicated CSM + $50K discount budget |
> | **Expected Return** | Retain $2.3M ARR (estimated 60-70% save rate) |
> | **Timeline** | Immediate start; run through Q4 |
>
> ---
>
> ## Risk If No Action
>
> Without intervention, the 127 high-risk accounts represent **$2.3M ARR at risk** in Q4. At current save rates without intervention (~20%), we would lose approximately **$1.8M ARR** and continue the trajectory into 2025.
>
> ---
>
> ## Next Steps
>
> 1. **Approve retention campaign budget** (CEO decision - this meeting)
> 2. **Assign dedicated CSM to high-risk accounts** (VP CS - this week)
> 3. **Prepare competitive response strategy** (VP Product - present in 2 weeks)
> 4. **Evaluate SMB pricing tier** (VP Finance - recommendation by month-end)
>
> ---
>
> ## 30-Second Verbal Brief
>
> "Churn increased in Q3, but the problem is concentrated and solvable. Our SMB segment is churning at 8% due to price sensitivity and competitor pressure. The good news: our predictive model identifies at-risk accounts, and CSM intervention reduces churn by 60%. We're recommending an immediate retention campaign targeting 127 high-risk accounts, which could save $2.3M in ARR. I need budget approval today to start this week."
>
> ---
>
> ## Anticipated Questions
>
> **Q: Why didn't we see this coming?**
> A: The segment-level detail wasn't visible in our standard reporting. This analysis was triggered by the Q2 uptick. We're now implementing segment-level churn tracking in our dashboards.
>
> **Q: What about the pricing concern long-term?**
> A: The retention campaign is a near-term fix. We're also recommending a pricing tier review for SMB, which VP Finance will present recommendations on by month-end.
>
> **Q: How confident are we in the $2.3M impact estimate?**
> A: The predictive model is 78% accurate. At a 60-70% save rate (based on historical intervention data), we expect to retain $1.4-1.6M with high confidence, with upside to $2.0M+.
>
> ---
>
> ## Full Report Guidance
>
> **Who should read the full report:**
> - VP Customer Success (required)
> - VP Sales (recommended - competitive intelligence)
> - VP Product (recommended - unmet needs section)
>
> **Most important sections:**
> - Section 5: Root Cause Analysis (6 pages)
> - Section 6: Predictive Model Findings (4 pages)
>
> **Skip if pressed for time:**
> - Section 2: Methodology
> - Section 8: Appendices

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Summary misses key points | Report not fully processed | Ensure critical sections are included in input; highlight key findings explicitly |
| Too much detail | Didn't calibrate to audience | Specify: "Executive level, focus on implications not methodology" |
| Recommendations unclear | Report didn't have clear recs | Ask: "Based on the findings, what should the organization do?" |
| Summary too generic | Losing specificity | Ask: "Include specific numbers, names, and concrete actions" |
| Tone inappropriate | Didn't specify audience | Add: "This is for [CEO/Board/etc.], calibrate tone accordingly" |
| Implications missing | Just restating findings | Ask: "For each finding, answer: So what? Why does this matter?" |

---

## Tips from Experience

1. **Start with the action.** Executives want to know what to do before why to do it.

2. **One headline, one decision.** What is the single most important takeaway?

3. **Numbers create credibility.** "$2.3M at risk" beats "significant revenue exposure."

4. **Anticipate questions.** Prepare for the pushback—it shows confidence.

5. **Make recommendations concrete.** "Improve retention" is useless; "Deploy 1 CSM to 127 accounts" is actionable.

6. **Acknowledge uncertainty.** Saying "we estimate" or "with 78% confidence" builds trust.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Summary is read completely
- [ ] Leaders make decisions based on it
- [ ] Follow-up questions are anticipated
- [ ] Key points are accurately represented
- [ ] Actions are taken on recommendations
- [ ] Time spent on summary creation decreases

**Track over time:**
- Whether summaries lead to decisions
- Executive feedback on clarity
- Time to create summaries
- Whether full reports get read when needed
- Questions during presentation (fewer = better summary)

---

## Variations

### Research Report Summary
For external research or studies:
```
Summarize research report emphasizing:
- Methodology credibility
- Key findings with statistical significance
- Applicability to our situation
- Caveats and limitations
- Actions we should take based on this research

Include: Source credibility assessment
```

### Audit Report Summary
For internal audit findings:
```
Summarize audit report with focus on:
- Risk ratings of findings
- Management action items
- Compliance implications
- Timeline requirements
- Remediation progress

Format: Match internal audit reporting standards
```

### Consultant Deliverable Summary
For external consultant reports:
```
Summarize consultant deliverable:
- Key recommendations
- Implementation requirements
- Cost/benefit of each recommendation
- What we agree/disagree with
- Suggested next steps with consultant

Include: Value assessment of engagement
```

### Competitive Analysis Summary
For competitive intelligence reports:
```
Summarize competitive analysis:
- Key competitor moves
- Our relative position
- Threats to address
- Opportunities to exploit
- Recommended responses

Format: Strategic implications focus
```

### Board Deck Summary
For long board presentations:
```
Create board-ready summary:
- Financial highlights (3 metrics)
- Operational highlights (3 metrics)
- Key risks (top 3)
- Strategic updates (major only)
- Decisions needed from board

Format: Can be read in 2 minutes
```

---

## Building Your Repeatable System

After several summaries, establish:

1. **Summary templates** for recurring report types
2. **Standard formats** by audience level
3. **Question library** for common concerns
4. **Executive preferences** documented
5. **Quality checklist** before distribution

**Sample Setup:**
```
executive-summaries/
├── templates/
│   ├── quarterly-report.md
│   ├── research-summary.md
│   ├── audit-findings.md
│   └── board-briefing.md
├── summaries/
│   ├── 2024-q3-churn-analysis-summary.md
│   ├── 2024-market-research-summary.md
│   └── [individual summaries]
├── full-reports/
│   └── [source reports]
├── reference/
│   ├── executive-preferences.md
│   ├── common-questions.md
│   └── quality-checklist.md
└── examples/
    └── best-practice-summaries/
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**extract essence → add implications → recommend action → enable decision**—applies broadly:

| Role | Application |
|------|-------------|
| **Analysts** | Any detailed analysis needing summary |
| **Consultants** | Client deliverable summaries |
| **Chiefs of Staff** | Leadership briefing preparation |
| **Project Managers** | Status report summaries |
| **Researchers** | Research finding communication |
| **Any professional** | Complex information distillation |

---

## Next Steps

1. **Identify a report:** Pick a detailed report needing a summary
2. **Know your audience:** Who will read it and what do they need?
3. **Gather content:** Extract or paste report content
4. **Generate summary:** Use this recipe
5. **Validate and customize:** Ensure accuracy and appropriate emphasis
6. **Deliver and observe:** Track whether it drives the intended action

---

*Recipe #60 of 100 in the Claude Code Knowledge Worker Recipe Collection*
