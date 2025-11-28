# Dashboard Narrative Generation

**Recipe #51: From Charts to Stories That Drive Action**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 5 minutes (first time) / 2 minutes (repeat) | 1-2 hours per report | Beginner | Analysts, Managers, Executives |

---

## The Problem

Dashboards show data but don't explain it. Executives stare at charts asking "so what?" Analysts spend hours writing commentary that nobody reads. Numbers without narrative fail to drive action. Every stakeholder interprets the same dashboard differently, leading to misaligned decisions. The data is there, but the insight is missing.

**Pain Points:**
- Charts without context or explanation
- "So what?" questions after every dashboard share
- Hours spent writing commentary nobody reads
- Different interpretations of the same data
- Numbers that don't drive action
- Insights buried in data complexity
- Recurring reports with recurring writing burden

---

## The Outcome

Clear, compelling narratives that transform dashboard data into actionable insights. Commentary that explains what the numbers mean, why they matter, and what to do about them. Stories that different audiences can understand and act on.

**What You'll Have When Done:**
- Executive summary of key findings
- Narrative explanations for each metric
- Trend analysis in plain language
- Action recommendations
- Talking points for presentations
- Audience-appropriate versions

---

## When to Use This Recipe

**Good Fit:**
- Weekly/monthly dashboard reviews
- Executive briefings on metrics
- Board and investor updates
- Team performance summaries
- Campaign performance reports
- Operational dashboards
- Any data presentation

**Not a Good Fit:**
- Deep technical analysis (need different approach)
- Exploratory data analysis (still discovering)
- Raw data validation (not ready for narrative)
- Data without context to interpret

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have dashboard data or screenshots
- [ ] You know the target audience
- [ ] You understand the business context
- [ ] You have 15-30 minutes for narrative development

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Translates numbers into plain language
- Identifies patterns and anomalies
- Generates explanatory narratives
- Creates action recommendations
- Adapts tone for different audiences
- Structures insights logically

**Where Human Judgment Is Essential:**
- Data accuracy verification
- Business context addition
- Causal explanations
- Sensitive interpretation
- Action prioritization
- Final approval

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Dashboard data | Numbers, metrics, KPIs | Core narrative content |
| Context | Business situation | Interpretation framework |
| Targets | Goals and benchmarks | Performance assessment |
| History | Previous periods | Trend analysis |
| Audience | Who will read this | Tone calibration |

**Sample Input:**
```
Dashboard Narrative Request

DASHBOARD: Monthly Sales Performance (November 2024)

DATA:
Revenue:
- Current month: $2.4M
- Prior month: $2.1M (+14%)
- Same month last year: $2.0M (+20%)
- Target: $2.5M (96% to target)

Pipeline:
- Total pipeline: $8.2M
- Qualified pipeline: $5.4M
- Win rate MTD: 28% (down from 32% last month)

New Business:
- New customers: 23 (target: 20)
- Average deal size: $45K (down from $52K)
- Sales cycle: 45 days (up from 38 days)

Team Performance:
- Top performer: Sarah Chen ($520K)
- Reps at quota: 7 of 12 (58%)
- Reps below 50%: 3 of 12

Activity Metrics:
- Demos: 145 (up 20%)
- Proposals: 68 (up 15%)
- Close rate on proposals: 34% (down from 42%)

CONTEXT:
- Q4 push in progress
- New product launched October 1
- Two new reps started in September
- Major competitor launched pricing promotion

AUDIENCE: Sales Leadership Team (weekly review)

WHAT THEY CARE ABOUT:
- Are we going to hit the quarter?
- What's working and what isn't?
- Where should we focus?
```

---

## Step-by-Step Implementation

### Step 1: Gather Dashboard Data
**Time: 5-10 minutes**

