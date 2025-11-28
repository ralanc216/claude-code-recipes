# Compensation Analysis and Recommendations

**Recipe #68: Make Data-Driven Pay Decisions**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 10 minutes (first time) / 5 minutes (repeat) | 4-8 hours per analysis | Intermediate | HR, Total Rewards, Finance, Managers |

---

## The Problem

Compensation decisions are made inconsistently—some squeaky wheels get raises while quiet performers don't. Market data exists but nobody has time to analyze it properly. Internal equity problems fester until someone threatens to leave. Offers are made without understanding the full picture. Leaders don't have clear rationale for pay decisions, leading to perceived unfairness and attrition.

**Pain Points:**
- No systematic approach to compensation decisions
- Market data underutilized
- Internal equity problems ignored until crisis
- Offers made without full context
- Can't explain why pay differs
- Managers making pay promises they can't keep
- Attrition due to compensation but discovered too late

---

## The Outcome

Comprehensive compensation analysis comparing internal pay to market data, identifying equity issues, and providing clear recommendations. Data-driven support for pay decisions that can withstand scrutiny and support retention.

**What You'll Have When Done:**
- Market positioning analysis
- Internal equity assessment
- Individual compensation reviews
- Adjustment recommendations
- Budget impact analysis
- Decision rationale documentation

---

## When to Use This Recipe

**Good Fit:**
- Annual compensation review cycles
- Offer calibration
- Retention risk assessment
- Promotion decisions
- Equity analysis
- Pay band development
- Budget planning

**Not a Good Fit:**
- Executive compensation (board-level, specialized)
- International pay where local expertise needed
- Sales compensation design (different model)
- Equity/stock compensation (specialized area)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have internal compensation data
- [ ] You have market data or benchmarks
- [ ] You understand job levels and grades
- [ ] You have 45-60 minutes for comprehensive analysis

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Analyzes compensation data systematically
- Identifies outliers and equity issues
- Compares to market benchmarks
- Generates recommendation rationale
- Creates budget scenarios
- Documents decision support

**Where Human Judgment Is Essential:**
- Validating market data relevance
- Understanding individual situations
- Making final pay decisions
- Considering political factors
- Ensuring legal compliance
- Approving recommendations

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Employee data | Current pay, level, tenure | Internal analysis |
| Market data | Salary surveys, benchmarks | External comparison |
| Pay structure | Bands, grades | Framework reference |
| Performance | Ratings, calibration | Merit consideration |
| Context | Budget, strategy | Constraint consideration |

**Sample Input:**
```
Compensation Analysis Request

COMPANY: CloudSync Pro
ANALYSIS TYPE: Annual compensation review
BUDGET: 4% of base salary budget for adjustments
TIMING: Effective February 1, 2025

PAY PHILOSOPHY:
- Target 50th percentile of market for base
- Target 75th percentile total compensation (with equity)
- Pay for performance—top performers above median
- Ensure internal equity within job families

MARKET DATA SOURCE: Radford Technology Survey 2024

EMPLOYEE DATA (Sample - Engineering Department):

| Name | Role | Level | Tenure | Base | Bonus Target | Equity Value | Total | Performance | Market 50th | Market 75th |
|------|------|-------|--------|------|--------------|--------------|-------|-------------|-------------|-------------|
| Sarah Chen | Software Engineer | E3 | 2.5 yrs | $145,000 | 10% | $30,000 | $189,500 | Exceeds | $155,000 | $175,000 |
| Mike Wong | Software Engineer | E3 | 1.2 yrs | $142,000 | 10% | $25,000 | $181,200 | Meets | $155,000 | $175,000 |
| Jennifer Lee | Software Engineer | E3 | 3.5 yrs | $138,000 | 10% | $35,000 | $186,800 | Exceeds | $155,000 | $175,000 |
| David Kim | Sr. Engineer | E4 | 2.0 yrs | $175,000 | 15% | $50,000 | $251,250 | Exceeds | $185,000 | $210,000 |
| Amy Johnson | Sr. Engineer | E4 | 0.8 yrs | $185,000 | 15% | $45,000 | $257,750 | Meets | $185,000 | $210,000 |
| Tom Rodriguez | Sr. Engineer | E4 | 4.2 yrs | $168,000 | 15% | $55,000 | $248,200 | Exceeds | $185,000 | $210,000 |
| Lisa Huang | Staff Engineer | E5 | 3.0 yrs | $210,000 | 20% | $80,000 | $332,000 | Exceeds | $225,000 | $260,000 |
| Kevin Park | Staff Engineer | E5 | 1.5 yrs | $220,000 | 20% | $75,000 | $339,000 | Meets | $225,000 | $260,000 |
| Brian Foster | Eng Manager | M1 | 2.8 yrs | $195,000 | 20% | $70,000 | $304,000 | Exceeds | $205,000 | $235,000 |
| Rachel Scott | Eng Manager | M1 | 1.0 yrs | $205,000 | 20% | $60,000 | $306,000 | Meets | $205,000 | $235,000 |

CURRENT ISSUES FLAGGED:
- Jennifer Lee (E3) has below-market base despite top performance and tenure
- Tom Rodriguez (E4) was passed over for Staff promotion; flight risk
- David Kim recently received competing offer (~$200K base)

BUDGET AVAILABLE:
- 4% of base salary pool = $177,800 (for this group)
- Promotion budget separate

QUESTIONS TO ANSWER:
1. Who is significantly below market?
2. Where are internal equity issues?
3. Who should receive adjustments and how much?
4. How should we prioritize within budget?
5. Who is at retention risk?
```

