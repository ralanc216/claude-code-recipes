# Financial Analysis and Trend Interpretation

**Recipe #25: From Numbers to Narrative**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 10 minutes (first time) / 5 minutes (repeat) | 2-4 hours per analysis | Intermediate | Finance Teams, FP&A, Executives, Analysts |

---

## The Problem

You have financial data—P&L, balance sheet, cash flow, operating metrics—but turning numbers into insight takes time. Executives don't want to see a spreadsheet; they want to understand what's happening, why, and what it means. Variance analysis is tedious. Trend identification requires careful review. And every month, you start from scratch explaining the same patterns in different words.

**Pain Points:**
- Numbers without narrative don't drive action
- Variance analysis is repetitive and time-consuming
- Hard to identify what matters in dense financial data
- Executives want "so what?" not just "what"
- Monthly reporting feels like reinventing the wheel
- Connecting financial results to operational drivers

---

## The Outcome

Financial analysis that tells a story—clear interpretation of what happened, why it happened, and what to do about it. Variance explanations that executives understand, trend identification that surfaces what matters, and forward-looking implications that inform decisions.

**What You'll Have When Done:**
- Financial performance narrative
- Variance analysis with explanations
- Trend identification and interpretation
- Key metrics dashboard with commentary
- Forward-looking implications
- Executive-ready financial summary

---

## When to Use This Recipe

**Good Fit:**
- Monthly/quarterly financial close analysis
- Board financial reporting
- Variance analysis and explanation
- Business unit financial reviews
- Financial trend analysis
- Budget vs. actual reporting

**Not a Good Fit:**
- Detailed accounting work (need accuracy, not narrative)
- Tax preparation (specialized requirements)
- Audit documentation (specific format requirements)
- Real-time financial monitoring (too slow)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have financial data exported (Excel, CSV)
- [ ] You know the comparison periods (vs. budget, vs. prior year, etc.)
- [ ] You understand the business context
- [ ] You have 1-2 hours for analysis

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Calculates variances and trends
- Identifies significant changes
- Generates narrative explanations
- Creates executive summaries
- Highlights areas needing attention
- Produces consistent reporting formats

**Where Human Judgment Is Essential:**
- Validating calculations (spot-check)
- Understanding true causes of variances
- Political and organizational context
- Knowing what's actionable
- Forward-looking assumptions
- Final approval of financial statements

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Income statement | P&L by period | Performance analysis |
| Balance sheet | Assets, liabilities | Position analysis |
| Comparison data | Budget, prior year | Variance analysis |
| Operating metrics | KPIs, drivers | Connecting numbers to operations |
| Business context | What happened this period | Explaining variances |

**Sample Input:**
```
Monthly Financial Review: October 2024

INCOME STATEMENT (000s)
                    Oct Actual  Oct Budget  Oct Prior Yr   YTD Actual  YTD Budget
Revenue               $4,250      $4,500      $3,900        $42,100    $44,000
COGS                  $1,785      $1,800      $1,560        $17,680    $17,600
Gross Profit          $2,465      $2,700      $2,340        $24,420    $26,400
Gross Margin           58.0%       60.0%       60.0%          58.0%      60.0%

Operating Expenses:
Sales & Marketing       $850        $900        $720         $8,400     $8,800
R&D                     $620        $600        $540         $6,100     $6,000
G&A                     $380        $400        $350         $3,850     $4,000
Total OpEx            $1,850      $1,900      $1,610        $18,350    $18,800

Operating Income        $615        $800        $730         $6,070     $7,600
Operating Margin       14.5%       17.8%       18.7%         14.4%      17.3%

KEY METRICS:
- New customers: 45 (budget: 55, prior year: 38)
- Churn rate: 2.8% (budget: 2.0%, prior year: 1.9%)
- Average deal size: $32K (budget: $30K, prior year: $28K)
- Sales headcount: 18 (budget: 20)
- Support tickets: 890 (budget: 750, prior year: 620)

CONTEXT:
- Sales team was 2 heads short all month (hiring delays)
- Major customer (Acme Corp) churned mid-month ($45K ARR)
- Launched new product tier which is cannibalizing gross margin
- R&D overspend due to contractor for security audit
```

---

## Step-by-Step Implementation

### Step 1: Prepare Your Data
**Time: 10-15 minutes**

Export and organize:
- Financial statements (P&L, balance sheet)
- Comparison periods (budget, prior year)
- Key operating metrics
- Business context (what happened this period)

Clean data formatting—Claude works better with clear structure.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
cd ~/Documents/finance
claude
```

---

### Step 3: Run the Financial Analysis Prompt
**Time: 5-7 minutes for Claude to process**

---

**PRIMARY PROMPT: Financial Analysis and Interpretation**

```
Please analyze these financial results and provide executive-ready interpretation.

