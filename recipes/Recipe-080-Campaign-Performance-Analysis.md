# Campaign Performance Analysis

**Recipe #80: From Campaign Dashboards to Actionable Marketing Insights**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 45 minutes (first time) / 20 minutes (repeat) | 2-4 hours per campaign | Intermediate | Marketing Analysts, Campaign Managers, Marketing Leadership |

---

## The Problem

Marketing campaigns generate vast amounts of data across multiple channels—email, paid advertising, social, content, events—but turning that data into actionable insights is time-consuming and often inconsistent. Campaign managers struggle to determine what actually worked, why some campaigns outperformed others, and how to optimize future efforts. Standard dashboards show what happened but don't explain why or what to do next.

**Pain Points:**
- Campaign data is scattered across multiple platforms and hard to aggregate
- Reports focus on vanity metrics instead of business impact
- No consistent methodology for analyzing campaign performance
- Hard to compare campaigns because metrics are tracked differently
- Attribution is messy and everyone argues about which channel gets credit
- Recommendations are generic ("do more of what works") not specific
- Post-campaign analysis happens too late to affect in-flight optimization

---

## The Outcome

A comprehensive campaign performance analysis with channel breakdowns, conversion analysis, ROI calculations, benchmark comparisons, and optimization recommendations—enabling continuous improvement in marketing effectiveness and investment decisions.

**What You'll Have When Done:**
- Complete campaign performance assessment vs. goals
- Channel-by-channel effectiveness analysis with grades
- Conversion funnel analysis identifying bottlenecks
- ROI and ROAS calculations across attribution models
- Prioritized optimization recommendations with expected impact
- Budget reallocation guidance for future campaigns

---

## When to Use This Recipe

**Good Fit:**
- Post-campaign analysis and reporting
- Quarterly marketing performance reviews
- Channel optimization decisions and budget reallocation
- A/B test interpretation and learning capture
- Campaign comparison studies to identify patterns
- Marketing ROI justification for leadership
- Planning input for future campaigns

**Not a Good Fit:**
- Very small campaigns with minimal data to analyze
- When you lack conversion tracking or attribution data
- Real-time campaign monitoring (use dashboards instead)
- Brand awareness campaigns without performance metrics

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] Campaign goals and targets are documented
- [ ] Channel-level performance data is available
- [ ] Conversion and revenue attribution exists
- [ ] Cost data by channel/campaign is accessible
- [ ] Benchmark data (historical or industry) is available
- [ ] Audience/segment information is tracked
- [ ] Creative/content performance data exists
- [ ] Timeline and context details are documented
- [ ] You have 60-90 minutes for comprehensive campaign analysis

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Transform raw campaign data from multiple channels into unified analysis
- Calculate ROI across different attribution models automatically
- Identify performance patterns and anomalies across channels
- Compare against benchmarks (historical and industry)
- Generate specific, actionable optimization recommendations
- Create executive summaries that highlight key insights

**Where Human Judgment Is Essential:**
- Interpreting context that data doesn't capture (market events, etc.)
- Deciding which attribution model to prioritize for decisions
- Balancing short-term performance vs. long-term brand building
- Determining feasibility of recommendations given resources
- Setting strategy for future campaigns based on insights

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Campaign Overview | Goals, targets, duration, investment | Framing analysis context |
| Channel Performance | Metrics by channel (impressions, clicks, conversions, cost) | Channel comparison |
| Conversion Data | Funnel metrics and conversion rates | Identifying bottlenecks |
| Context & Benchmarks | Historical data, industry standards, market events | Comparative assessment |
| Creative Performance | A/B test results, message testing | Understanding what resonated |

**Sample Input:** *(see Example Inputs in original recipe for detailed examples)*

The recipe includes comprehensive example inputs showing:
- Campaign overview with objectives and targets
- Detailed channel performance data
- Conversion funnel analysis
- Historical and industry benchmark comparisons

---

## Step-by-Step Implementation

### Step 1: Prepare Your Inputs
**Time: 15-20 minutes**

Gather your campaign data and organize it:
- Document campaign goals and targets
- Export performance data by channel
- Compile conversion funnel metrics
- Collect cost/investment data
- Note context (market events, changes during campaign)

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Campaign Analysis Prompt
**Time: 8-10 minutes for Claude to process**

---

**PRIMARY PROMPT: Framework the Analysis**

```
Claude, I need to analyze performance for our [CAMPAIGN NAME] marketing campaign.

Campaign overview:
[PASTE CAMPAIGN SUMMARY, GOALS, TIMELINE]

I want to understand:
1. Overall campaign performance vs. objectives
2. Channel-level effectiveness
3. What worked and what didn't
4. Specific optimization recommendations

Help me structure the analysis and identify any data gaps.
```

---

