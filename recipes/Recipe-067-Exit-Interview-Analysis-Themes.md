# Exit Interview Analysis and Themes

**Recipe #67: Transform Departures into Retention Intelligence**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 5 minutes (first time) / 2 minutes (repeat) | 3-5 hours per analysis | Intermediate | HR, People Analytics, Leadership |

---

## The Problem

People leave, HR conducts exit interviews, and the data goes into a folder never to be seen again. Exit interviews capture valuable insights about why people leave, but nobody has time to analyze them systematically. The same issues surface repeatedly, but without pattern recognition, leadership doesn't see the trends. Retention problems persist because exit feedback isn't translated into action.

**Pain Points:**
- Exit interview data sits unused
- Same issues appear repeatedly without recognition
- No systematic analysis of departure reasons
- Feedback not translated to action
- Leadership unaware of patterns
- Retention efforts misaligned with actual causes
- No way to prioritize interventions

---

## The Outcome

Comprehensive analysis of exit interview data that identifies themes, trends, and actionable patterns. Clear visibility into why people leave, which groups are most affected, and what the organization can do about it. Data-driven retention strategies based on what departing employees actually say.

**What You'll Have When Done:**
- Theme identification and frequency
- Trend analysis over time
- Segment patterns (by dept, tenure, level)
- Root cause insights
- Representative quotes
- Prioritized recommendations
- Executive summary

---

## When to Use This Recipe

**Good Fit:**
- Quarterly or annual retention reviews
- After unusual attrition spikes
- Retention strategy development
- Leadership team briefings
- Board or investor updates
- HR program evaluation

**Not a Good Fit:**
- Real-time attrition monitoring (need dashboards)
- Individual departure analysis
- Very small sample sizes (<10 exits)
- Involuntary terminations (different data)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have exit interview data (structured or narrative)
- [ ] You know the time period to analyze
- [ ] You have demographic context (department, tenure, level)
- [ ] You have 30-60 minutes for comprehensive analysis

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Identifies themes across multiple interviews
- Groups similar feedback together
- Extracts representative quotes
- Analyzes patterns by segment
- Generates actionable recommendations
- Creates executive summaries

**Where Human Judgment Is Essential:**
- Validating theme accuracy
- Understanding context behind feedback
- Weighing political sensitivities
- Prioritizing actions
- Connecting to organizational reality
- Final recommendations

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Exit interviews | Full transcripts or summaries | Theme extraction |
| Demographics | Dept, tenure, level, performance | Segment analysis |
| Departure reasons | Stated reason for leaving | Reason categorization |
| Benchmark data | Industry turnover rates | Context |
| Context | Org changes, market conditions | Interpretation |