FINANCIAL DATA:
"""
[PASTE YOUR FINANCIAL DATA - P&L, BALANCE SHEET, METRICS]
"""

COMPARISON PERIODS:
- Primary comparison: [vs. Budget / vs. Prior Year / vs. Forecast]
- Secondary comparison: [if any]

BUSINESS CONTEXT:
"""
[PASTE KNOWN EVENTS AND CONTEXT THAT AFFECTED RESULTS]
"""

COMPANY CONTEXT:
- Company/Business Unit: [Name]
- Industry: [Industry]
- Key priorities: [What leadership cares about]
- Reporting period: [Month/Quarter]

PLEASE PROVIDE:

1. EXECUTIVE SUMMARY
   - 2-3 paragraph narrative of financial performance
   - Key takeaways (what you need to know)
   - Overall assessment (on track / concerning / strong)

2. VARIANCE ANALYSIS
   | Line Item | Actual | Budget | Variance $ | Variance % | Explanation |

   For each significant variance (>5% or >$X):
   - What happened
   - Why it happened
   - One-time vs. recurring
   - Controllable vs. uncontrollable

3. TREND ANALYSIS
   - Revenue trend (with interpretation)
   - Margin trends (with interpretation)
   - Expense trends (with interpretation)
   - Key ratio trends

4. KEY METRICS COMMENTARY
   | Metric | Actual | Target | Status | Commentary |

   For each metric:
   - Performance vs. target
   - Trend direction
   - Implication for financials

5. AREAS OF CONCERN
   - Issues requiring attention
   - Severity assessment
   - Recommended actions

6. POSITIVE HIGHLIGHTS
   - Where we exceeded expectations
   - What's working
   - How to build on success

7. FORWARD IMPLICATIONS
   - What this means for full-year forecast
   - Risks to watch
   - Opportunities identified
   - Recommended forecast adjustments

8. DASHBOARD COMMENTARY
   For a one-page financial dashboard, provide:
   - Headline (1 sentence)
   - Key metrics with RAG status
   - Top 3 focus areas

9. QUESTIONS FOR LEADERSHIP
   - What you'd want to discuss
   - Areas needing decisions
   - Information gaps

10. MONTH-END NARRATIVE
    Ready-to-use paragraph for monthly business review.
```

---

### Step 4: Review and Validate
**Time: 15-20 minutes**

Check the analysis:

**Verify calculations:**
- Spot-check variance calculations
- Verify percentage calculations
- Check trend directions

**Validate interpretations:**
- Are explanations accurate?
- Any variances misinterpreted?
- Missing context Claude couldn't know?

**Check completeness:**
- All significant variances addressed?
- Key metrics covered?
- Forward implications reasonable?

---

### Step 5: Refine Analysis
**Time: 10-15 minutes**

**To add missing context:**
```
The R&D overspend actually relates to a one-time security audit that won't recur. Adjust the analysis and forward implications accordingly.
```

**To dig deeper on an area:**
```
Go deeper on the gross margin decline. What are all possible causes? What additional data would help us understand this better?
```

**To improve the narrative:**
```
The executive summary is too financial. Rewrite it to connect financial results to business outcomes in language a non-finance executive would understand.
```

**To add forecasting:**
```
Based on October results and YTD trends, provide a revised full-year forecast with high/medium/low scenarios and key assumptions.
```

---

### Step 6: Create Final Deliverables
**Time: 10 minutes**

```
Create these outputs:

1. EXECUTIVE FINANCIAL SUMMARY (1 page)
   - Key metrics dashboard
   - Narrative summary
   - Areas of focus

2. VARIANCE MEMO
   - Detailed variance analysis
   - Explanations for leadership

3. PRESENTATION SLIDES (5-7 slides)
   - Financial performance summary
   - Key trends and insights
   - Forward outlook
   - Discussion items

4. BOARD FINANCE SECTION
   - Board-appropriate summary
   - Key data points
   - Management commentary
