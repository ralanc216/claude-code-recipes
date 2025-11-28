# Sales Pipeline Analysis and Commentary

**Recipe #55: Transform Pipeline Data into Sales Strategy**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 5 minutes (first time) / 2 minutes (repeat) | 2-3 hours per pipeline review | Beginner | Sales Leaders, Revenue Operations, Finance |

---

## The Problem

Pipeline reviews happen weekly, but the same questions come up every time: "Are we going to hit the number?" "Which deals will close?" "Where are we stuck?" Sales leaders spend hours in CRM exports trying to answer these questions. The data is there, but the insight isn't. Pipeline coverage ratios give false confidence. Stalled deals hide in plain sight. Forecasts miss because commentary doesn't match reality.

**Pain Points:**
- Hours spent analyzing CRM data for each pipeline review
- "We have enough coverage" followed by missed quarters
- Stalled deals invisible until it's too late
- Same deals "closing next month" for three months
- No systematic view of pipeline health
- Forecast accuracy is poor
- Can't identify patterns across deals

---

## The Outcome

Structured pipeline analysis that reveals the true health of your revenue forecast. Commentary that identifies which deals are real, which are at risk, and where to focus. Insights that improve forecast accuracy and drive strategic action.

**What You'll Have When Done:**
- Pipeline health assessment
- Deal-level risk scoring
- Stage conversion analysis
- Velocity trends
- Forecast confidence levels
- Focus recommendations
- Executive-ready summary

---

## When to Use This Recipe

**Good Fit:**
- Weekly pipeline reviews
- Monthly forecast preparation
- Quarterly business reviews
- Sales strategy sessions
- Territory planning
- Deal review meetings
- Board prep on revenue outlook

**Not a Good Fit:**
- Real-time deal monitoring (need CRM alerts)
- Individual deal strategy (too detailed)
- Commission calculations (use finance tools)
- CRM data cleanup (different process)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have pipeline data exported from CRM
- [ ] You know the period targets (quota)
- [ ] You have historical conversion rates
- [ ] You have 30-45 minutes for comprehensive analysis

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Analyzes pipeline metrics systematically
- Identifies patterns across deals
- Calculates conversion probabilities
- Generates risk assessments
- Structures findings clearly
- Creates actionable commentary

**Where Human Judgment Is Essential:**
- Validating deal-level assessments
- Understanding relationship dynamics
- Knowing competitive situations
- Assessing rep credibility
- Making final forecast calls
- Prioritizing action

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Pipeline data | Deal list with stages, amounts | Core analysis |
| Historical rates | Win rates by stage | Probability assessment |
| Targets | Quota by period | Gap analysis |
| Activity data | Last touch, next steps | Velocity analysis |
| Context | Known situations | Deal assessment |

