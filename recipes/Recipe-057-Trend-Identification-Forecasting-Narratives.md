# Trend Identification and Forecasting Narratives

**Recipe #57: Turn Historical Patterns into Forward-Looking Stories**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 5 minutes (first time) / 3 minutes (repeat) | 2-4 hours per forecast narrative | Intermediate | Finance, Strategy, Analysts, Planning |

---

## The Problem

Numbers tell you what happened; they don't tell you what's coming or why it matters. Forecasts come with uncertainty but get presented as certainties. Trends are visible in data but invisible in reports. Leaders make decisions based on single-point forecasts when they should understand ranges. The person presenting the forecast often can't explain the assumptions or articulate why this future is more likely than alternatives.

**Pain Points:**
- Forecasts presented without narrative context
- Single-point estimates hide uncertainty
- Trends visible in spreadsheets but not communicated
- Can't explain assumptions behind projections
- Historical patterns not connected to future expectations
- Scenarios not developed or presented
- "What if we're wrong?" never addressed

---

## The Outcome

Compelling forecast narratives that explain what the data shows, what it suggests about the future, and what could change the outlook. Multiple scenarios with probabilities. Clear articulation of assumptions and risks. Stories that help leaders make decisions, not just numbers that fill slides.

**What You'll Have When Done:**
- Trend identification and explanation
- Forecast narrative with context
- Scenario analysis (base, upside, downside)
- Assumption documentation
- Risk factors and sensitivities
- Decision-relevant insights
- Executive-ready presentation

---

## When to Use This Recipe

**Good Fit:**
- Annual planning and budgeting
- Quarterly forecast updates
- Market analysis and projections
- Demand forecasting narratives
- Financial modeling communication
- Strategic planning inputs
- Board presentations on outlook

**Not a Good Fit:**
- Detailed statistical forecasting (need specialized tools)
- Real-time predictions
- Machine learning model building
- Forecasts requiring complex algorithms

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have historical time-series data
- [ ] You have or can develop forecast numbers
- [ ] You understand the business context
- [ ] You have 30-60 minutes for comprehensive narrative

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Identifies patterns in historical data
- Generates narrative explanations
- Creates scenario frameworks
- Documents assumptions clearly
- Structures forecast communication
- Highlights risks and sensitivities

**Where Human Judgment Is Essential:**
- Validating trend identification
- Setting forecast assumptions
- Determining scenario probabilities
- Understanding market dynamics
- Making final forecasts
- Approving narratives

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Historical data | Monthly metrics, 2-3 years | Trend identification |
| Forecast numbers | Projected values | Narrative foundation |
| Assumptions | Growth rates, drivers | Scenario parameters |
| Context | Market conditions | Interpretation framework |
| Risks | Known uncertainties | Sensitivity analysis |