**Sample Input:**
```
Exit Interview Analysis Request

COMPANY: CloudSync Pro (150 employees)
ANALYSIS PERIOD: Q3 2024 (July - September)

ATTRITION DATA:
- Total departures: 18 (12% quarterly turnover, up from 8% Q2)
- Voluntary: 15
- Involuntary: 3
- Industry benchmark: 5-7% quarterly

EXIT INTERVIEW DATA (15 voluntary departures):

#1: Sarah M. | Sr. Engineer | Engineering | 2.5 years | High performer
Departure reason: Better opportunity
Key feedback:
- "I loved the team but felt stuck. No clear path to Staff Engineer."
- "Compensation wasn't competitive—I got a 40% raise at new company."
- "Management kept changing priorities. Hard to feel accomplished."

#2: Mike T. | Account Executive | Sales | 1.2 years | Solid performer
Departure reason: Career change
Key feedback:
- "The product is hard to sell right now—too many gaps."
- "Commission structure changed twice in my year here. Lost trust."
- "Sales and product don't communicate. We promise things we can't deliver."

#3: Jennifer L. | Product Manager | Product | 3.5 years | High performer
Departure reason: Better opportunity
Key feedback:
- "I learned so much here but it's time for a new challenge."
- "VP Product and I had different visions. I felt unheard."
- "Work-life balance deteriorated over the past year."

#4: David K. | Support Specialist | Customer Success | 8 months | Solid performer
Departure reason: Returning to school
Key feedback:
- "Good first job but I'm going back to school for my MBA."
- "Support is understaffed—too stressful."
- "No real growth path in support here."

#5: Amy C. | Marketing Manager | Marketing | 1.8 years | High performer
Departure reason: Better opportunity
Key feedback:
- "Marketing is underfunded. Can't compete with peers at other companies."
- "CEO doesn't value marketing—we're always the first cut."
- "Got an offer I couldn't refuse—30% raise plus director title."

#6: Tom R. | Engineer | Engineering | 11 months | Solid performer
Departure reason: Culture fit
Key feedback:
- "Engineering culture is toxic. Senior engineers are dismissive."
- "Code reviews are brutal—not constructive."
- "My manager was fine but couldn't shield us from the dysfunction."

#7: Lisa H. | Customer Success Manager | CS | 2.3 years | Top performer
Departure reason: Better opportunity
Key feedback:
- "I was burning out. Portfolio was too big, no relief in sight."
- "Loved my customers but leadership doesn't invest in CS."
- "Competitor offered me a better title, more money, and smaller portfolio."

[Continue with exits 8-15 with similar detail...]

#8: Kevin P. | Engineer | Engineering | 1.5 years | Solid performer
"Tech debt is crushing. We spend more time fixing than building."

#9: Rachel S. | Designer | Product | 2.1 years | High performer
"Design is treated as a service, not a partner. Tired of being an order-taker."

#10: James W. | SDR | Sales | 6 months | Low performer
"Quota was unrealistic. Set up to fail from day one."

#11: Michelle D. | HR Coordinator | HR | 1.1 years | Solid performer
"HR is understaffed. Can't do anything well because we're doing everything."

#12: Brian F. | Engineer | Engineering | 3.2 years | High performer
"Been passed over for Staff twice. Going somewhere that values my contributions."

#13: Nicole K. | Account Executive | Sales | 1.4 years | Solid performer
"Product gaps, constantly changing comp plan, and unrealistic quotas."

#14: Chris M. | Support Lead | CS | 2.8 years | High performer
"Promoted but no raise. Asked for 6 months, was told 'later'. Found 'now' elsewhere."

#15: Angela T. | Product Manager | Product | 1.9 years | High performer
"Vision changed three times this year. No strategy, just reaction."

DEMOGRAPHIC BREAKDOWN:
Engineering: 5 departures (20% of eng team)
Sales: 4 departures (26% of sales)
Customer Success: 3 departures (20% of CS)
Product: 2 departures (25% of product)
Other: 1 departure

BY TENURE:
<1 year: 4 (27%)
1-2 years: 7 (47%)
2-3 years: 3 (20%)
>3 years: 1 (6%)

BY PERFORMANCE:
High performer: 9 (60%)
Solid performer: 5 (33%)
Low performer: 1 (7%)

CONTEXT:
- Product roadmap reset in June (new VP Product)
- Sales comp plan changed January and June
- No company-wide raises in 2024 (cost controls)
- Support team headcount frozen since Q1
- Engineering promoted 2 to Staff in Q2 (out of 8 candidates)

AUDIENCE: Leadership team
PURPOSE: Quarterly retention review
```

---

## Step-by-Step Implementation

### Step 1: Compile Exit Interview Data
**Time: 10-15 minutes**

Gather:
- Exit interview notes or transcripts
- Demographic information
- Departure reasons
- Performance ratings
- Tenure information

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Exit Interview Analysis Prompt
**Time: 5-10 minutes for Claude to process**

---

**PRIMARY PROMPT: Exit Interview Analysis**

