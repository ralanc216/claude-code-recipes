# Pricing Analysis and Recommendation

**Recipe #78: From Guesswork Pricing to Data-Driven Value Capture**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 60 minutes (first time) / 30 minutes (repeat) | 4-6 hours per analysis | Advanced | Pricing Analysts, Product, Finance, Sales Leadership |

---

## The Problem

Pricing decisions significantly impact revenue, market position, and customer relationships, yet most organizations make them with incomplete analysis. Teams struggle to balance competitive positioning, value delivery, cost coverage, and customer willingness to pay. Pricing analysis typically requires synthesizing data from multiple sources—costs, competitors, win/loss data, customer feedback—and modeling various scenarios, which is time-intensive and often done superficially or not at all.

**Pain Points:**
- Pricing decisions made based on intuition rather than data analysis
- Competitive intelligence is anecdotal and inconsistent
- Win/loss data shows pricing issues but root causes are unclear
- Cost-plus pricing leaves money on the table or prices you out
- No systematic way to test or validate pricing changes
- Cross-functional disagreement (finance wants higher, sales wants lower)
- Customer willingness-to-pay is unknown or misunderstood

---

## The Outcome

A comprehensive pricing analysis with market context, cost structures, competitive positioning, elasticity assessment, and scenario-based recommendations—enabling informed pricing decisions that maximize value capture while maintaining market competitiveness.

**What You'll Have When Done:**
- Complete cost structure analysis by product tier or segment
- Competitive price positioning map with strategic options
- Customer value analysis and willingness-to-pay assessment
- Multiple pricing scenarios modeled with expected outcomes
- Clear pricing recommendations with implementation roadmap
- Risk analysis and success metrics defined

---

## When to Use This Recipe

**Good Fit:**
- New product or feature pricing requiring market analysis
- Annual pricing strategy reviews and adjustments
- Competitive pricing responses to market changes
- Cost structure changes requiring price adjustments
- Market expansion pricing decisions for new segments
- Packaging and bundling optimization
- Win/loss analysis showing pricing as a key issue
- Margin improvement initiatives

**Not a Good Fit:**
- Very early stage with no comparable products or customers
- Regulated pricing where flexibility is extremely limited
- When you lack basic cost data to analyze
- Single transaction pricing (use negotiation tactics instead)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] Current pricing and packaging details are documented
- [ ] Cost data is available (COGS, delivery, support)
- [ ] Competitive pricing intelligence has been gathered
- [ ] Win/loss data by price point is accessible
- [ ] Customer segment information exists
- [ ] Value metrics and customer outcomes are tracked
- [ ] Historical pricing changes and impact are documented
- [ ] Market and demand context is understood
- [ ] You have 90-120 minutes for comprehensive pricing analysis

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Synthesize cost data, competitive intelligence, and win/loss insights
- Model multiple pricing scenarios with revenue and margin projections
- Assess elasticity implications based on historical data
- Evaluate different pricing strategies (cost-plus, value-based, competitive)
- Generate clear recommendations with supporting rationale
- Create implementation plans with risk mitigation

**Where Human Judgment Is Essential:**
- Setting strategic pricing philosophy and market positioning
- Determining acceptable margins and business constraints
- Validating competitive intelligence accuracy
- Deciding which scenarios are politically and strategically feasible
- Balancing short-term revenue vs. long-term market position

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Current Pricing | Price list by tier with typical discounts | Understanding baseline |
| Cost Structure | Variable and fixed costs by product/tier | Calculating margins and floors |
| Competitive Intel | Competitor prices and positioning | Benchmarking and gap analysis |
| Win/Loss Data | Conversion rates and reasons by price band | Understanding elasticity |
| Business Context | Growth goals, constraints, market dynamics | Framing recommendations |

**Sample Input:** *(see Example Inputs in original recipe for detailed examples)*

The recipe includes comprehensive example inputs showing:
- Current pricing structure with costs
- Competitive pricing intelligence by player
- Win/loss analysis by price range
- Business objectives and constraints

---

## Step-by-Step Implementation

### Step 1: Prepare Your Inputs
**Time: 20-30 minutes**

Gather your pricing data and organize clearly:
- Document current pricing by tier/segment
- Compile cost data (variable and fixed)
- Collect competitive pricing intelligence
- Export win/loss data with price context
- Note business objectives and constraints

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Pricing Analysis Prompt
**Time: 10-15 minutes for Claude to process**

---

**PRIMARY PROMPT: Structure the Analysis**

```
Claude, I need to conduct a pricing analysis for [PRODUCT/SERVICE].

Current situation:
[PASTE CURRENT PRICING, COSTS, AND BUSINESS CONTEXT]

Business objectives:
[WHAT ARE YOU TRYING TO ACHIEVE WITH PRICING]

Key questions to answer:
1. Are we priced correctly for our market position?
2. What pricing changes would improve business outcomes?
3. How should we adjust packaging and tiers?
4. What's the right competitive pricing response?

Help me structure a comprehensive pricing analysis approach.
```

