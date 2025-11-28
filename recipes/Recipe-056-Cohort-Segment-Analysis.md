# Cohort and Segment Analysis

**Recipe #56: Uncover Patterns Hidden in Customer Groups**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 5 minutes (first time) / 3 minutes (repeat) | 3-4 hours per analysis | Intermediate | Product, Marketing, Customer Success, Finance |

---

## The Problem

Your aggregate metrics look fine, but they're hiding important stories. Overall retention is 85%, but is that consistent across all customer segments? Average revenue is growing, but which cohorts are driving it? When you treat all customers the same, you miss the patterns that explain performance differences. Cohort and segment analysis takes hours to do properly, so it rarely gets done—and when it does, the insights don't get actioned.

**Pain Points:**
- Aggregate metrics mask segment-level differences
- "Average customer" doesn't actually exist
- Can't tell which acquisition channels produce best customers
- Retention problems invisible until too late
- No clear view of customer lifecycle patterns
- Marketing treats all customers the same
- Product decisions not informed by segment behavior

---

## The Outcome

Clear visibility into how different customer groups behave over time. Identification of your best and worst segments. Cohort analysis that reveals lifecycle patterns. Strategic recommendations tailored to each segment's characteristics.

**What You'll Have When Done:**
- Cohort performance comparison
- Segment behavior profiles
- Lifecycle pattern analysis
- Retention curves by cohort
- Revenue contribution by segment
- Strategic segment recommendations
- Action priorities by group

---

## When to Use This Recipe

**Good Fit:**
- Quarterly business reviews
- Customer retention analysis
- Marketing channel evaluation
- Pricing tier analysis
- Product usage analysis
- Geographic expansion decisions
- Customer health scoring design

**Not a Good Fit:**
- Individual customer analysis
- Real-time personalization
- Statistical significance testing (need specialized tools)
- Very small sample sizes (<100 per segment)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have customer data by cohort or segment
- [ ] You have relevant metrics per group
- [ ] You understand the business questions to answer
- [ ] You have 30-60 minutes for comprehensive analysis

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Structures cohort/segment comparisons
- Identifies patterns across groups
- Generates insight narratives
- Creates actionable recommendations
- Highlights anomalies and outliers
- Formats findings for stakeholders

**Where Human Judgment Is Essential:**
- Validating segment definitions
- Understanding business context
- Determining statistical significance
- Prioritizing action items
- Making investment decisions
- Final recommendations

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Cohort data | Monthly acquisition groups | Time-based pattern analysis |
| Segment data | Customer groups by attribute | Group comparison |
| Metrics | Revenue, retention, usage | Performance measurement |
| Timeframes | Months since acquisition | Lifecycle analysis |
| Context | Business situation | Interpretation framework |

