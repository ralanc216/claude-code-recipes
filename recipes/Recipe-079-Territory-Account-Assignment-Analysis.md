# Territory and Account Assignment Analysis

**Recipe #79: From Arbitrary Territories to Data-Driven Sales Coverage**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 60 minutes (first time) / 30 minutes (repeat) | 4-8 hours per analysis | Advanced | Sales Operations, Sales Leadership |

---

## The Problem

Territory and account assignments significantly impact sales productivity and rep satisfaction, yet most organizations do them poorly. Common problems include unbalanced workloads, geographic inefficiencies, mismatched skills to opportunities, and constant re-territorialization that disrupts customer relationships. Creating fair, productive territory designs requires analyzing multiple variables—opportunity potential, account characteristics, rep capacity, travel efficiency, and historical performance—which is analytically complex and politically sensitive.

**Pain Points:**
- Some reps have twice the opportunity of others with same quota
- Geographic territories result in excessive travel and inefficiency
- Top accounts assigned to wrong reps based on tenure not skill
- Constant territory changes disrupt customer relationships and rep morale
- New hires get leftover accounts that set them up to fail
- No data-driven process—territories set by politics and squeaky wheels
- Workload imbalances create resentment and turnover

---

## The Outcome

A data-driven territory and account assignment analysis with workload balancing, opportunity distribution, geographic optimization, and assignment recommendations—enabling equitable, productive sales coverage that maximizes revenue potential while maintaining rep fairness and customer relationships.

**What You'll Have When Done:**
- Complete analysis of current territory imbalances
- Ideal territory distribution targets by role and capacity
- Specific account movement recommendations with rationale
- New rep territory design for upcoming hires
- Implementation plan with phasing and communication strategy
- Success metrics to track improvement

---

## When to Use This Recipe

**Good Fit:**
- Annual sales planning and territory design
- Sales team expansion or contraction
- New market or product expansion requiring coverage changes
- Geographic expansion into new regions
- Major account list changes or ICP shifts
- Merger or acquisition territory integration
- Rep performance disparity investigation
- After market changes requiring rebalancing

**Not a Good Fit:**
- Very small teams (fewer than 5 reps) where informal works
- Fully pooled/round-robin assignment models
- When you lack basic account data (size, location, potential)
- Extremely dynamic markets where territories change weekly

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] Account list with attributes (size, industry, location) is available
- [ ] Territory/assignment history is documented
- [ ] Rep roster with capacity and skills exists
- [ ] Historical performance data by territory is accessible
- [ ] Opportunity/potential scoring data is available
- [ ] Geographic considerations are understood (if relevant)
- [ ] Customer relationship data is tracked
- [ ] Business rules and constraints are defined
- [ ] You have 90-120 minutes for comprehensive territory analysis

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Analyze account and rep data to identify workload imbalances
- Calculate opportunity distribution equity across territories
- Model alternative assignment scenarios with trade-offs
- Evaluate geographic optimization opportunities
- Generate specific account movement recommendations
- Create implementation plans with transition support

**Where Human Judgment Is Essential:**
- Determining strategic priorities (growth vs. fairness vs. relationships)
- Validating that customer relationship disruption is acceptable
- Deciding on politically sensitive account reassignments
- Setting acceptable disruption levels (how many accounts can move)
- Balancing data recommendations with rep preferences and morale

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Account Data | List with size, industry, location, potential | Understanding distribution |
| Current Assignments | Rep-to-account mapping with performance | Identifying imbalances |
| Rep Performance | Conversion rates, attainment by territory | Skill-to-opportunity matching |
| Business Context | Growth goals, expansion plans, constraints | Framing recommendations |
| Capacity Assumptions | Standard account loads by role | Calculating ideal distribution |

**Sample Input:** *(see Example Inputs in original recipe for detailed examples)*

The recipe includes comprehensive example inputs showing:
- Account inventory by segment and region
- Current territory assignments with performance
- Rep capacity and performance data
- Business objectives and constraints

---

## Step-by-Step Implementation

### Step 1: Prepare Your Inputs
**Time: 20-30 minutes**

Gather your territory and account data:
- Export account list with all relevant attributes
- Document current territory assignments
- Compile rep performance data by territory
- Note business objectives and constraints
- Identify capacity assumptions by role

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Territory Analysis Prompt
**Time: 10-15 minutes for Claude to process**

---

**PRIMARY PROMPT: Analyze Current State**

