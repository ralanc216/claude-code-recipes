# Product Feature Prioritization Analysis

**Recipe #89: From Political Feature Decisions to Data-Driven Priority**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 30 minutes (first time) / 15 minutes (repeat) | 2-4 hours per prioritization cycle | Intermediate | Product Managers, Product Owners, Development Leads |

---

## The Problem

Product teams face an endless backlog of feature requests, bug fixes, technical debt, and stakeholder demands. Everyone believes their request is the highest priority. Without a rigorous framework, prioritization becomes political—whoever shouts loudest or has the most seniority wins. This leads to products that chase shiny objects, neglect foundational issues, and don't systematically deliver user value.

**Pain Points:**
- Every feature request claimed as "critical" with no objective criteria to differentiate
- Prioritization driven by politics and who has the loudest voice rather than data
- Valuable technical debt and infrastructure work deprioritized for flashy features
- Time wasted in endless debates about what to build next
- Lack of transparent rationale for why features were chosen or rejected
- Difficulty saying "no" to stakeholders without defensible reasoning
- Product roadmaps that shift constantly based on latest request

---

## The Outcome

A defensible, transparent feature prioritization using established frameworks (RICE, MoSCoW, weighted scoring) that balances user impact, business value, effort, and strategic alignment—giving teams confidence they're working on the right things.

**What You'll Have When Done:**
- Feature backlog scored using RICE or similar framework
- Prioritization matrix mapping impact vs. effort
- Strategic alignment assessment for each feature
- Recommended roadmap with clear inclusion/exclusion rationale
- Communication talking points for stakeholders on why features made the cut
- Documentation of prioritization criteria for future consistency

---

## When to Use This Recipe

**Good Fit:**
- Quarterly roadmap planning
- Sprint planning and backlog grooming
- Resource allocation decisions
- Feature trade-off discussions
- Stakeholder alignment meetings
- Launch scope decisions
- Technical debt prioritization

**Not a Good Fit:**
- Emergency hotfixes (no time for analysis)
- Single-option decisions (build it or don't—no prioritization needed)
- When strategic direction is completely unclear
- Very early-stage exploration before any data exists

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] Feature request list with descriptions
- [ ] User feedback/research data
- [ ] Business metrics and goals
- [ ] Technical complexity estimates (at least rough)
- [ ] Resource availability (how much capacity you have)
- [ ] Strategic objectives for the planning period
- [ ] Stakeholder input on requests
- [ ] You have 45-60 minutes for analysis

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Applies prioritization frameworks (RICE, weighted scoring) consistently
- Scores features across multiple dimensions without bias
- Identifies dependencies and conflicts between features
- Creates visual priority matrices for stakeholder communication
- Generates documentation that explains prioritization rationale
- Balances quantitative scoring with strategic alignment

**Where Human Judgment Is Essential:**
- Estimating user impact and reach (requires market knowledge)
- Assessing strategic fit within organizational context
- Making final calls on confidence levels for uncertain features
- Navigating political dynamics when stakeholders disagree
- Deciding when to override scoring based on strategic imperatives
- Balancing short-term wins vs. long-term platform investments

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Feature descriptions | "Add dark mode: System-wide dark color scheme option" | Understanding what's being prioritized |
| User feedback | "500+ forum votes for dark mode" | Assessing reach and impact |
| Business context | "Q1 goal: land 5 enterprise customers" | Strategic alignment |
| Effort estimates | "SSO integration: 6 weeks" | RICE scoring effort component |
| Strategic priorities | "Reduce support tickets by 20%" | Filtering and weighting features |

**Sample Input:**
```
FEATURE BACKLOG - Q1 2024 Candidates

1. Advanced Search Filters
   - Description: Add date range, category, and status filters to search
   - Requester: Customer Success (top 5 customer requests)
   - User Impact: 40% of users search daily

2. Bulk Import Tool
   - Description: Import data from CSV/Excel files
   - Requester: Sales (blocking enterprise deals)
   - User Impact: Enterprise customers, new user onboarding

3. SSO/SAML Integration
   - Description: Enterprise single sign-on support
   - Requester: Sales (requirement for 3 enterprise deals)
   - User Impact: Enterprise customers

STRATEGIC PRIORITIES FOR Q1:
1. Land 5 new enterprise customers ($500K+ ARR impact)
2. Reduce support ticket volume by 20%
3. Improve user activation rate (30-day retention)

CONSTRAINTS:
- Engineering capacity: 3 developers, 1 QA
- Timeline: 12 weeks
- No new hires this quarter

ENGINEERING ESTIMATES (in weeks):
1. Advanced Search Filters: 3 weeks
2. Bulk Import Tool: 4 weeks
3. SSO/SAML Integration: 6 weeks
[etc.]
```