**Sample Input:**
```
Cohort and Segment Analysis Request

PRODUCT: CloudSync Pro (SaaS subscription)
ANALYSIS PERIOD: Q1-Q3 2024

COHORT ANALYSIS DATA (by sign-up month):

Retention by Cohort (% still active):
| Cohort | Month 0 | Month 1 | Month 2 | Month 3 | Month 4 | Month 5 | Month 6 |
|--------|---------|---------|---------|---------|---------|---------|---------|
| Jan 24 | 100% | 82% | 74% | 68% | 63% | 59% | 56% |
| Feb 24 | 100% | 78% | 69% | 62% | 57% | 53% | - |
| Mar 24 | 100% | 75% | 65% | 58% | 52% | - | - |
| Apr 24 | 100% | 71% | 61% | 53% | - | - | - |
| May 24 | 100% | 68% | 57% | - | - | - | - |
| Jun 24 | 100% | 72% | 63% | - | - | - | - |
| Jul 24 | 100% | 76% | - | - | - | - | - |
| Aug 24 | 100% | 79% | - | - | - | - | - |

Revenue per Customer by Cohort ($MRR):
| Cohort | Month 0 | Month 1 | Month 2 | Month 3 | Month 4 | Month 5 | Month 6 |
|--------|---------|---------|---------|---------|---------|---------|---------|
| Jan 24 | $85 | $88 | $91 | $94 | $96 | $99 | $102 |
| Feb 24 | $82 | $84 | $86 | $88 | $90 | $92 | - |
| Mar 24 | $78 | $79 | $80 | $81 | $82 | - | - |
| Apr 24 | $72 | $73 | $73 | $74 | - | - | - |
| May 24 | $68 | $68 | $69 | - | - | - | - |
| Jun 24 | $75 | $77 | $79 | - | - | - | - |
| Jul 24 | $82 | $85 | - | - | - | - | - |
| Aug 24 | $88 | $91 | - | - | - | - | - |

SEGMENT ANALYSIS DATA (by customer attribute):

By Company Size:
| Segment | Customers | % of Total | MRR | Retention (6mo) | NPS | Support Tickets/Mo |
|---------|-----------|------------|-----|-----------------|-----|-------------------|
| Enterprise (500+) | 85 | 8% | $320 | 92% | 48 | 2.1 |
| Mid-Market (50-500) | 420 | 42% | $125 | 78% | 38 | 1.4 |
| SMB (10-50) | 380 | 38% | $65 | 65% | 32 | 0.8 |
| Startup (<10) | 115 | 12% | $35 | 48% | 28 | 0.4 |

By Acquisition Channel:
| Channel | Customers | % of Total | Avg MRR | Retention (6mo) | CAC | LTV | LTV:CAC |
|---------|-----------|------------|---------|-----------------|-----|-----|---------|
| Direct/Organic | 340 | 34% | $145 | 82% | $280 | $2,850 | 10.2 |
| Paid Search | 285 | 28.5% | $88 | 68% | $520 | $1,440 | 2.8 |
| Partner Referral | 180 | 18% | $165 | 85% | $180 | $3,360 | 18.7 |
| Content/Inbound | 125 | 12.5% | $112 | 75% | $340 | $2,010 | 5.9 |
| Outbound Sales | 70 | 7% | $280 | 88% | $850 | $5,920 | 7.0 |

By Pricing Tier:
| Tier | Customers | % of Total | MRR | Retention (6mo) | Usage (% of limits) | Upgrade Rate |
|------|-----------|------------|-----|-----------------|---------------------|--------------|
| Starter | 420 | 42% | $35 | 58% | 45% | 8% |
| Professional | 385 | 38.5% | $95 | 78% | 72% | 12% |
| Business | 145 | 14.5% | $225 | 88% | 85% | 5% |
| Enterprise | 50 | 5% | $650 | 94% | 68% | N/A |

By Use Case (self-reported):
| Use Case | Customers | Retention | Expansion Rate | NPS |
|----------|-----------|-----------|----------------|-----|
| Team Collaboration | 380 | 82% | 18% | 42 |
| Client Sharing | 285 | 71% | 8% | 35 |
| Personal/Backup | 220 | 52% | 3% | 28 |
| Developer Workflow | 115 | 88% | 22% | 52 |

CONTEXT:
- Major marketing push via paid search in Mar-May
- Partner program launched in June
- Free trial extended from 7 to 14 days in June
- Starter tier pricing decreased in April

QUESTIONS TO ANSWER:
1. Which cohorts are healthiest/most concerning?
2. Which segments should we focus on?
3. Where is there opportunity vs. risk?
4. What's driving the patterns we see?
5. What should we do differently?

AUDIENCE: Leadership team strategy session
```

---

## Step-by-Step Implementation

### Step 1: Prepare Cohort/Segment Data
**Time: 10-15 minutes**

Extract from your analytics/data warehouse:
- Cohort retention curves
- Segment metrics comparison
- Relevant dimensions for analysis
- Time-series where available

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Cohort/Segment Analysis Prompt
**Time: 5-10 minutes for Claude to process**

---

**PRIMARY PROMPT: Cohort and Segment Analysis**