```
Please analyze these exit interviews to identify themes and retention insights.

COMPANY CONTEXT:
[Company background]

PERIOD: [Time period]
TOTAL VOLUNTARY DEPARTURES: [Number]
TURNOVER RATE: [Rate vs benchmark]

EXIT INTERVIEW DATA:
[Paste all exit interview summaries]

DEMOGRAPHIC BREAKDOWN:
[Departures by department, tenure, performance]

ORGANIZATIONAL CONTEXT:
[Recent changes, known issues]

ANALYSIS REQUIREMENTS:

1. EXECUTIVE SUMMARY
   - Overall finding
   - Top 3 themes
   - Most affected segments
   - Recommended immediate action
   - Risk assessment

2. THEME ANALYSIS

   For each identified theme:

   **THEME: [Name]**

   Frequency: [X] of [Total] exits ([%])
   Trend: [Increasing/Stable/Decreasing]
   Segments Affected: [Departments, levels, tenure]

   Summary: [2-3 sentence description]

   Representative Quotes:
   - "[Quote 1]" — [Person/role]
   - "[Quote 2]" — [Person/role]

   Root Cause Analysis:
   [What's driving this theme]

   Business Impact:
   [Cost, risk, operational impact]

   Recommended Action:
   - [Specific intervention]
   - Expected impact: [Result]

3. SEGMENT ANALYSIS

   **By Department:**
   | Department | Exits | Rate | Primary Theme | Risk Level |
   |------------|-------|------|---------------|------------|

   **By Tenure:**
   | Tenure Band | Exits | Rate | Primary Theme | Insight |
   |-------------|-------|------|---------------|---------|

   **By Performance:**
   | Performance | Exits | % | Concern Level | Implication |
   |-------------|-------|---|---------------|-------------|

4. HIGH PERFORMER ANALYSIS

   High performer departures: [X] of [Total] ([%])

   Common themes among high performers:
   - [Theme 1]
   - [Theme 2]

   This tells us:
   [Insight about what's driving top talent away]

5. TREND ANALYSIS

   Compared to previous period (if available):
   - Emerging themes: [New patterns]
   - Persistent themes: [Ongoing issues]
   - Improving themes: [What's getting better]

6. ROOT CAUSE MAPPING

   | Theme | Immediate Cause | Underlying Cause | Systemic Factor |
   |-------|-----------------|------------------|-----------------|

7. ACTIONABLE RECOMMENDATIONS

   **Immediate (30 days):**
   | Action | Addresses | Owner | Impact |
   |--------|-----------|-------|--------|

   **Short-term (90 days):**
   | Action | Addresses | Owner | Impact |
   |--------|-----------|-------|--------|

   **Strategic (6+ months):**
   | Action | Addresses | Owner | Impact |
   |--------|-----------|-------|--------|

8. RISK ASSESSMENT

   **Current Employees at Risk:**
   Based on patterns, these segments may be at higher risk:
   - [Segment]: [Why]

   **Estimated Retention Risk:**
   [Number] additional departures likely if no action taken

9. QUOTE LIBRARY

   Powerful quotes for leadership discussion:

   On [Theme 1]:
   - "[Quote]" — [Role, tenure]

   On [Theme 2]:
   - "[Quote]" — [Role, tenure]

10. WHAT WE'RE DOING WELL

    Positive feedback to preserve:
    - [Positive 1]: [Quote or evidence]

11. QUESTIONS FOR LEADERSHIP

    Issues requiring executive decision:
    - [Question 1]
    - [Question 2]

Provide frank, actionable analysis. Don't soften difficult findings.
```

---

### Step 4: Validate and Refine
**Time: 10-15 minutes**

Review:
- Are themes accurately identified?
- Do root causes seem correct?
- Are recommendations appropriate?
- Any sensitivities to handle?

---

### Step 5: Add Context and Nuance
**Time: 5-10 minutes**