**Sample Input:**
```
Trend and Forecast Narrative Request

METRIC: Monthly Recurring Revenue (MRR)
COMPANY: CloudSync Pro
PERIOD: Historical (24 months) + Forecast (12 months)

HISTORICAL DATA (Monthly MRR in $000s):
| Month | MRR | MoM Growth | YoY Growth | New | Expansion | Churn |
|-------|-----|------------|------------|-----|-----------|-------|
| Nov 22 | 245 | 2.5% | - | 28 | 12 | -18 |
| Dec 22 | 251 | 2.4% | - | 25 | 14 | -19 |
| Jan 23 | 262 | 4.4% | - | 32 | 15 | -16 |
| Feb 23 | 275 | 5.0% | - | 35 | 16 | -18 |
| Mar 23 | 290 | 5.5% | - | 38 | 18 | -21 |
| Apr 23 | 302 | 4.1% | - | 35 | 17 | -20 |
| May 23 | 315 | 4.3% | - | 36 | 19 | -22 |
| Jun 23 | 328 | 4.1% | - | 38 | 18 | -23 |
| Jul 23 | 339 | 3.4% | - | 34 | 17 | -24 |
| Aug 23 | 348 | 2.7% | - | 32 | 16 | -25 |
| Sep 23 | 358 | 2.9% | - | 33 | 17 | -24 |
| Oct 23 | 368 | 2.8% | - | 34 | 18 | -26 |
| Nov 23 | 378 | 2.7% | 54% | 35 | 17 | -27 |
| Dec 23 | 388 | 2.6% | 55% | 36 | 18 | -28 |
| Jan 24 | 401 | 3.4% | 53% | 40 | 20 | -27 |
| Feb 24 | 415 | 3.5% | 51% | 42 | 21 | -28 |
| Mar 24 | 428 | 3.1% | 48% | 41 | 20 | -29 |
| Apr 24 | 438 | 2.3% | 45% | 38 | 18 | -28 |
| May 24 | 448 | 2.3% | 42% | 38 | 19 | -29 |
| Jun 24 | 458 | 2.2% | 40% | 39 | 18 | -29 |
| Jul 24 | 470 | 2.6% | 39% | 42 | 20 | -30 |
| Aug 24 | 485 | 3.2% | 39% | 48 | 22 | -30 |
| Sep 24 | 502 | 3.5% | 40% | 52 | 24 | -31 |
| Oct 24 | 520 | 3.6% | 41% | 55 | 26 | -33 |

PRELIMINARY FORECAST:
| Month | Base Case | Upside | Downside |
|-------|-----------|--------|----------|
| Nov 24 | 538 | 550 | 525 |
| Dec 24 | 555 | 575 | 535 |
| Jan 25 | 575 | 605 | 545 |
| Feb 25 | 595 | 635 | 555 |
| Mar 25 | 615 | 665 | 565 |
| Apr 25 | 635 | 695 | 575 |
| May 25 | 655 | 725 | 585 |
| Jun 25 | 675 | 755 | 595 |
| Jul 25 | 695 | 785 | 605 |
| Aug 25 | 720 | 820 | 615 |
| Sep 25 | 745 | 855 | 625 |
| Oct 25 | 770 | 890 | 635 |

KEY ASSUMPTIONS:
Base Case:
- MoM growth normalizes at 3.0-3.5%
- New customer acquisition continues current trajectory
- Expansion rate stable at 5% of base
- Churn stabilizes at 6%
- No major market disruption

Upside:
- Enterprise deal pipeline converts (3 deals, $150K+ combined)
- Partner channel scales to 40% of new business
- Price increase (10%) holds with no churn impact
- Market tailwind from competitor issues

Downside:
- Economic slowdown impacts SMB segment
- Competitor launches aggressive pricing
- Key enterprise renewals at risk
- New customer acquisition drops 20%

KNOWN CONTEXT:
- Series B funding closed August 2024 ($25M)
- Enterprise sales team expanding (3 new reps)
- Partner program launched June 2024
- New pricing effective January 2025 (+10%)
- Major competitor (RivalSync) acquired, integration uncertainty

AUDIENCE: Board presentation, quarterly update
```

---

## Step-by-Step Implementation

### Step 1: Gather Historical Data and Forecast
**Time: 10-15 minutes**

Compile:
- 24+ months of historical data
- Component breakdown (new, expansion, churn)
- Preliminary forecast numbers
- Key assumptions
- Known risks and opportunities

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Trend and Forecast Prompt
**Time: 5-10 minutes for Claude to process**

---

**PRIMARY PROMPT: Trend Identification and Forecast Narrative**

