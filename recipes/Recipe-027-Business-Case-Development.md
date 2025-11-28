# Business Case Development

**Recipe #27: From Good Idea to Funded Initiative**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 15 minutes (first time) / 10 minutes (repeat) | 4-8 hours per business case | Intermediate | All Professionals Proposing Initiatives |

---

## The Problem

You have an idea, initiative, or investment you want to pursue, but getting it approved requires a compelling business case. The CFO wants ROI, the CEO wants strategic alignment, operations wants feasibility, and everyone wants to know the risks. Building a comprehensive case that addresses all perspectives takes hours—and even then, you're not sure you've covered everything.

**Pain Points:**
- Unclear what to include in a business case
- Difficulty quantifying benefits
- Missing stakeholder concerns
- Weak financial analysis
- Generic templates that don't fit your situation
- Getting rejected for gaps you didn't anticipate

---

## The Outcome

A comprehensive, compelling business case that addresses strategic fit, financial return, operational feasibility, and risk. A document structured to answer the questions decision-makers will ask, with analysis that supports informed approval decisions. Your proposals get approved because they're thorough.

**What You'll Have When Done:**
- Executive summary with clear ask
- Strategic rationale and alignment
- Financial analysis (costs, benefits, ROI)
- Implementation approach
- Risk assessment
- Success metrics and governance
- Presentation-ready materials

---

## When to Use This Recipe

**Good Fit:**
- New initiatives requiring budget approval
- Capital investment requests
- Headcount requests
- Technology purchases
- Process improvement proposals
- Strategic projects seeking funding

**Not a Good Fit:**
- Routine budget items within existing authority
- Very small expenses (overkill)
- Already-approved initiatives
- Emergency situations requiring immediate action

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You understand what you're proposing
- [ ] You know the approval process and decision-makers
- [ ] You have cost estimates (at least rough)
- [ ] You can articulate benefits (quantified or qualitative)
- [ ] You have 2-3 hours for comprehensive case development

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Structures comprehensive business cases
- Generates financial models (NPV, ROI, payback)
- Identifies risks and mitigations
- Creates compelling narratives
- Ensures logical flow and completeness
- Produces presentation-ready materials

**Where Human Judgment Is Essential:**
- Validating cost and benefit estimates
- Understanding organizational politics
- Knowing decision-maker priorities
- Strategic context and alternatives
- Commitment to implementation
- Final recommendation

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Initiative description | What you want to do | Core proposal |
| Cost estimates | Investment required | Financial analysis |
| Benefit estimates | Value created | ROI calculation |
| Strategic context | Company priorities | Alignment narrative |
| Alternatives | Other options considered | Comparison analysis |
| Risks | What could go wrong | Risk section |

**Sample Input:**
```
Business Case: Marketing Automation Platform

PROPOSAL:
Implement a marketing automation platform to replace manual email campaigns and lead management processes.

COSTS:
- Software license: $85K/year (3-year commitment)
- Implementation: $60K one-time
- Training: $15K one-time
- Internal effort: 2 FTEs for 3 months = $80K
- Annual maintenance/admin: $25K ongoing

Total Year 1: $265K
Annual ongoing: $110K

EXPECTED BENEFITS:
- Marketing team efficiency: Currently 5 FTEs spending 60% time on manual tasks. Expect to reduce to 30%, saving 1.5 FTE equivalent (~$120K/year)
- Improved lead conversion: 15% improvement in lead-to-opportunity conversion (worth ~$400K in pipeline annually based on current volumes)
- Reduced email vendor costs: Consolidating 3 tools = $40K/year savings
- Better attribution: Hard to quantify, but significant value

STRATEGIC CONTEXT:
- Company is prioritizing sales efficiency
- Marketing ops is a known bottleneck
- Competitors have already automated
- CEO mentioned this in all-hands last quarter

ALTERNATIVES CONSIDERED:
1. Do nothing (status quo)
2. Hire more marketing operations staff
3. Build custom solution in-house

RISKS:
- Implementation could take longer than planned
- Adoption may be slow
- Integration with Salesforce may be complex

APPROVAL NEEDED FROM:
- CFO (budget authority)
- CMO (sponsor)
- CTO (technical approval)
```

---

## Step-by-Step Implementation

### Step 1: Organize Your Inputs
**Time: 15-20 minutes**

