# Budget Scenario Modeling and Narrative Generation

**Recipe #16: From Spreadsheets to Strategic Budget Stories**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 15 minutes (first time) / 10 minutes (repeat) | 4-8 hours per planning cycle | Intermediate | Finance, Executives, Department Heads, Budget Owners |

---

## The Problem

Budget planning involves juggling multiple scenarios—what if revenue is 10% higher? What if we cut costs by 15%? What if we delay that initiative?—across dozens of line items. You build spreadsheets, but explaining the trade-offs to stakeholders requires translating numbers into narrative. The CFO asks "what happens if we cut marketing by 20%?" and you need to articulate not just the numbers but the business implications.

**Pain Points:**
- Multiple scenarios to model and keep straight
- Spreadsheets don't tell the strategic story
- Executives want implications, not just numbers
- Trade-off analysis requires narrative explanation
- Sensitivity analysis is time-consuming
- Same questions asked repeatedly need fresh explanations

---

## The Outcome

Clear budget scenario comparisons with narrative explanations of trade-offs, implications, and recommendations. Numbers are translated into business impact stories that executives can understand and act upon. Scenario modeling becomes a conversation tool, not just a calculation exercise.

**What You'll Have When Done:**
- Multiple budget scenarios with clear comparisons
- Narrative explanation of each scenario's implications
- Trade-off analysis in plain language
- Recommendations with supporting rationale
- Sensitivity analysis for key assumptions
- Presentation-ready budget story

---

## When to Use This Recipe

**Good Fit:**
- Annual budget planning and scenario development
- Mid-year reforecasting
- Cost reduction analysis
- Investment decision support
- "What if" scenario exploration
- Budget defense preparation

**Not a Good Fit:**
- Detailed line-item accounting (use spreadsheets)
- Real-time financial tracking (use systems)
- Audit-ready documentation (requires specific formats)
- Complex financial modeling with interdependencies (may need specialized tools)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have baseline budget data (can be CSV, Excel summary, or text)
- [ ] You know the scenarios you want to model
- [ ] You understand key business drivers and constraints
- [ ] You know your audience and what they care about
- [ ] You have 30-60 minutes for analysis and narrative development

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Calculates scenario variations quickly
- Generates narrative explanations of numbers
- Identifies trade-offs and implications
- Creates comparison tables and summaries
- Produces executive-ready language
- Asks clarifying questions about assumptions

**Where Human Judgment Is Essential:**
- Validating financial accuracy (check the math)
- Understanding business context and constraints
- Making strategic recommendations
- Knowing what trade-offs are actually acceptable
- Political and organizational dynamics
- Final approval of any budget decisions

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Baseline budget | Current budget breakdown | Starting point for scenarios |
| Scenario parameters | "Model 10%, 15%, 20% cuts" | Scenario definitions |
| Constraints | "Cannot cut customer support" | Guardrails |
| Priorities | "Revenue growth is priority 1" | Trade-off evaluation |
| Historical context | Prior year actuals | Baseline comparison |

**Sample Budget Data:**
```
2024 Budget - Marketing Department

Category            Budget      % of Total
------------------------------------------
Personnel           $2,400,000     48%
Advertising         $1,200,000     24%
Events/Conferences    $600,000     12%
Technology/Tools      $400,000      8%
Content Production    $250,000      5%
Agency Fees           $150,000      3%
------------------------------------------
Total               $5,000,000    100%

Context:
- Company revenue target: $50M
- Marketing typically 10% of revenue
- Last year actual spend: $4.2M
- CEO wants to explore 10-20% reduction scenarios
- Cannot reduce headcount without long process
- Events drive 30% of our qualified leads
```

---

## Step-by-Step Implementation

### Step 1: Prepare Your Budget Data
**Time: 5-10 minutes**

Gather:
- Current budget or forecast by category
- Key constraints (what can/cannot change)
- Scenarios leadership wants to see
- Business context (what drives value)