---

## Step-by-Step Implementation

### Step 1: Gather Compensation Data
**Time: 10-15 minutes**

Collect:
- Current employee compensation (all components)
- Market benchmark data
- Performance ratings
- Tenure and level information
- Known issues or risks

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Compensation Analysis Prompt
**Time: 5-8 minutes for Claude to process**

---

**PRIMARY PROMPT: Compensation Analysis**

```
Please analyze this compensation data and provide recommendations.

COMPANY: [Company name]
PAY PHILOSOPHY: [Compensation philosophy]

MARKET DATA SOURCE: [Survey or benchmark]

EMPLOYEE COMPENSATION DATA:
[Paste employee compensation table]

KNOWN ISSUES:
[Any flagged concerns]

BUDGET AVAILABLE:
[Budget for adjustments]

ANALYSIS REQUIREMENTS:

1. EXECUTIVE SUMMARY
   - Overall compensation health
   - Key issues identified
   - Budget utilization recommendation
   - Highest priority actions
   - Risk assessment

2. MARKET POSITIONING ANALYSIS

   **By Level:**
   | Level | # Employees | Avg Base | Market 50th | Position | Gap |
   |-------|-------------|----------|-------------|----------|-----|

   **Overall Market Position:**
   - Below market (<90% of 50th): [X] employees
   - At market (90-110%): [X] employees
   - Above market (>110%): [X] employees

   **Market Position by Performance:**
   | Performance | Avg Market Ratio | Concern |
   |-------------|------------------|---------|

3. INTERNAL EQUITY ANALYSIS

   **Within-Level Equity:**
   | Level | Min | Max | Spread | Concern |
   |-------|-----|-----|--------|---------|

   **Equity Issues Identified:**
   - [Issue 1]: [Description]
   - [Issue 2]: [Description]

   **Compa-Ratio Analysis:**
   | Employee | Compa-Ratio | Position | Flag |
   |----------|-------------|----------|------|

4. INDIVIDUAL ANALYSIS

   For each employee:

   **[Name] — [Role] — [Level]**

   Current Compensation:
   - Base: $[X] | Market 50th: $[X] | Position: [X]%
   - Total: $[X] | Market 75th: $[X] | Position: [X]%

   Performance: [Rating]
   Tenure: [X] years
   Internal Equity: [Comparison to peers]

   Assessment:
   [Overall assessment of comp appropriateness]

   Recommendation:
   - [Recommended action]
   - Amount: $[X] ([X]% increase)
   - Rationale: [Why]
   - Priority: [High/Medium/Low]

5. RETENTION RISK ASSESSMENT

   **High Risk:**
   | Employee | Risk Factors | Impact if Lost | Recommended Action |
   |----------|--------------|----------------|-------------------|

   **Medium Risk:**
   | Employee | Risk Factors | Monitoring |
   |----------|--------------|------------|

6. BUDGET ALLOCATION

   **Recommended Distribution:**
   | Category | # Employees | Amount | % of Budget |
   |----------|-------------|--------|-------------|
   | Market corrections | X | $X | X% |
   | Equity adjustments | X | $X | X% |
   | Performance merit | X | $X | X% |
   | Retention/proactive | X | $X | X% |

   **Individual Allocations:**
   | Employee | Adjustment | % Increase | Rationale | Priority |
   |----------|------------|------------|-----------|----------|

   **Budget Summary:**
   - Total recommended: $[X]
   - Budget available: $[X]
   - Variance: $[X] ([over/under])

7. SCENARIO ANALYSIS

   **Scenario 1: Budget Constrained**
   If budget reduced to [X]%, prioritize:
   - [Priority 1]
   - [Priority 2]

   **Scenario 2: Budget Increased**
   If additional [X]% available, add:
   - [Addition 1]
   - [Addition 2]

8. PAY EQUITY CHECK

   **Gender Analysis:**
   | Level | Male Avg | Female Avg | Gap |
   |-------|----------|------------|-----|

   **Tenure Analysis:**
   | Level | <2yr Avg | >2yr Avg | Gap |
   |-------|----------|----------|-----|

   **Issues Identified:**
   - [Issue if any]

9. MANAGER TALKING POINTS

   For each recommended adjustment:

   **[Employee Name]:**
   - What to say: [Script]
   - Rationale to share: [Points]
   - Questions to anticipate: [Q&A]

10. DOCUMENTATION

    **Decision Record:**
    For compliance and future reference:

    | Employee | Current | New | Change | Effective | Rationale |
    |----------|---------|-----|--------|-----------|-----------|

Provide specific, defensible recommendations with clear rationale.
```