```
Please analyze this historical data and create a forecast narrative.

METRIC: [Metric name]
BUSINESS CONTEXT: [Company/product]
PERIOD: [Historical period] + [Forecast period]

HISTORICAL DATA:
[Paste time-series data]

FORECAST SCENARIOS:
[Paste forecast numbers by scenario]

ASSUMPTIONS:
[Key assumptions by scenario]

KNOWN CONTEXT:
[Market conditions, company events, risks]

ANALYSIS REQUIREMENTS:

1. EXECUTIVE SUMMARY
   - Where we've been (trend summary)
   - Where we're headed (forecast summary)
   - Confidence level
   - Key assumption that matters most
   - Biggest risk to forecast

2. HISTORICAL TREND ANALYSIS

   **Overall Pattern:**
   [Describe the shape of the historical data]

   **Growth Trajectory:**
   | Period | Average Growth | Trend | Driver |
   |--------|---------------|-------|--------|
   [Break into meaningful periods]

   **Key Inflection Points:**
   - [Date]: [What changed and why]

   **Component Analysis:**
   | Component | Trend | Impact | Outlook |
   |-----------|-------|--------|---------|
   [New, expansion, churn, etc.]

   **Seasonality:**
   [Any seasonal patterns observed]

   **What the History Tells Us:**
   [Key takeaways from historical analysis]

3. TREND IDENTIFICATION

   **Primary Trends:**
   1. [Trend 1]: [Description, evidence, implication]
   2. [Trend 2]: [Description, evidence, implication]

   **Emerging Patterns:**
   - [Pattern]: [Early signal, potential significance]

   **Trends to Watch:**
   - [Pattern]: [Why it matters]

4. FORECAST NARRATIVE

   **Base Case Story:**
   [Narrative description of what happens in base case]

   Key Numbers:
   - End of period: [Value]
   - Growth rate: [X%] MoM, [Y%] annual
   - Trajectory: [Accelerating/Linear/Decelerating]

   Why This Outcome:
   - [Reason 1]
   - [Reason 2]

   What Must Be True:
   - [Assumption 1]
   - [Assumption 2]

5. SCENARIO ANALYSIS

   **Upside Case ([X]% probability)**

   Story: [What happens]
   End of period: [Value] ([+X%] vs base)

   Triggers:
   - [What would cause this]

   Early Indicators:
   - [How we'd know we're on this path]

   **Downside Case ([X]% probability)**

   Story: [What happens]
   End of period: [Value] ([-X%] vs base)

   Triggers:
   - [What would cause this]

   Early Indicators:
   - [How we'd know we're on this path]

6. ASSUMPTION SENSITIVITY

   | Assumption | Base Value | +/- Change | Forecast Impact |
   |------------|------------|------------|-----------------|
   [Rank by sensitivity]

   Most Critical Assumption:
   [Which assumption matters most and why]

7. RISKS TO FORECAST

   **Internal Risks:**
   - [Risk 1]: [Probability] — [Impact if realized]

   **External Risks:**
   - [Risk 1]: [Probability] — [Impact if realized]

   **Black Swan Potential:**
   - [Low probability but high impact scenarios]

8. OPPORTUNITIES NOT IN FORECAST

   Upside not fully captured:
   - [Opportunity 1]: [Potential impact]

9. COMPARISON TO ALTERNATIVES

   How this forecast compares:
   - vs. last forecast: [Better/Worse/Same]
   - vs. market expectations: [Above/Below/In-line]
   - vs. company goals: [Tracking/Gap]

10. DECISION-RELEVANT INSIGHTS

    What leaders should take away:
    1. [Insight 1]: [Implication for decisions]
    2. [Insight 2]: [Implication for decisions]

    Questions this forecast raises:
    - [Question 1]
    - [Question 2]

11. RECOMMENDED ACTIONS

    To achieve forecast:
    - [Action 1]

    To capture upside:
    - [Action 1]

    To mitigate downside:
    - [Action 1]

Write narrative that explains, not just describes. Make the story clear.
```

---

### Step 4: Validate Trends and Assumptions
**Time: 10-15 minutes**

Review:
- Are identified trends accurate?
- Do assumptions seem reasonable?
- Are scenarios comprehensive?
- Is sensitivity analysis correct?

---

### Step 5: Refine the Narrative
**Time: 5-10 minutes**

```
Update the forecast narrative with these refinements:

TREND ADJUSTMENTS:
- [Trend X] should be characterized as: [Refinement]

ASSUMPTION UPDATES:
- [Assumption X] more likely at: [Value]

SCENARIO REFINEMENTS:
- Upside probability is more like: [X%]
- Add this downside trigger: [Trigger]

ADDITIONAL CONTEXT:
- Leaders will want to know: [Information]
- Politically sensitive topic: [Area]
```