```
Please analyze this cohort and segment data to uncover strategic insights.

PRODUCT/BUSINESS: [Name and type]
ANALYSIS PERIOD: [Timeframe]

COHORT DATA:
[Paste cohort retention/revenue data]

SEGMENT DATA:
[Paste segment comparison data]

CONTEXT:
[Business events that might explain patterns]

KEY QUESTIONS:
[What you need to answer]

ANALYSIS REQUIREMENTS:

1. EXECUTIVE SUMMARY
   - Most important finding
   - Best performing cohort/segment
   - Most concerning cohort/segment
   - Biggest opportunity
   - Recommended strategic shift

2. COHORT ANALYSIS

   **Cohort Health Overview:**
   | Cohort | Health Score | Trend | Key Characteristic |
   |--------|--------------|-------|-------------------|
   [Rank cohorts by overall performance]

   **Retention Curve Analysis:**
   - Shape of curves: [Steep early drop vs gradual decline]
   - Stabilization point: [When churn levels off]
   - Best cohort: [Which and why]
   - Worst cohort: [Which and why]
   - Trend over time: [Improving or declining]

   **Cohort-Specific Insights:**
   For notable cohorts:
   - [Cohort]: [What's different about this group]

   **Revenue per Customer Trends:**
   - Expansion pattern: [Growing, flat, declining]
   - Best expanders: [Which cohorts]
   - Concerns: [Any revenue contraction]

3. SEGMENT ANALYSIS

   **Segment Value Matrix:**
   | Segment | Revenue Contribution | Growth Potential | Retention Risk | Strategic Priority |
   |---------|---------------------|-----------------|----------------|-------------------|
   [Rank and categorize each segment]

   **Segment Deep Dives:**

   For each significant segment:

   **[Segment Name]**

   Profile:
   - Size: [X customers, Y%]
   - Revenue: [$X, Y% of total]
   - Retention: [X% at 6 months]

   Behavior Patterns:
   - [Pattern 1]
   - [Pattern 2]

   Opportunity:
   - [What could be captured]

   Risk:
   - [What could be lost]

   Recommendation:
   - [Strategic approach for this segment]

4. CROSS-DIMENSIONAL INSIGHTS

   Interactions between dimensions:
   - [Dimension A] × [Dimension B] insight
   Example: "Partner-acquired Enterprise customers have 95% retention vs 88% for direct Enterprise"

5. LIFECYCLE PATTERNS

   Customer journey insights:
   - First 30 days: [Critical patterns]
   - Month 2-3: [Inflection points]
   - Month 6+: [Stable state characteristics]

   Red flags to monitor:
   - [Early warning sign 1]
   - [Early warning sign 2]

6. BEST CUSTOMER PROFILE

   Based on analysis, ideal customers are:
   - Size: [X]
   - Channel: [X]
   - Use case: [X]
   - Tier: [X]

   These customers represent [X%] of base but [Y%] of value.

7. AT-RISK SEGMENTS

   Segments requiring intervention:
   | Segment | Risk Level | Revenue at Risk | Intervention |
   |---------|------------|-----------------|--------------|
   [Prioritize by impact]

8. OPPORTUNITY SIZING

   Growth opportunities identified:
   | Opportunity | Segment | Potential | Investment | Priority |
   |-------------|---------|-----------|------------|----------|
   [Quantify where possible]

9. STRATEGIC RECOMMENDATIONS

   Based on cohort and segment analysis:

   **Double Down On:**
   - [Segment/approach] — Why: [Evidence]

   **Fix or Improve:**
   - [Segment/approach] — Why: [Evidence]

   **Reconsider or Exit:**
   - [Segment/approach] — Why: [Evidence]

10. ACTION ITEMS

    Immediate (this quarter):
    1. [Action] — [Segment] — [Expected impact]

    Strategic (roadmap):
    1. [Action] — [Segment] — [Expected impact]

    Measurement:
    - Track: [Metric] for [Segment]

Provide quantified insights where possible. Be direct about what the data shows.
```

---

### Step 4: Validate Findings
**Time: 10-15 minutes**

Review the analysis:
- Do segment profiles match reality?
- Are causal explanations plausible?
- Any segments missing from analysis?
- Do recommendations align with strategy?

---

