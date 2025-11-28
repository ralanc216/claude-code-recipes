# KPI Variance Analysis and Commentary

**Recipe #53: Turn Performance Gaps into Actionable Explanations**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 5 minutes (first time) / 2 minutes (repeat) | 2-3 hours per variance report | Beginner | Finance, Operations, Analysts, Managers |

---

## The Problem

KPIs missed their targets, and everyone's asking "why?" You have the numbers but not the narrative. Leadership wants explanations, not excuses. Finance needs documentation. Operations needs action items. Writing variance commentary is tedious, political, and takes hours—often repeated monthly for the same metrics. Meanwhile, meaningful variances get lost among immaterial fluctuations.

**Pain Points:**
- Hours spent explaining why numbers missed targets
- Same variance explanations written month after month
- Material variances buried among immaterial noise
- No clear framework for what constitutes a good explanation
- Lack of consistent format across departments
- Explanations that describe but don't diagnose
- Missing the "what now?" after the "what happened?"

---

## The Outcome

Clear, structured variance commentary that explains what happened, why it matters, and what to do about it. Analysis that separates signal from noise, prioritizes material variances, and provides actionable recommendations—not just descriptions of what changed.

**What You'll Have When Done:**
- Materiality-filtered variance analysis
- Root cause explanations for each significant variance
- Impact quantification
- Action recommendations
- Management-ready commentary
- Trend context for recurring variances

---

## When to Use This Recipe

**Good Fit:**
- Monthly financial variance reporting
- Operational KPI reviews
- Budget-to-actual analysis
- Quarterly business reviews
- Performance scorecards
- Any metric with targets

**Not a Good Fit:**
- Initial target setting (use forecasting recipes)
- Deep statistical analysis (need specialized tools)
- Real-time monitoring (different cadence)
- Metrics without defined targets

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have actual vs. target data
- [ ] You have prior period comparisons
- [ ] You understand the business context driving variances
- [ ] You know the materiality thresholds
- [ ] You have 30-45 minutes for comprehensive analysis

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Structures variance commentary consistently
- Calculates variance percentages and materiality
- Generates explanation frameworks
- Identifies patterns across periods
- Creates action recommendations
- Formats for different audiences

**Where Human Judgment Is Essential:**
- Validating root cause explanations
- Understanding true business drivers
- Determining appropriate actions
- Political sensitivity in explanations
- Confirming accuracy of context
- Final sign-off

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Actual results | Current period performance | What happened |
| Targets/Budget | Expected performance | What was planned |
| Prior period | Last month/quarter/year | Trend context |
| Materiality | Threshold criteria | What to focus on |
| Context | Known business factors | Why explanations |

**Sample Input:**
```
KPI Variance Analysis Request

PERIOD: November 2024 (Month 11)

KPIS WITH VARIANCES:

Revenue KPIs:
| Metric | Actual | Target | Variance | Var % | Prior Month |
|--------|--------|--------|----------|-------|-------------|
| Total Revenue | $4.2M | $4.5M | -$300K | -6.7% | $4.4M |
| New Business Revenue | $1.1M | $1.3M | -$200K | -15.4% | $1.2M |
| Renewal Revenue | $2.8M | $2.9M | -$100K | -3.4% | $2.9M |
| Expansion Revenue | $0.3M | $0.3M | $0 | 0% | $0.3M |

Operational KPIs:
| Metric | Actual | Target | Variance | Var % | Prior Month |
|--------|--------|--------|----------|-------|-------------|
| Customer Satisfaction | 82% | 85% | -3 pts | -3.5% | 84% |
| First Response Time | 4.2 hrs | 2 hrs | +2.2 hrs | +110% | 2.8 hrs |
| Ticket Resolution | 18 hrs | 12 hrs | +6 hrs | +50% | 14 hrs |
| Employee Utilization | 78% | 75% | +3 pts | +4% | 76% |

Cost KPIs:
| Metric | Actual | Target | Variance | Var % | Prior Month |
|--------|--------|--------|----------|-------|-------------|
| Operating Expenses | $2.1M | $2.0M | +$100K | +5% | $1.9M |
| Customer Acquisition Cost | $2,400 | $2,000 | +$400 | +20% | $2,100 |
| Cost per Ticket | $45 | $35 | +$10 | +28.6% | $38 |

MATERIALITY THRESHOLDS:
- Financial: >5% or >$50K
- Operational: >10% or significant trend

KNOWN BUSINESS CONTEXT:
- Major customer implementation in November (pulled support resources)
- Sales team transition (2 senior reps left, 3 new reps ramping)
- New support ticketing system went live November 1
- Competitor launched aggressive pricing promotion

AUDIENCE: Executive Leadership Team
PURPOSE: Monthly performance review meeting
```