Gather and organize:
- What you're proposing (clear description)
- Cost estimates (as detailed as possible)
- Benefit estimates (quantified where possible)
- Strategic context (how it aligns)
- Alternatives (what else you considered)
- Risks (what could go wrong)

Better inputs = stronger business case.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Business Case Prompt
**Time: 5-7 minutes for Claude to process**

---

**PRIMARY PROMPT: Business Case Development**

```
Please help me develop a comprehensive business case for this initiative.

INITIATIVE OVERVIEW:
- Name: [Initiative name]
- Description: [What you're proposing]
- Sponsor: [Who's championing this]
- Approval needed from: [Decision-makers]

COST ESTIMATES:
"""
[PASTE YOUR COST BREAKDOWN]
"""

BENEFIT ESTIMATES:
"""
[PASTE YOUR BENEFIT ESTIMATES]
"""

STRATEGIC CONTEXT:
- Company priorities: [Current strategic focus areas]
- How this aligns: [Why this matters now]
- Competitive context: [What competitors are doing]

ALTERNATIVES CONSIDERED:
1. [Alternative 1]
2. [Alternative 2]
3. [Alternative 3]

KNOWN RISKS:
- [Risk 1]
- [Risk 2]
- [Risk 3]

PLEASE DEVELOP A BUSINESS CASE WITH:

1. EXECUTIVE SUMMARY (1 page)
   - The ask (what and how much)
   - Strategic rationale (why this, why now)
   - Financial summary (key numbers)
   - Recommendation

2. STRATEGIC RATIONALE
   - Problem statement (what's broken or missing)
   - Opportunity description (what's possible)
   - Strategic alignment (connection to company priorities)
   - Competitive context (market dynamics)
   - Why now (urgency and timing)

3. PROPOSED SOLUTION
   - Solution description
   - Scope (what's included, what's not)
   - Key features/capabilities
   - Success criteria
   - Why this solution vs. alternatives

4. ALTERNATIVES ANALYSIS
   | Criteria | Proposed | Alt 1 | Alt 2 | Alt 3 |

   For each alternative:
   - Description
   - Pros and cons
   - Why not selected (or why selected)

5. FINANCIAL ANALYSIS
   - Cost summary table
     | Category | Year 1 | Year 2 | Year 3 | Total |
   - Benefit summary table
     | Category | Year 1 | Year 2 | Year 3 | Total |
   - Financial metrics:
     * Net Present Value (NPV) at 10% discount rate
     * Return on Investment (ROI)
     * Payback period
     * Internal Rate of Return (IRR)
   - Sensitivity analysis (what if benefits are 20% lower?)
   - Assumptions and dependencies

6. IMPLEMENTATION APPROACH
   - High-level timeline
   - Key phases and milestones
   - Resource requirements
   - Dependencies
   - Go-live approach

7. RISK ASSESSMENT
   | Risk | Likelihood | Impact | Mitigation |

   For top risks:
   - What could go wrong
   - How likely
   - Impact if occurs
   - How we'll mitigate

8. ORGANIZATIONAL IMPACT
   - Teams affected
   - Change management needs
   - Training requirements
   - Process changes

9. SUCCESS METRICS
   - How we'll measure success
   - Key milestones and checkpoints
   - When we'll know it's working
   - Review cadence

10. GOVERNANCE AND OVERSIGHT
    - Project ownership
    - Decision-making authority
    - Review and approval gates
    - Escalation path

11. RECOMMENDATION
    - Clear recommendation (approve/modify/defer)
    - Conditions for approval
    - Immediate next steps
    - Key decisions needed

Format as a professional business case document suitable for executive review.
```

---

### Step 4: Review and Strengthen
**Time: 20-30 minutes**

Review the business case:

**Check the math:**
- Are calculations correct?
- Do NPV/ROI calculations make sense?
- Are assumptions reasonable?

**Check the logic:**
- Does strategic rationale hold?
- Is alternatives analysis fair?
- Are risks properly weighted?

**Check completeness:**
- Any obvious gaps?
- Questions decision-makers will ask?
- Missing stakeholder concerns?

---

### Step 5: Refine and Customize
**Time: 15-20 minutes**

**To strengthen the financial case:**
```
The CFO will push back on the benefit estimates. Make the financial analysis more conservative and add a break-even scenario showing minimum benefits needed for approval.
```