### Step 5: Add Business Context
**Time: 5-10 minutes**

```
Update the analysis with this business context:

SEGMENT: [Name]
- Why this pattern exists: [Your knowledge]
- What we've tried: [Previous interventions]
- Constraints: [Limitations on action]

ADDITIONAL CONTEXT:
- Strategic priority is: [Focus area]
- We cannot change: [Constraints]
- Upcoming changes: [Relevant plans]
```

---

### Step 6: Generate Final Deliverables
**Time: 5 minutes**

```
Create final analysis package:

1. EXECUTIVE ONE-PAGER
   - Key findings (3-5 bullets)
   - Strategic implications
   - Recommended actions
   - Segment priority matrix visualization

2. DETAILED ANALYSIS
   Full cohort and segment analysis as developed

3. SEGMENT PLAYBOOKS
   For each priority segment:
   - Profile summary
   - Key metrics to track
   - Recommended approach
   - Success criteria

4. MONITORING DASHBOARD DESIGN
   Recommended metrics to track by segment going forward
```

---

## Example Output

Below is an abbreviated cohort/segment analysis example:

---

> **COHORT AND SEGMENT ANALYSIS**
>
> **CloudSync Pro | Q1-Q3 2024**
>
> ---
>
> ## Executive Summary
>
> **Most Important Finding:** The March-May paid search push acquired high-volume, low-quality customers who are now churning at 2x the rate of organic acquisitions. This masks improving cohort quality in recent months.
>
> **Best Performing Segment:** Partner-referred customers deliver 18.7x LTV:CAC with 85% retention. This channel is dramatically under-invested.
>
> **Most Concerning Segment:** Startup tier (<10 employees) has 48% 6-month retention and negative unit economics. We're spending to acquire customers who churn.
>
> **Biggest Opportunity:** Developer workflow use case shows 88% retention and 22% expansion. This segment is 11.5% of customers but represents our stickiest, most valuable users.
>
> **Recommended Strategic Shift:** Reduce paid search spend, increase partner program investment, develop product features for developer workflow use case, and consider eliminating or restructuring Starter tier.
>
> ---
>
> ## Cohort Analysis
>
> ### Cohort Health Overview
>
> | Cohort | Health Score | Trend | Key Characteristic |
> |--------|--------------|-------|-------------------|
> | Jan 24 | A | Stable | Pre-marketing push, organic |
> | Feb 24 | B+ | Stable | Mostly organic |
> | Mar 24 | C | Declining | First paid push cohort |
> | Apr 24 | C- | Declining | Heavy paid + pricing change |
> | May 24 | C- | Declining | Peak paid acquisition |
> | Jun 24 | B | Improving | Partner program launch |
> | Jul 24 | B+ | Improving | Mix normalizing |
> | Aug 24 | A- | Early but strong | Recent improvements |
>
> ### Retention Curve Analysis
>
> **Shape of Curves:**
> Retention follows classic SaaS pattern with steep Month 1 drop (18-32% churn) followed by gradual decline. Concerning: Mar-May cohorts show steeper curves that aren't stabilizing.
>
> **Stabilization Point:**
> - Healthy cohorts (Jan-Feb, Jul-Aug): Stabilize around Month 4-5 at ~60%
> - Concerning cohorts (Mar-May): Still declining at Month 3-4, not yet stabilizing
>
> **Best Cohort: January 2024**
> - Highest Month 6 retention: 56%
> - Highest revenue per customer: $102 by Month 6
> - Characteristic: Pre-paid-push, mostly organic and referral
>
> **Worst Cohort: May 2024**
> - Lowest Month 1 retention: 68%
> - Lowest revenue per customer: $68
> - Characteristic: Peak of paid search campaign
>
> **Trend:** V-shaped. Quality declined Mar-May, recovering Jun-Aug. Recent cohorts showing improvement.
>
> ### Cohort-Specific Insights
>
> **January 2024:** Benchmark cohort. Organic acquisition produced highest-quality customers. 56% 6-month retention and $102 MRR by Month 6 represents the ceiling.
>
> **March-May 2024:** The paid search cohorts. Month 1 retention dropped from 82% (Jan) to 68% (May). These customers came for free trial, didn't convert to engaged users. We paid to acquire 680 customers who are churning at 2x normal rate.
>
> **June 2024:** Inflection point. Partner program launched, extended trial. Quality immediately improved. This validates channel matters more than trial length.
>
> **August 2024:** Too early to celebrate, but Month 1 retention (79%) approaching Jan levels. If this holds, channel mix optimization is working.
>
> ### Revenue per Customer Trends
>
> **Expansion Pattern:** Healthy cohorts show $3-5/month MRR expansion. This is positive but modest (~5% annual expansion from existing customers).
>
> **Best Expanders:** Jan cohort grew from $85 to $102 (20% in 6 months). Developer workflow use case drives upgrades.
>
> **Concern:** Mar-May cohorts show almost no expansion ($68→$69 for May). These customers aren't engaging deeply enough to need more.
>
> ---
>
> ## Segment Analysis
>
> ### Segment Value Matrix
>
> | Segment | Revenue Contribution | Growth Potential | Retention Risk | Strategic Priority |
> |---------|---------------------|-----------------|----------------|-------------------|
> | Enterprise (500+) | High (27%) | Medium | Low | Protect |
> | Mid-Market (50-500) | High (52%) | High | Medium | Invest |
> | SMB (10-50) | Medium (25%) | Medium | Medium | Optimize |
> | Startup (<10) | Low (4%) | Low | High | Reconsider |
> | Partner Referral | High value/customer | Very High | Low | Scale |
> | Paid Search | High volume | Low | High | Reduce |
> | Developer Workflow | Low volume | Very High | Low | Invest |
>
> ### Segment Deep Dives
>
> #### Enterprise (500+ employees)
>
> **Profile:**
> - Size: 85 customers, 8% of total
> - Revenue: $27,200 MRR, 27% of total
> - Retention: 92% at 6 months
>
> **Behavior Patterns:**
> - High touch onboarding required
> - Long sales cycle (60+ days)
> - Extensive security/compliance review
> - Multi-year contracts common
>
> **Opportunity:**
> - $320 MRR is below potential; upsell to additional teams
> - Only 68% usage of limits suggests room for expansion
>
> **Risk:**
> - Low volume (8% of customers) means each loss is significant
> - Competitor enterprise features advancing
>
> **Recommendation:**
> Protect and expand. Assign dedicated success managers. Quarterly business reviews. Feature roadmap input.
>
> ---
>
> #### Mid-Market (50-500 employees)
>
> **Profile:**
> - Size: 420 customers, 42% of total
> - Revenue: $52,500 MRR, 52% of total
> - Retention: 78% at 6 months
>
> **Behavior Patterns:**
> - Self-service friendly
> - Upgrades driven by team expansion
> - 22% churn in first 3 months, then stabilizes
> - Support-sensitive (1.4 tickets/month)
>
> **Opportunity:**
> - Core segment with best volume/value balance
> - 72% usage of limits = expansion trigger
> - Multi-team expansion potential
>
> **Risk:**
> - 78% retention below enterprise; room to improve
> - Competitor mid-market push
>
> **Recommendation:**
> Primary investment focus. Automated expansion triggers. Proactive retention outreach at Month 2. Product features for team collaboration.
>
> ---
>
> #### Startup (<10 employees)
>
> **Profile:**
> - Size: 115 customers, 12% of total
> - Revenue: $4,025 MRR, 4% of total
> - Retention: 48% at 6 months
>
> **Behavior Patterns:**
> - High churn in Month 1 (32%)
> - Low usage (45% of limits)
> - Low support engagement (0.4 tickets)
> - Price sensitive
>
> **Opportunity:**
> - Some startups grow into SMB/Mid-Market
> - Brand awareness in startup ecosystem
>
> **Risk:**
> - Negative unit economics: CAC not recovered before churn
> - Consumes support resources at low revenue
> - Drags down NPS (score: 28)
>
> **Recommendation:**
> Strategic reconsideration. Options: (1) Eliminate tier, (2) Free tier to reduce churn friction, (3) Strict qualification criteria, (4) Different product (lightweight version).
>
> ---
>
> #### Partner Referral Channel
>
> **Profile:**
> - Size: 180 customers, 18% of total
> - Avg MRR: $165
> - Retention: 85% at 6 months
> - LTV:CAC: 18.7x (best of all channels)
>
> **Behavior Patterns:**
> - Pre-qualified by partner
> - Higher starting tier
> - Faster time to value
> - Lower support needs
>
> **Opportunity:**
> - Dramatically underinvested: only 18% of volume
> - Scalable: partners do the selling
> - Best economics in the business
>
> **Risk:**
> - Partner dependency
> - Channel conflict potential
>
> **Recommendation:**
> Scale aggressively. Double partner recruitment. Increase referral incentives. This should be 40%+ of acquisition.
>
> ---
>
> #### Developer Workflow Use Case
>
> **Profile:**
> - Size: 115 customers (11.5%)
> - Retention: 88%
> - Expansion Rate: 22%
> - NPS: 52 (highest)
>
> **Behavior Patterns:**
> - API-heavy usage
> - Integration with dev tools
> - Team-based expansion
> - High engagement
>
> **Opportunity:**
> - Product-market fit strongest here
> - Viral within dev teams
> - High expansion rate
>
> **Risk:**
> - Only 11.5% of current customers
> - May require specialized product investment
>
> **Recommendation:**
> Double down. Developer-focused marketing. API improvements. VS Code/GitHub integrations. This use case could be 30%+ of business.
>
> ---
>
> ## Best Customer Profile
>
> Based on analysis, ideal customers are:
> - **Size:** Mid-Market (50-500 employees)
> - **Channel:** Partner referral or organic
> - **Use Case:** Team collaboration or developer workflow
> - **Tier:** Professional or Business
>
> These customers represent **~25% of current base** but generate **~55% of value** with **85%+ retention**.
>
> ---
>
> ## Strategic Recommendations
>
> ### Double Down On:
>
> 1. **Partner Channel** — Evidence: 18.7x LTV:CAC, 85% retention, scalable
>    - Action: 3x partner recruitment, increase referral bonus
>
> 2. **Developer Workflow** — Evidence: 88% retention, 52 NPS, 22% expansion
>    - Action: Developer-focused features and marketing
>
> 3. **Mid-Market Focus** — Evidence: Best volume/value balance, improvable retention
>    - Action: Product investment for team use cases
>
> ### Fix or Improve:
>
> 1. **Paid Search Channel** — Evidence: 2.8x LTV:CAC (barely viable), 68% retention
>    - Action: Reduce spend 50%, improve landing page qualification
>
> 2. **Month 1 Retention** — Evidence: Losing 18-32% immediately
>    - Action: Onboarding optimization, early engagement triggers
>
> ### Reconsider or Exit:
>
> 1. **Startup Tier** — Evidence: 48% retention, 4% of revenue, negative economics
>    - Action: Strategic review. Either eliminate or convert to free tier.
>
> ---
>
> ## Action Items
>
> **Immediate (This Quarter):**
> 1. Reduce paid search spend by 50% — Redirect to partner incentives
> 2. Launch developer-focused landing page — Test developer workflow acquisition
> 3. Implement Month 2 retention outreach for Mid-Market — Target 5% retention improvement
>
> **Strategic (Next Quarter):**
> 1. Partner program 3x expansion — Target 40% of new acquisition
> 2. Developer feature sprint — API v2, VS Code extension
> 3. Startup tier decision — Present options to leadership
>
> **Measurement:**
> - Track cohort retention by channel weekly
> - Segment-level NPS quarterly
> - Partner acquisition volume monthly

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Segments too broad | Insufficient granularity | Ask: "Break down [segment] by [additional dimension]" |
| No clear patterns | Data quality or sample size | Check: Are segments mutually exclusive? Are counts sufficient? |
| Can't explain differences | Missing context | Add: "What business changes occurred that might explain [pattern]?" |
| Recommendations too generic | Not tied to specific segments | Ask: "For each recommendation, specify which segment and quantify expected impact" |
| Cohorts not comparable | Different sizes or timing | Normalize: "Compare on per-customer basis, account for seasonality" |