---

## Step-by-Step Implementation

### Step 1: Gather Variance Data
**Time: 5-10 minutes**

Collect:
- Current period actual results
- Target/budget figures
- Prior period comparisons
- Materiality thresholds
- Known business context

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Variance Analysis Prompt
**Time: 5-8 minutes for Claude to process**

---

**PRIMARY PROMPT: KPI Variance Analysis**

```
Please analyze these KPI variances and generate management commentary.

PERIOD: [Period name]

KPI DATA:
[Paste your variance data table]

MATERIALITY THRESHOLDS:
- [Financial thresholds]
- [Operational thresholds]

KNOWN CONTEXT:
[Business factors that may explain variances]

PRIOR PERIOD TRENDS:
[Any relevant historical patterns]

ANALYSIS REQUIREMENTS:

1. EXECUTIVE SUMMARY
   - Overall performance headline
   - Number of KPIs on track vs. off track
   - Most significant positive variance
   - Most significant negative variance
   - Key theme/pattern across variances

2. MATERIALITY ASSESSMENT
   | KPI | Variance | Material? | Priority |
   |-----|----------|-----------|----------|
   [For each KPI]

   Focus remaining analysis on material variances only.

3. VARIANCE COMMENTARY (for each material variance)

   **[KPI Name]**

   Performance: [Actual] vs [Target] ([Variance amount], [%])
   Trend: [vs prior period] [improving/stable/declining]

   What happened:
   [Factual description of the variance]

   Why it happened (root cause analysis):
   - Primary driver: [Main cause with quantified impact if possible]
   - Contributing factors: [Secondary causes]
   - One-time vs recurring: [Assessment]

   Why it matters:
   [Business impact of this variance]

   Recommended action:
   - [Specific action] — [Expected impact]

   Outlook:
   [Expected direction next period]

4. PATTERN ANALYSIS
   Identify any patterns across KPIs:
   - Related variances (common root cause)
   - Leading/lagging indicator relationships
   - Systemic issues vs. isolated events

5. ACTION SUMMARY
   Priority actions based on variance analysis:
   1. [Highest priority action] — Addresses: [KPIs affected]
   2. [Second priority action] — Addresses: [KPIs affected]
   3. [Third priority action] — Addresses: [KPIs affected]

6. WATCHLIST
   Non-material variances to monitor:
   - [KPI] — [Why watching]

7. FORECAST IMPACT
   Based on these variances, implications for:
   - Quarter-end outlook
   - Full-year outlook
   - Any target adjustments to consider

Write commentary that explains, not just describes. Focus on diagnosis and action, not just observation.
```

---

### Step 4: Validate Root Causes
**Time: 10-15 minutes**

Review generated explanations against your knowledge:
- Are the root causes accurate?
- Have any explanations been oversimplified?
- Are there political sensitivities to address?
- Do the actions make sense?

---

### Step 5: Add Business Context
**Time: 5-10 minutes**

Enhance with information only you know:
```
Update the variance commentary with this additional context:

[KPI Name]:
- Additional root cause detail: [What you know]
- Management has already: [Actions taken]
- Sensitivity note: [Political considerations]

[Other updates as needed]
```

---

### Step 6: Generate Final Deliverables
**Time: 5 minutes**