---

### Step 4: Validate Analysis
**Time: 10-15 minutes**

Review:
- Are market comparisons appropriate?
- Are individual situations understood?
- Do recommendations align with philosophy?
- Any concerns with proposed distribution?

---

### Step 5: Refine Recommendations
**Time: 5-10 minutes**

```
Refine the compensation analysis:

INDIVIDUAL ADJUSTMENTS:
- [Employee X]: Adjust recommendation to [amount] because [reason]
- [Employee Y]: Needs [special consideration]

BUDGET CONSTRAINTS:
- Must prioritize [X] over [Y]
- Cannot exceed [amount]

POLITICAL CONSIDERATIONS:
- [Person] recently had [situation]
- [Team] needs careful messaging

ADDITIONAL CONTEXT:
- [Employee X] was recently promoted/hired at [terms]
- [Market data] may be dated for [role]
```

---

### Step 6: Generate Final Package
**Time: 5 minutes**

```
Create final compensation package:

1. EXECUTIVE SUMMARY (for leadership approval)
2. DETAILED ANALYSIS (for HR records)
3. INDIVIDUAL RECOMMENDATIONS (for implementation)
4. MANAGER COMMUNICATION GUIDE
5. EMPLOYEE LETTERS (templates)
6. BUDGET RECONCILIATION
```

---

## Example Output

Below is an abbreviated compensation analysis example:

---

