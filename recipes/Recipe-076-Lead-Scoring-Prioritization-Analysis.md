# Lead Scoring and Prioritization Analysis

**Recipe #76: From Gut-Feel Lead Routing to Data-Driven Scoring Models**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 45 minutes (first time) / 20 minutes (repeat) | 2-4 hours per analysis | Advanced | Marketing Ops, Sales Ops, Demand Generation |

---

## The Problem

Sales teams waste time chasing leads that never convert while high-potential prospects go cold. Without effective lead scoring, every lead gets equal treatment—or worse, reps rely on gut instinct. Building and refining scoring models requires analyzing historical conversion data, identifying predictive factors, weighting criteria appropriately, and continuously tuning based on results. Most organizations either have no scoring or outdated models that don't reflect current buyer behavior.

**Pain Points:**
- Sales reps spend equal effort on low-quality and high-quality leads
- High-potential leads sit unworked while reps chase dead ends
- Historical conversion analysis is time-consuming and complex
- Existing scoring models become stale and inaccurate over time
- Behavioral signals are underweighted compared to firmographic data
- Sales complains about "junk leads" but can't quantify the problem
- No systematic way to identify which factors actually predict conversion

---

## The Outcome

A data-driven lead scoring framework with clear criteria, appropriate weighting, and prioritization logic—enabling sales and marketing to focus on leads most likely to convert and optimize resource allocation for maximum pipeline efficiency.

**What You'll Have When Done:**
- Comprehensive analysis of which factors predict conversion
- Recommended scoring model with point values and rationale
- Clear MQL and SQL threshold recommendations based on data
- Prioritization framework beyond simple score thresholds
- Implementation plan for your marketing automation platform
- Success metrics and monitoring approach

---

## When to Use This Recipe

**Good Fit:**
- Building lead scoring from scratch
- Auditing existing scoring model effectiveness
- After significant changes in ICP or product positioning
- When conversion rates are declining unexpectedly
- Quarterly or annual scoring model tuning
- New market segment expansion requiring updated criteria
- After marketing channel changes that affect lead quality
- Sales complaining about lead quality with no data to support changes

**Not a Good Fit:**
- Very early stage with less than 6 months of lead data
- Extremely simple sales process where all leads are qualified
- When you lack conversion outcome data (won/lost tracking)
- Sales process is primarily inbound/transactional with no scoring needed

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have historical lead data from at least 6 months
- [ ] Conversion outcome data is available (won/lost/no decision)
- [ ] Lead attributes are tracked (firmographic, demographic, behavioral)
- [ ] Marketing engagement data is accessible (if available)
- [ ] Sales feedback on lead quality has been collected
- [ ] Current scoring model documentation (if one exists)
- [ ] Ideal customer profile is documented
- [ ] You have 60-90 minutes for initial analysis

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Analyze historical lead data to identify predictive conversion factors
- Calculate correlation between attributes and conversion outcomes
- Recommend scoring criteria and appropriate point weights
- Evaluate existing scoring model effectiveness against actual data
- Generate implementation recommendations for marketing automation
- Create prioritization frameworks that go beyond simple scores

**Where Human Judgment Is Essential:**
- Validating that data quality is sufficient for analysis
- Deciding which factors are strategically important vs. statistically significant
- Setting business constraints (acceptable MQL volume, sales capacity)
- Reviewing recommendations with sales for real-world sanity check
- Determining implementation timeline and change management approach

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Historical Lead Data | Summary of total leads, conversions, attributes available | Understanding data scope and quality |
| Conversion Analysis | Tables showing conversion rates by segment, source, behavior | Identifying predictive patterns |
| Current Scoring Model | Existing point values and thresholds | Evaluating what's working and what's not |
| Business Context | Goals, constraints, current challenges | Framing recommendations appropriately |
| Behavioral Data | Engagement metrics and conversion correlation | Finding high-intent signals |

**Sample Input:** *(see Example Inputs section for detailed examples)*

The recipe includes comprehensive example inputs showing:
- Lead database summary with attributes
- Conversion data by company size, industry, and source
- Behavioral indicators and their conversion impact
- Current scoring model performance

---

## Step-by-Step Implementation

### Step 1: Prepare Your Inputs
**Time: 15-20 minutes**

Gather your lead data and organize it into clear summaries:
- Export historical lead data with conversion outcomes
- Create conversion tables by key segments
- Document current scoring model (if exists)
- Collect sales feedback themes
- Note any recent business changes affecting leads

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Lead Scoring Analysis Prompt
**Time: 5-8 minutes for Claude to process**

---

**PRIMARY PROMPT: Historical Data Analysis**

```
Claude, I need to analyze our lead data to build/improve our lead scoring model.

Here's our historical data summary:
[PASTE LEAD DATABASE SUMMARY WITH TOTAL LEADS, CONVERSIONS, TIMEFRAME]

Conversion data by segment:
[PASTE CONVERSION TABLES BY COMPANY SIZE, INDUSTRY, SOURCE, ETC.]

Please:
1. Identify which factors most strongly predict conversion
2. Calculate the predictive power of each attribute
3. Flag any surprising patterns
4. Note data quality issues that might affect analysis
5. Suggest additional data points we should track
```