```
Create final deliverable package:

1. EXECUTIVE SUMMARY (one page)
   - Performance headline
   - Top 3 variances requiring attention
   - Recommended actions
   - Outlook

2. DETAILED COMMENTARY
   Full variance analysis as developed

3. DISCUSSION GUIDE
   Talking points for the performance review meeting:
   - What to lead with
   - Questions to anticipate
   - Actions to propose

4. APPENDIX
   - All KPIs with variance status
   - Materiality criteria applied
   - Period-over-period trend data
```

---

## Example Output

Below is an abbreviated variance analysis example:

---

> **KPI VARIANCE ANALYSIS**
>
> **November 2024 | Monthly Performance Review**
>
> ---
>
> ## Executive Summary
>
> November performance was mixed, with revenue 6.7% below target while operational metrics showed strain from a major customer implementation. Of 12 tracked KPIs, 5 are materially off-target requiring attention. The revenue shortfall (-$300K) is primarily driven by new business underperformance (-$200K) tied to sales team transition. Operational metrics reflect temporary resource reallocation, not systemic issues.
>
> **Headline:** Revenue gap is addressable through pipeline acceleration; support metrics are transitional.
>
> ---
>
> ## Materiality Assessment
>
> | KPI | Variance | Material? | Priority |
> |-----|----------|-----------|----------|
> | Total Revenue | -6.7% (-$300K) | Yes | High |
> | New Business Revenue | -15.4% (-$200K) | Yes | High |
> | Renewal Revenue | -3.4% (-$100K) | Borderline | Medium |
> | First Response Time | +110% (+2.2 hrs) | Yes | High |
> | Ticket Resolution | +50% (+6 hrs) | Yes | Medium |
> | Customer Acquisition Cost | +20% (+$400) | Yes | Medium |
> | Customer Satisfaction | -3.5% (-3 pts) | Borderline | Watch |
> | Operating Expenses | +5% (+$100K) | Borderline | Watch |
>
> ---
>
> ## Variance Commentary
>
> ### Total Revenue
>
> **Performance:** $4.2M vs $4.5M target (-$300K, -6.7%)
> **Trend:** Down from $4.4M prior month (declining)
>
> **What happened:**
> November revenue fell $300K short of target, marking the second consecutive month below plan. The gap widened from $100K in October to $300K in November.
>
> **Why it happened:**
> - **Primary driver:** New business underperformance (-$200K) due to sales team transition. Two senior reps (combined historical production: $180K/month) departed mid-October. Three replacement reps are in ramp period with minimal production expected until January.
> - **Contributing factor:** Renewal shortfall (-$100K) from one delayed contract (expected to close December)
> - **One-time vs recurring:** Mixed. Sales ramp is temporary (3-4 months); competitive pressure may be ongoing.
>
> **Why it matters:**
> November gap puts Q4 target at risk. Current trajectory suggests Q4 revenue of $12.8M vs $13.5M target (-5%). Pipeline coverage for December is 2.8x, below the 3.5x typically needed for target attainment.
>
> **Recommended action:**
> - Accelerate new rep ramp with additional deal support from managers
> - Pull forward Q1 pipeline opportunities where possible
> - Deploy senior reps on largest December opportunities
>
> **Outlook:** December improvement expected as delayed renewal closes and pipeline matures, but target attainment unlikely without extraordinary effort.
>
> ---
>
> ### First Response Time
>
> **Performance:** 4.2 hours vs 2 hour target (+2.2 hours, +110%)
> **Trend:** Up from 2.8 hours prior month (significant decline)
>
> **What happened:**
> First response time more than doubled from target, with November showing the worst performance in 12 months.
>
> **Why it happened:**
> - **Primary driver:** Major customer implementation (Acme Corp) consumed 60% of Tier 2 support capacity for 3 weeks. Normal staffing was insufficient for both implementation support and queue management.
> - **Contributing factor:** New ticketing system went live November 1, causing learning curve delays (~0.5 hrs added per ticket initially)
> - **One-time vs recurring:** Primarily one-time. Implementation completes December 15; ticketing system efficiency improving weekly.
>
> **Why it matters:**
> Customer satisfaction (82% vs 85% target) is directly correlated with response time. Each hour of response delay historically correlates with 1.5 point CSAT decline. Extended poor performance risks churn in affected accounts.
>
> **Recommended action:**
> - Temporarily contract 2 additional support resources through December
> - Implement priority queue for accounts not involved in Acme implementation
> - Accelerate ticketing system training for remaining team members
>
> **Outlook:** Expect improvement in December as implementation winds down. Target of 2.5 hours realistic for December; full recovery to 2 hours in January.
>
> ---
>
> ### Customer Acquisition Cost
>
> **Performance:** $2,400 vs $2,000 target (+$400, +20%)
> **Trend:** Up from $2,100 prior month (increasing)
>
> **What happened:**
> CAC exceeded target for third consecutive month, with November showing highest CAC of the year.
>
> **Why it happened:**
> - **Primary driver:** Reduced new customer volume (23 vs 28 target) while marketing spend held constant. Fixed costs spread over fewer acquisitions.
> - **Contributing factor:** Competitor pricing promotion required additional sales effort (more touches, longer cycles) per won deal
> - **One-time vs recurring:** Concerning trend. If competitor promotion continues, elevated CAC may persist.
>
> **Why it matters:**
> At current CAC ($2,400) and average contract value ($8,500), payback period extends to 3.4 months (vs 2.8 month target). Unit economics remain positive but margin pressure increases.
>
> **Recommended action:**
> - Review marketing channel mix; shift spend to highest-efficiency channels
> - Analyze competitor promotion impact on win rates by segment
> - Consider targeted counter-promotion for high-value segments
>
> **Outlook:** CAC likely to remain elevated while competitor promotion active. Recommend planning for $2,200 CAC in December.
>
> ---
>
> ## Pattern Analysis
>
> **Interconnected Variances:**
> Several variances share common drivers:
>
> 1. **Sales Transition Impact:** New business revenue, CAC, and total revenue all affected by rep departures and ramp time. These are operationally connected and will improve together.
>
> 2. **Resource Constraint Impact:** First response time, ticket resolution, cost per ticket, and customer satisfaction all affected by the Acme implementation resource draw. These are temporary and interdependent.
>
> **Leading Indicator Alert:**
> Customer satisfaction (82%) is a leading indicator for renewal and expansion revenue. November's decline, if it continues, will impact Q1 revenue metrics.
>
> ---
>
> ## Action Summary
>
> | Priority | Action | Addresses | Owner | Timeline |
> |----------|--------|-----------|-------|----------|
> | 1 | Accelerate new rep ramp | Revenue, CAC | Sales VP | Immediate |
> | 2 | Add temporary support resources | Response time, CSAT | Support Dir | This week |
> | 3 | Review marketing channel efficiency | CAC | Marketing VP | Next 2 weeks |
>
> ---
>
> ## Watchlist
>
> Non-material but monitoring:
> - **Operating Expenses (+5%):** Currently within tolerance but third consecutive increase. Review in December for pattern.
> - **Renewal Revenue (-3.4%):** Just below materiality threshold. One delayed contract explains it; watching for any pattern.
>
> ---
>
> ## Forecast Impact
>
> Based on November variances:
>
> **Q4 Outlook:**
> - Revenue: Likely $12.6-12.9M vs $13.5M target (93-96%)
> - Risk: Downside if December pipeline doesn't convert
> - Upside: Recovery if delayed renewal closes and reps accelerate ramp
>
> **Full Year:**
> - Currently tracking to 97% of annual target
> - Q4 variance unlikely to change full-year materially
>
> **Target Adjustment:**
> - No recommendation to adjust targets
> - Variances explained by identifiable factors
> - Underlying business health intact

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Generic explanations | Insufficient context | Add: "The specific business factors affecting [KPI] are: [details]" |
| All variances seem equal | No prioritization | Specify: "Apply materiality thresholds: [X%] or [$X] minimum" |
| Descriptions not diagnoses | Surface-level analysis | Ask: "For each variance, answer: Why did this happen? What's the root cause?" |
| No actionable recommendations | Missing action focus | Add: "For each material variance, provide specific recommended actions with expected impact" |
| Overly optimistic/pessimistic | Tone miscalibration | Specify: "Be balanced. Acknowledge both positives and concerns honestly" |
| Missing trends | Point-in-time only | Add: "Include trend analysis: Is this improving, stable, or declining over past 3 periods?" |