---

## Step-by-Step Implementation

### Step 1: Prepare Your Feature Data
**Time: 15 minutes**

Compile your feature backlog with descriptions, requesters, and known user impact. Gather rough effort estimates from engineering (even high-level "small/medium/large" works). Document your strategic priorities for the planning period.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the RICE Scoring Prompt
**Time: 10-15 minutes for Claude to process**

---

**PRIMARY PROMPT: Feature Prioritization Using RICE**

```
Claude, I need to prioritize our feature backlog using the RICE framework.

Business context:
[Paste strategic priorities, constraints, timeline, capacity]

Feature list:
[Paste backlog with descriptions, requesters, known impact]

Effort estimates:
[Paste engineering estimates]

For each feature, apply RICE scoring:
- REACH: How many users/customers affected per quarter (estimate)
- IMPACT: Effect on individuals (3=massive, 2=high, 1=medium, 0.5=low, 0.25=minimal)
- CONFIDENCE: How sure are we of reach/impact? (100%, 80%, 50%)
- EFFORT: Person-weeks to build

Calculate RICE score: (Reach × Impact × Confidence) / Effort

Explain your reasoning for each estimate. Include a summary table ranking
features by RICE score.
```

---

### Step 4: Apply Strategic Alignment
**Time: 10 minutes**

```
Assess strategic alignment for each feature:

Features with RICE scores: [Paste from Step 3]
Strategic priorities:
[Paste your Q1/annual priorities]

For each feature:
1. Which strategic priority does it support? (can be multiple)
2. How directly does it contribute? (Direct blocker removal / Strong support / Indirect / None)
3. Should we apply a strategic multiplier?
   - Direct enabler: 1.5×
   - Strong support: 1.2×
   - Indirect: 1.0×
   - No alignment: 0.8×

Create final priority ranking combining RICE score with strategic alignment.
```

---

### Step 5: Analyze Dependencies and Constraints
**Time: 5-10 minutes**

```
Analyze dependencies and create feasible roadmap:

Prioritized features: [Paste ranked list]
Dependencies: [Paste any known dependencies]
Constraints:
- Available capacity: [X developer-weeks]
- Timeline: [weeks/months]
- Must-have vs. nice-to-have designation

Identify:
1. Feature dependencies (what must come first?)
2. Features that can't be done simultaneously (resource conflicts)
3. Technical prerequisites
4. Features that together exceed capacity

Create a recommended roadmap that fits within constraints, sequenced
appropriately.
```

---

### Step 6: Generate Stakeholder Communication
**Time: 5-10 minutes**

```
Create stakeholder communication for the prioritization:

Recommended roadmap: [Paste from Step 5]
Features NOT included: [List deferred features]
Scoring rationale: [Summary of methodology]

Generate:
1. Executive summary (why these features, why not others)
2. Stakeholder-specific talking points:
   - For Sales team (enterprise features)
   - For Customer Success (user-requested features)
   - For Engineering (technical debt and infrastructure)
   - For Executive team (strategic alignment)
3. FAQ addressing likely objections
4. Clear criteria for when deferred features will be reconsidered

Make this transparent and defensible.
```

---

### Step 7: Review and Validate
**Time: 15 minutes**

**Check immediately:**
- RICE scores seem reasonable given your market knowledge
- Strategic alignment correctly assessed
- Resource constraints respected in roadmap
- Dependencies identified and sequenced properly

**Spot-check specifics:**
- Reach estimates align with user base size
- Impact ratings match severity of user pain points
- Confidence levels reflect certainty appropriately
- Effort estimates from engineering are preserved

---

### Step 8: Refine and Iterate
**Time: 5-10 minutes**

**To adjust scoring:**
```
The REACH estimate for [Feature X] should be higher - this affects all 10,000
users, not just the subset estimated. Recalculate RICE score and update ranking.
```

**To add features:**
```
Add these 3 additional features to the analysis:
[Feature descriptions with estimated effort]

Score them using same RICE framework and re-rank the entire backlog.
```

**To create alternative scenarios:**
```
Create alternative roadmap if we had 4 developers instead of 3.
Which additional features would we include?
```

---

### Step 9: Export Final Prioritization
**Time: 5 minutes**

```
Format the prioritization analysis as:
1. Executive summary (1 page: recommendation and rationale)
2. Detailed feature scoring (RICE table with explanations)
3. Priority matrix visualization (impact vs. effort)
4. Recommended roadmap (sequenced by quarter/sprint)
5. Deferred features (with rationale for exclusion)
```

---

## Example Output

Below is an abbreviated example of what a well-executed prioritization analysis looks like:

---