### Step 4: Review and Validate
**Time: 8-10 minutes**

**Check immediately:**
- Do the goal attainment calculations look correct?
- Are channels being compared fairly (apples to apples)?
- Does the overall assessment align with your intuition?

**Spot-check specifics:**
- Verify ROI calculations are using correct formulas
- Confirm conversion funnel math is accurate
- Check that cost data includes all relevant expenses
- Ensure attribution logic makes sense for your model

---

### Step 5: Refine and Iterate
**Time: 20-30 minutes**

**Prompt: Channel Deep Dive**
```
Analyze performance by channel:

Channel data:
[PASTE ALL CHANNEL PERFORMANCE DATA]

For each channel, assess:
1. Efficiency metrics (CPC, CPM, Cost/MQL)
2. Quality metrics (conversion rates, lead scores)
3. Volume contribution
4. ROI/ROAS
5. Performance vs. benchmarks
6. Anomalies or notable patterns
```

**Prompt: Conversion Analysis**
```
Analyze the conversion funnel:

Funnel data:
[PASTE FUNNEL AND CONVERSION DATA]

Identify:
1. Where conversion is strong/weak
2. Stage-by-stage drop-off analysis
3. Channel comparison on conversion quality
4. Lead quality patterns
5. Revenue attribution analysis
```

**Prompt: Identify What Worked**
```
Based on the data, identify what worked well in this campaign:

Consider:
1. Channels that outperformed
2. Content or creative that resonated
3. Audience segments that converted
4. Timing or tactical elements that drove results
5. Any positive surprises

Support findings with specific data points.
```

**Prompt: Generate Recommendations**
```
Based on the complete analysis, provide optimization recommendations:

Structure as:
1. IMMEDIATE ACTIONS (for in-flight campaigns)
2. CHANNEL OPTIMIZATION (budget reallocation)
3. CONVERSION OPTIMIZATION (funnel improvements)
4. STRATEGIC RECOMMENDATIONS (longer-term changes)
5. BUDGET RECOMMENDATIONS (where to invest/reduce)

Include expected impact for each recommendation.
```

---

### Step 6: Export Final Output
**Time: 5 minutes**

```
Create an executive summary of the campaign analysis for leadership:

Include:
1. One-paragraph performance summary
2. Key metrics table (3-5 most important)
3. Top 3 wins
4. Top 3 improvement areas
5. Strategic recommendations
6. Resource/budget asks (if any)

Keep it to one page maximum.
```

---

## Example Output

Below is an abbreviated example of what a well-executed campaign analysis looks like:

---

> ### Campaign Performance Analysis: Q4 Product Launch "DataSync 3.0"
>
> #### Executive Summary
>
> **Campaign:** DataSync 3.0 Product Launch | **Duration:** Oct 1 - Dec 15, 2024 | **Investment:** $450,000
>
> **Performance at a Glance:**
>
> | Metric | Target | Actual | Status |
> |--------|--------|--------|--------|
> | Pipeline Generated | $4.5M | $3.8M | 84% |
> | MQLs | 1,200 | 980 | 82% |
> | SQL Conversion | 25% | 28% | 112% |
> | Campaign ROI | 8.0x | 8.4x | 105% |
>
> **Key Takeaway:** Campaign delivered strong efficiency and quality metrics (ROI +14% YoY, SQL conversion +3pts) but fell short on volume targets due to underperformance in top-of-funnel reach.
>
> **Top 3 Wins:**
> 1. **LinkedIn outperformed** - 11.7x ROAS, best CTR in campaign history (1.5% vs. 0.8% benchmark)
> 2. **Lead quality improved** - 28% MQL→SQL (vs. 25% target)
> 3. **Webinar with influencer** - 65% attendance rate, highest conversion to SQL
>
> **Strategic Recommendations:**
> 1. Reallocate $30K from industry pubs to LinkedIn (expected +95 MQLs)
> 2. Pause Google Display, redirect to Search (better quality)
> 3. Double down on influencer webinars ($10K incremental investment)
>
> ---
>
> #### Channel Performance Comparison
>
> | Channel | Spend | MQLs | Cost/MQL | Pipeline | ROAS | Grade |
> |---------|-------|------|----------|----------|------|-------|
> | LinkedIn | $120K | 385 | $312 | $1.4M | 11.7x | A |
> | Google Search | $65K | 220 | $295 | $920K | 14.2x | A |
> | Email/Nurture | $25K | 85 | $294 | $520K | 20.8x | A+ |
> | Google Display | $35K | 85 | $412 | $245K | 7.0x | C |
> | Industry Pubs | $30K | 45 | $667 | $180K | 6.0x | D |
>
> *(Full analysis includes detailed channel deep dives, conversion funnel, and optimization plan)*

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Attribution data incomplete | Can't track conversions across channels | Use available data; acknowledge limitations; combine first-touch, last-touch, multi-touch views |
| Too many variables changed | Can't isolate what drove performance | Focus on biggest changes; use A/B test data; document changes for future; recommend controlled testing |
| Benchmarks outdated or irrelevant | Not sure if performance is good or bad | Use year-over-year as primary benchmark; supplement with industry data; document own benchmarks |
| Results mixed across metrics | Some metrics up, some down—hard to assess | Weight metrics by business goal importance; focus on ROI as ultimate arbiter; tell coherent story |
| Channel data inconsistent | Different platforms track metrics differently | Standardize definitions; document what each metric means; focus on directionally correct insights |
| Budget allocation disputes | Teams fight for their channels | Use ROI and efficiency data to ground discussion; model scenarios; show trade-offs quantitatively |