---

### Step 4: Review and Validate
**Time: 10-15 minutes**

**Check immediately:**
- Do the cost calculations align with your financial data?
- Are competitive comparisons accurate and fair?
- Do the business objectives match your strategy?

**Spot-check specifics:**
- Verify margin calculations are using correct formulas
- Confirm competitive pricing data is current
- Check that all relevant cost components are included
- Ensure price points make sense for your market

---

### Step 5: Refine and Iterate
**Time: 30-45 minutes**

**Prompt: Analyze Cost Structure**
```
Analyze our cost structure and margin potential:

Cost data:
[PASTE VARIABLE AND FIXED COSTS BY TIER/PRODUCT]

Revenue data:
[PASTE REVENUE BY TIER/SEGMENT]

Please provide:
1. Unit economics by tier
2. Margin analysis by customer segment
3. Cost-based pricing floor
4. Margin sensitivity analysis
5. Cost reduction opportunities
```

**Prompt: Competitive Positioning**
```
Analyze our competitive pricing position:

Our pricing:
[PASTE CURRENT PRICING]

Competitor pricing:
[PASTE COMPETITIVE INTELLIGENCE]

Win/loss data:
[PASTE PRICE-RELATED WIN/LOSS DATA]

Please assess:
1. Price positioning map (us vs. competitors)
2. Price/value perception
3. Where we're over/under-priced
4. Competitive response options
5. Sustainable price differentiation
```

**Prompt: Model Pricing Scenarios**
```
Model the following pricing scenarios:

Scenario 1: [DESCRIPTION - E.G., 10% PRICE INCREASE ACROSS ALL TIERS]
Scenario 2: [DESCRIPTION - E.G., NEW LOWER ENTRY TIER]
Scenario 3: [DESCRIPTION - E.G., USAGE-BASED COMPONENT]
Scenario 4: [DESCRIPTION - E.G., COMPETITIVE RESPONSE]

For each scenario, estimate:
1. Revenue impact (volume × price)
2. Margin impact
3. Market share impact
4. Customer perception
5. Implementation complexity
6. Risks and mitigation
```

---

### Step 6: Export Final Output
**Time: 10 minutes**

```
Based on the complete analysis, provide pricing recommendations:

Include:
1. PRIMARY RECOMMENDATION
   - Proposed pricing changes
   - Expected outcomes
   - Implementation approach

2. ALTERNATIVE OPTIONS
   - Other viable strategies
   - Trade-offs of each

3. IMPLEMENTATION PLAN
   - Phasing and timing
   - Communication strategy
   - Risk mitigation

4. METRICS AND MONITORING
   - How to measure success
   - Decision triggers for adjustment
```

---

## Example Output

Below is an abbreviated example of what a well-executed pricing analysis looks like:

---

> ### Pricing Analysis: DataSync Pro
>
> #### Executive Summary
>
> **Current State:** DataSync Pro is positioned as a mid-market value player, priced 15-20% below market leader SyncMaster. Margins are healthy (72% gross) but win rate at lower price points is concerning.
>
> **Key Findings:**
> 1. **Starter tier is underperforming** - High churn (18%), low win rate at <$15K deals, margin squeeze
> 2. **Professional tier is the sweet spot** - Best balance of win rate, retention, and margin
> 3. **We're leaving money on the table at Enterprise** - Wide variance ($72K-$180K) suggests inconsistent value capture
> 4. **QuickSync is a threat at lower end** - Winning price-sensitive deals with aggressive discounting
>
> **Recommended Strategy:** "Barbell Strategy" - strengthen value at Professional/Enterprise tiers, introduce limited Starter tier designed for conversion, stop competing with QuickSync on price.
>
> **Expected Impact:**
> - Revenue: +$4.2M ARR (15% growth from pricing alone)
> - Margin: +3 points (72% → 75%)
> - Average deal size: +18%
>
> ---
>
> #### Recommended Pricing Structure
>
> | Tier | Current | Proposed | Change | Rationale |
> |------|---------|----------|--------|-----------|
> | Growth (new) | - | $9,000 | N/A | Replaces Starter; conversion-focused |
> | Professional | $36,000 | $39,000 | +8% | Feature enhancement justifies increase |
> | Enterprise Std | $72,000 | $85,000 | +18% | Baseline Enterprise |
> | Enterprise Plus | - | $120,000 | N/A | Dedicated support tier |
>
> *(Full analysis includes cost structure, competitive positioning, scenario modeling, and implementation plan)*

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Insufficient competitive data | Competitors don't publish prices | Use win/loss data as proxy; conduct customer research; purchase competitive intelligence; analyze public pricing |
| Stakeholder disagreement | Finance wants higher, Sales wants lower | Model scenarios with full P&L impact; show trade-offs quantitatively; use data to ground discussion |
| Fear of customer backlash | Relationship concerns about increases | Survey value perception; test with new customers first; communicate value clearly; grandfather existing customers |
| Too many variables | Price, packaging, features, tiers all interrelated | Identify biggest lever first; make one change at a time; use experiments where possible; progress over perfection |
| Win/loss data insufficient | Not enough history or poor tracking | Use longer time periods; supplement with surveys; apply industry benchmarks; document limitations clearly |
| Cost allocation disputes | Disagreement on how to allocate fixed costs | Use multiple allocation methods; focus on variable costs for floor; document assumptions transparently |