> **FEATURE PRIORITIZATION ANALYSIS**
> **Q1 2024 Planning**
>
> ---
>
> #### Executive Summary
>
> This analysis evaluates 10 candidate features for Q1 using RICE scoring and strategic alignment. Given 36 developer-weeks capacity, we recommend prioritizing 5 features totaling 21 weeks, leaving buffer for tech debt and unexpected work.
>
> **Recommended Q1 Roadmap:**
> 1. SSO/SAML Integration (strategic, unblocks $500K+ revenue)
> 2. API Rate Limiting Dashboard (quick win, reduces support)
> 3. Advanced Search Filters (high user impact)
> 4. Accessibility Improvements (compliance requirement)
> 5. Bulk Import Tool (enterprise enablement)
>
> ---
>
> #### Detailed Feature Scoring
>
> ##### 1. SSO/SAML Integration
>
> | Factor | Value | Rationale |
> |--------|-------|-----------|
> | **Reach** | 500 | 3 blocked deals × estimated users + future enterprise |
> | **Impact** | 3 (Massive) | Deal blocker → deal enabler |
> | **Confidence** | 80% | Clear requirement, proven technology |
> | **Effort** | 6 weeks | Complex but well-understood |
> | **RICE Score** | 200 | (500 × 3 × 0.8) / 6 |
> | **Strategic** | 1.5× | Directly enables enterprise goal |
> | **Final Score** | **300** | |
>
> **Analysis:** SSO directly unblocks 3 enterprise deals worth ~$400K ARR. Highest strategic impact despite moderate RICE score. Must-do for Q1.
>
> ---
>
> ##### 3. Advanced Search Filters
>
> | Factor | Value | Rationale |
> |--------|-------|-----------|
> | **Reach** | 4,000 | 40% of 10K users search daily |
> | **Impact** | 2 (High) | Significantly improves core workflow |
> | **Confidence** | 80% | Clear user requests, standard feature |
> | **Effort** | 3 weeks | Moderate complexity |
> | **RICE Score** | 2,133 | (4,000 × 2 × 0.8) / 3 |
> | **Strategic** | 1.0× | Supports activation (indirect) |
> | **Final Score** | **2,133** | |
>
> **Analysis:** Top customer request with strong RICE score. Improves daily experience for active users. Good NPS impact potential.
>
> ---
>
> #### Priority Matrix
>
> ```
>                         STRATEGIC ALIGNMENT
>                         Low              High
>                     ┌─────────────────┬─────────────────┐
>               High  │  CONSIDER       │  PRIORITIZE     │
>                     │                 │                 │
>     RICE            │  Dark Mode      │  SSO/SAML       │
>     SCORE           │  (1,050)        │  Accessibility  │
>                     │                 │  Search Filters │
>                     ├─────────────────┼─────────────────┤
>               Low   │  DEPRIORITIZE   │  QUICK WINS     │
>                     │                 │                 │
>                     │  Push Notif     │  API Dashboard  │
>                     │  Perf Dashboard │                 │
>                     └─────────────────┴─────────────────┘
> ```
>
> ---
>
> #### Recommended Q1 Roadmap
>
> | Feature | Effort | Start | End | Strategic Fit |
> |---------|--------|-------|-----|---------------|
> | API Rate Limiting Dashboard | 2 wks | Week 1 | Week 2 | ★★★ |
> | Advanced Search Filters | 3 wks | Week 1 | Week 3 | ★★ |
> | Accessibility Improvements | 6 wks | Week 1 | Week 6 | ★★ |
> | SSO/SAML Integration | 6 wks | Week 3 | Week 8 | ★★★ |
> | Bulk Import Tool | 4 wks | Week 4 | Week 7 | ★★★ |
>
> **Total: 21 weeks planned of 36 available (buffer: 15 weeks for tech debt, bugs, unknowns)**
>
> ---
>
> #### Features Not in Q1
>
> | Feature | Reason for Deferral | Reconsider When |
> |---------|---------------------|-----------------|
> | Workflow Automation | Too large (12 weeks) | Q2 major initiative |
> | Dark Mode | Lower strategic value despite votes | Q2 if capacity |
> | Push Notifications | Medium impact, no urgent need | Q2 based on retention data |

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Stakeholders disagree with scores | Scoring seems arbitrary or biased | Make criteria transparent; invite stakeholder input on estimates; let data drive, not opinions |
| Everything rated "must-have" | No differentiation in priority | Force ranking; use opportunity cost framing ("if we do X, we can't do Y"); require trade-offs |
| Effort estimates unreliable | Engineering uncertainty or sandbagging | Use ranges (2-4 weeks); add confidence factor; track actual vs. estimated to improve over time |
| Strategic priorities unclear | No direction from leadership | Escalate to leadership for clarity; use customer/revenue impact as proxy; document assumptions |
| Prioritization changes constantly | No discipline or commitment | Establish re-prioritization cadence (quarterly); require threshold for out-of-cycle changes |
| Political pressure overrides analysis | Leadership doesn't trust framework | Start with small wins showing framework works; make process transparent; get executive buy-in |