**Sample Input:**
```
Pipeline Analysis Request

PERIOD: Q4 2024 (October - December)
CURRENT DATE: November 15, 2024
DAYS REMAINING: 46 days

TARGETS:
- Q4 Quota: $3.2M
- Closed to Date: $1.4M (44% of quota)
- Remaining to Close: $1.8M

CURRENT PIPELINE:

| Deal | Account | Stage | Amount | Days in Stage | Close Date | Rep | Last Activity |
|------|---------|-------|--------|---------------|------------|-----|---------------|
| D001 | Acme Corp | Negotiation | $280K | 12 | Dec 15 | Sarah | Nov 12 - Contract sent |
| D002 | TechStart | Proposal | $150K | 22 | Dec 1 | Mike | Oct 25 - Awaiting legal |
| D003 | GlobalCo | Discovery | $420K | 8 | Dec 30 | Sarah | Nov 14 - Demo scheduled |
| D004 | MidMarket | Negotiation | $95K | 5 | Nov 30 | James | Nov 14 - Pricing discussion |
| D005 | Enterprise1 | Verbal | $350K | 3 | Nov 22 | Sarah | Nov 13 - PO expected |
| D006 | StartupXYZ | Proposal | $45K | 35 | Nov 30 | Mike | Oct 10 - No response |
| D007 | RetailMax | Discovery | $180K | 18 | Dec 20 | James | Nov 5 - Champion changed |
| D008 | FinServ | Qualification | $520K | 6 | Dec 30 | Sarah | Nov 12 - Meeting set |
| D009 | HealthTech | Proposal | $125K | 14 | Dec 10 | Mike | Nov 8 - Budget confirmed |
| D010 | Manufacturing | Verbal | $180K | 8 | Dec 5 | James | Nov 10 - Awaiting signature |

PIPELINE SUMMARY:
- Total Pipeline: $2.345M
- Weighted Pipeline: $1.42M (using standard stage weights)
- Pipeline Coverage: 1.3x remaining target

HISTORICAL BENCHMARKS:
| Stage | Avg Days | Win Rate from Stage |
|-------|----------|---------------------|
| Qualification | 15 | 18% |
| Discovery | 20 | 32% |
| Proposal | 14 | 55% |
| Negotiation | 10 | 75% |
| Verbal | 5 | 92% |

Average Sales Cycle: 45 days

KNOWN CONTEXT:
- Sarah is top performer, historically beats forecast
- Mike struggling this quarter, deals slipping
- James new (60 days), still ramping
- Enterprise1 deal has executive sponsor
- GlobalCo has been in pipeline for 2 quarters
- StartupXYZ went dark after initial enthusiasm

REP QUOTA STATUS:
| Rep | Q4 Quota | Closed | Pipeline | Gap |
|-----|----------|--------|----------|-----|
| Sarah | $1.2M | $680K | $1.05M | -$520K |
| Mike | $1.0M | $380K | $320K | -$620K |
| James | $1.0M | $340K | $455K | -$660K |

AUDIENCE: Sales leadership weekly pipeline review
```

---

## Step-by-Step Implementation

### Step 1: Export Pipeline Data
**Time: 5-10 minutes**

From your CRM, export:
- All open opportunities
- Stage, amount, close date
- Days in current stage
- Last activity date
- Owner information

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Pipeline Analysis Prompt
**Time: 5-8 minutes for Claude to process**

---

**PRIMARY PROMPT: Pipeline Analysis and Commentary**

```
Please analyze this sales pipeline and provide strategic commentary.

PERIOD: [Period]
CURRENT DATE: [Date]
DAYS REMAINING: [Number]

TARGETS:
- Quota: [Amount]
- Closed to Date: [Amount]
- Remaining: [Amount]

PIPELINE DATA:
[Paste your pipeline export]

HISTORICAL CONVERSION RATES:
[Paste stage conversion data]

KNOWN CONTEXT:
[Any relevant deal or rep information]

ANALYSIS REQUIREMENTS:

1. EXECUTIVE SUMMARY
   - Forecast outlook: Will we hit the number?
   - Key risks to the forecast
   - Biggest opportunities
   - Recommended focus areas
   - Confidence level: High/Medium/Low

2. PIPELINE HEALTH ASSESSMENT

   Overall Metrics:
   | Metric | Current | Benchmark | Status |
   |--------|---------|-----------|--------|
   | Coverage Ratio | X | 3x | ⚠️ |
   | Weighted Pipeline | $X | $X needed | |
   | Avg Days in Stage | X | X | |
   | Deals at Risk | X | | |

   Health Indicators:
   - ✅ Healthy: [What's working]
   - ⚠️ Caution: [Areas of concern]
   - 🔴 Critical: [Urgent issues]

3. DEAL-LEVEL ANALYSIS

   For each significant deal:

   **[Deal Name] — $[Amount] — [Stage]**

   Risk Score: [Low/Medium/High]
   Probability Assessment: [%] (explain vs. stage default)

   Positive Indicators:
   - [Factor 1]

   Risk Factors:
   - [Factor 1]

   Velocity Check:
   - Days in stage: [X] vs benchmark [X]
   - Last activity: [Date] — [Assessment]

   Forecast Recommendation:
   [Include at X% / Move to commit / Exclude]

   Action Needed:
   - [Specific action]

4. STALLED DEAL ALERT
   Deals showing warning signs:

   | Deal | Red Flag | Days Stalled | Risk | Action |
   |------|----------|--------------|------|--------|
   [Deals with concerning patterns]

5. STAGE ANALYSIS

   | Stage | Deals | Value | Avg Days | vs Benchmark | Conversion Needed |
   |-------|-------|-------|----------|--------------|-------------------|
   [By stage analysis]

   Stage-specific observations:
   - [Stage]: [What's notable]

6. REP-LEVEL VIEW

   **[Rep Name]**
   Quota: $X | Closed: $X | Gap: $X | Pipeline: $X
   Coverage: Xx | Deals: X

   Assessment: [On track / At risk / Behind]
   Top Opportunity: [Deal]
   Key Risk: [Issue]
   Recommendation: [Action]

7. VELOCITY ANALYSIS
   Time-based patterns:

   | Deals closing this month | Value | Probability |
   | Deals closing next month | Value | Probability |
   | Deals closing in 46+ days | Value | Probability |

   Velocity concerns:
   - [Pattern 1]

8. FORECAST SCENARIOS

   | Scenario | Assumption | Q4 Result | vs Quota |
   |----------|------------|-----------|----------|
   | Best Case | All deals close as dated | $X | X% |
   | Likely | Adjusted probabilities | $X | X% |
   | Worst Case | Only commits close | $X | X% |

   Recommended Forecast: $[Amount] ([X]% of quota)

9. ACTION PRIORITIES

   This Week:
   1. [Action] — [Deal] — [Why urgent]
   2. [Action] — [Deal] — [Why urgent]

   This Month:
   1. [Action] — [Impact]

   Pipeline Generation:
   - Gap to fill: $[Amount]
   - Focus: [Where to source]

10. WATCH LIST
    Deals to monitor closely:
    - [Deal] — [Why watching]

Generate clear, actionable commentary. Be direct about risks.
```

