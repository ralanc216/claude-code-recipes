# Project Status and Health Reporting

**Recipe #86: From Scattered Project Data to Comprehensive Status Insights**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 15 minutes (first time) / 5 minutes (repeat) | 2-3 hours per week | Beginner | Project Managers, Program Managers, PMO |

---

## The Problem

Project status reports are a necessary but time-consuming ritual. Every week (or day), project managers gather updates from multiple sources—task boards, team meetings, risk logs, budget trackers—and synthesize them into a report that different stakeholders can actually use. The executive wants a one-page summary, the sponsor wants to know about risks, and the team wants detailed progress. Creating multiple versions takes hours that could be spent actually managing the project.

**Pain Points:**
- Manually aggregating data from task boards, risk logs, budgets, and team meetings takes hours
- Different stakeholders need different levels of detail and focus areas
- Inconsistent health assessments across reporting periods reduce credibility
- Translating technical progress into business-relevant language is time-intensive
- Risk identification and trend analysis require pattern recognition across data sources
- Late nights creating status reports instead of managing the actual project
- Missing important patterns or trends buried in the raw data

---

## The Outcome

Comprehensive yet scannable status reports that accurately reflect project health, highlight the right issues to the right audiences, and maintain consistency across reporting periods—enabling stakeholders to quickly understand where the project stands and what needs attention.

**What You'll Have When Done:**
- Executive summary capturing project status in 3-4 sentences
- Detailed status report with health indicators, accomplishments, and metrics
- Multiple audience-specific views (executive, steering committee, team, portfolio)
- Consistent health ratings with documented rationale
- Risk and issue analysis with impact assessments
- Professional, repeatable format you can use week after week

---

## When to Use This Recipe

**Good Fit:**
- Weekly project status updates
- Monthly portfolio reviews
- Steering committee presentations
- Executive dashboard updates
- Risk escalation reports
- Program-level rollups

**Not a Good Fit:**
- Real-time project tracking (use live dashboards instead)
- Detailed technical work tracking (use task management tools)
- Single-stakeholder informal updates (just send an email)
- Projects so simple they don't need formal reporting

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] Current task/milestone status
- [ ] Recent accomplishments list
- [ ] Upcoming deliverables/deadlines
- [ ] Risk and issue log
- [ ] Budget/resource status
- [ ] Team capacity information
- [ ] Blockers requiring escalation
- [ ] You have 30-45 minutes for initial report creation

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Aggregates data from multiple project sources into coherent narratives
- Calculates health indicators consistently across reporting periods
- Translates technical progress into business-appropriate language
- Identifies patterns in project trajectory and emerging risks
- Generates multiple report versions for different audiences from same data
- Maintains consistent formatting and structure across reports

**Where Human Judgment Is Essential:**
- Determining overall project health based on context and stakeholder expectations
- Deciding what to escalate and when
- Assessing political and organizational dynamics
- Making final calls on risk severity and mitigation strategies
- Validating that generated reports accurately reflect project reality
- Choosing what details to include or omit for specific audiences

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Milestone status | "Backend API 60% complete, Frontend 45%, UAT not started" | Progress tracking and completion percentages |
| Accomplishments | "Completed authentication API ahead of schedule" | Highlighting wins and momentum |
| Risks/issues | "R-001: Vendor API delayed, probability High, impact Medium" | Risk assessment and escalation decisions |
| Budget data | "Spent $187K of $450K, 42% consumed vs 38% timeline" | Variance analysis and forecasting |
| Team capacity | "2 developers at 100%, 1 at 50%, QA joining next week" | Resource constraint identification |

**Sample Input:**
```
PROJECT: Customer Portal Redesign
PHASE: Development (Phase 2 of 4)
REPORTING PERIOD: Week of Jan 15-19, 2024

MILESTONES:
- Requirements Complete: Done (Jan 5)
- Design Approved: Done (Jan 12)
- Backend API Development: In Progress (60% complete)
- Frontend Development: In Progress (45% complete)
- Integration Testing: Not Started (scheduled Feb 15)
- UAT: Not Started (scheduled Mar 1)
- Go-Live: Scheduled Mar 15

ACCOMPLISHED THIS WEEK:
- Completed user authentication API (ahead of schedule)
- Dashboard wireframes approved with minor revisions
- Security review initiated (ongoing)
- Resolved 3 critical bugs from previous sprint

NOT COMPLETED:
- Payment integration not started (blocked by vendor)

ACTIVE RISKS:
R-001: Payment vendor API documentation incomplete
- Probability: High | Impact: Medium
- Status: Mitigating - scheduled call with vendor Jan 22

ACTIVE ISSUES:
I-001: Vendor API access credentials delayed
- Severity: High
- Status: Escalated to vendor management
- Impact: Blocking payment integration work

BUDGET SUMMARY:
Total Budget: $450,000
Spent to Date: $187,500 (42%)
Phase Progress: 38% complete
Variance: -4% (slightly over plan)
```