**To address skepticism:**
```
The CTO is skeptical about implementation timeline. Strengthen the implementation section with more detail on risks, dependencies, and realistic timeline scenarios.
```

**To add comparables:**
```
Add a section on comparable implementations—what have similar companies achieved with this type of investment? Include benchmarks and case studies.
```

**To strengthen alternatives analysis:**
```
The "build vs. buy" question will come up. Go deeper on the build-in-house alternative, including hidden costs and timeline, to clearly show why buying is better.
```

---

### Step 6: Create Final Deliverables
**Time: 10 minutes**

```
Create these final outputs:

1. FULL BUSINESS CASE (10-15 pages)
   - Complete analysis
   - All appendices and supporting data

2. EXECUTIVE SUMMARY (1 page)
   - One-page standalone summary
   - Key ask and rationale
   - Essential numbers

3. APPROVAL PRESENTATION (8-10 slides)
   - Visual format for decision meeting
   - Clear storyline
   - Financial summary
   - Discussion questions

4. APPROVAL REQUEST MEMO (1-2 pages)
   - Formal approval request format
   - Clear ask and conditions
   - Signature lines if needed

5. FAQ DOCUMENT
   - Anticipated questions
   - Prepared responses
```

---

## Example Output

Below is an abbreviated business case example:

---