---

## Tips from Experience

1. **Aggregate metrics lie.** Always break down by segment before drawing conclusions.

2. **Watch for Simpson's Paradox.** A metric improving overall can be declining in every segment if mix shifts.

3. **Cohort timing matters.** What happened when each cohort joined explains their behavior.

4. **Best customers define strategy.** Profile your best segment and find more like them.

5. **Kill your losers.** Segments with negative economics drain resources from winners.

6. **Track trends, not snapshots.** A segment improving from bad to medium may be better than one stable at good.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Hidden patterns are surfaced
- [ ] Strategy shifts based on findings
- [ ] Resource allocation changes
- [ ] Segment-specific programs launch
- [ ] Overall metrics improve via segment focus
- [ ] Analysis becomes routine

**Track over time:**
- Segment mix shifts
- Retention by segment trends
- LTV:CAC by channel evolution
- Best customer concentration
- Cohort quality trends

---

## Variations

### Subscription Cohort Analysis
For SaaS/subscription businesses:
```
Focus on:
- Monthly cohort retention curves
- MRR expansion/contraction by cohort
- Upgrade/downgrade patterns
- Seasonal effects on cohorts
- Pricing tier migration

Include: Net Revenue Retention, Gross Dollar Retention by cohort
```

### E-commerce Cohort Analysis
For retail/e-commerce:
```
Focus on:
- Purchase frequency by cohort
- Average order value progression
- Category migration patterns
- Channel acquisition lifetime value
- Seasonal purchase patterns

Include: Repeat purchase rate, Days between purchases
```