---

### Step 4: Validate Deal Assessments
**Time: 10-15 minutes**

Review deal-level analysis:
- Are risk assessments accurate?
- Any context missing?
- Do probability adjustments make sense?
- Are stalled deals correctly identified?

---

### Step 5: Add Deal Intelligence
**Time: 5-10 minutes**

```
Update the pipeline analysis with this deal intelligence:

[Deal Name]:
- Insider information: [What you know]
- Competitive situation: [Status]
- Relationship strength: [Assessment]
- True close probability: [Your estimate]

[Other deals as needed]

Also adjust:
- [Any rep assessments]
- [Any timeline updates]
```

---

### Step 6: Generate Final Deliverables
**Time: 5 minutes**

```
Create final pipeline review package:

1. PIPELINE SCORECARD (one page)
   - Quota attainment projection
   - Pipeline health metrics
   - Top 5 deals to watch
   - This week's priorities

2. DEAL REVIEW AGENDA
   Structure for pipeline meeting:
   - Commits review (X minutes)
   - At-risk deals (X minutes)
   - Stalled deals (X minutes)
   - Pipeline generation (X minutes)

3. REP ONE-ON-ONE PREP
   For each rep:
   - Key deals to discuss
   - Questions to ask
   - Coaching points

4. FORECAST SUBMISSION
   Recommended numbers with rationale
```

---

## Example Output

Below is an abbreviated pipeline analysis example:

---