> **COMPENSATION ANALYSIS**
>
> **Engineering Department | Annual Review 2025**
>
> ---
>
> ## Executive Summary
>
> **Overall Compensation Health:** Needs Attention
>
> The Engineering team has several below-market situations, particularly at the E3 (mid-level engineer) level. Internal equity issues exist where tenure and performance haven't been rewarded appropriately. The 4% budget is sufficient to address critical issues but not enough for comprehensive market alignment.
>
> **Key Issues:**
> 1. Jennifer Lee (E3) significantly below market despite top performance
> 2. Tom Rodriguez (E4) below market and recent promotion pass-over creates risk
> 3. David Kim (E4) needs retention action due to competing offer
>
> **Budget Utilization:** Recommend using full 4% ($177,800), heavily weighted toward market corrections and retention.
>
> **Highest Priority Actions:**
> 1. Address David Kim competing offer situation immediately
> 2. Correct Jennifer Lee market gap
> 3. Proactive adjustment for Tom Rodriguez
>
> **Risk Assessment:** Without action, high probability of losing 2-3 senior engineers in Q1, costing $400K+ in replacement costs.
>
> ---
>
> ## Market Positioning Analysis
>
> ### By Level
>
> | Level | # | Avg Base | Market 50th | Position | Assessment |
> |-------|---|----------|-------------|----------|------------|
> | E3 | 3 | $141,667 | $155,000 | 91% | Below target |
> | E4 | 3 | $176,000 | $185,000 | 95% | Slightly below |
> | E5 | 2 | $215,000 | $225,000 | 96% | Slightly below |
> | M1 | 2 | $200,000 | $205,000 | 98% | At target |
>
> **Overall Position:** The team averages 94% of market 50th percentile, below the 100% target. E3 level is most concerning.
>
> **Market Position by Performance:**
>
> | Performance | Avg Market Ratio | Concern |
> |-------------|------------------|---------|
> | Exceeds | 93% | High—top performers below market |
> | Meets | 98% | Acceptable |
>
> **Critical Finding:** Top performers (Exceeds) are paid 5% less than solid performers (Meets) relative to market. This is backwards and creates retention risk.
>
> ---
>
> ## Internal Equity Analysis
>
> ### Within-Level Spread
>
> | Level | Min | Max | Spread | Concern |
> |-------|-----|-----|--------|---------|
> | E3 | $138,000 | $145,000 | 5% | Low spread, but lowest paid is top performer |
> | E4 | $168,000 | $185,000 | 10% | Acceptable, but recent hire paid most |
> | E5 | $210,000 | $220,000 | 5% | Acceptable |
> | M1 | $195,000 | $205,000 | 5% | Acceptable |
>
> ### Equity Issues Identified
>
> 1. **Jennifer Lee vs. Sarah Chen (E3):** Jennifer has 1 year more tenure, both Exceeds performers, but Jennifer is paid $7K less. Jennifer should be paid more, not less.
>
> 2. **Tom Rodriguez vs. Amy Johnson (E4):** Tom has 3.4 years more tenure, better performance, but paid $17K less than recent hire Amy. Tom has been "rewarded" for loyalty with lower pay.
>
> 3. **Performance inversion:** In both E3 and E4, there are situations where top performers are paid at or below solid performers.
>
> ---
>
> ## Individual Analysis
>
> ### Jennifer Lee — Software Engineer — E3
>
> **Current Compensation:**
> - Base: $138,000 | Market 50th: $155,000 | Position: 89%
> - Total: $186,800 | Market 75th: $220,000 | Position: 85%
>
> **Performance:** Exceeds
> **Tenure:** 3.5 years (longest at E3)
>
> **Assessment:**
> Jennifer is the top-tenured, top-performing E3 but the lowest paid. She's 11% below market on base. Given her performance and tenure, she should be at or above market 50th, not 11% below. High flight risk if not addressed.
>
> **Recommendation:**
> - Action: Market adjustment
> - Amount: +$17,000 (12.3% increase)
> - New Base: $155,000
> - Rationale: Top performer, longest tenure, currently below market and lowest paid at level
> - Priority: **High**
>
> ---
>
> ### David Kim — Sr. Engineer — E4
>
> **Current Compensation:**
> - Base: $175,000 | Market 50th: $185,000 | Position: 95%
> - Total: $251,250 | Market 75th: $305,000 | Position: 82%
>
> **Performance:** Exceeds
> **Tenure:** 2.0 years
>
> **Assessment:**
> David recently received a competing offer at ~$200K base. He's currently 5% below market with Exceeds performance. Without action, we will lose him. Counter-offer typically costs more than proactive adjustment.
>
> **Recommendation:**
> - Action: Retention adjustment (proactive counter)
> - Amount: +$20,000 (11.4% increase)
> - New Base: $195,000
> - Rationale: Competing offer, top performer, below market
> - Priority: **Urgent**
>
> ---
>
> ### Tom Rodriguez — Sr. Engineer — E4
>
> **Current Compensation:**
> - Base: $168,000 | Market 50th: $185,000 | Position: 91%
> - Total: $248,200 | Market 75th: $305,000 | Position: 81%
>
> **Performance:** Exceeds
> **Tenure:** 4.2 years
>
> **Assessment:**
> Tom was passed over for Staff promotion despite strong performance. He's the lowest-paid E4 despite being the most tenured and a top performer. This is a significant equity and retention issue. He's paid $17K less than Amy Johnson who has been here 3 years less.
>
> **Recommendation:**
> - Action: Market correction + equity adjustment
> - Amount: +$17,000 (10.1% increase)
> - New Base: $185,000
> - Rationale: Market correction, equity with peers, retention (passed over for promo)
> - Priority: **High**
>
> ---
>
> ## Budget Allocation
>
> ### Recommended Distribution
>
> | Category | # Employees | Amount | % of Budget |
> |----------|-------------|--------|-------------|
> | Market corrections | 3 | $47,000 | 26% |
> | Equity adjustments | 2 | $10,000 | 6% |
> | Performance merit | 4 | $28,800 | 16% |
> | Retention/proactive | 2 | $37,000 | 21% |
> | Reserve | — | $55,000 | 31% |
>
> ### Individual Allocations
>
> | Employee | Current | Adjustment | New | % Inc | Rationale | Priority |
> |----------|---------|------------|-----|-------|-----------|----------|
> | David Kim | $175,000 | +$20,000 | $195,000 | 11.4% | Competing offer, retention | Urgent |
> | Jennifer Lee | $138,000 | +$17,000 | $155,000 | 12.3% | Market, equity, performance | High |
> | Tom Rodriguez | $168,000 | +$17,000 | $185,000 | 10.1% | Market, equity, retention | High |
> | Sarah Chen | $145,000 | +$7,000 | $152,000 | 4.8% | Performance merit | Medium |
> | Lisa Huang | $210,000 | +$12,000 | $222,000 | 5.7% | Market, performance | Medium |
> | Brian Foster | $195,000 | +$8,000 | $203,000 | 4.1% | Performance merit | Medium |
> | Mike Wong | $142,000 | +$5,000 | $147,000 | 3.5% | Standard merit | Low |
> | Amy Johnson | $185,000 | $0 | $185,000 | 0% | Recent hire, at market | None |
> | Kevin Park | $220,000 | $0 | $220,000 | 0% | At market, meets perf | None |
> | Rachel Scott | $205,000 | $0 | $205,000 | 0% | Recent hire, at market | None |
>
> ### Budget Summary
>
> - Total recommended: $86,000
> - Budget available: $177,800
> - Remaining: $91,800 (reserve for mid-year adjustments or additional needs)
>
> ---
>
> ## Retention Risk Assessment
>
> ### High Risk
>
> | Employee | Risk Factors | Impact if Lost | Action |
> |----------|--------------|----------------|--------|
> | David Kim | Competing offer, below market | Critical project knowledge | Urgent adjustment |
> | Tom Rodriguez | Passed over for promo, equity issue | 4+ years tenure, high performer | Adjustment + career conversation |
> | Jennifer Lee | Below market, top performer | Team productivity | Immediate adjustment |
>
> ### Medium Risk
>
> | Employee | Risk Factors | Monitoring |
> |----------|--------------|------------|
> | Lisa Huang | Below market Staff | Monitor competitor activity |
>
> **Cost of Losing High-Risk Employees:**
> - 3 senior engineers × $200K replacement cost = $600K
> - Plus: Project delays, team morale, knowledge loss
>
> **Cost of Recommended Adjustments:** $54,000
> **ROI:** Prevent $600K loss with $54K investment = 11x return
>
> ---
>
> ## Manager Talking Points
>
> ### For David Kim:
>
> **What to say:**
> "David, I want to talk about your compensation. We know you received an offer, and more importantly, we know your value. We're adjusting your base to $195,000, effective February 1. This puts you above market and reflects your performance. We want you here, and this is us showing that commitment."
>
> **Rationale to share:**
> - Market correction—we want you above market given your performance
> - Recognition of your contributions to [specific project]
> - Investment in you long-term
>
> **Questions to anticipate:**
> - "Why didn't this happen sooner?" — "We should have been more proactive. We're fixing that now and implementing better monitoring."
> - "What about equity?" — "Let's discuss that separately. I want to review your equity position in our Q2 refresh."
>
> ---
>
> ### For Tom Rodriguez:
>
> **What to say:**
> "Tom, I want to address your compensation and also talk about your career. First, we're adjusting your base to $185,000. This corrects a gap that should have been addressed earlier. Second, I want to discuss the Staff path with you..."
>
> **Rationale to share:**
> - Market correction and internal equity
> - Recognition of tenure and consistent top performance
> - Commitment to his growth
>
> **Questions to anticipate:**
> - "What about Staff?" — "Let's map out specifically what you need to demonstrate for Staff. I want to be your advocate in the next cycle."

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Market data seems off | Survey mismatch to roles | Verify: "Confirm job matching. Is Survey Role X really comparable to our Role Y?" |
| Recommendations exceed budget | Too many issues | Prioritize: "Rank recommendations by risk and impact. What's non-negotiable?" |
| Internal equity conflicts | Competing considerations | Document: "Show the analysis, explain the trade-offs, let leadership decide" |
| Recent hires complicate things | Higher starting salaries | Address: "May need to bring others up; document compression issues" |
| Performance ratings questionable | Inconsistent calibration | Flag: "Analysis assumes ratings are accurate. If calibration uncertain, note as limitation." |