> **BUSINESS CASE: Marketing Automation Platform**
> **Date: November 2024 | Requested Approval: Q1 2025 Start**
>
> ---
>
> **EXECUTIVE SUMMARY**
>
> **The Ask:** $265,000 Year 1 investment ($110K annually thereafter) to implement a marketing automation platform, replacing manual email campaigns and fragmented lead management processes.
>
> **Strategic Rationale:** Marketing operations is a documented bottleneck limiting our ability to scale demand generation. Competitors have automated their marketing operations, and our manual processes consume 60% of marketing team capacity. This initiative directly supports the CEO's stated priority of improving sales efficiency.
>
> **Financial Summary:**
> - 3-Year NPV: $487,000 (at 10% discount)
> - ROI: 184%
> - Payback: 8 months
> - Annual benefit: $560K/year (steady state)
>
> **Recommendation:** Approve with Q1 2025 start date. Delay increases competitive disadvantage and continues operational inefficiency.
>
> ---
>
> **STRATEGIC RATIONALE**
>
> **Problem Statement:**
> Marketing operations is constrained by manual processes that limit scale, quality, and speed. Current state:
> - 5 FTEs spend 60% of time on manual email and lead tasks
> - Lead response time averages 48 hours vs. industry best practice of 5 minutes
> - 3 separate email tools with no unified view
> - Manual lead scoring missing 40% of qualified leads
> - No automated nurture campaigns for the 80% of leads not sales-ready
>
> **Opportunity:**
> Marketing automation enables:
> - 15% improvement in lead-to-opportunity conversion
> - Reduction of manual work from 60% to 30% of team time
> - Real-time lead routing and instant response
> - Scalable nurture programs recapturing dormant leads
>
> **Strategic Alignment:**
>
> | Company Priority | How This Supports |
> |-----------------|-------------------|
> | Sales efficiency | Higher quality leads, faster handoff |
> | Operational excellence | Automation of manual processes |
> | Data-driven decisions | Attribution and analytics |
> | Customer experience | Personalized, timely communications |
>
> ---
>
> **FINANCIAL ANALYSIS**
>
> **Cost Summary**
>
> | Category | Year 1 | Year 2 | Year 3 | Total |
> |----------|--------|--------|--------|-------|
> | Software | $85K | $85K | $85K | $255K |
> | Implementation | $60K | - | - | $60K |
> | Training | $15K | $5K | $5K | $25K |
> | Internal effort | $80K | - | - | $80K |
> | Admin/maintenance | $25K | $25K | $25K | $75K |
> | **Total** | **$265K** | **$115K** | **$115K** | **$495K** |
>
> **Benefit Summary**
>
> | Category | Year 1 | Year 2 | Year 3 | Total |
> |----------|--------|--------|--------|-------|
> | Labor efficiency (1.5 FTE) | $60K* | $120K | $120K | $300K |
> | Improved conversion (15%) | $200K* | $400K | $400K | $1,000K |
> | Tool consolidation | $40K | $40K | $40K | $120K |
> | **Total** | **$300K** | **$560K** | **$560K** | **$1,420K** |
>
> *Year 1 benefits prorated for 6-month implementation
>
> **Key Financial Metrics**
>
> | Metric | Value | Assessment |
> |--------|-------|------------|
> | Net Present Value (10%) | $487,000 | ✅ Strong positive |
> | Return on Investment | 184% | ✅ Exceeds 50% threshold |
> | Payback Period | 8 months | ✅ Under 18-month target |
> | Internal Rate of Return | 89% | ✅ Well above cost of capital |
>
> **Sensitivity Analysis**
>
> | Scenario | NPV | ROI | Payback |
> |----------|-----|-----|---------|
> | Base case | $487K | 184% | 8 mo |
> | Benefits 20% lower | $312K | 127% | 11 mo |
> | Benefits 40% lower | $137K | 70% | 15 mo |
> | Benefits 50% lower | $50K | 42% | 18 mo |
>
> **Break-even:** Benefits must be at least 55% of projections to achieve positive NPV.
>
> ---
>
> **ALTERNATIVES ANALYSIS**
>
> | Criteria | Proposed Platform | Status Quo | Hire Staff | Build Custom |
> |----------|-------------------|------------|------------|--------------|
> | 3-Year Cost | $495K | $0 | $900K | $800K |
> | 3-Year Benefit | $1,420K | $0 | $400K | $1,200K |
> | Time to value | 6 months | N/A | 3 months | 18+ months |
> | Risk | Medium | Low | Low | High |
> | Scalability | High | None | Low | Medium |
> | **Recommendation** | ✅ **Best option** | ❌ | ❌ | ❌ |
>
> **Why Alternatives Were Not Selected:**
>
> **Status Quo:** Unacceptable. We lose competitive ground daily. Marketing capacity remains constrained. Sales efficiency goal is not achievable without change.
>
> **Hire Staff:** More expensive than automation, doesn't solve process issues, adds management overhead, and doesn't scale.
>
> **Build Custom:** 18+ month timeline, significant technical risk, ongoing maintenance burden, diverts engineering from product work.
>
> ---
>
> **RISK ASSESSMENT**
>
> | Risk | L | I | Score | Mitigation |
> |------|---|---|-------|------------|
> | Implementation delays | 3 | 3 | 9 | Phased approach, vendor SLAs |
> | User adoption resistance | 3 | 4 | 12 | Change management plan, training |
> | Salesforce integration issues | 2 | 4 | 8 | Pre-implementation technical review |
> | Benefits not realized | 2 | 5 | 10 | Clear metrics, quarterly reviews |
> | Vendor issues | 2 | 3 | 6 | Established vendor, SLAs, escrow |
>
> **Top Risk: User Adoption**
> - Mitigation: Dedicated change management lead, training program, executive communication, power user champions
> - Contingency: Extended training period, additional support resources
> - Success metric: >80% active usage by Month 4
>
> ---
>
> **IMPLEMENTATION TIMELINE**
>
> ```
> Q1 2025: Planning & Setup
> - Week 1-2: Kickoff, requirements finalization
> - Week 3-6: Technical setup, Salesforce integration
> - Week 7-10: Configuration, initial campaigns
> - Week 11-12: User training, pilot
>
> Q2 2025: Rollout & Optimization
> - Month 4: Full rollout to marketing team
> - Month 5-6: Optimization, additional automation
>
> Q3 2025: Expansion
> - Advanced features and integrations
> - Extended team training
> ```
>
> ---
>
> **RECOMMENDATION**
>
> **Approve this initiative** with Q1 2025 start date.
>
> **Conditions:**
> 1. CMO confirmed as executive sponsor
> 2. Technical review with CTO team within 2 weeks
> 3. Change management lead identified
>
> **Next Steps if Approved:**
> 1. Finalize vendor contract (December)
> 2. Resource allocation confirmed
> 3. Kickoff meeting scheduled for January 2

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Benefits seem inflated | Overly optimistic estimates | Add: "Create a conservative scenario with reduced benefit assumptions" |
| Costs seem incomplete | Missing hidden costs | Ask: "What costs might we be missing? Training, maintenance, internal time?" |
| Strategic rationale weak | Not connected to priorities | Add: "Connect more explicitly to [company priority]—how does this directly enable it?" |
| Alternatives not fair | Straw man comparisons | Ask: "Steel-man each alternative—make the best case for them before comparing" |
| Risk section too light | Underestimating challenges | Ask: "What would a skeptical stakeholder say could go wrong?" |
| No urgency | Timing not compelling | Add: "What's the cost of delay? Why must this happen now?" |