> **PIPELINE ANALYSIS**
>
> **Q4 2024 | Week of November 15 | 46 Days Remaining**
>
> ---
>
> ## Executive Summary
>
> **Forecast Outlook: At Risk — Likely to Miss by 10-15%**
>
> Current trajectory points to $2.7-2.9M against a $3.2M quota (84-91%). The math is challenging: we need $1.8M from a $2.35M pipeline with 1.3x coverage—below the 3x rule of thumb for this stage of quarter.
>
> **Key Risks:**
> - Two deals totaling $195K have stalled (StartupXYZ, RetailMax)
> - Mike's pipeline is insufficient to cover his gap
> - Only 46 days left with $520K in early-stage deals
>
> **Biggest Opportunities:**
> - Enterprise1 verbal ($350K) — Close this week for momentum
> - Acme Corp ($280K) — Contract out, push for signature
> - GlobalCo ($420K) — Large deal, demo scheduled
>
> **Recommended Focus:** Close verbals immediately, de-risk negotiations, qualify out stalled deals.
>
> **Confidence Level:** Medium-Low
>
> ---
>
> ## Pipeline Health Assessment
>
> | Metric | Current | Benchmark | Status |
> |--------|---------|-----------|--------|
> | Coverage Ratio | 1.3x | 3x | 🔴 Critical |
> | Weighted Pipeline | $1.42M | $1.8M needed | ⚠️ Short |
> | Avg Days in Current Stage | 13 | 10 | ⚠️ Slow |
> | Deals Past Due Date | 1 | 0 | ⚠️ |
>
> **Health Indicators:**
> - ✅ **Healthy:** $530K in late-stage (Verbal/Negotiation), Sarah's pipeline is solid
> - ⚠️ **Caution:** Insufficient early-stage to backfill if deals slip
> - 🔴 **Critical:** Mike's coverage at 0.52x—cannot make quota from current pipeline
>
> ---
>
> ## Deal-Level Analysis
>
> ### Enterprise1 — $350K — Verbal
>
> **Risk Score:** Low
> **Probability Assessment:** 90% (vs 92% stage default)
>
> **Positive Indicators:**
> - Executive sponsor secured
> - PO expected Nov 22
> - Only 3 days at verbal stage (healthy)
> - Top performer owns deal
>
> **Risk Factors:**
> - Large deal may require additional approvals
>
> **Velocity Check:**
> - Days in stage: 3 vs benchmark 5 ✅
> - Last activity: Nov 13 ✅
>
> **Forecast Recommendation:** Include at 90% ($315K). Strong commit candidate.
>
> **Action Needed:**
> - Daily check-in until PO received
> - Prepare for procurement questions
>
> ---
>
> ### Acme Corp — $280K — Negotiation
>
> **Risk Score:** Low-Medium
> **Probability Assessment:** 70% (vs 75% stage default)
>
> **Positive Indicators:**
> - Contract sent Nov 12
> - Sarah (top performer) owns deal
> - Dec 15 close date has buffer
>
> **Risk Factors:**
> - 12 days in negotiation (slightly above benchmark)
> - No response since contract sent
>
> **Velocity Check:**
> - Days in stage: 12 vs benchmark 10 ⚠️
> - Last activity: Nov 12 — Contract sent, awaiting response
>
> **Forecast Recommendation:** Include at 70% ($196K). Solid but monitor.
>
> **Action Needed:**
> - Follow up today on contract status
> - Identify any legal concerns
>
> ---
>
> ### StartupXYZ — $45K — Proposal
>
> **Risk Score:** High
> **Probability Assessment:** 15% (vs 55% stage default)
>
> **Positive Indicators:**
> - None currently
>
> **Risk Factors:**
> - 35 days in stage (2.5x benchmark!)
> - Last activity Oct 10 — over 5 weeks ago
> - "Went dark after initial enthusiasm"
> - Close date Nov 30 is 15 days away with no engagement
>
> **Velocity Check:**
> - Days in stage: 35 vs benchmark 14 🔴
> - Last activity: Oct 10 🔴 — Deal is dead
>
> **Forecast Recommendation:** Exclude from forecast. Qualify out or mark lost.
>
> **Action Needed:**
> - Break-up email or final attempt this week
> - If no response by Friday, close lost
>
> ---
>
> ### GlobalCo — $420K — Discovery
>
> **Risk Score:** Medium
> **Probability Assessment:** 25% (vs 32% stage default)
>
> **Positive Indicators:**
> - Demo scheduled
> - Large deal size
> - Recent activity (Nov 14)
>
> **Risk Factors:**
> - "In pipeline for 2 quarters" — history of slipping
> - Discovery stage with Dec 30 close — aggressive timeline
> - Only 46 days to move through proposal and negotiation
>
> **Velocity Check:**
> - Days in stage: 8 vs benchmark 20 ✅ (this stage)
> - BUT: Overall deal age is concerning
>
> **Forecast Recommendation:** Include at 25% ($105K). Upside but not in commit.
>
> **Action Needed:**
> - Nail the demo, create urgency
> - Understand why it's slipped before
> - Get clear decision timeline
>
> ---
>
> ## Stalled Deal Alert
>
> | Deal | Red Flag | Days Stalled | Risk | Action |
> |------|----------|--------------|------|--------|
> | StartupXYZ | No contact 35+ days | 35 | 🔴 Dead | Qualify out |
> | RetailMax | Champion changed | 10 | 🔴 High | Re-engage new champion |
> | TechStart | "Awaiting legal" 22 days | 22 | ⚠️ Medium | Escalate to executive |
>
> **Total at-risk value:** $375K (16% of pipeline)
>
> ---
>
> ## Rep-Level View
>
> ### Sarah Chen
>
> **Quota:** $1.2M | **Closed:** $680K | **Gap:** $520K | **Pipeline:** $1.05M
> **Coverage:** 2.0x | **Deals:** 3
>
> **Assessment:** On Track ✅
>
> Sarah has the strongest position. Enterprise1 verbal should close this month, Acme Corp negotiation is solid, and GlobalCo is her upside. If GlobalCo moves, she beats quota.
>
> **Top Opportunity:** Enterprise1 ($350K) — Close this week
> **Key Risk:** GlobalCo has slipped before — don't count on it
> **Recommendation:** Close Enterprise1, pressure Acme, qualify GlobalCo properly
>
> ---
>
> ### Mike Roberts
>
> **Quota:** $1.0M | **Closed:** $380K | **Gap:** $620K | **Pipeline:** $320K
> **Coverage:** 0.52x | **Deals:** 3
>
> **Assessment:** Behind 🔴
>
> Mike cannot make quota from current pipeline. Even at 100% close rate, he's $300K short. Two of his three deals show warning signs (TechStart legal delay, StartupXYZ dark).
>
> **Top Opportunity:** HealthTech ($125K) — Only healthy deal
> **Key Risk:** Insufficient pipeline, struggling deals
> **Recommendation:** Focus entirely on HealthTech close, source Q1 pipeline, accept Q4 miss
>
> ---
>
> ### James Wilson
>
> **Quota:** $1.0M | **Closed:** $340K | **Gap:** $660K | **Pipeline:** $455K
> **Coverage:** 0.69x | **Deals:** 3
>
> **Assessment:** At Risk ⚠️
>
> James is ramping (60 days) so some gap is expected. MidMarket and Manufacturing are both progressing well. RetailMax champion change is concerning.
>
> **Top Opportunity:** Manufacturing ($180K) — Awaiting signature
> **Key Risk:** RetailMax champion change could kill the deal
> **Recommendation:** Close Manufacturing ASAP, engage new RetailMax champion immediately
>
> ---
>
> ## Forecast Scenarios
>
> | Scenario | Assumption | Q4 Result | vs Quota |
> |----------|------------|-----------|----------|
> | Best Case | All deals close as dated | $3.74M | 117% |
> | Likely Case | Risk-adjusted probabilities | $2.82M | 88% |
> | Worst Case | Only commits (verbal + negotiation at 60%) | $2.38M | 74% |
>
> **Recommended Forecast: $2.75-2.85M (86-89% of quota)**
>
> Rationale: Verbal deals should close (high confidence), negotiations at 65-70%, proposals at 40%, discovery unlikely to contribute this quarter.
>
> ---
>
> ## Action Priorities
>
> **This Week:**
> 1. **Close Enterprise1 verbal** — $350K — PO expected, follow daily
> 2. **Acme Corp contract follow-up** — $280K — 3 days since sent, need response
> 3. **StartupXYZ decision** — $45K — Qualify out if no response
> 4. **RetailMax champion meeting** — $180K — New champion relationship critical
>
> **This Month:**
> 1. Accelerate TechStart legal resolution — Escalate if needed
> 2. Push GlobalCo through demo to proposal — Test if this deal is real
> 3. Manufacturing signature — James's most closeable deal
>
> **Pipeline Generation:**
> - Gap to fill: $500K+ for Q1 head start
> - Focus: Mike needs to build pipe, James needs coaching support
> - Source: Customer expansion, partner referrals
>
> ---
>
> ## Watch List
>
> Deals requiring close monitoring:
>
> - **TechStart ($150K):** Legal delay extending. Check daily.
> - **GlobalCo ($420K):** History of slipping. Verify commitment post-demo.
> - **HealthTech ($125K):** Mike's only healthy deal. Can't afford to lose.

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| All deals show same probability | Using stage defaults | Add: "Adjust probability based on deal-specific factors like velocity, engagement, and competitive situation" |
| Missing rep context | Insufficient input | Add: "Here's what I know about each rep: [Performance patterns]" |
| Overly optimistic forecast | Sales bias in data | Ask: "Apply skepticism to close dates. If a deal has slipped before, assume it will slip again" |
| No actionable output | Generic analysis | Ask: "For each deal, specify the one action that would most increase close probability this week" |
| Can't identify stalled deals | No velocity benchmarks | Add: "Benchmark days in stage: [Your data]. Flag anything 1.5x above benchmark" |