```
Claude, I need to analyze our territory and account assignments for optimization.

Account data:
[PASTE ACCOUNT INVENTORY AND ATTRIBUTES]

Current assignments:
[PASTE CURRENT TERRITORY STRUCTURE]

Please analyze:
1. Workload distribution across reps
2. Opportunity potential distribution
3. Geographic coverage efficiency
4. Skill/account matching
5. Identify obvious imbalances and issues
```

---

### Step 4: Review and Validate
**Time: 10-15 minutes**

**Check immediately:**
- Do the imbalance calculations align with rep complaints?
- Are capacity assumptions realistic for your sales model?
- Does the geographic analysis match reality?

**Spot-check specifics:**
- Verify account counts and potential calculations
- Confirm rep performance data is accurate
- Check that all critical accounts are included
- Ensure skill assessments are fair

---

### Step 5: Refine and Iterate
**Time: 30-45 minutes**

**Prompt: Calculate Ideal Distribution**
```
Based on our team structure and objectives, calculate ideal territory distribution.

Team structure: [X ENTERPRISE, Y MID-MARKET, Z COMMERCIAL REPS]
Total potential: [TOTAL $$]
Business objectives:
[PASTE OBJECTIVES]

Provide:
1. Ideal accounts per rep by segment
2. Ideal potential per rep
3. Coverage ratio targets
4. Geographic distribution targets
5. Gap analysis vs. current state
```

**Prompt: Model Scenarios**
```
Model the following territory scenarios:

Scenario 1: Minor rebalancing (minimize disruption)
Scenario 2: Geographic optimization (travel efficiency)
Scenario 3: Vertical specialization (industry focus)
Scenario 4: Performance-based (reward top performers)

For each scenario provide:
1. Account movements required
2. Coverage changes
3. Expected impact on productivity
4. Rep-level impact
5. Disruption score
```

**Prompt: Design New Rep Territories**
```
Design territory for new reps being added:

New reps: [2 ENTERPRISE, 3 MID-MARKET]
Start dates: [DATES]
Ramp assumptions: [6 MONTHS TO FULL PRODUCTIVITY]

Provide:
1. Initial account assignments for each new rep
2. Source accounts from (which existing territories)
3. Ramp period targets
4. Mentor/shadow assignments
5. Success metrics for ramp
```

---

### Step 6: Export Final Output
**Time: 10 minutes**

```
Based on all analysis, provide territory optimization recommendations:

Include:
1. RECOMMENDED CHANGES
   - Account movements by rep
   - New territory definitions
   - Expected impact

2. IMPLEMENTATION PLAN
   - Phasing approach
   - Communication strategy
   - Customer notification

3. RISK MITIGATION
   - Customer relationship protection
   - Rep concerns
   - Transition support

4. SUCCESS METRICS
   - How to measure improvement
   - Timeline for evaluation
```

---

## Example Output

Below is an abbreviated example of what a well-executed territory analysis looks like:

---

> ### Territory Analysis & Optimization Report
>
> #### Executive Summary
>
> **Current State Assessment:**
> - Workload imbalance: 40% variance in account potential across comparable reps
> - Geographic inefficiency: Northeast over-covered by 25%; West under-covered by 30%
> - Skill mismatch: 15% of accounts with wrong vertical alignment
> - Capacity issues: 3 reps under-utilized, 4 reps over-capacity
>
> **Recommended Approach:** Moderate rebalancing (~15% of accounts move) combined with strategic geographic and vertical realignment.
>
> **Expected Impact:**
> - Reduce territory variance from 40% to 15%
> - Improve West coverage by adding 1 Enterprise, 2 Mid-Market
> - Create healthcare specialty pod with focused expertise
> - Set up new reps with viable territories
>
> ---
>
> #### Workload Distribution Analysis
>
> **Enterprise Team:**
>
> | Rep | Accounts | Potential | vs. Avg | Issue |
> |-----|----------|-----------|---------|-------|
> | E1 | 18 | $4.8M | +27% | Over-loaded |
> | E8 | 13 | $3.1M | -18% | Under-potential |
> | **Avg** | **15** | **$3.75M** | - | - |
>
> **Variance:** 40% (target: <15%)
>
> *(Full output includes detailed rebalancing recommendations, scenario analysis, and implementation plan)*

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Rep resistance to changes | Fear of losing good accounts | Be transparent about rationale; show data; ensure fairness perception; allow input period |
| Data quality issues | Account potential/attributes inaccurate | Validate data before analysis; use multiple sources; allow estimation ranges; caveat recommendations |
| Politics override analysis | Leadership makes assignments based on relationships | Present clear trade-offs; document alternatives; measure outcomes to show impact |
| Too much disruption required | Optimal assignment requires moving most accounts | Constrain analysis to acceptable disruption level; prioritize highest-impact changes; phase over time |
| New rep territories not viable | Carved from weakest accounts only | Ensure new reps get mix of easy wins and growth accounts; set realistic ramp targets |
| Geographic constraints ignored | Analysis doesn't account for travel time | Include travel efficiency as explicit constraint; use drive-time data; consider remote coverage |