---

### Step 6: Generate Final Deliverables
**Time: 5 minutes**

```
Create final forecast package:

1. EXECUTIVE SUMMARY (one page)
   - Headline forecast number
   - Range (low-high)
   - Key trend
   - Primary assumption
   - Main risk
   - Recommended action

2. FULL NARRATIVE
   Complete analysis as developed

3. BOARD PRESENTATION OUTLINE
   Slide structure:
   - Slide 1: Headline and range
   - Slide 2: Historical context
   - Slide 3: Scenarios
   - Slide 4: Key assumptions and risks
   - Slide 5: What we're watching

4. FAQ DOCUMENT
   Anticipated questions and answers:
   - Q: [Likely question]
   - A: [Prepared answer]
```

---

## Example Output

Below is an abbreviated trend and forecast narrative example:

---

> **MRR FORECAST NARRATIVE**
>
> **CloudSync Pro | Q4 2024 Board Update**
>
> ---
>
> ## Executive Summary
>
> CloudSync Pro is entering a growth acceleration phase after 18 months of maturation. MRR is forecast to reach **$770K by October 2025** (base case), representing **48% YoY growth** and a return to the growth rates last seen in early 2023.
>
> **Where We've Been:** After rapid early growth (5%+ MoM in early 2023), growth normalized to 2.5-3% MoM through mid-2024 as the business scaled and churn increased proportionally.
>
> **Where We're Headed:** Series B investment, enterprise sales expansion, and partner channel traction are inflecting growth back upward. The past three months show acceleration (2.6% → 3.6% MoM).
>
> **Confidence Level:** Medium-High for base case. Recent acceleration provides evidence, but must be sustained.
>
> **Key Assumption:** Enterprise pipeline conversion. Three large deals representing $150K+ combined MRR must close for upside; losing them doesn't cause downside but caps growth.
>
> **Biggest Risk:** Economic headwinds impacting SMB segment (40% of customer base). A recession scenario could trigger churn spike.
>
> ---
>
> ## Historical Trend Analysis
>
> ### Overall Pattern
>
> The MRR trajectory shows a classic growth curve: rapid acceleration in 2023 (product-market fit scaling), normalization in mid-2024 (scale challenges), and early signs of re-acceleration in late 2024 (investment unlocking).
>
> ### Growth Trajectory
>
> | Period | Avg MoM Growth | Trend | Primary Driver |
> |--------|---------------|-------|----------------|
> | Nov 22 - Mar 23 | 4.0% | Accelerating | PMF momentum |
> | Apr 23 - Sep 23 | 3.3% | Decelerating | Scale friction |
> | Oct 23 - Jun 24 | 2.6% | Stabilizing | Maturation |
> | Jul 24 - Oct 24 | 3.2% | Accelerating | Investment impact |
>
> ### Key Inflection Points
>
> 1. **March 2023 (5.5% MoM):** Peak growth month. Product launch + marketing push. Unsustainable but set high-water mark.
>
> 2. **August 2023 (2.7% MoM):** Growth trough. Churn caught up to acquisition. Team capacity constrained growth.
>
> 3. **July 2024 (2.6% → 3.2% acceleration):** Series B closed. Enterprise team hired. Partner channel launched. Inflection back upward.
>
> ### Component Analysis
>
> | Component | Trend | Recent Change | Outlook |
> |-----------|-------|---------------|---------|
> | New MRR | Stable → Growing | +30% (Jul-Oct) | Positive (Enterprise + Partner) |
> | Expansion | Steady | Slight uptick | Positive (pricing + upsell) |
> | Churn | Growing with base | Stable rate | Watchpoint |
>
> **Net Revenue Retention:** 108% (stable). Expansion exceeds churn at customer level. This is a key strength to maintain.
>
> ### What History Tells Us
>
> 1. **Growth at scale is harder.** The 5% months aren't coming back without step-change.
> 2. **Churn scales proportionally.** Must continue improving retention as base grows.
> 3. **Investment accelerates growth.** Post-Series B trajectory validates thesis.
> 4. **Seasonality is minimal.** January shows slight uptick; otherwise consistent.
>
> ---
>
> ## Primary Trends
>
> ### Trend 1: Growth Re-Acceleration
>
> **Pattern:** After 12 months of 2.3-2.8% MoM growth, the past 4 months show consistent acceleration (2.6% → 3.2% → 3.5% → 3.6%).
>
> **Evidence:**
> - New customer acquisition up 30% (Jul-Oct vs Apr-Jun)
> - Expansion MRR growing faster than base
> - Churn rate stabilized despite larger base
>
> **Implication:** If sustained, we're entering a new growth phase. The question is whether this is structural (Series B capacity) or temporary (pent-up demand).
>
> ### Trend 2: Enterprise Traction
>
> **Pattern:** Average deal size increasing. Enterprise segment growing from 8% to 12% of new MRR.
>
> **Evidence:**
> - Three enterprise reps hired (Aug-Sep)
> - Pipeline value up 2.5x
> - Two enterprise deals closed in October
>
> **Implication:** Enterprise success would fundamentally change unit economics and growth trajectory. This is the upside driver.
>
> ### Trend 3: Channel Diversification
>
> **Pattern:** Partner referrals growing from 0% to 18% of new customers since June launch.
>
> **Evidence:**
> - 45 new partners onboarded
> - Partner-referred customers show higher LTV
> - Channel is scaling faster than direct sales at current stage
>
> **Implication:** Scalable acquisition channel developing. Could reach 40% of new business by end of 2025.
>
> ---
>
> ## Forecast Narrative
>
> ### Base Case Story
>
> CloudSync Pro continues its growth re-acceleration through 2025, reaching **$770K MRR by October 2025** (48% YoY growth).
>
> The story: Series B investment translates to sustained growth. The enterprise team hits stride in Q1, contributing 2-3 medium deals per quarter. Partner channel scales to 30% of new business. Churn holds at 6% as customer success investments mature. The January price increase adds 8% to existing base with minimal churn impact.
>
> This isn't explosive growth—it's disciplined scaling. Monthly growth averages 3.3% MoM, consistent with recent trajectory.
>
> **Key Numbers:**
> - October 2025 MRR: $770K
> - YoY Growth: 48%
> - MoM Average: 3.3%
> - Exit ARR Run Rate: $9.2M
>
> **Why This Outcome:**
> 1. Recent acceleration (3.5%+ MoM) provides momentum
> 2. Enterprise investment should yield returns in 2-3 quarters
> 3. Partner channel is proven and scaling
> 4. Net revenue retention (108%) means base compounds
>
> **What Must Be True:**
> 1. Enterprise pipeline converts at 30%+ (historical: 25%)
> 2. Partner channel continues scaling (currently 18% → target 30%)
> 3. Churn doesn't spike despite price increase
> 4. No major competitive disruption
>
> ---
>
> ## Scenario Analysis
>
> ### Upside Case (25% Probability)
>
> **October 2025 MRR: $890K** (+16% vs base)
>
> **Story:** Everything clicks. The three enterprise pipeline deals close in Q1 ($150K+ combined). Partner channel exceeds expectations, reaching 40% of new business. Price increase holds with zero incremental churn. RivalSync acquisition creates market chaos, driving customers to CloudSync.
>
> **Triggers:**
> - Enterprise deals close Q1
> - Partner channel hits 40% by June
> - Price increase shows no churn impact by March
> - RivalSync integration issues make news
>
> **Early Indicators (by Feb 2025):**
> - Two enterprise deals closed
> - Partner contribution at 25%+
> - January churn < 6.5%
>
> ### Downside Case (20% Probability)
>
> **October 2025 MRR: $635K** (-18% vs base)
>
> **Story:** Economic headwinds bite. SMB segment (40% of base) tightens budgets. Enterprise deals slow as procurement freezes. Price increase triggers 15% churn in Q1. New customer acquisition drops 25% as companies cut software spend.
>
> **Triggers:**
> - Recession indicators worsen
> - Enterprise deals push to H2 or cancel
> - SMB churn spikes above 8%
> - Competitor aggressive pricing war
>
> **Early Indicators (by Feb 2025):**
> - January churn > 8%
> - Enterprise pipeline deals stalling
> - SMB trials converting < 15%
>
> ---
>
> ## Assumption Sensitivity
>
> | Assumption | Base Value | Sensitivity | Impact Range |
> |------------|------------|-------------|--------------|
> | Monthly growth rate | 3.3% MoM | ±0.5% | $700K - $840K |
> | Churn rate | 6.0% | ±1.5% | $710K - $830K |
> | Enterprise conversion | 30% | ±15% | $740K - $810K |
> | Price increase impact | +8% MRR | Full vs none | $720K - $770K |
>
> **Most Critical Assumption:** Monthly growth rate. Every 0.5% change in sustained MoM growth equals $70K in year-end MRR. This is why the recent acceleration trend matters so much—if it sustains at 3.5%, we beat base case; if it falls to 2.5%, we miss significantly.
>
> ---
>
> ## Risks to Forecast
>
> ### Internal Risks
>
> | Risk | Probability | Impact | Mitigation |
> |------|-------------|--------|------------|
> | Enterprise sales execution | 30% | -$50K MRR | Pipeline reviews, coaching |
> | Price increase backlash | 20% | -$40K MRR | Grandfathering, value communication |
> | Key hire departures | 15% | -$30K MRR | Retention packages |
>
> ### External Risks
>
> | Risk | Probability | Impact | Mitigation |
> |------|-------------|--------|------------|
> | Economic recession | 25% | -$100K MRR | SMB to annual billing |
> | Competitor price war | 20% | -$60K MRR | Value differentiation |
> | RivalSync emerges stronger | 15% | -$40K MRR | Accelerate enterprise |
>
> ### Black Swan
>
> - **Major security breach:** Low probability but existential impact. Investment in security pays insurance value.
>
> ---
>
> ## Decision-Relevant Insights
>
> **What Leaders Should Take Away:**
>
> 1. **Growth is re-accelerating—this is real.** Four consecutive months of improving growth, driven by identifiable investments (Enterprise, Partner). The question isn't "is this happening" but "will it sustain?"
>
> 2. **Enterprise is the upside lever.** Base case includes modest enterprise contribution. Full pipeline conversion would add $100K+ to year-end MRR. This is where incremental investment could pay off.
>
> 3. **The price increase is a calculated risk.** +$40K benefit vs -$40K churn risk if it goes wrong. We're betting on value delivery. January churn will be the signal.
>
> 4. **Downside is manageable but not trivial.** A recession scenario takes us from $770K to $635K—still 22% YoY growth, but significantly below plan.
>
> ---
>
> ## Recommended Actions
>
> **To Achieve Base Case:**
> - Sustain current sales and marketing execution
> - Close 2 of 3 enterprise pipeline deals
> - Scale partner channel to 30%
>
> **To Capture Upside:**
> - Add one enterprise rep in Q1 (ahead of plan)
> - Increase partner incentives to accelerate scaling
> - Execute competitor win-back campaign during RivalSync uncertainty
>
> **To Mitigate Downside:**
> - Push annual billing hard in Q4 (locks in revenue)
> - Build enterprise segment to offset SMB risk
> - Prepare recession playbook (pricing flexibility, retention focus)

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Trends too obvious | Surface-level analysis | Ask: "What's the second-order trend? What does this trend imply about underlying dynamics?" |
| Forecast seems arbitrary | Disconnected from trends | Ask: "Connect each forecast scenario explicitly to the trends identified" |
| Scenarios too similar | Narrow range | Ask: "What would have to happen for this forecast to be completely wrong? Include that scenario." |
| No actionable insight | Academic analysis | Ask: "For each finding, add: What decision should leadership make based on this?" |
| Assumptions buried | Not highlighted | Ask: "Rank assumptions by sensitivity. What single assumption would change this forecast most?" |