---

## Step-by-Step Implementation

### Step 1: Prepare Your Inputs
**Time: 10 minutes**

Gather your current project data from task boards, risk logs, budget trackers, and meeting notes. You don't need perfect data—just compile what you have about status, accomplishments, risks, and metrics.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Project Status Analysis Prompt
**Time: 5-10 minutes for Claude to process**

---

**PRIMARY PROMPT: Project Status Report Generation**

```
Claude, I need to create a project status report.

Project: [Project Name]
Reporting period: [Dates]

Here's the current status:
[Paste milestone status, accomplishments, planned vs actual]

Risks and issues:
[Paste risk log and issue log]

Budget status:
[Paste budget data]

Help me create:
1. Overall health assessment (Green/Yellow/Red) with rationale
2. Executive summary (3-4 sentences)
3. Key accomplishments section
4. Planned vs actual comparison
5. Risk analysis with escalation recommendations
6. Budget variance explanation
7. Upcoming milestones with confidence levels

Format this as a comprehensive project status report that I can share with stakeholders.
```

---

### Step 4: Review and Validate
**Time: 5-10 minutes**

**Check immediately:**
- Health ratings match your understanding of project reality
- No critical risks or issues were missed
- Budget variance explanations are accurate
- Accomplishments are properly highlighted

**Spot-check specifics:**
- Milestone completion percentages align with task tracking
- Risk impact assessments match stakeholder expectations
- Executive summary captures most important points
- Tone is appropriate for your organizational culture

---

### Step 5: Refine and Iterate
**Time: 5-10 minutes**

**For audience-specific versions:**
```
Create an executive version of this status report:
- One page maximum
- Lead with most critical information
- Focus on decisions needed and blockers
- No technical jargon
```

**To adjust health assessment:**
```
The overall health should be Yellow instead of Green because [reason].
Please update the assessment and adjust the executive summary accordingly.
```

**To add context:**
```
Add a section explaining why we're 4% over budget - security consultant
engagement was necessary due to [reason], but will be offset by reduced
testing contractor needs.
```

---

### Step 6: Export Final Output
**Time: 2 minutes**

```
Format this status report for:
1. Email distribution (clean text format)
2. Presentation slides (key points only)
3. Portfolio dashboard entry (metrics summary)
```

---

## Example Output

Below is an abbreviated example of what a well-executed project status report looks like:

---

> **PROJECT STATUS REPORT**
> **Customer Portal Redesign**
> Week of January 15-19, 2024
>
> ---
>
> #### Executive Summary
>
> The Customer Portal Redesign project remains on track for the March 15 go-live date, with Phase 2 development progressing at 52% completion. Authentication API was completed ahead of schedule this week, and dashboard designs received approval. One blocking issue requires attention: vendor API credentials for payment integration are delayed, potentially impacting the timeline by one week if not resolved by January 26. QA resource confirmation expected by end of week.
>
> ---
>
> #### Overall Health Assessment
>
> | Dimension | Status | Trend | Notes |
> |-----------|--------|-------|-------|
> | **Overall** | 🟡 Yellow | Stable | Vendor dependency creating risk |
> | Schedule | 🟢 Green | Stable | Development ahead on key items |
> | Budget | 🟡 Yellow | Stable | 4% over plan, forecast within tolerance |
> | Scope | 🟢 Green | Stable | No scope changes this period |
> | Resources | 🟡 Yellow | Improving | QA start date pending confirmation |
> | Risk | 🟡 Yellow | Stable | Vendor issue being actively managed |
>
> ---
>
> #### Key Accomplishments This Week
>
> ✅ **User Authentication API Completed** - Finished 2 days ahead of schedule, enabling frontend integration to begin
>
> ✅ **Dashboard Wireframes Approved** - Minor revisions incorporated, design phase for this component complete
>
> ✅ **Security Review Initiated** - First pass underway, preliminary results positive
>
> ✅ **Bug Resolution** - 3 critical bugs from Sprint 3 resolved, improving system stability
>
> ---
>
> #### Risks Requiring Attention
>
> **HIGH PRIORITY**
>
> 🔴 **Payment Vendor API Documentation** (R-001)
> - *Impact:* Potential 1-week delay to payment integration
> - *Status:* Vendor call scheduled January 22
> - *Action Required:* None - being actively managed
> - *Escalation:* Will escalate to sponsor if not resolved by Jan 26
>
> ---
>
> #### Budget Status
>
> | Category | Budget | Actual | Variance |
> |----------|--------|--------|----------|
> | **Total** | **$450,000** | **$187,500** | **-4%** |
>
> **Forecast:** $455,000 at completion (+1.1% over budget)
> **Confidence:** Medium-High
>
> *Note: Security consultant engagement ($15k) offset by expected contractor savings*

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Inconsistent health ratings across reports | No clear criteria for Green/Yellow/Red | Establish documented thresholds (e.g., >2 weeks late = Yellow) and apply consistently |
| Executive summary too detailed | Including too much information | Lead with most important point, limit to 3-4 sentences, focus on decisions needed |
| Risks seem stale or outdated | Not reviewing risk log regularly | Review ALL risks during status process, close resolved items, add new ones |
| Numbers presented without meaning | Data without interpretation | Always pair metrics with "what it means" - is this good or bad, improving or declining? |
| Multiple versions show different status | Creating from scratch each time | Use same underlying data, just adjust detail level and focus for different audiences |
| Report takes as long as before | Trying to make it perfect | Use 80/20 rule - good enough report created quickly beats perfect report delivered late |