---

## Tips from Experience

1. **Focus on the vital few.** Five material variances analyzed well beats twenty superficial explanations.

2. **Distinguish one-time from recurring.** This affects the response urgency and type of action needed.

3. **Connect the dots.** Often multiple variances share a root cause—highlight these connections.

4. **Lead with the "so what."** Don't bury the implication. State why the variance matters up front.

5. **Be honest about uncertainty.** If you don't know the root cause, say so and propose investigation.

6. **Recommend, don't just report.** Every material variance should have a suggested action.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Variance reports are completed faster
- [ ] Management accepts explanations as credible
- [ ] Actions are taken based on analysis
- [ ] Root causes are validated as accurate
- [ ] Patterns are identified proactively
- [ ] Recurring variances decrease over time

**Track over time:**
- Time to complete variance analysis
- Acceptance rate of explanations
- Actions implemented from recommendations
- Forecast accuracy improvement
- Reduction in repeat variance explanations

---

## Variations

### Financial Variance Analysis
For budget-to-actual reporting:
```
Analyze financial variances with emphasis on:
- Dollar and percentage variance
- Controllable vs. non-controllable factors
- Timing differences vs. run-rate changes
- Impact on cash flow and profitability
- Reforecast implications

Format for finance committee review.
Include journal entry implications if needed.
```