---

## Tips from Experience

1. **Ranges beat point estimates.** Leaders understand uncertainty when you show it clearly.

2. **Name your scenarios.** "Economic headwind case" is more memorable than "Downside case."

3. **Connect past to future.** The best forecast narratives explain why the future will differ from the past.

4. **Make assumptions auditable.** Anyone should be able to understand and challenge your assumptions.

5. **Define early indicators.** How will you know which scenario is playing out?

6. **Include what's NOT in the forecast.** Upside you haven't captured is a strategic opportunity.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Forecasts are presented with scenarios, not single points
- [ ] Leadership asks better questions (about assumptions, not just numbers)
- [ ] Early indicators are monitored
- [ ] Forecast accuracy improves over time
- [ ] Decisions account for uncertainty
- [ ] Assumptions are explicitly revisited

**Track over time:**
- Forecast accuracy (actual vs. predicted)
- Scenario accuracy (which scenario played out)
- Assumption accuracy (were assumptions validated)
- Time to create forecast narrative
- Leadership confidence in forecasts

---

## Variations

### Financial Forecast Narrative
For P&L and balance sheet projections:
```
Create forecast narrative for financial projections:
- Revenue composition by segment
- Cost structure evolution
- Margin trajectory
- Cash flow implications
- Key financial ratios
- Investment requirements

Include: Variance to prior forecast, variance to budget
```