---

### Step 4: Review and Validate
**Time: 10-15 minutes**

**Check immediately:**
- Do the predictive factors align with sales intuition?
- Are there any obvious data quality issues flagged?
- Do conversion lifts make logical sense?

**Spot-check specifics:**
- Verify conversion calculations against your own data
- Confirm that sample sizes are large enough to be meaningful
- Check if any critical attributes are missing from analysis
- Review whether time periods are appropriate (not too old/recent)

---

### Step 5: Refine and Iterate
**Time: 15-20 minutes**

**Prompt: Behavioral Factor Analysis**
```
Based on this behavioral data, identify the strongest predictive factors:

[PASTE BEHAVIORAL ANALYSIS DATA: PRICING PAGE VISITS, CONTENT ENGAGEMENT, EMAIL OPENS, TIME TO ACTION, MULTI-CONTACT SIGNALS]

Please:
1. Rank factors by predictive strength
2. Identify interaction effects (combinations that are stronger)
3. Note factors that don't predict as well as expected
4. Distinguish leading indicators from lagging indicators
5. Recommend thresholds for each factor
```

**Prompt: Evaluate Current Model**
```
Evaluate our current scoring model against actual conversion data:

Current model:
[PASTE EXISTING SCORING MODEL WITH POINT VALUES]

Actual conversions:
[SUMMARY OF WHAT ACTUALLY CONVERTED]

Please assess:
1. Which criteria are over/under-weighted?
2. What factors are missing?
3. Where do false positives come from?
4. Where do false negatives come from?
5. What's the optimal MQL/SQL threshold based on data?
```

**Prompt: Design New Scoring Model**
```
Based on the analysis, design an improved lead scoring model.

Constraints:
- Must be implementable in [MARKETING AUTOMATION PLATFORM NAME]
- Scores should range from 0-100
- Need clear MQL and SQL thresholds
- Must balance volume with quality
- Consider both fit (firmographic/demographic) and engagement (behavioral)

Please provide:
1. Fit scoring criteria with point values
2. Engagement scoring criteria with point values
3. Negative scoring factors (deductions)
4. Score decay rules (for aging leads)
5. MQL and SQL threshold recommendations
6. Rationale for each decision
```

---

### Step 6: Export Final Output
**Time: 5 minutes**

```
Create a final implementation plan for the new scoring model.

Current system: [MARKETING AUTOMATION PLATFORM]
Sales CRM: [CRM SYSTEM]
Team size: [MARKETING OPS RESOURCES]

Include:
1. Technical implementation steps
2. Migration plan from old to new model
3. Testing approach
4. Rollout phases
5. Change management for sales team
6. Success metrics and review cadence
```

---

## Example Output

Below is an abbreviated example of what a well-executed lead scoring analysis looks like:

---