---

## Tips from Experience

1. **Consistency builds trust.** Same time, same format every week creates pattern recognition. Stakeholders know where to look for what they need.

2. **Status, not history.** Focus on current state and what's coming next. Don't rehash old news unless it provides necessary context.

3. **Highlight what changed.** If nothing changed from last report, say so explicitly. Changes deserve attention and explanation.

4. **Every issue needs an owner.** Never report a problem without identifying who's responsible for addressing it and what the next action is.

5. **Be honest about Yellow and Red.** Hiding problems prevents getting help. Yellow status enables support; perpetual Green status reduces credibility when things actually go wrong.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Weekly status report creation takes under 1 hour (down from 2-3 hours)
- [ ] Stakeholders can quickly understand project health without asking clarifying questions
- [ ] You're using the same format consistently across reporting periods
- [ ] Health assessments are backed by clear, documented rationale
- [ ] Different audience versions are generated from same underlying data

**Track over time:**
- Time spent creating status reports (target: <1 hour)
- Stakeholder questions after receiving report (fewer = clearer reporting)
- Accuracy of forecasts compared to actuals (improving = better assessment)

---

## Variations

### Agile Sprint Report
**When to use:** Scrum/Agile projects with 2-week sprints
```
Focus on velocity, burndown, sprint goals, and retrospective insights rather than
traditional milestones. Include:
- Sprint goal achievement (Met/Partially Met/Missed)
- Velocity trend (last 3 sprints)
- Impediments and resolutions
- Team capacity and availability
```

### Program Status Rollup
**When to use:** Multiple related projects under single program
```
Aggregate multiple project statuses into program-level view with:
- Cross-project dependencies
- Resource conflicts across projects
- Program-level risks affecting multiple projects
- Consolidated budget and timeline view
```

### Recovery Plan Status
**When to use:** Troubled project requiring corrective action
```
When project is Yellow or Red, focus on:
- Recovery actions being taken
- Corrective measures and their effectiveness
- Path back to Green status
- Timeline for recovery with milestones
```

---

## Building Your Repeatable System

After using this recipe 2-3 times, establish your system:

1. **Create your standard templates** - Lock in the sections you use every time: executive summary, health assessment, accomplishments, risks, budget, milestones.

2. **Define your health criteria** - Document exactly what Green/Yellow/Red means for schedule, budget, scope, resources, and risk. Remove subjectivity.

3. **Establish data collection rhythm** - Same time each week, pull data from same sources. Make it a habit, not a scramble.

4. **Build your distribution lists** - Know who gets the executive version, who gets the detailed version, who gets the portfolio entry.

**Sample Folder Structure:**
```
project-status-reports/
├── templates/
│   ├── executive-summary-template.md
│   ├── detailed-status-template.md
│   └── health-assessment-criteria.md
├── 2024-Q1/
│   ├── week-2024-01-15.md
│   ├── week-2024-01-22.md
│   └── week-2024-01-29.md
└── archive/
    └── 2023/
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**aggregating scattered data into audience-appropriate summaries with consistent assessment criteria**—applies broadly:

| Role | Application |
|------|-------------|
| **IT Operations** | System health reports, incident summaries, SLA performance dashboards |
| **Sales** | Pipeline status, forecast reports, deal health assessments by region |
| **Support** | Ticket volume trends, SLA compliance, escalation reports to leadership |
| **Finance** | Budget variance reports, spend tracking, forecast accuracy assessments |
| **HR** | Hiring pipeline status, onboarding progress, retention metrics reporting |

---

## Next Steps

1. **This week:** Create your first AI-assisted status report and compare time spent vs. your usual process.

2. **Track your results:** Note time savings and stakeholder feedback on clarity.

3. **Iterate:** Refine your prompts and templates based on what works for your organization.

4. **Share:** Show other PMs in your organization how you're creating better reports in less time.

---

*Recipe #86 of 100 in the Claude Code Knowledge Worker Recipe Collection*