---

## Tips from Experience

1. **Know your audience.** CFOs want numbers. CEOs want strategy. Tech leaders want feasibility. Tailor emphasis accordingly.

2. **Front-load the ask.** Don't bury the request at the end. Lead with what you want.

3. **Address the "do nothing" option.** The alternative is never neutral. What happens if we don't do this?

4. **Be honest about uncertainties.** Acknowledge what you don't know. Credibility matters more than certainty.

5. **Include an exit strategy.** What if it doesn't work? Knowing you've thought about this builds confidence.

6. **Quantify what you can, describe what you can't.** Don't let unquantifiable benefits disappear—describe their value qualitatively.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Business case is approved
- [ ] Decision-makers' questions were anticipated and answered
- [ ] No major gaps identified in review
- [ ] Financial analysis holds up to scrutiny
- [ ] Initiative proceeds successfully

**Track over time:**
- Approval rate for your business cases
- Time from submission to approval
- Actual vs. projected costs and benefits (post-implementation)
- Feedback from decision-makers

---

## Variations

### Quick Business Case
For smaller requests:
```
Create a brief business case (1-2 pages) for:

[Initiative description]

Include only:
1. What and why (1 paragraph)
2. Cost and benefit summary (1 table)
3. Risks and mitigations (bullet points)
4. Recommendation

Keep it simple and actionable.
```

### Investment Proposal
For capital expenditure:
```
Create a capital investment proposal for:

[Asset or investment description]

Include:
1. Investment description and purpose
2. Capital and operating cost breakdown
3. Depreciation schedule
4. Tax implications
5. Cash flow analysis
6. Financial metrics (NPV, IRR, Payback)
7. Sensitivity analysis
8. Approval recommendation
```

### Headcount Request
For hiring business case:
```
Create a business case for adding headcount:

Position(s): [Role(s) and level(s)]
Department: [Where]
Need: [Why]

Include:
1. Current state and problem
2. Role description and requirements
3. Fully-loaded cost calculation
4. Expected productivity/value
5. What happens without this hire
6. Alternatives considered
7. Recommendation
```

### Program Funding
For multi-initiative programs:
```
Create a business case for this program:

[Program description with multiple initiatives]

Include:
1. Program overview and strategic rationale
2. Component initiatives and dependencies
3. Consolidated financial analysis
4. Phasing and sequencing
5. Program-level risks
6. Governance structure
7. Success metrics
```

---

## Building Your Repeatable System

After several business cases, establish your system:

1. **Create standard templates** for different request types
2. **Build a benefits library** with quantification approaches
3. **Maintain a costs checklist** to avoid missing items
4. **Document approval criteria** for your organization
5. **Track actuals vs. projections** to improve estimates

**Sample Setup:**
```
business-cases/
├── templates/
│   ├── full-business-case-prompt.txt
│   ├── quick-business-case.txt
│   ├── headcount-request.txt
│   └── capex-proposal.txt
├── active/
│   ├── marketing-automation/
│   │   ├── business-case.md
│   │   ├── presentation.pptx
│   │   └── approval-status.md
│   └── [other cases]/
├── approved/
│   └── [approved cases with outcomes]
├── reference/
│   ├── benefits-quantification-guide.md
│   ├── cost-checklist.md
│   └── approval-criteria.md
└── actuals-tracking/
    └── projections-vs-actuals.xlsx
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**define proposal → build strategic rationale → analyze financials → assess alternatives → evaluate risks → recommend**—applies broadly:

| Role | Application |
|------|-------------|
| **All Professionals** | Initiative proposals |
| **Finance** | Investment analysis |
| **Operations** | Process improvement cases |
| **IT** | Technology investment cases |
| **HR** | Headcount and program requests |
| **Sales** | Customer investment cases |

---

## Next Steps

1. **Pick your initiative:** What do you want to get approved?
2. **Gather inputs:** Costs, benefits, context, alternatives
3. **Build the case:** Use this recipe for comprehensive development
4. **Socialize early:** Get feedback before formal submission
5. **Present and follow up:** Guide the approval process

---

*Recipe #27 of 100 in the Claude Code Knowledge Worker Recipe Collection*