---

## Tips from Experience

1. **Address retention risk before it becomes resignation.** Proactive adjustments cost less than counter-offers.

2. **Fix equity issues even if no complaint.** Just because they haven't complained doesn't mean they don't know.

3. **Document everything.** Decisions should be defensible if audited later.

4. **Consider total compensation.** Base isn't everything—look at the whole picture.

5. **Prepare managers.** They'll be delivering the news. Make sure they understand the rationale.

6. **Plan for the "why me?" questions.** Every adjustment raises questions from those who didn't get one.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Compensation decisions are data-driven
- [ ] Internal equity issues are addressed
- [ ] Market positioning improves
- [ ] Retention improves
- [ ] Budget is used strategically
- [ ] Managers feel equipped to communicate

**Track over time:**
- Market position by level
- Internal equity metrics
- Comp-related attrition
- Offer acceptance rates
- Employee satisfaction with comp
- Time to complete analysis

---

## Variations

### New Hire Offer Calibration
For setting competitive offers:
```
Analyze for offer setting:
- Market range for role
- Internal equity implications
- Candidate experience level
- Offer recommendation with rationale
- Counter-offer threshold

Include: Offer range guidance, negotiation room
```

### Promotion Compensation
For promotion-related adjustments:
```
Focus on:
- New level market data
- Appropriate promotion increase (typically 10-15%)
- Internal equity at new level
- Total compensation alignment
- Timeline for next review

Include: Promotion vs hire comparison
```