### Demand Forecast Narrative
For operations and supply chain:
```
Create demand forecast narrative:
- Volume projections by product/SKU
- Seasonality patterns
- Channel mix shifts
- Capacity implications
- Inventory recommendations
- Risk factors (supply chain, demand)

Include: Service level implications, safety stock recommendations
```

### Market Forecast Narrative
For market analysis and strategy:
```
Create market forecast narrative:
- Market size trajectory
- Share projections
- Competitive dynamics
- Segment growth rates
- Disruption scenarios
- Entry/exit implications

Include: TAM/SAM/SOM evolution, competitive response scenarios
```

### Headcount Forecast Narrative
For HR and workforce planning:
```
Create workforce forecast narrative:
- Headcount projections by function
- Hiring velocity requirements
- Attrition assumptions
- Skill mix evolution
- Cost implications
- Scenario planning (fast growth, hiring freeze)

Include: Recruiter capacity, time-to-fill assumptions
```

---

## Building Your Repeatable System

After several forecast cycles, establish:

1. **Standard data structure** for historical input
2. **Consistent scenario framework** (base, upside, downside)
3. **Assumption tracking** over time
4. **Accuracy measurement** to improve future forecasts
5. **Regular cadence** for forecast updates

**Sample Setup:**
```
forecast-narratives/
├── quarterly/
│   ├── q4-2024-mrr-forecast.md
│   ├── q3-2024-mrr-forecast.md
│   └── [quarter by quarter]
├── data/
│   ├── historical-mrr.csv
│   └── forecast-models/
├── assumptions/
│   ├── q4-2024-assumptions.md
│   └── assumption-tracking.md
├── accuracy/
│   └── forecast-vs-actual.md
└── presentations/
    └── board-forecast-deck.pptx
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**identify trends → build scenarios → document assumptions → communicate uncertainty**—applies broadly:

| Role | Application |
|------|-------------|
| **Finance** | Budget, revenue, cost projections |
| **Sales** | Pipeline, quota, territory forecasts |
| **Operations** | Demand, capacity, resource planning |
| **Marketing** | Lead, conversion, attribution projections |
| **Strategy** | Market, competitive, growth scenarios |
| **HR** | Headcount, attrition, hiring forecasts |

---

## Next Steps

1. **Gather historical data:** 24+ months of time-series
2. **Develop forecast scenarios:** Base, upside, downside
3. **Document assumptions:** What must be true for each scenario
4. **Generate narrative:** Use this recipe
5. **Validate with stakeholders:** Are assumptions reasonable?
6. **Present and monitor:** Share forecast, track early indicators

---

*Recipe #57 of 100 in the Claude Code Knowledge Worker Recipe Collection*