### Operational Variance Deep-Dive
For operations-focused analysis:
```
Analyze operational KPI variances with emphasis on:
- Process breakdowns causing variance
- Resource utilization impact
- Quality/speed tradeoffs
- Customer experience implications
- Specific process improvement recommendations

Include: Root cause diagrams, correlation analysis, leading indicators
```

### Sales Performance Variance
For sales metrics:
```
Analyze sales KPI variances including:
- Pipeline stage conversion analysis
- Rep-level performance variance
- Product/segment mix impact
- Competitive win/loss impact
- Territory/region patterns

Focus on: What's different about top performers? Where are deals stalling?
```

### Project Portfolio Variance
For project-based metrics:
```
Analyze project KPI variances:
- Schedule variance (SV)
- Cost variance (CV)
- Scope changes impact
- Resource utilization variance
- Quality metrics deviation

Use EVM methodology where applicable.
```

---

## Building Your Repeatable System

After several variance cycles, optimize:

1. **Create variance templates** for each KPI category
2. **Build a root cause library** of common explanations
3. **Establish standard language** for recurring patterns
4. **Track variance history** for trend analysis
5. **Document actions taken** to measure effectiveness

**Sample Setup:**
```
variance-analysis/
├── templates/
│   ├── revenue-variance.md
│   ├── operational-variance.md
│   ├── cost-variance.md
│   └── project-variance.md
├── monthly/
│   ├── 2024-11-variance-report.md
│   ├── 2024-10-variance-report.md
│   └── [month by month]
├── reference/
│   ├── materiality-thresholds.md
│   ├── root-cause-library.md
│   └── action-tracking.md
└── kpi-definitions/
    ├── revenue-kpis.md
    ├── operational-kpis.md
    └── financial-kpis.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**compare to target → assess materiality → explain root cause → recommend action**—applies broadly:

| Role | Application |
|------|-------------|
| **Finance** | Budget variance, forecast accuracy, cost analysis |
| **Operations** | SLA performance, efficiency metrics, quality KPIs |
| **Sales** | Pipeline, conversion, quota attainment |
| **Marketing** | Campaign performance, CAC, conversion metrics |
| **HR** | Headcount, turnover, engagement scores |
| **Project Management** | Schedule, budget, scope variance |

---

## Next Steps

1. **Gather your KPI data:** Actual vs. target, plus prior period
2. **Define materiality:** What variance level requires explanation?
3. **Document known context:** Business factors affecting performance
4. **Generate analysis:** Use this recipe
5. **Validate root causes:** Confirm explanations match reality
6. **Present and act:** Share with stakeholders, track actions

---

*Recipe #53 of 100 in the Claude Code Knowledge Worker Recipe Collection*