### Product Usage Cohort Analysis
For product/engagement analysis:
```
Focus on:
- Feature adoption by cohort
- Usage depth progression
- Aha moment timing
- Power user identification
- Churn predictors from usage

Include: DAU/MAU ratio, Feature adoption curves
```

### Geographic Segment Analysis
For market expansion decisions:
```
Focus on:
- Market-by-market comparison
- Localization impact
- Pricing sensitivity by region
- Support cost variation
- Growth potential by geography

Include: Market penetration, Competitive position
```

---

## Building Your Repeatable System

After several cohort/segment cycles, establish:

1. **Standard segment definitions** across organization
2. **Regular analysis cadence** (monthly or quarterly)
3. **Consistent metrics set** for comparison
4. **Trend tracking** over time
5. **Action linkage** from insights to initiatives

**Sample Setup:**
```
cohort-segment-analysis/
├── quarterly/
│   ├── q3-2024-analysis.md
│   ├── q2-2024-analysis.md
│   └── [quarter by quarter]
├── data/
│   ├── cohort-retention.csv
│   ├── segment-metrics.csv
│   └── channel-performance.csv
├── segments/
│   ├── enterprise-playbook.md
│   ├── mid-market-playbook.md
│   └── [by segment]
├── reference/
│   ├── segment-definitions.md
│   └── benchmark-targets.md
└── presentations/
    └── q3-cohort-review.pptx
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**group by meaningful dimension → compare metrics → identify patterns → target actions**—applies broadly:

| Role | Application |
|------|-------------|
| **Marketing** | Channel performance, campaign cohorts |
| **Product** | Feature adoption, user segments |
| **Customer Success** | Health score segments, lifecycle |
| **Finance** | Revenue cohorts, customer economics |
| **HR** | Hire cohorts, employee segments |
| **Sales** | Deal segments, rep cohorts |

---

## Next Steps

1. **Define your segments:** What dimensions matter for your business?
2. **Extract data:** Cohort retention, segment metrics
3. **Note context:** What business events explain patterns?
4. **Run analysis:** Use this recipe
5. **Validate findings:** Check against intuition and frontline knowledge
6. **Take action:** Resource allocation, program design

---

*Recipe #56 of 100 in the Claude Code Knowledge Worker Recipe Collection*