---

## Tips from Experience

1. **Involve the team.** Get engineering estimates, customer success feedback, sales input. Prioritization done in isolation lacks credibility.

2. **Show your work.** Transparent scoring builds trust. Stakeholders may disagree with conclusions but should understand the process.

3. **Use multiple frameworks.** RICE, MoSCoW, weighted scoring each have strengths. Try different approaches and see what resonates with your organization.

4. **Revisit regularly.** Priorities change—market shifts, strategy evolves, new data emerges. Reassess quarterly, not annually.

5. **Document decisions.** Why something was deprioritized matters as much as why it was chosen. Save future debates by recording rationale.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Prioritization completed in 2-3 hours (down from days of debate)
- [ ] 80%+ of stakeholders understand and accept the prioritization rationale
- [ ] Roadmap is actually followed (not constantly changed based on latest request)
- [ ] Team has confidence they're working on highest-impact items
- [ ] Clear criteria exist for when to say "yes" vs. "no" to new requests

**Track over time:**
- Roadmap predictability (% delivered as planned)
- Stakeholder satisfaction with prioritization process
- Business outcomes of shipped features vs. predictions
- Time spent in prioritization discussions (should decrease)

---

## Variations

### Technical Debt Prioritization
**When to use:** Prioritizing tech debt and infrastructure work
```
Apply similar framework weighing:
- Risk (what breaks if we don't fix this?)
- Engineering productivity impact
- Effort to address
- Time criticality

Mix tech debt items with features in single backlog for holistic prioritization.
```

### Bug Triage
**When to use:** Rapid prioritization for incoming bugs
```
Fast framework for bug prioritization:
- Severity: How bad is it? (Critical/High/Medium/Low)
- Frequency: How many users affected?
- Workaround: Is there a viable workaround?
- Risk: Security/data loss implications?

Scoring: (Severity × Frequency) / Workaround Availability
```

### OKR-Driven Prioritization
**When to use:** Organizations with strong OKR culture
```
Features scored purely on contribution to quarterly OKRs:
- Which key result does this move?
- By how much (estimated impact on metric)?
- How confident are we?

Only build features that meaningfully advance OKR progress.
```

---

## Building Your Repeatable System

After using this recipe 2-3 times, establish your system:

1. **Create standard templates** - Feature scoring template with RICE fields, prioritization matrix template for visualization, roadmap communication template, decision log for documenting why features were/weren't chosen.

2. **Build process integration** - Quarterly prioritization cycle aligned with planning, monthly backlog review with updated scores, sprint planning pulls from prioritized backlog, feature request intake feeds scoring pipeline.

3. **Establish scoring discipline** - Document your RICE scoring criteria (what's a "3" vs. "2" impact?), calibrate reach estimates to your actual user base, track actual effort vs. estimates to improve, build historical effort data for similar features.

4. **Close the loop** - Track feature outcomes vs. predictions, celebrate when prioritization was right, learn when it was wrong, share lessons to improve framework.

**Sample Folder Structure:**
```
feature-prioritization/
├── templates/
│   ├── rice-scoring-template.xlsx
│   ├── priority-matrix-template.pptx
│   └── roadmap-template.md
├── quarterly/
│   ├── 2024-Q1/
│   │   ├── feature-scoring.xlsx
│   │   ├── analysis-report.md
│   │   └── stakeholder-presentation.pptx
│   └── 2024-Q2/
├── decisions/
│   └── prioritization-decision-log.md
└── reference/
    ├── scoring-criteria.md
    └── effort-estimates-historical.xlsx
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**systematic evaluation across multiple criteria to make defensible priority decisions**—applies broadly:

| Role | Application |
|------|-------------|
| **IT/PMO** | Project portfolio prioritization across competing initiatives |
| **Marketing** | Campaign prioritization balancing reach, cost, and strategic fit |
| **Support** | Ticket triage and escalation based on severity, frequency, and impact |
| **HR** | Initiative prioritization (training, benefits, culture programs) |
| **Personal** | Task and goal prioritization using similar frameworks (impact/effort) |

---

## Next Steps

1. **This week:** Score your current backlog using RICE framework and identify top 5 priorities.

2. **Track your results:** Compare your data-driven prioritization to current roadmap. What would change?

3. **Iterate:** Refine estimates based on engineering feedback and market knowledge.

4. **Share:** Present prioritization rationale to stakeholders and get feedback on methodology.

---

*Recipe #89 of 100 in the Claude Code Knowledge Worker Recipe Collection*