---

## Tips from Experience

1. **Ground in data, not intuition.** Intuition about pricing is often wrong. Customer willingness-to-pay surprises most teams when actually measured.

2. **Think about value, not just cost.** Cost sets your floor; value sets your ceiling. The money is made in the gap between them.

3. **Consider pricing psychology.** Anchoring, decoys, and price presentation matter as much as the number itself.

4. **Test when possible.** A/B test prices with new customers if you have volume. Small tests beat big assumptions.

5. **Don't just raise prices—add value.** Price increases with feature additions or packaging changes feel fair. Naked price increases feel like gouging.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Revenue grows from pricing changes without unacceptable volume loss
- [ ] Win rate stability or improvement after pricing changes
- [ ] Average deal size increases by target percentage
- [ ] Gross margin improves to target levels
- [ ] Price realization (actual vs. list) improves

**Track over time:**
- Revenue growth attributable to pricing
- Win rate by price band
- Customer perception (NPS, satisfaction) stability

---

## Variations

### Variation 1: New Product Pricing
Focus on market entry pricing strategy with competitive positioning and penetration vs. skimming analysis.
```
Modify the primary prompt to include:
"This is a new product launch. Analyze market entry pricing considering: penetration pricing to gain share quickly vs. skimming to capture early adopters, competitive positioning from day one, and ramp strategy over first 12 months."
```

### Variation 2: Discount Policy Analysis
Analyze discount patterns and create optimized discount guidelines.
```
Add to your analysis:
"Analyze our discounting patterns by deal size, segment, and rep. Identify where discounts are value-destroying vs. strategic. Create discount policy guidelines with authorization thresholds."
```

### Variation 3: Usage-Based Pricing Design
Design consumption-based pricing models with metering and predictability.
```
Include in scenario modeling:
"Design a usage-based pricing component. Consider: what usage metric to charge on, predictability for customers, revenue recognition implications, and hybrid models combining base + usage."
```

---

## Building Your Repeatable System

After using this recipe 2-3 times, establish your system:

1. **Create Pricing Analysis Templates.** Standardize the sections and data requirements so future analyses are consistent and comparable over time.

2. **Build a Competitive Price Tracker.** Continuously monitor competitor pricing changes. Don't wait until you need the data—track it proactively.

3. **Establish an Annual Pricing Review Cycle.** Schedule pricing analysis as part of annual planning. Reactive pricing is always worse than strategic pricing.

4. **Connect to Win/Loss Analysis.** Every win/loss review should capture pricing feedback. Make pricing insights a standard part of sales feedback loops.

**Sample Folder Structure:**
```
pricing-analysis/
├── current-pricing/
│   ├── price-list-2024.md
│   └── packaging-structure.md
├── competitive-intelligence/
│   ├── competitor-tracking.xlsx
│   └── market-positioning-map.png
├── analysis/
│   ├── 2024-annual-pricing-review.md
│   ├── scenario-models.xlsx
│   └── customer-value-research.md
└── implementation/
    └── pricing-change-rollout-plan.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**synthesizing cost, competitive, and customer data to optimize value capture**—applies broadly:

| Role | Application |
|------|-------------|
| **Professional Services** | Consulting rate setting and packaging analysis |
| **Internal IT** | Chargeback and transfer pricing for internal services |
| **Channel/Partnerships** | Partner margin and referral pricing structures |
| **Product Management** | Feature monetization and add-on pricing |
| **Real Estate** | Property pricing based on comps and value drivers |

---

## Next Steps

1. **This week:** Run the cost structure and competitive analysis using your current data. Identify obvious gaps.
2. **Track your results:** Set up win rate and margin tracking by price band to validate model assumptions.
3. **Iterate:** Share draft recommendations with sales for sanity check on customer reactions.
4. **Share:** Present pricing recommendations to leadership with expected impact and risks clearly articulated.

---

*Recipe #78 of 100 in the Claude Code Knowledge Worker Recipe Collection*