---

## Tips from Experience

1. **Coverage ratios lie.** A $6M pipeline doesn't mean you'll close $2M. Quality and velocity matter more than quantity.

2. **Trust patterns, not promises.** If a deal has slipped three times, it will slip again. Adjust probability accordingly.

3. **Watch activity, not stage.** A "negotiation" deal with no contact in 3 weeks isn't really in negotiation.

4. **Different reps need different discounts.** Apply history-based adjustments. New reps overcall, struggling reps undercall.

5. **Early-stage deals don't save quarters.** In the last 45 days, focus on late-stage only.

6. **The commit is what counts.** Build your review around commits, not total pipeline.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Forecast accuracy improves
- [ ] Stalled deals are identified earlier
- [ ] Pipeline review time decreases
- [ ] Actions from reviews are completed
- [ ] Fewer end-of-quarter surprises
- [ ] Win rates improve from better focus

**Track over time:**
- Forecast accuracy (predicted vs. actual)
- Deal velocity trends
- Stalled deal conversion rates
- Time to complete pipeline review
- Actions completed from recommendations

---

## Variations

### Territory Pipeline Review
For geographic or segment views:
```
Analyze pipeline by territory/segment:
- Coverage by territory
- Velocity comparison across territories
- Best practices from top territory
- Resource allocation recommendations
- Territory-specific risks and opportunities

Format: Comparative view with territory rankings
```