```
Refine the analysis with additional context:

THEME ADJUSTMENTS:
- [Theme X] is partly explained by: [Context]
- [Theme Y] should be weighted higher because: [Reason]

SENSITIVE INFORMATION:
- [Exit X] involved: [Context leadership should know]
- Don't attribute quote about [topic] by name

ADDITIONAL PATTERNS:
- I also notice: [Pattern]
- Connect this to: [Related issue]
```

---

### Step 6: Generate Final Deliverables
**Time: 5 minutes**

```
Create final analysis package:

1. EXECUTIVE SUMMARY (1 page)
   - Key findings
   - Priority actions
   - Risk assessment

2. DETAILED ANALYSIS
   Full thematic analysis

3. LEADERSHIP DISCUSSION GUIDE
   Talking points for retention review

4. ACTION TRACKER
   Recommendations with owners and timelines

5. DASHBOARD DATA
   Metrics for ongoing tracking
```

---

## Example Output

Below is an abbreviated exit interview analysis example:

---

> **EXIT INTERVIEW ANALYSIS**
>
> **Q3 2024 | CloudSync Pro**
>
> ---
>
> ## Executive Summary
>
> **Overall Finding:** Q3 voluntary turnover (10%) is nearly double Q2 (5.3%) and significantly above industry benchmark (5-7%). This is no longer normal attrition—it's a retention crisis that requires immediate action.
>
> **Top 3 Themes:**
> 1. **Compensation Gap (53%):** Pay hasn't kept pace with market; high performers leaving for 30-40% raises
> 2. **Career Stagnation (40%):** Limited growth paths, promotions blocked, titles without raises
> 3. **Strategic Whiplash (33%):** Constantly changing priorities making work feel meaningless
>
> **Most Affected Segments:**
> - **High performers:** 60% of departures—we're losing our best people
> - **1-2 year tenure:** 47% of departures—the "figured it out, ready to grow" cohort
> - **Sales & Engineering:** 26% and 20% department turnover respectively
>
> **Recommended Immediate Action:**
> 1. Market compensation adjustment for top performers before more leave
> 2. Clear communication on Staff Engineer criteria (Engineering)
> 3. Sales comp plan stability commitment
>
> **Risk Assessment:** Without intervention, expect 5-8 additional departures in Q4, concentrated in Engineering and Sales high performers.
>
> ---
>
> ## Theme Analysis
>
> ### THEME 1: Compensation Gap
>
> **Frequency:** 8 of 15 exits (53%)
> **Trend:** Increasing (was 3rd theme in Q2)
> **Segments Affected:** Engineering (4), Sales (2), CS (1), Marketing (1)
>
> **Summary:**
> Departing employees report leaving for 30-40% pay increases. After no company-wide raises in 2024, the gap between CloudSync compensation and market has become untenable, especially for high performers with options.
>
> **Representative Quotes:**
> - "Compensation wasn't competitive—I got a 40% raise at new company." — Sarah M., Sr. Engineer
> - "Got an offer I couldn't refuse—30% raise plus director title." — Amy C., Marketing Manager
> - "Promoted but no raise. Asked for 6 months, was told 'later'. Found 'now' elsewhere." — Chris M., Support Lead
>
> **Root Cause Analysis:**
> - No raises in 2024 (cost controls) while market rates increased 5-8%
> - High performers who would normally be retained through equity/raises have no retention mechanism
> - Promotions without compensation adjustments ("empty promotions")
>
> **Business Impact:**
> - Replacement cost: $150K-200K per engineer (recruiting, ramp time, lost productivity)
> - Knowledge loss: Senior engineers and tenured employees taking institutional knowledge
> - Remaining team signal: "Leaving is how you get a raise"
>
> **Recommended Action:**
> - Conduct market compensation analysis for all high performers (Immediate)
> - Implement retention bonuses for critical roles (30 days)
> - Establish clear compensation philosophy and communicate it (90 days)
>
> ---
>
> ### THEME 2: Career Stagnation
>
> **Frequency:** 6 of 15 exits (40%)
> **Trend:** Stable (consistent theme)
> **Segments Affected:** Engineering (3), Product (2), CS (1)
>
> **Summary:**
> Employees feel stuck with unclear paths to advancement. Engineering's Staff promotion process is opaque, leaving high performers feeling passed over. Other functions lack defined career ladders entirely.
>
> **Representative Quotes:**
> - "No clear path to Staff Engineer." — Sarah M., Sr. Engineer
> - "Been passed over for Staff twice. Going somewhere that values my contributions." — Brian F., Engineer
> - "No real growth path in support here." — David K., Support Specialist
>
> **Root Cause Analysis:**
> - Engineering Staff promotion criteria unclear; 2 promoted from 8 candidates in Q2
> - Non-engineering functions lack career frameworks
> - Growth conversations not happening in 1:1s
>
> **Business Impact:**
> - High performers leave for "Senior" or "Staff" titles elsewhere
> - Mid-career employees (1-3 years) particularly affected
> - Creates perception that leaving is the only way to advance
>
> **Recommended Action:**
> - Document and communicate Staff Engineer criteria (30 days)
> - Develop career frameworks for CS and Support (90 days)
> - Train managers on career development conversations (90 days)
>
> ---
>
> ### THEME 3: Strategic Whiplash
>
> **Frequency:** 5 of 15 exits (33%)
> **Trend:** New/Increasing (tied to June roadmap reset)
> **Segments Affected:** Product (2), Engineering (2), Sales (1)
>
> **Summary:**
> The June product roadmap reset, combined with two sales comp plan changes, has created a sense that priorities change arbitrarily. Work feels meaningless when what mattered yesterday doesn't matter today.
>
> **Representative Quotes:**
> - "Management kept changing priorities. Hard to feel accomplished." — Sarah M., Sr. Engineer
> - "Vision changed three times this year. No strategy, just reaction." — Angela T., Product Manager
> - "Commission structure changed twice in my year here. Lost trust." — Mike T., Account Executive
>
> **Root Cause Analysis:**
> - New VP Product in June brought new priorities (expected but disruptive)
> - Sales comp changes driven by missed targets (reactive, not strategic)
> - Leadership not communicating "why" behind changes
>
> **Business Impact:**
> - Decreased engagement and discretionary effort
> - Product and Sales collaboration breaking down
> - Trust erosion affects future change management
>
> **Recommended Action:**
> - Commit to roadmap stability for remainder of 2024 (Immediate)
> - Commit to comp plan stability through 2025 (Immediate)
> - Conduct retrospective on change management and communicate learnings (60 days)
>
> ---
>
> ## High Performer Analysis
>
> **High Performer Departures:** 9 of 15 (60%)
>
> This is the most alarming finding. We are disproportionately losing our best people.
>
> **Common themes among high performers:**
> 1. Compensation (7 of 9) — They have options and they're exercising them
> 2. Career growth (5 of 9) — They're ready for more; we're not offering it
> 3. Feeling unheard (4 of 9) — "Different visions," "treated as a service"
>
> **What this tells us:**
> High performers are leaving because they can, and because we're not giving them reasons to stay. They have market-competitive options, they're ambitious about growth, and they want to feel valued. We're failing on all three.
>
> **The cost:**
> Losing a high performer costs 150-200% of salary in replacement and productivity loss. 9 high performers = $1.5-2M in direct and indirect costs.
>
> ---
>
> ## Segment Analysis
>
> ### By Department
>
> | Department | Exits | Turnover Rate | Primary Theme | Risk Level |
> |------------|-------|---------------|---------------|------------|
> | Sales | 4 | 26% | Comp + Instability | 🔴 Critical |
> | Product | 2 | 25% | Strategy + Voice | 🔴 Critical |
> | Engineering | 5 | 20% | Comp + Growth | 🔴 Critical |
> | Customer Success | 3 | 20% | Comp + Burnout | ⚠️ High |
> | Marketing | 1 | 14% | Comp + Recognition | ⚠️ Medium |
>
> ### By Tenure
>
> | Tenure | Exits | % of Total | Primary Theme | Insight |
> |--------|-------|------------|---------------|---------|
> | <1 year | 4 | 27% | Expectations | Early disillusionment |
> | 1-2 years | 7 | 47% | Growth + Comp | "Figured it out, ready for more" |
> | 2-3 years | 3 | 20% | Growth + Burnout | Veterans tired of fighting |
> | >3 years | 1 | 6% | Voice | Long-timers feel unheard |
>
> **The 1-2 Year Problem:**
> Nearly half of departures are from the 1-2 year tenure band. These are employees who've learned the role, proven themselves, and are ready for the next step—but they're finding that step outside CloudSync.
>
> ---
>
> ## Actionable Recommendations
>
> ### Immediate (30 days)
>
> | Action | Addresses | Owner | Impact |
> |--------|-----------|-------|--------|
> | Market adjustment for high performers | Comp gap | CFO/HR | Retain remaining top talent |
> | Publish Staff Engineer criteria | Career clarity | VP Eng | Stop Engineering bleeding |
> | Comp plan stability commitment | Sales trust | VP Sales | Rebuild Sales confidence |
>
> ### Short-term (90 days)
>
> | Action | Addresses | Owner | Impact |
> |--------|-----------|-------|--------|
> | Career frameworks for CS/Support | Growth paths | HR | Reduce CS turnover |
> | Compensation philosophy communication | Comp expectations | CEO | Transparency, manage expectations |
> | Manager training: career conversations | Career development | HR | Better retention conversations |
>
> ### Strategic (6+ months)
>
> | Action | Addresses | Owner | Impact |
> |--------|-----------|-------|--------|
> | Annual comp benchmarking process | Market competitiveness | HR/Finance | Prevent future gaps |
> | Retention bonus program | High performer retention | HR/Finance | Proactive retention |
> | Change management improvement | Strategic stability | Leadership | Reduce whiplash perception |
>
> ---
>
> ## Risk Assessment
>
> **Current Employees at Risk:**
>
> Based on exit patterns, these segments show highest flight risk:
> - Engineering high performers at 2+ years tenure (5-7 people)
> - Sales reps in first 2 years (4-6 people)
> - Product team members who worked under previous VP (2-3 people)
>
> **Estimated Additional Departures:**
> Without intervention: 5-8 departures in Q4
> With immediate action: 2-3 departures in Q4
>
> **Cost of Inaction:**
> - Direct costs: $750K-1.2M (replacement + ramp)
> - Indirect costs: Remaining team demoralization, customer impact, project delays
>
> ---
>
> ## What We're Doing Well
>
> Don't lose sight of positives mentioned:
>
> - "I loved the team" — Team relationships are strong
> - "I learned so much here" — We develop talent
> - "Loved my customers" — Customer relationships are valued
> - "My manager was fine" — Front-line management is acceptable
>
> **These are assets to protect.** Retention efforts should not undermine what's working.
>
> ---
>
> ## Questions for Leadership
>
> 1. **Are we prepared to make market comp adjustments?** Without this, expect continued bleeding.
>
> 2. **What is our actual career framework commitment?** Words without action will backfire.
>
> 3. **Can we commit to strategy stability?** Another pivot will accelerate departures.
>
> 4. **Do we accept higher turnover as the cost of our choices?** If so, plan for it explicitly.

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Themes too generic | Surface-level analysis | Ask: "Go deeper on [theme]. What's the specific driver? What makes this unique to us?" |
| Missing patterns | Not enough data | Acknowledge: "Sample size is limited. These are directional insights, not statistically significant." |
| Recommendations too obvious | Not actionable enough | Ask: "Make recommendations specific. Who does what by when? What would success look like?" |
| Feedback contradictory | Different experiences | Present both: "Some say X while others say Y. This may indicate department/manager variation." |
| Too negative | All criticism | Add: "Include positive feedback. What do people appreciate? What should we protect?" |