### Pay Equity Audit
For compliance and fairness:
```
Statistical analysis:
- Gender pay analysis by level
- Race/ethnicity analysis (if available)
- Tenure analysis
- Regression analysis for unexplained gaps
- Remediation recommendations

Include: Legal defensibility considerations
```

### Annual Merit Planning
For organization-wide merit:
```
Budget modeling:
- Performance distribution
- Merit matrix design
- Budget allocation by org
- Manager discretion guidelines
- Communication timeline

Include: Merit increase grid, exception process
```

---

## Building Your Repeatable System

After several compensation cycles, establish:

1. **Standard analysis template**
2. **Market data update schedule**
3. **Consistent market matching**
4. **Decision documentation format**
5. **Communication templates**

**Sample Setup:**
```
compensation-analysis/
├── annual-reviews/
│   ├── 2025/
│   │   ├── engineering-analysis.md
│   │   ├── sales-analysis.md
│   │   └── [by department]
│   └── [by year]
├── market-data/
│   ├── radford-2024.xlsx
│   └── market-summary.md
├── templates/
│   ├── analysis-template.md
│   ├── manager-talking-points.md
│   └── employee-letter.md
├── reference/
│   ├── pay-philosophy.md
│   ├── job-matching-guide.md
│   └── grade-structure.md
└── documentation/
    └── decision-records/
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**compare to benchmark → identify gaps → prioritize actions → document decisions**—applies broadly:

| Role | Application |
|------|-------------|
| **HR/Total Rewards** | All compensation decisions |
| **Finance** | Budget allocation, vendor pricing |
| **Sales** | Territory/quota analysis |
| **Operations** | Staffing level analysis |
| **Procurement** | Vendor cost analysis |
| **Product** | Pricing decisions |

---

## Next Steps

1. **Gather data:** Current comp, market benchmarks
2. **Define scope:** Which roles/levels to analyze
3. **Run analysis:** Use this recipe
4. **Validate with stakeholders:** HR, Finance, leadership
5. **Finalize recommendations:** Within budget
6. **Communicate:** Equip managers, inform employees

---

*Recipe #68 of 100 in the Claude Code Knowledge Worker Recipe Collection*