Collect:
- Current period numbers
- Comparison periods (prior period, prior year)
- Targets and benchmarks
- Context (what's happening in the business)

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Narrative Generation Prompt
**Time: 3-5 minutes for Claude to process**

---

**PRIMARY PROMPT: Dashboard Narrative Generation**

```
Please generate a narrative analysis of this dashboard data.

DASHBOARD: [Dashboard name and period]

DATA:
[Paste your metrics, organized by category]

CONTEXT:
[Business situation, recent events, known factors]

COMPARISON BENCHMARKS:
- Prior period: [Data]
- Same period last year: [Data]
- Targets: [Data]

AUDIENCE: [Who will read this]
THEIR KEY QUESTIONS: [What they want to know]

PLEASE CREATE:

1. EXECUTIVE SUMMARY (3-4 sentences)
   - The headline: What's the most important takeaway?
   - The trend: Are things getting better or worse?
   - The implication: What does this mean?
   - The action: What should we do?

2. KEY METRICS NARRATIVE

   For each major metric area:

   **[Metric Category]**
   - The numbers: [State the key figures]
   - The context: [Compare to targets, history]
   - The story: [What's driving this?]
   - The implication: [Why it matters]

3. BRIGHT SPOTS
   What's working well:
   - [Positive finding 1] — [Why it matters]
   - [Positive finding 2] — [Why it matters]

4. AREAS OF CONCERN
   What needs attention:
   - [Concern 1] — [Why it matters] — [Suggested action]
   - [Concern 2] — [Why it matters] — [Suggested action]

5. TREND ANALYSIS
   What the patterns tell us:
   - Short-term trends (this period)
   - Medium-term trends (quarter/year)
   - What's changing vs. what's stable

6. RECOMMENDED ACTIONS
   Based on this data:
   1. [Action 1] — [Why] — [Expected impact]
   2. [Action 2] — [Why] — [Expected impact]
   3. [Action 3] — [Why] — [Expected impact]

7. QUESTIONS TO INVESTIGATE
   Data raises these questions:
   - [Question 1]
   - [Question 2]

8. TALKING POINTS
   If presenting this dashboard:
   - Lead with: [Opening statement]
   - Emphasize: [Key points]
   - Anticipate questions about: [Topics]

Write in clear, confident language. State what the data shows, not just what the data is.
```

---

### Step 4: Add Business Context
**Time: 5-10 minutes**

Review the narrative and add:
- Explanations only you know
- Causal factors not in the data
- Nuance about what's really happening
- Corrections if interpretation is off

---

### Step 5: Adapt for Audience
**Time: 5 minutes**

**For executives:**
```
Shorten this to a one-minute read. Lead with implications and actions. Remove details that don't affect decisions.
```

**For operational teams:**
```
Add more detail on the specific drivers. What exactly is causing these numbers? What should the team do differently?
```

**For board/investors:**
```
Make this more strategic. Focus on trajectory, market position, and long-term implications. Less operational detail.
```

---

### Step 6: Create Final Deliverables
**Time: 5 minutes**

```
Create the final narrative package:

1. DASHBOARD SUMMARY
   Complete narrative as developed

2. ONE-SLIDE VERSION
   Key points for a single presentation slide:
   - Headline
   - 3 key metrics
   - 2 insights
   - 1 action

3. EMAIL VERSION
   Narrative formatted for email distribution

4. VERBAL BRIEFING
   30-second version for quick verbal update
```

---

## Example Output

Below is an abbreviated dashboard narrative example:

---

> **SALES PERFORMANCE NARRATIVE**
>
> **November 2024 | Weekly Leadership Review**
>
> ---
>
> ## Executive Summary
>
> November is tracking strong on volume but showing margin compression. We hit 96% of revenue target with 20% YoY growth, but deal sizes are shrinking and win rates are declining. The new product is driving activity—demos up 20%—but we're not converting at historical rates. **Recommendation:** Focus the final weeks on deal velocity and conversion, not just pipeline generation.
>
> ---
>
> ## Key Metrics Narrative
>
> ### Revenue
>
> **$2.4M | 96% to target | +20% YoY**
>
> We're close but not there yet. The 14% month-over-month growth shows strong momentum, and we're well ahead of last November. However, we're below target for the first time since July. The gap is explainable—two large deals pushed to December—but it means we need a strong close to hit Q4.
>
> *Bottom line: Good but not safe. December needs to be exceptional.*
>
> ---
>
> ### Pipeline Health
>
> **$8.2M total | $5.4M qualified | 28% win rate**
>
> Pipeline quantity looks healthy, but quality is concerning. Win rate dropped from 32% to 28%—that's 12% lower conversion on a larger pipeline. If this rate holds, we're looking at $1.5M in closes from current qualified pipeline, which puts Q4 at risk.
>
> The question is: Is this a quality problem (wrong deals in pipeline) or a conversion problem (right deals, poor execution)?
>
> *Bottom line: More pipeline isn't the answer. Better conversion is.*
>
> ---
>
> ### New Business
>
> **23 new customers | $45K average deal size**
>
> We're winning more customers but smaller ones. 23 new logos beats our target of 20—that's great for land-and-expand strategy. But average deal size dropped from $52K to $45K (13% decline). This could be:
> - New product attracting smaller buyers
> - Reps discounting to hit unit targets
> - Competitor pricing pressure affecting deals
>
> Sales cycle extending to 45 days (from 38) suggests deals are getting harder to close, not easier.
>
> *Bottom line: Investigate deal size decline. Is this strategic (land smaller) or problematic (discounting)?*
>
> ---
>
> ### Team Performance
>
> **58% of reps at quota | 3 reps below 50%**
>
> Sarah Chen continues to outperform ($520K, 108% to target). But the distribution is concerning: 7 reps are hitting quota while 3 are seriously struggling. The new September hires aren't on the board yet—expected, but we need to accelerate their ramp.
>
> *Bottom line: Identify what Sarah is doing differently. Three struggling reps need intervention now, not January.*
>
> ---
>
> ## Bright Spots
>
> ✅ **Demo volume up 20%** — New product is generating interest. This is leading indicator for Q1.
>
> ✅ **New customer count exceeds target** — We're expanding the customer base even with pricing pressure.
>
> ✅ **YoY growth at 20%** — Underlying business health is strong despite competitive pressure.
>
> ---
>
> ## Areas of Concern
>
> ⚠️ **Win rate declining** (28% vs. 32%)
> - Why it matters: Same pipeline yields 12% less revenue
> - Suggested action: Pipeline quality review; identify stuck deals
>
> ⚠️ **Deal size shrinking** ($45K vs. $52K)
> - Why it matters: Need more deals to hit same revenue; margin pressure
> - Suggested action: Review recent closed deals; identify discounting patterns
>
> ⚠️ **Proposal close rate down** (34% vs. 42%)
> - Why it matters: We're losing deals at the finish line
> - Suggested action: Win/loss analysis on recent losses; competitor intel
>
> ---
>
> ## Recommended Actions
>
> 1. **Focus on deal velocity, not pipeline volume**
>    - Why: We have enough pipeline; we need to close it
>    - Action: Daily deal reviews on everything closing in December
>    - Expected impact: 3-5% improvement in close rate = ~$150K
>
> 2. **Investigate deal size decline**
>    - Why: 13% smaller deals significantly impacts revenue attainment
>    - Action: Review last 20 closed deals; identify discounting patterns
>    - Expected impact: Reverse trend or confirm it's strategic
>
> 3. **Intervention for struggling reps**
>    - Why: 3 reps below 50% won't self-correct
>    - Action: Ride-along, deal review, coaching plan before year-end
>    - Expected impact: Even 1 rep improving adds $50-100K
>
> ---
>
> ## Questions to Investigate
>
> - Why did close rate on proposals drop 8 points? What changed?
> - Is the competitor promotion actually affecting us, or is it something else?
> - What's different about Sarah's deals vs. the team average?
>
> ---
>
> ## Talking Points for Review Meeting
>
> **Lead with:** "We're tracking to a strong November but Q4 is not yet secure. The key question isn't whether we're generating enough activity—we are. It's whether we're converting well enough."
>
> **Emphasize:**
> - Volume metrics are healthy; conversion metrics are concerning
> - This is about execution, not effort
> - Three specific actions for the next two weeks
>
> **Anticipate questions about:**
> - Why deal sizes are shrinking
> - What's causing the win rate decline
> - Specific plans for struggling reps

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Narrative states obvious | Just restating numbers | Ask: "Don't tell me the numbers—tell me what they MEAN and why it matters" |
| Missing context | Data without explanation | Add: "Here's the business context: [situation]. Interpret data with this in mind" |
| Too long | Over-detailed | Ask: "Prioritize. What are the 3 things an executive must know?" |
| Wrong tone | Audience mismatch | Specify: "This is for [audience]. Adjust tone and detail level accordingly" |
| No clear action | Insight without recommendation | Ask: "For each finding, add: What should we DO about this?" |
| Causal confusion | Correlation stated as causation | Ask: "Be careful about causation. What do we KNOW vs. what do we SUSPECT?" |

---

## Tips from Experience

1. **Lead with the "so what."** Don't build up to the insight—start with it, then support.

2. **Compare to make numbers meaningful.** "$2.4M" means nothing. "$2.4M vs. $2.5M target" tells a story.

3. **Separate observation from interpretation.** State what the data shows, then what you think it means.

4. **Always end with action.** Insight without recommended action is academic.

5. **Know your audience's questions.** Answer what they'll ask, not what's interesting to you.

6. **Use consistent format.** Readers learn where to look. Same structure every time.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Narratives are read and referenced
- [ ] "So what?" questions decrease
- [ ] Dashboards drive aligned action
- [ ] Stakeholders understand the data
- [ ] Writing time decreases
- [ ] Decision quality improves

**Track over time:**
- Time to create dashboard narratives
- Stakeholder feedback on clarity
- Questions during presentations
- Actions taken based on insights
- Decision alignment across team

---

## Variations

### Board/Investor Dashboard
For external stakeholders:
```
Generate narrative for board-level dashboard.

Focus on:
- Strategic implications
- Market position context
- Long-term trajectory
- Risk identification
- Capital allocation implications

Tone: Confident, strategic, forward-looking
Avoid: Operational minutiae, excuses
```

### Operational Dashboard
For operations teams:
```
Generate narrative for operational dashboard.

Focus on:
- Specific drivers of each metric
- What to do TODAY
- Resource allocation
- Process improvements
- Individual/team performance

Tone: Direct, actionable, specific
Include: Who should do what by when
```

### Campaign Performance
For marketing/sales campaigns:
```
Generate narrative for campaign dashboard.

Focus on:
- Performance vs. goals
- What's working, what's not
- Optimization opportunities
- Budget implications
- Next steps

Include: A/B test results, channel comparison, recommendations for remaining budget
```

### Weekly Team Update
For recurring team reviews:
```
Generate narrative for weekly team dashboard.

Focus on:
- Week-over-week changes
- Progress against goals
- Issues needing attention
- Wins to celebrate
- Focus for next week

Tone: Motivating but honest
Length: 5-minute read maximum
```

---

## Building Your Repeatable System

After several narratives, build your system:

1. **Create narrative templates** for each recurring dashboard
2. **Establish standard comparisons** (vs. target, vs. prior, vs. last year)
3. **Build context library** (what affects each metric)
4. **Track what questions arise** to anticipate in future narratives
5. **Iterate on format** based on feedback

**Sample Setup:**
```
dashboard-narratives/
├── templates/
│   ├── sales-dashboard.md
│   ├── marketing-dashboard.md
│   ├── operations-dashboard.md
│   └── executive-dashboard.md
├── recurring/
│   ├── weekly-sales/
│   │   ├── 2024-11-15.md
│   │   ├── 2024-11-22.md
│   │   └── [week by week]
│   └── monthly-executive/
│       └── [month by month]
├── context/
│   ├── metric-definitions.md
│   ├── known-drivers.md
│   └── common-questions.md
└── reference/
    ├── audience-profiles.md
    └── style-guide.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**take data → add context → explain meaning → recommend action**—applies broadly:

| Role | Application |
|------|-------------|
| **Analysts** | All reporting and presentations |
| **Finance** | Financial performance commentary |
| **Sales** | Pipeline and performance reviews |
| **Marketing** | Campaign and channel reporting |
| **Operations** | Operational metrics communication |
| **Any** | Any data that needs explanation |

---

## Next Steps

1. **Gather dashboard data:** Export or capture current metrics
2. **Add context:** What's happening in the business?
3. **Generate narrative:** Use this recipe
4. **Review and refine:** Add your knowledge and judgment
5. **Distribute and discuss:** Share with stakeholders
6. **Track actions:** Did the narrative drive decisions?

---

*Recipe #51 of 100 in the Claude Code Knowledge Worker Recipe Collection*