---

## Tips from Experience

1. **Start with clear objectives.** Are you optimizing for fairness, revenue, growth, or rep retention? You can't maximize all simultaneously—be explicit about priorities.

2. **Use multiple metrics, not just account count.** Balance accounts, potential, and pipeline coverage. Equal account counts with wildly different potential isn't fair.

3. **Consider rep input seriously.** They know accounts better than data shows. A rep saying "this account won't work with that rep" is usually right.

4. **Minimize disruption—100% optimal with 50% disruption isn't worth it.** Protect customer relationships and rep morale. Incremental improvement beats theoretical perfection.

5. **Phase changes over time.** Big bang territory changes are risky. Pilot with one segment, learn, then expand.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Territory variance decreases to target level (<15-20%)
- [ ] Win rate improves or stays stable post-change
- [ ] New rep time to productivity meets targets
- [ ] Customer retention through transition is >95%
- [ ] Rep satisfaction with territories improves

**Track over time:**
- Territory variance (potential distribution equity)
- Win rate by territory
- New rep ramp performance

---

## Variations

### Variation 1: Named Account Assignments Only
Focus on strategic account assignment without geographic territorialization.
```
Modify the analysis prompt:
"Analyze named account assignments only (no geographic territories). Focus on: account size/complexity match to rep capability, industry expertise alignment, relationship continuity, and workload balance measured in account count and total potential."
```

### Variation 2: Overlay Team Design
Design specialist overlay territories that work across core territories.
```
Add to your scenario modeling:
"Design overlay specialist territories for [product specialists / industry experts / enterprise overlays]. Define how overlays interact with core reps, account ownership rules, and comp split arrangements."
```

### Variation 3: M&A Territory Integration
Integrate acquired company territories with existing structure.
```
Include in business context:
"We're integrating [acquired company] sales team. Analyze: duplicate account coverage, geographic overlap, rep skill/capability differences, and integration scenarios (full integration vs. separate teams vs. hybrid)."
```

---

## Building Your Repeatable System

After using this recipe 2-3 times, establish your system:

1. **Create Account Scoring Templates.** Standardize how you calculate account potential so territories are comparable over time.

2. **Build Territory Card Templates.** Document each territory with standard format: accounts, potential, coverage ratio, success metrics.

3. **Establish Annual Planning Cycle.** Schedule territory planning as part of annual sales kickoff. Don't do ad hoc changes.

4. **Create Change Request Workflow.** Implement process for ongoing adjustment requests. Not every complaint needs territory change.

**Sample Folder Structure:**
```
territory-planning/
├── current-state/
│   ├── account-list-2024.csv
│   └── current-assignments.xlsx
├── analysis/
│   ├── 2024-territory-analysis.md
│   ├── scenario-models.xlsx
│   └── workload-balance-dashboard.png
├── implementation/
│   ├── account-movements.xlsx
│   ├── communication-plan.md
│   └── new-rep-onboarding-plan.md
└── archive/
    └── 2023-territory-analysis.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**optimizing resource allocation with multiple constraints**—applies broadly:

| Role | Application |
|------|-------------|
| **Customer Success** | CSM account load optimization and segmentation |
| **Support** | Ticket assignment and routing optimization |
| **Field Service** | Technician territory and route optimization |
| **Marketing** | ABM account assignment to marketing managers |
| **Recruiting** | Recruiter requisition assignment and load balancing |

---

## Next Steps

1. **This week:** Run the current state analysis on your territory data. Identify the biggest imbalances.
2. **Track your results:** Set up territory variance tracking to monitor equity over time.
3. **Iterate:** Share draft recommendations with sales managers for feedback on feasibility.
4. **Share:** Present territory plan to leadership with expected productivity impact and transition risks.

---

*Recipe #79 of 100 in the Claude Code Knowledge Worker Recipe Collection*