Export or summarize your data in a format Claude can read.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
cd ~/Documents/budget-planning
claude
```

---

### Step 3: Run the Budget Scenario Prompt
**Time: 3-5 minutes for Claude to process**

---

**PRIMARY PROMPT: Budget Scenario Modeling**

```
Please help me model budget scenarios and generate executive-ready analysis.

CURRENT BUDGET:
"""
[PASTE YOUR BUDGET DATA - CATEGORIES AND AMOUNTS]
"""

BUSINESS CONTEXT:
- Department/Function: [e.g., Marketing]
- Company revenue target: [amount]
- This budget as % of revenue: [percentage]
- Prior year spend: [amount]
- Key business drivers: [what this budget enables]

CONSTRAINTS:
- Cannot change: [areas that must stay fixed]
- Difficult to change: [areas that are hard but possible]
- Flexible areas: [areas with more discretion]

SCENARIOS TO MODEL:
1. [Scenario 1: e.g., 10% reduction]
2. [Scenario 2: e.g., 15% reduction]
3. [Scenario 3: e.g., 20% reduction]
4. [Optional: Growth scenario or specific strategic scenario]

KEY QUESTIONS TO ADDRESS:
- [Question 1 leadership has asked]
- [Question 2]

PLEASE PROVIDE:

1. SCENARIO COMPARISON TABLE
   - Side-by-side comparison of all scenarios
   - Show dollar amounts and % changes
   - Highlight significant differences

2. NARRATIVE FOR EACH SCENARIO
   For each scenario, explain:
   - What changes and what stays the same
   - Business impact and risks
   - What capabilities are affected
   - Trade-offs being made

3. TRADE-OFF ANALYSIS
   - What do we gain/lose in each scenario
   - Risk assessment (low/medium/high)
   - Reversibility (easy/hard to undo)

4. SENSITIVITY ANALYSIS
   - What assumptions matter most?
   - What happens if [key variable] is different?

5. RECOMMENDATION
   - Which scenario do you recommend?
   - Rationale
   - Key risks to monitor

6. EXECUTIVE SUMMARY
   - One-page summary suitable for leadership
   - Clear recommendation
   - Key discussion points