> ### Lead Scoring Analysis & Model Recommendations
>
> ---
>
> #### Executive Summary
>
> **Current State:** Your existing scoring model has a 40% "junk lead" rate according to sales, primarily due to over-weighting firmographic fit and under-weighting behavioral signals.
>
> **Key Findings:**
> 1. **Behavioral signals are stronger predictors than firmographic** - Pricing page visits and demo requests predict conversion 3x better than company size
> 2. **Industry scoring is backwards** - Technology shows lowest conversion despite highest score; Healthcare performs best
> 3. **Missing critical signals** - Multi-contact accounts and recency of engagement are strong predictors not in current model
> 4. **Thresholds are too low** - MQL at 50 points generates volume but not quality; 65+ performs significantly better
>
> **Recommended Changes:**
> - Reweight: Behavioral 60%, Firmographic 25%, Demographic 15%
> - Add: Multi-contact signal, recency scoring, score decay
> - Remove: Technology industry premium (data doesn't support)
> - Threshold: MQL at 65, SQL at 80
>
> **Expected Impact:** Based on historical data, these changes should reduce MQL volume by 25% while improving MQL-to-opportunity rate from 32% to 45%+.
>
> ---
>
> #### Predictive Factor Analysis
>
> | Factor | Without | With | Lift | Predictive Power |
> |--------|---------|------|------|------------------|
> | Demo request | 2.0% | 18.9% | 9.5x | ⭐⭐⭐⭐⭐ |
> | Multi-contact (2+) | 2.8% | 7.8% | 2.8x | ⭐⭐⭐⭐ |
> | Pricing page (3+) | 2.1% | 12.4% | 5.9x | ⭐⭐⭐⭐ |
> | Referral source | 3.0% | 15.0% | 5.0x | ⭐⭐⭐⭐ |
>
> *(Full analysis includes detailed scoring model, threshold recommendations, and implementation plan)*

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Scores cluster at thresholds | Not enough gradation in criteria | Add more scoring tiers; use engagement recency as tiebreaker; implement priority levels within MQL |
| Model doesn't match sales intuition | Different between data and field experience | Review edge cases together; explain the data; consider soft factors not captured; iterate and adjust |
| Insufficient historical data | Small sample sizes or short timeframe | Use longer time periods; combine similar categories; apply industry benchmarks; start simpler and add complexity |
| Gaming of scoring system | People or systems artificially inflate scores | Focus on harder-to-fake behavioral signals; weight intent actions higher; audit suspicious patterns; add negative scoring |
| Model works initially but degrades | Market or buyer behavior changed | Set up quarterly review cadence; monitor conversion rates by score band; adjust weights as needed |
| Too many factors to evaluate | Analysis paralysis from complex data | Focus on top 5-7 factors first; add complexity iteratively; accept that good enough beats perfect |

---

## Tips from Experience

1. **Start simple and iterate.** Better to have a basic model that works than a complex one nobody trusts. Launch with core factors, prove it works, then add sophistication.

2. **Weight behavior over demographics.** What people do predicts better than who they are. Demo requests and pricing page visits trump company size and title in most B2B scenarios.

3. **Include sales in design from day one.** Their input improves the model AND ensures adoption. A technically perfect model that sales rejects is worthless.

4. **Plan for decay from the beginning.** Scores without decay create false positives. A lead that was hot 6 months ago isn't hot today—build decay rules into the initial model.

5. **Document your logic extensively.** Future you (and your successor) will need to understand why decisions were made. Clear documentation enables confident iteration.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] MQL-to-opportunity conversion rate improves by 10+ percentage points
- [ ] Sales acceptance rate of MQLs increases (fewer "junk" complaints)
- [ ] Average lead score of won deals is higher than lost deals
- [ ] Model can explain 60%+ of conversion variance
- [ ] Sales and marketing agree the model reflects reality

**Track over time:**
- MQL-to-opportunity conversion rate (primary metric)
- Sales acceptance rate of MQLs
- Average score of won vs. lost deals (model validation)

---

## Variations

### Variation 1: Account-Based Scoring
Aggregate individual lead scores to account level for account-based marketing prioritization.
```
Adapt the scoring prompt to include:
"Create account-level scoring by aggregating individual contacts. Factor in number of engaged contacts, seniority distribution, and account-wide engagement patterns."
```

### Variation 2: Product-Led Growth Scoring
Incorporate in-product usage signals for product-led growth models.
```
Add to your behavioral analysis:
"Include product usage data: feature adoption, frequency of use, depth of engagement, team expansion signals. Weight these as heavily as traditional behavioral indicators."
```

### Variation 3: Expansion/Upsell Scoring
Score existing customers for upsell and cross-sell propensity.
```
Modify the scoring model prompt:
"Design an expansion scoring model for existing customers. Consider: product usage trends, support engagement, renewal proximity, org changes, and historical expansion patterns."
```

---

## Building Your Repeatable System

After using this recipe 2-3 times, establish your system:

1. **Quarterly Scoring Review Calendar.** Schedule recurring scoring model reviews every quarter. Don't wait for problems—proactive tuning maintains model accuracy.

2. **Automated Performance Dashboards.** Build dashboards that track MQL-to-opportunity conversion, score distribution, and sales acceptance rate automatically. Surface issues early.

3. **Feedback Loop with Sales.** Create a standing process for sales to flag "great lead, low score" and "terrible lead, high score" examples. These edge cases inform model improvements.

4. **Version Control for Models.** Document every scoring model change with version numbers, dates, rationale, and expected impact. Track actual outcomes against predictions.

**Sample Folder Structure:**
```
lead-scoring/
├── models/
│   ├── v1.0-baseline-model.md
│   ├── v2.0-behavioral-reweight.md
│   └── current-model.md
├── analysis/
│   ├── 2024-Q4-scoring-analysis.md
│   └── historical-conversion-data.csv
├── performance/
│   └── model-performance-tracking.xlsx
└── documentation/
    └── implementation-guide.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**analyzing historical outcomes to build predictive scoring models**—applies broadly:

| Role | Application |
|------|-------------|
| **Customer Success** | Health scoring to predict churn or expansion readiness |
| **Support** | Ticket prioritization based on severity prediction |
| **Product** | Feature request prioritization based on value/adoption signals |
| **HR** | Candidate scoring for hiring pipeline efficiency |
| **Finance** | Credit scoring or payment risk assessment |

---

## Next Steps

1. **This week:** Run the analysis on your lead data using this recipe's prompts. Get initial results.
2. **Track your results:** Set up conversion rate tracking by score band to validate model performance.
3. **Iterate:** Share findings with sales, collect feedback, refine the model based on their input.
4. **Share:** Present recommendations to leadership with expected impact and implementation plan.

---

*Recipe #76 of 100 in the Claude Code Knowledge Worker Recipe Collection*