---

## Tips from Experience

1. **Start with goals—frame everything around what you were trying to achieve.** Campaign analysis without objectives is just number reporting.

2. **Use consistent methodology for comparability.** Calculate metrics the same way every time so you can compare campaigns over time and identify real patterns.

3. **Go beyond the numbers—provide the "why" behind performance.** Data says what happened; insights explain why it happened and what to do differently.

4. **Be honest about what didn't work.** Campaigns that "succeeded" at everything teach you nothing. Bad news improves future campaigns.

5. **Connect to revenue, not just marketing metrics.** Pipeline and revenue matter most; impressions and clicks are means to an end, not the end itself.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Key campaign metrics improve over time (ROI, cost/MQL, conversion rates)
- [ ] Recommendations are implemented and impact is tracked
- [ ] Waste in underperforming channels is reduced
- [ ] Future campaign predictions become more accurate
- [ ] Marketing and sales align on what's working

**Track over time:**
- Campaign ROI trend
- Cost per MQL/SQL by channel
- Conversion rates by funnel stage

---

## Variations

### Variation 1: Always-On Channel Analysis
Ongoing analysis of demand gen channels without campaign wrapper.
```
Modify the primary prompt:
"Analyze our always-on demand generation channels for [TIME PERIOD]. Focus on: sustained performance trends, channel contribution to pipeline, efficiency over time, and optimization opportunities for continuous programs (not campaign-based)."
```

### Variation 2: ABM Campaign Analysis
Account-based campaign analysis with account engagement metrics.
```
Add to your analysis structure:
"This is an ABM campaign. Include: account engagement scores, contacts engaged per target account, pipeline created by target account tier, account-level conversion funnel, and account coverage efficiency."
```

### Variation 3: Content Performance Analysis
Deep dive on content marketing performance across assets and topics.
```
Modify focus to content:
"Analyze content performance for [TIME PERIOD]. Break down by: content type (blog, ebook, video, etc.), topic/theme, stage of buyer journey, distribution channel, and conversion contribution. Identify top-performing content and themes."
```

---

## Building Your Repeatable System

After using this recipe 2-3 times, establish your system:

1. **Create Campaign Report Templates.** Standardize sections and metrics so every campaign analysis is comparable and complete.

2. **Build a Channel Scorecard.** Develop consistent grading framework for channels that you apply to every campaign.

3. **Maintain a Benchmark Library.** Track your own historical performance and industry benchmarks in a central repository.

4. **Implement a Recommendation Tracker.** Log all recommendations and track which ones were implemented and what impact they had.

**Sample Folder Structure:**
```
campaign-analysis/
├── templates/
│   ├── campaign-report-template.md
│   └── channel-scorecard.xlsx
├── campaigns/
│   ├── 2024-Q4-product-launch-analysis.md
│   ├── 2024-Q3-demand-gen-analysis.md
│   └── campaign-data/
├── benchmarks/
│   ├── historical-benchmarks.xlsx
│   └── industry-benchmarks.md
└── recommendations/
    └── recommendation-tracker.xlsx
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**synthesizing multi-channel performance data into actionable insights**—applies broadly:

| Role | Application |
|------|-------------|
| **Sales Operations** | Outbound sales campaign effectiveness analysis |
| **Customer Success** | Customer engagement campaign analysis and optimization |
| **Product Marketing** | Feature launch campaign performance assessment |
| **Events** | Conference and event ROI analysis across events |
| **Content Marketing** | Content strategy performance and topic optimization |

---

## Next Steps

1. **This week:** Run analysis on your most recent completed campaign using this recipe's prompts.
2. **Track your results:** Implement the top 3 recommendations and measure impact over 30 days.
3. **Iterate:** Share analysis with stakeholders and incorporate their feedback into next analysis.
4. **Share:** Present campaign insights at next marketing team meeting to establish analysis as standard practice.

---

*Recipe #80 of 100 in the Claude Code Knowledge Worker Recipe Collection*