### Product Line Pipeline
For product-specific analysis:
```
Analyze pipeline by product line:
- Mix of products in pipeline
- Cross-sell/upsell opportunities
- Product-specific win rates
- Competitive positioning by product
- Pricing trends by product

Include: Product penetration recommendations
```

### New Business vs Expansion
For acquisition vs growth analysis:
```
Separate analysis for:
- New logo pipeline (health, velocity, sources)
- Expansion pipeline (account health, timing)
- Different benchmarks for each
- Resource allocation between

Include: Logo vs dollar trade-off analysis
```

### Board-Level Pipeline Summary
For executive/board presentation:
```
Create board-ready pipeline summary:
- High-level forecast with confidence range
- Major deal highlights
- Risk summary (no deal-level detail)
- Market trends observed
- Resource needs

Format: One page with supporting appendix
```

---

## Building Your Repeatable System

After several pipeline reviews, optimize:

1. **Standard data export** from CRM
2. **Consistent benchmarks** for velocity and conversion
3. **Rep-specific probability adjustments** based on history
4. **Deal score tracking** over time
5. **Action accountability** from each review

**Sample Setup:**
```
pipeline-analysis/
├── weekly/
│   ├── 2024-11-15-pipeline.md
│   ├── 2024-11-08-pipeline.md
│   └── [week by week]
├── data/
│   ├── raw-exports/
│   │   └── [CRM exports]
│   └── benchmarks/
│       ├── stage-conversion.md
│       └── rep-accuracy.md
├── forecasts/
│   ├── q4-forecast-log.md
│   └── accuracy-tracking.md
├── actions/
│   └── weekly-action-tracker.md
└── templates/
    ├── pipeline-review.md
    └── deal-analysis.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**assess health → identify risks → prioritize action → forecast outcome**—applies broadly:

| Role | Application |
|------|-------------|
| **Sales** | Deal review, territory planning |
| **Customer Success** | Renewal pipeline, expansion opportunities |
| **Recruiting** | Candidate pipeline analysis |
| **Partnerships** | Partner deal flow |
| **Project Management** | Project portfolio health |
| **Product** | Feature delivery pipeline |

---

## Next Steps

1. **Export your pipeline:** Get current data from CRM
2. **Gather benchmarks:** Historical conversion rates by stage
3. **Note context:** What you know about key deals
4. **Run analysis:** Use this recipe
5. **Validate assessments:** Check deal-level conclusions
6. **Take action:** Focus on highest-impact moves

---

*Recipe #55 of 100 in the Claude Code Knowledge Worker Recipe Collection*