---

## Tips from Experience

1. **High performer departures matter most.** Track this separately—it's your canary in the coal mine.

2. **Look for patterns, not just themes.** Who is leaving (not just why) tells you where to focus.

3. **Quote with care.** Quotes are powerful but can identify people. Anonymize appropriately.

4. **Connect to business impact.** "9 exits" becomes urgent when it's "$1.5M cost."

5. **Don't wait for large samples.** Trends can be seen in small numbers if you're paying attention.

6. **Close the loop.** Tell leadership what you found, what you did, and whether it worked.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Themes are validated by leadership
- [ ] Actions are taken on recommendations
- [ ] Turnover trends improve
- [ ] High performer retention improves
- [ ] Exit interview themes shift
- [ ] Analysis becomes routine

**Track over time:**
- Voluntary turnover rate (overall, by segment)
- High performer turnover specifically
- Theme frequency changes
- Action implementation rate
- Time from exit to analysis
- Leadership engagement with findings

---

## Variations

### Regrettable vs Non-Regrettable Analysis
For nuanced retention view:
```
Separate analysis:
- Regrettable departures (wanted to keep)
- Non-regrettable departures (acceptable loss)
- Different patterns and recommendations for each
- Investment focus on regrettable departure causes

Include: Regret rate tracking over time
```