Format numbers with appropriate rounding and include percentages for easy comparison.
```

---

### Step 4: Review the Analysis
**Time: 10-15 minutes**

Validate Claude's calculations and logic:

**Check the math:**
- Do the scenarios add up correctly?
- Are percentages calculated properly?
- Any obvious errors?

**Check the logic:**
- Do the implications make sense?
- Any trade-offs missed?
- Is the business impact realistic?

**Check the tone:**
- Is the narrative appropriate for your leadership?
- Any politically sensitive areas that need adjustment?

---

### Step 5: Refine and Explore
**Time: 10-20 minutes**

**To explore specific trade-offs:**
```
What if instead of cutting events by 50%, we cut advertising by 30% and events by 20%? Show me that scenario compared to the 15% reduction scenario.
```

**To add business context:**
```
Add context that our Q1 events are already committed and paid for. The event cuts can only happen Q2 onwards. What does that mean for the 15% scenario?
```

**To strengthen the recommendation:**
```
I'm leaning toward the 15% scenario. Build a stronger case for it, including what risks we're accepting and how we'd mitigate them.
```

**To prepare for pushback:**
```
The CMO will push back on advertising cuts. Generate 3 counter-arguments and data points I can use to defend the recommendation.
```

**To model sensitivity:**
```
The 20% cut assumes we can renegotiate agency contracts by 50%. Model what happens if we only achieve 25% reduction there.
```

---

### Step 6: Create Presentation Materials
**Time: 5 minutes**

```
Create three outputs:
1. One-page executive summary for the CFO
2. Detailed scenario comparison table for the finance team
3. Talking points for my budget review meeting tomorrow
```

---

## Example Output

Below is an abbreviated scenario analysis example:

---

> **BUDGET SCENARIO ANALYSIS: Marketing Department 2024**
>
> ---
>
> **SCENARIO COMPARISON**
>
> | Category | Baseline | Scenario A (-10%) | Scenario B (-15%) | Scenario C (-20%) |
> |----------|----------|-------------------|-------------------|-------------------|
> | Personnel | $2,400K | $2,400K (0%) | $2,400K (0%) | $2,160K (-10%)* |
> | Advertising | $1,200K | $1,080K (-10%) | $960K (-20%) | $840K (-30%) |
> | Events | $600K | $540K (-10%) | $420K (-30%) | $360K (-40%) |
> | Technology | $400K | $360K (-10%) | $320K (-20%) | $280K (-30%) |
> | Content | $250K | $225K (-10%) | $200K (-20%) | $175K (-30%) |
> | Agency | $150K | $100K (-33%) | $75K (-50%) | $50K (-67%) |
> | **Total** | **$5,000K** | **$4,500K** | **$4,375K** | **$3,865K** |
>
> *Scenario C requires personnel reduction through attrition/restructuring
>
> ---
>
> **SCENARIO B NARRATIVE (-15% / $625K reduction)**
>
> **What Changes:**
> - Advertising reduced 20% ($240K): Shift from broad awareness to targeted demand gen
> - Events reduced 30% ($180K): Attend tier-1 events only; eliminate smaller conferences
> - Agency fees cut 50% ($75K): Bring creative work in-house; project-based only
> - Technology and content reduced proportionally
>
> **What Stays the Same:**
> - Full marketing team preserved (critical capability)
> - Digital infrastructure maintained
> - Brand campaigns continue (reduced scale)
>
> **Business Impact:**
> - Lead generation capacity reduced ~15-20%
> - Event-driven leads specifically down ~30% (these are 30% of qualified pipeline)
> - Time-to-impact longer (reduced paid amplification)
>
> **Risk Level: MEDIUM**
> - Achievable without structural change
> - Pipeline risk manageable with sales productivity improvements
> - Brand equity impact minimal if executed well
>
> ---
>
> **TRADE-OFF ANALYSIS**
>
> | Scenario | Savings | Lead Impact | Revenue Risk | Reversibility |
> |----------|---------|-------------|--------------|---------------|
> | A (-10%) | $500K | -10% leads | Low | Easy |
> | B (-15%) | $625K | -18% leads | Medium | Moderate |
> | C (-20%) | $1.14M | -30% leads | High | Difficult |
>
> **Critical Trade-off:** Each 5% reduction in marketing correlates to approximately 6% reduction in lead generation, which translates to ~4% revenue risk (based on historical conversion rates).
>
> ---
>
> **RECOMMENDATION: Scenario B (-15%)**
>
> **Rationale:**
> 1. Achievable without personnel changes, preserving team capability
> 2. Focuses cuts on lowest-ROI activities (broad awareness, tier-2 events)
> 3. Maintains core demand generation engine
> 4. Aligns with company's efficiency focus while protecting growth
>
> **Key Risks to Monitor:**
> - Pipeline leading indicators monthly (leads, MQLs, SQLs)
> - Event ROI for remaining conferences
> - Competitor share of voice in reduced advertising channels
>
> **If Revenue At Risk:** Can restore ~$200K in Q3 with 6-week lead time on advertising

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Numbers don't add up | Rounding or calculation errors | Ask: "Recalculate the totals and verify each scenario sums correctly" |
| Missing important constraints | Not specified in input | Add: "Also account for: [specific constraint]" |
| Implications seem wrong | Missing business context | Add: "This budget funds [X] which drives [Y] revenue" |
| Too finance-focused | Audience needs business language | Ask: "Rewrite for business leaders—focus on capabilities and outcomes, not line items" |
| Scenarios too similar | Not enough differentiation | Ask: "Make the scenarios more distinct—show me a conservative, moderate, and aggressive option" |
| Recommendation too weak | Not enough conviction | Ask: "Take a stronger position. What would you actually recommend and why?" |

---

## Tips from Experience

1. **Lead with the story, not the spreadsheet.** Executives want to understand implications first, then see the numbers. Structure your presentation narrative-first.

2. **Always include the "what we lose" story.** Budget cuts have consequences. Make them explicit so leadership makes informed trade-offs.

3. **Model the cliff edge.** There's usually a point where cuts go from painful-but-manageable to catastrophic. Identify and articulate where that line is.

4. **Build in reversibility.** Cuts that can be undone in 30 days are different from cuts that take 6 months to reverse. Make reversibility explicit.

5. **Have the revenue impact conversation.** Finance often treats budget cuts as neutral to revenue. Push back with data on what budget enables.

6. **Prepare for the "why not more?" question.** If you recommend 15%, leadership will ask why not 20%. Have that answer ready.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Budget scenarios are understood in business terms, not just numbers
- [ ] Leadership can make informed trade-off decisions
- [ ] Your recommendation is clear and defensible
- [ ] Scenario comparisons are presented clearly
- [ ] You can answer follow-up "what if" questions quickly

**Track over time:**
- Time spent on scenario modeling
- Quality of budget discussions (informed vs. confused)
- Accuracy of impact predictions (revisit after the fact)

---

## Variations

### Cost Reduction Analysis
For targeted cost-cutting:
```
I need to find $X in cost reductions. Here's my current budget:

[Budget data]

Constraints:
- Cannot cut: [protected areas]
- Must maintain: [minimum capabilities]

Show me multiple paths to achieve $X in savings, ranked by:
1. Lowest business impact
2. Easiest to implement
3. Most sustainable long-term

For each path, explain what we're giving up.
```

### Investment Analysis
For evaluating new budget requests:
```
I'm considering this new investment:

Investment: [description]
Cost: [amount]
Timeline: [duration]
Expected return: [projected benefit]

Analyze:
1. ROI calculation
2. Payback period
3. Risk factors
4. Comparison to alternative uses of capital
5. Recommendation: Fund / Don't fund / Fund with modifications
```

### Budget Variance Explanation
For explaining actuals vs. budget:
```
Here's our budget vs. actual for [period]:

[Variance data]

Create a variance narrative that:
1. Explains each significant variance (>5%)
2. Categorizes as: timing, permanent, one-time
3. Identifies areas of concern
4. Projects full-year impact
5. Recommends actions

Tone: Honest but not alarmist. Focus on what's actionable.
```

### Multi-Year Budget Model
For strategic planning:
```
Model a 3-year budget projection based on:

Baseline: [current budget]
Growth assumptions: [revenue growth, etc.]
Known changes: [headcount plans, initiatives, etc.]
Investment priorities: [strategic areas]

Create a multi-year model showing:
1. Year-over-year changes
2. Mix shifts over time
3. Investment vs. run-rate split
4. Key inflection points
5. Sensitivity to growth assumptions
```

---

## Building Your Repeatable System

After a few budget cycles, establish your system:

1. **Create a scenario template** with your standard scenarios
2. **Build an implications library** for common budget changes
3. **Maintain historical data** for calibrating impact predictions
4. **Document constraints** that apply across cycles
5. **Save executive summaries** as examples for future use

**Sample Setup:**
```
budget-planning/
├── templates/
│   ├── scenario-prompt.txt
│   └── executive-summary-template.md
├── data/
│   ├── current-budget.csv
│   └── historical-actuals.csv
├── analysis/
│   ├── 2024-scenarios/
│   └── 2025-planning/
└── reference/
    ├── impact-benchmarks.md
    └── constraint-documentation.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**model scenarios → generate implications → create narrative → make recommendation**—applies broadly:

| Role | Application |
|------|-------------|
| **Finance** | All budget and planning activities |
| **Executives** | Strategic investment decisions |
| **Operations** | Capacity and resource planning |
| **Product** | Feature prioritization with resource constraints |
| **HR** | Compensation and headcount modeling |
| **Any manager** | Department budget management |

---

## Next Steps

1. **Next planning cycle:** Use this for your budget scenario development
2. **Build your templates:** Customize prompts for your organization's context
3. **Track predictions:** Note impact predictions and check against actuals later
4. **Share the approach:** Help colleagues move from spreadsheets to stories

---

*Recipe #16 of 100 in the Claude Code Knowledge Worker Recipe Collection*