```

---

## Example Output

Below is an abbreviated financial analysis example:

---

> **FINANCIAL ANALYSIS: October 2024**
>
> ---
>
> **EXECUTIVE SUMMARY**
>
> October financial results reflect the impact of sales capacity constraints and elevated churn, resulting in revenue 6% below budget ($4.25M actual vs. $4.50M budget). Operating income was $185K unfavorable primarily due to the revenue shortfall, partially offset by lower sales & marketing spend from open headcount.
>
> The month's performance is consistent with YTD trends showing persistent pressure on both the top line (revenue 4% below plan) and gross margin (200bps below target). However, operational expenses remain controlled, and the business fundamentals—average deal size and customer quality—remain strong.
>
> **Assessment: ⚠️ Concerning but not critical.** The revenue and margin gaps are manageable, but the churn increase (2.8% vs. 2.0% target) requires immediate attention as it represents a potential trend rather than a one-time issue.
>
> ---
>
> **VARIANCE ANALYSIS: Significant Items**
>
> | Line Item | Actual | Budget | Var $ | Var % | Explanation |
> |-----------|--------|--------|-------|-------|-------------|
> | Revenue | $4,250K | $4,500K | ($250K) | -6% | Sales capacity (2 heads short) + Acme churn |
> | COGS | $1,785K | $1,800K | $15K | -1% | Favorable, but margin % impacted by product mix |
> | Gross Margin | 58.0% | 60.0% | -200bps | - | New tier cannibalization + mix shift |
> | S&M | $850K | $900K | $50K | -6% | Open headcount savings |
> | R&D | $620K | $600K | ($20K) | +3% | Security audit contractor (one-time) |
> | Operating Income | $615K | $800K | ($185K) | -23% | Revenue shortfall impact |
>
> **Variance Details:**
>
> **Revenue ($250K unfavorable)**
> - Sales capacity impact: ~$150K (2 heads × estimated productivity)
> - Acme Corp churn: $45K (mid-month, so ~50% impact)
> - Pipeline conversion: ~$55K general softness
> - *Controllable:* Hiring delays are controllable; churn partially controllable
> - *Recurring risk:* Churn increase may indicate trend
>
> **Gross Margin (200bps unfavorable)**
> - New product tier: ~100bps (lower margin by design)
> - Mix shift to smaller deals: ~60bps
> - Support cost allocation: ~40bps
> - *Recurring:* New tier impact will persist; may worsen as adoption grows
>
> ---
>
> **TREND ANALYSIS**
>
> **Revenue Trend**
> ```
> Jun    Jul    Aug    Sep    Oct   (Budget)
> $4.1M  $4.2M  $4.3M  $4.4M  $4.3M  $4.5M
> ```
> *Interpretation:* Revenue has plateaued over the last three months despite budget expectations of continued growth. The October decline breaks a 4-month growth streak. Sales capacity is the primary driver, but increasing churn is a secondary concern.
>
> **Gross Margin Trend**
> ```
> Jun    Jul    Aug    Sep    Oct   (Budget)
> 61%    60%    59%    59%    58%   60%
> ```
> *Interpretation:* Steady decline from June high. The new product tier is driving structural margin compression. At current adoption rates, expect margin to stabilize around 57-58%.
>
> **Operating Margin Trend**
> ```
> Jun    Jul    Aug    Sep    Oct   (Budget)
> 17%    16%    15%    15%    14%   18%
> ```
> *Interpretation:* Operating margin compression reflects both gross margin pressure and under-absorption of fixed costs due to revenue shortfall. Expense control is helping (OpEx under budget), but can't fully offset revenue miss.
>
> ---
>
> **KEY METRICS COMMENTARY**
>
> | Metric | Actual | Target | Status | Commentary |
> |--------|--------|--------|--------|------------|
> | New customers | 45 | 55 | 🔴 | 18% below plan; capacity constraint |
> | Churn rate | 2.8% | 2.0% | 🔴 | Up 40% vs. target; Acme + 2 others |
> | Average deal size | $32K | $30K | ✅ | Bright spot; deal quality improving |
> | Sales headcount | 18 | 20 | 🟡 | Still 2 short; offers out to both |
> | Support tickets | 890 | 750 | 🔴 | 19% above plan; new tier issues |
>
> **Churn Deep Dive:**
> October churn included Acme Corp ($45K) plus two smaller customers ($22K combined). Exit interviews indicate:
> - Acme: Budget cuts, not product dissatisfaction
> - Others: Feature gaps vs. competition
>
> *Trend concern:* YTD churn is now 2.4% vs. 2.0% target. This is the 3rd consecutive month above plan.
>
> ---
>
> **AREAS OF CONCERN**
>
> 1. **Churn Trend** 🔴 High Concern
>    - Three consecutive months above plan
>    - Exit reasons suggest some competitive pressure
>    - *Action:* Conduct win/loss analysis; product team review of competitive gaps
>
> 2. **Gross Margin Compression** 🟡 Medium Concern
>    - Structural pressure from new tier
>    - May continue as adoption grows
>    - *Action:* Model margin impact at scale; consider pricing adjustments
>
> 3. **Revenue Plateau** 🟡 Medium Concern
>    - Growth has stalled for 3 months
>    - Capacity is main driver but not only factor
>    - *Action:* Accelerate hiring; review pipeline quality
>
> ---
>
> **FORWARD IMPLICATIONS**
>
> **Full-Year Forecast Impact:**
>
> | Scenario | Full-Year Revenue | Operating Income | Key Assumptions |
> |----------|------------------|------------------|-----------------|
> | Original Budget | $53.0M | $9.2M | Full hiring by Sept |
> | Current Forecast | $51.2M | $7.8M | Hiring complete Nov, current churn |
> | Downside | $49.5M | $6.5M | Churn increases further |
>
> **Recommended Forecast Adjustments:**
> - Revenue: Reduce full-year by $1.8M (3.4%)
> - Operating income: Reduce by $1.4M (15%)
> - Maintain expense plan (don't cut into future capacity)
>
> **Risks to Watch:**
> 1. Churn continues above 2.5%
> 2. Gross margin drops below 57%
> 3. New sales hires ramp slower than expected

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Variance explanations are wrong | Missing business context | Add: "The actual reason for X was [context]" |
| Calculations seem off | Data formatting issues | Clean data, use consistent formatting, spot-check |
| Too finance-focused | Audience is non-financial | Ask: "Rewrite for a business audience, not accountants" |
| Missing important variances | Materiality threshold too high | Specify: "Flag anything over $X or Y%" |
| Forward implications weak | Not enough context | Add: "Here are known future events: [list]" |
| Narrative too long | Too much detail | Ask: "Condense to executive summary—what are the 5 things they need to know?" |

---

## Tips from Experience

1. **Lead with insight, not numbers.** The story is more important than the spreadsheet. Start with what matters.

2. **Separate signal from noise.** Not every variance needs explanation. Focus on material items that drive action.

3. **Always answer "so what?"** Every variance explanation should include what it means and what to do about it.

4. **Distinguish one-time from recurring.** This is often the most important classification for forward-looking.

5. **Connect to operations.** Financial results are outputs of operational drivers. Make the connection explicit.

6. **Be honest about uncertainty.** Where you don't know the cause, say so. Speculation presented as fact erodes trust.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Executives understand financial results without asking clarifying questions
- [ ] Variance explanations are accepted without challenge
- [ ] Analysis enables decisions, not just information
- [ ] Monthly reporting time is reduced
- [ ] Forward implications prove directionally accurate

**Track over time:**
- Time to produce monthly analysis
- Questions/clarifications from leadership
- Forecast accuracy vs. actual results
- Quality of financial discussions

---

## Variations

### Quick Monthly Flash
For rapid monthly summary:
```
Provide a flash summary of these monthly results:

[Financial data]

In 300 words or less:
1. Headline (1 sentence)
2. Revenue summary
3. Profitability summary
4. Top 3 things to know
5. One sentence outlook
```

### Quarterly Deep Dive
For comprehensive quarterly analysis:
```
Conduct a comprehensive quarterly financial analysis:

[Q data including all three months]

Include:
1. Quarter performance vs. budget and prior year
2. Monthly trend within quarter
3. Full variance waterfall
4. Rolling 12-month trends
5. Updated full-year forecast
6. Board-ready narrative
```

### Cash Flow Analysis
For cash-focused analysis:
```
Analyze cash flow and liquidity:

[Cash flow statement and balance sheet]

Provide:
1. Operating cash flow analysis
2. Working capital trends
3. Capital expenditure review
4. Cash runway calculation
5. Liquidity concerns or highlights
6. Cash management recommendations
```

### Budget Variance Package
For formal budget reporting:
```
Create a formal budget variance report:

[Budget vs. actual data]

Format as:
1. Summary dashboard
2. Detailed variance schedule
3. Variance commentary by department
4. Year-end implications
5. Reforecast recommendations
```

---

## Building Your Repeatable System

After several reporting cycles, establish your system:

1. **Create standard data templates** for consistent input
2. **Build commentary library** for recurring explanations
3. **Establish review workflow** with finance team
4. **Maintain forecast accuracy log** to improve over time
5. **Document lessons learned** each cycle

**Sample Setup:**
```
financial-analysis/
├── templates/
│   ├── analysis-prompt.txt
│   ├── data-template.xlsx
│   └── presentation-template.pptx
├── monthly/
│   ├── 2024-10/
│   │   ├── data/
│   │   ├── analysis.md
│   │   └── deliverables/
│   └── archive/
├── quarterly/
├── reference/
│   ├── variance-explanations-library.md
│   └── forecast-accuracy-log.xlsx
└── board/
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**aggregate data → calculate variances → interpret trends → generate narrative → create implications**—applies broadly:

| Role | Application |
|------|-------------|
| **Finance/FP&A** | Monthly, quarterly reporting |
| **Executives** | Business review preparation |
| **Operations** | Operational metrics analysis |
| **Sales** | Sales performance analysis |
| **Product** | Product financial performance |
| **Investors** | Portfolio financial review |

---

## Next Steps

1. **Start with this month:** Use the recipe for your next close
2. **Build your template:** Customize for your specific reports
3. **Track accuracy:** Note where analysis was right/wrong
4. **Iterate:** Improve prompts based on feedback

---

*Recipe #25 of 100 in the Claude Code Knowledge Worker Recipe Collection*