### Manager-Level Analysis
For identifying manager patterns:
```
Add layer:
- Departures by manager
- Theme variation by manager
- High vs low turnover managers
- Manager intervention recommendations

Sensitive: Handle carefully, focus on patterns not individuals
```

### Stay Interview Comparison
For proactive retention:
```
Compare exit data to stay interviews:
- What do people who stay say vs those who leave?
- Early warning indicators
- Intervention timing recommendations
- Prediction model inputs

Include: At-risk employee identification
```

### Department Deep Dive
For focused analysis:
```
Single department analysis:
- All exits from [department]
- Unique departmental factors
- Department-specific recommendations
- Comparison to company-wide trends

Include: Department leader action plan
```

---

## Building Your Repeatable System

After several analysis cycles, establish:

1. **Consistent exit interview format** for better data
2. **Regular analysis cadence** (quarterly or monthly)
3. **Standard theme taxonomy** for tracking
4. **Action tracking system** for follow-through
5. **Trend dashboard** for ongoing visibility

**Sample Setup:**
```
exit-analysis/
├── quarterly/
│   ├── q3-2024-analysis.md
│   ├── q2-2024-analysis.md
│   └── [quarter by quarter]
├── data/
│   ├── exit-interviews/
│   │   └── [individual interview notes]
│   ├── demographics.csv
│   └── themes-tracking.csv
├── templates/
│   ├── exit-interview-guide.md
│   └── analysis-template.md
├── actions/
│   └── retention-action-tracker.md
├── dashboards/
│   └── turnover-metrics.md
└── presentations/
    └── leadership-briefings/
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**collect feedback → identify themes → analyze patterns → recommend action**—applies broadly:

| Role | Application |
|------|-------------|
| **HR** | All employee feedback analysis |
| **Customer Success** | Churn reason analysis |
| **Product** | Feature request synthesis |
| **Sales** | Lost deal analysis |
| **Support** | Complaint pattern analysis |
| **Operations** | Incident pattern analysis |

---

## Next Steps

1. **Gather exit data:** Compile interviews from target period
2. **Add context:** Department, tenure, performance info
3. **Run analysis:** Use this recipe
4. **Validate findings:** Check with HR and managers
5. **Present to leadership:** Share findings and recommendations
6. **Track action:** Ensure follow-through on recommendations

---

*Recipe #67 of 100 in the Claude Code Knowledge Worker Recipe Collection*
