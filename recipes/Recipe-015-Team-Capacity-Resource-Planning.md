# Team Capacity and Resource Planning

**Recipe #15: From Gut Feel to Data-Driven Allocation**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 15 minutes (first time) / 10 minutes (repeat) | 2-4 hours per planning cycle | Intermediate | Managers, Project Managers, Resource Planners |

---

## The Problem

You need to figure out if your team can handle the upcoming work. Right now, capacity planning is spreadsheets and gut feel—you think the team is at capacity, but you can't articulate why or show the data. When new requests come in, you either say yes to everything (overcommitting) or push back without evidence (appearing unhelpful). When leadership asks "can you take on X?" you genuinely don't know.

**Pain Points:**
- No clear picture of current team utilization
- Saying yes to everything until the team breaks
- Can't justify resource requests with data
- New work gets added without understanding trade-offs
- Some people overloaded while others have bandwidth
- Planning feels like guessing rather than analysis

---

## The Outcome

A clear analysis of your team's current capacity, planned work, and gap between demand and supply. You can answer "can we do this?" with data, identify who has bandwidth, and justify resource requests with evidence. Planning becomes proactive rather than reactive.

**What You'll Have When Done:**
- Team capacity analysis with utilization percentages
- Gap analysis: demand vs. available capacity
- Work allocation recommendations
- Trade-off analysis for new requests
- Resource request justification
- Visual representation of team workload

---

## When to Use This Recipe

**Good Fit:**
- Quarterly or sprint planning
- Responding to "can your team take on X?" requests
- Justifying headcount requests
- Rebalancing workload across team
- Understanding why the team feels stretched
- Planning for a demanding period

**Not a Good Fit:**
- Individual task management (too detailed)
- Very small teams where informal conversation suffices
- Highly fluid work that can't be estimated
- Real-time daily planning (too slow)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You know your team members and their roles/skills
- [ ] You have a sense of upcoming work/commitments
- [ ] You know standard capacity assumptions for your team
- [ ] You have current allocations (even rough estimates)
- [ ] You have 30-45 minutes for analysis and planning

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Calculates utilization and capacity percentages
- Identifies overloaded and underutilized team members
- Models different allocation scenarios
- Generates visual representations of workload
- Creates trade-off analyses for decisions
- Produces documentation for leadership requests

**Where Human Judgment Is Essential:**
- Knowing actual capabilities (who's really good at what)
- Understanding hidden work (operational overhead, support)
- Political and relationship considerations
- Deciding trade-offs (quality vs. speed vs. scope)
- Validating effort estimates
- Team dynamics and growth considerations

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Team roster | Names, roles, working hours | Capacity baseline |
| Current allocations | Who's on what projects | Current utilization |
| Planned work | Upcoming projects/sprints | Future demand |
| Time off | PTO, holidays, training | Reduced capacity |
| Historical data | Past project durations | Effort estimation |
| Constraints | Skills, dependencies | Allocation constraints |

**Sample Input (What You Might Provide):**
```
Team: Platform Engineering (6 people)

Team members:
- Sarah Chen (Senior) - Full time
- Alex Jones (Mid) - Full time
- Jordan Park (Junior) - Full time
- Mike Wilson (Senior) - Full time, but 20% on-call rotation
- Lisa Wang (Mid) - 80% allocation (20% grad school)
- New hire starting Feb 1 (Junior level expected)

Current commitments:
- API Migration: Sarah (lead, 60%), Alex (40%), Mike (30%) - ends Feb 15
- Platform Stability: Mike (50%), Jordan (60%) - ongoing
- Tech Debt Backlog: Alex (40%), Jordan (40%), Lisa (40%) - ongoing
- On-call/Support: rotates, ~20% average per person

New requests on the table:
1. AI Feature Infrastructure (estimate: 2 senior FTE for 3 months)
2. Security Audit Support (estimate: 1 FTE for 6 weeks)
3. Developer Portal (estimate: 1.5 FTE for 4 months)

Planning period: Feb-April 2024 (Q1)
```

---

## Step-by-Step Implementation

### Step 1: Gather Team and Work Data
**Time: 10-15 minutes**

Collect:
- Team roster with availability (FTEs, working hours)
- Current project allocations (% per person per project)
- Upcoming work with effort estimates
- Known time off and constraints
- Any skills or capability constraints

Don't worry about perfect precision—directionally correct is valuable.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Capacity Analysis Prompt
**Time: 3-5 minutes for Claude to process**

---

**PRIMARY PROMPT: Team Capacity and Resource Planning**

```
Please analyze my team's capacity and help me plan resource allocation.

TEAM INFORMATION:
"""
[PASTE YOUR TEAM ROSTER WITH AVAILABILITY]
"""

CURRENT COMMITMENTS:
"""
[PASTE CURRENT PROJECT ALLOCATIONS]
"""

NEW WORK REQUESTS:
"""
[PASTE NEW WORK WITH EFFORT ESTIMATES]
"""

PLANNING PERIOD: [Start date] to [End date]

ASSUMPTIONS:
- Standard capacity per person: [e.g., 40 hours/week, 80% productive after meetings/overhead]
- Sprint/cycle length: [e.g., 2 weeks]
- Buffer for unplanned work: [e.g., 10%]

PLEASE PROVIDE:

1. CURRENT STATE ANALYSIS
   - Team capacity summary (total FTEs available)
   - Current utilization by person (% allocated)
   - Current utilization by project
   - Identify: overloaded (>100%), fully loaded (90-100%), has bandwidth (<90%)

2. CAPACITY TABLE
   Create a table showing:
   | Person | Role | Available % | Allocated % | Free % | Notes |

3. GAP ANALYSIS
   - Total capacity available (in FTE-weeks or hours)
   - Total demand from current + new work
   - Gap (surplus or deficit)
   - Risk assessment

4. ALLOCATION RECOMMENDATIONS
   For new work requests, provide:
   - Can we take this on? (Yes/Yes with trade-offs/No)
   - Recommended team assignments
   - Impact on other work
   - Required trade-offs

5. SCENARIO MODELING
   Model these scenarios:
   A: Accept all new work (what breaks?)
   B: Accept priority work only (what do we defer?)
   C: Request additional resources (what do we need?)

6. RESOURCE REQUEST JUSTIFICATION
   If we need more resources:
   - How many FTEs needed
   - Skills/level required
   - Business justification based on this analysis
   - What we can/cannot deliver without additional resources

7. VISUAL REPRESENTATION
   Create a text-based visualization of team workload.
```

---

### Step 4: Review the Analysis
**Time: 10-15 minutes**

Check Claude's analysis against your knowledge:

**Validate capacity numbers:**
- Do utilization percentages match your intuition?
- Are there hidden work items not captured?
- Is the effort estimation reasonable?

**Check recommendations:**
- Are the suggested allocations realistic given skills and experience?
- Are there dependencies or constraints Claude missed?
- Would the trade-offs actually work?

---

### Step 5: Model Scenarios and Decisions
**Time: 10-15 minutes**

**To explore a specific scenario:**
```
Model the scenario where we prioritize the AI Feature Infrastructure and defer the Developer Portal. Show the new allocation and identify who would work on what.
```

**To understand trade-offs:**
```
If we say yes to the Security Audit but need to complete it in 4 weeks instead of 6, what would need to change? What's the impact?
```

**To justify a resource request:**
```
Create a one-page resource request for leadership explaining why we need 1 additional senior engineer to meet Q1 commitments without sacrificing quality.
```

**To rebalance the team:**
```
Jordan seems overloaded and Lisa has bandwidth. Suggest how to rebalance current work to bring everyone into the 80-90% utilization range.
```

---

### Step 6: Create Planning Documents
**Time: 5 minutes**

```
Create three outputs:
1. A capacity summary I can share with my team
2. A resource request memo for leadership
3. My planning notes with decisions made
```

---

## Example Output

Below is an abbreviated capacity analysis example:

---

> **TEAM CAPACITY ANALYSIS: Platform Engineering | Q1 2024 (Feb-Apr)**
>
> ---
>
> **EXECUTIVE SUMMARY**
>
> The team is currently at **94% utilization** with existing commitments. Adding all requested new work would require **137% capacity**—a clear deficit. We can accommodate 1-2 of the three new requests with trade-offs, or we need 1 additional FTE to meet all demands.
>
> ---
>
> **CURRENT CAPACITY TABLE**
>
> | Team Member | Role | Available | Allocated | Free | Status |
> |-------------|------|-----------|-----------|------|--------|
> | Sarah Chen | Senior | 100% | 60% | 40% | ✅ Bandwidth |
> | Alex Jones | Mid | 100% | 80% | 20% | ⚠️ Near capacity |
> | Jordan Park | Junior | 100% | 100% | 0% | 🔴 At capacity |
> | Mike Wilson | Senior | 80% | 80% | 0% | 🔴 At capacity |
> | Lisa Wang | Mid | 80% | 40% | 40% | ✅ Bandwidth |
> | New Hire | Junior | 50%* | 0% | 50% | ✅ Onboarding |
>
> *New hire at 50% productivity during February ramp-up
>
> **Total Capacity:** 5.1 FTE | **Currently Allocated:** 4.8 FTE | **Available:** 0.3 FTE
>
> ---
>
> **NEW WORK ASSESSMENT**
>
> | Request | Effort | Can We? | Recommendation |
> |---------|--------|---------|----------------|
> | AI Feature Infrastructure | 2 Sr FTE × 3mo | ⚠️ With trade-offs | Defer to March; assign Sarah + Mike after API migration |
> | Security Audit | 1 FTE × 6wk | ✅ Yes | Assign Lisa (40%) + Alex (20%) + contractor support |
> | Developer Portal | 1.5 FTE × 4mo | ❌ Not now | Defer to Q2 or request additional headcount |
>
> ---
>
> **SCENARIO ANALYSIS**
>
> **Scenario A: Accept All Work**
> - Team utilization: 137% (unsustainable)
> - Risk: Burnout, quality issues, all projects slip
> - Not recommended
>
> **Scenario B: Prioritize (AI + Security, Defer Portal)**
> - Team utilization: 108% (tight but manageable short-term)
> - Trade-off: Tech debt backlog pauses; some stability risk
> - Feasible if Portal truly can defer
>
> **Scenario C: Request 1 Additional Senior FTE**
> - Team utilization: 91% (healthy)
> - Enables all Q1 commitments
> - Lead time issue: hire won't be productive until late Q1
>
> ---
>
> **RECOMMENDED PATH FORWARD**
>
> 1. **Accept** Security Audit—can staff with current team
> 2. **Conditionally accept** AI Feature Infrastructure—starts March after API Migration completes, Sarah leads
> 3. **Defer** Developer Portal to Q2 or submit resource request
> 4. **Rebalance** Jordan's workload—move 20% of stability work to Lisa
> 5. **Begin hiring** for senior role to create buffer for Q2

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Numbers don't feel right | Hidden work not captured | Add: "Include estimate for operational overhead—on-call, meetings, support requests" |
| Junior treated same as senior | Skill levels not factored | Add: "Account for productivity differences: Senior 100%, Mid 80%, Junior 60% for complex work" |
| Plan falls apart immediately | Too rigid, no buffer | Add: "Include 15-20% buffer for unplanned work in all allocations" |
| Can't get effort estimates | Work isn't well-defined | Estimate ranges: "Use T-shirt sizing and convert: S=0.5 FTE-month, M=1, L=2, XL=3+" |
| Leadership doesn't believe the data | Analysis too abstract | Add concrete examples: "Without additional capacity, Project X slips 4 weeks" |
| Team pushes back on allocations | Didn't involve them | Review allocations with each person before finalizing |

---

## Tips from Experience

1. **Build in buffer.** Plans that assume 100% utilization fail immediately. 80-85% planned utilization leaves room for reality.

2. **Don't confuse "busy" with "allocated."** Someone can be in meetings all day but allocated to nothing strategic. Track project allocation, not calendar fullness.

3. **Account for skill constraints.** Three juniors don't equal one senior for complex work. Model accordingly.

4. **Update regularly.** Capacity analysis isn't a one-time exercise. Refresh monthly or each sprint.

5. **Make it visual.** Leadership grasps a visual capacity chart faster than a spreadsheet. Create something that communicates at a glance.

6. **Track actual vs. planned.** After each planning period, compare what happened to what you planned. Calibrate your estimates.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] You can answer "can we take this on?" with data
- [ ] Resource requests get approved because they're well-justified
- [ ] Team workload is balanced (no one burned out while others idle)
- [ ] You can model trade-offs before committing to new work
- [ ] Planning feels proactive rather than reactive

**Track over time:**
- Accuracy of effort estimates (actual vs. planned)
- Team satisfaction with workload balance
- Success rate of resource requests
- Frequency of over-commitment and resulting delays

---

## Variations

### Sprint Planning Capacity
For agile sprint capacity:
```
Help me calculate sprint capacity for the upcoming sprint.

Team:
[List with sprint availability - PTO, etc.]

Sprint length: [X days/weeks]
Historical velocity: [points per sprint]

Factors:
- Planned PTO this sprint: [who and when]
- Known interruptions: [meetings, demos, etc.]
- Carryover from last sprint: [items]

Calculate realistic sprint capacity and recommend how much work to pull into the sprint.
```

### Annual Headcount Planning
For budget and headcount:
```
Help me build headcount plan for next year.

Current team: [roster]
Planned departures: [if any]
Known major initiatives: [list with rough effort]

Calculate:
1. Capacity gap analysis for planned work
2. Headcount needed by quarter
3. Roles and levels needed
4. Business justification narrative

Format for inclusion in annual budget request.
```

### Cross-Team Resource Request
When borrowing resources:
```
I need to request resources from another team.

I need: [X skills for Y duration for Z purpose]
Why: [business justification]
Timeline: [when needed]

Create a professional resource request that:
- Clearly states the ask
- Provides business justification
- Shows I've exhausted internal options
- Proposes specific arrangement
- Addresses their concerns (what's in it for them)
```

### Team Growth Planning
For scaling a team:
```
I need to plan team growth over the next year.

Current team: [roster with skills]
Growth targets: [company/org growth plans]
Anticipated demand: [new products, features, etc.]

Model:
1. When demand will exceed current capacity
2. Recommended hiring timeline
3. Roles to hire and sequence
4. Onboarding capacity constraints
5. Budget implications
```

---

## Building Your Repeatable System

After a few planning cycles, establish your system:

1. **Create a capacity template** updated each planning period
2. **Track effort actuals** to calibrate future estimates
3. **Build a request queue** for incoming work with estimates
4. **Maintain skills inventory** for your team
5. **Set regular planning cadence** (monthly or quarterly)

**Sample Setup:**
```
capacity-planning/
├── templates/
│   ├── capacity-analysis-prompt.txt
│   └── resource-request-template.md
├── team-data/
│   ├── roster-and-skills.md
│   └── historical-velocity.csv
├── planning-cycles/
│   ├── 2024-Q1/
│   │   ├── capacity-analysis.md
│   │   └── decisions.md
│   └── 2024-Q2/
└── tracking/
    └── planned-vs-actual.csv
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**inventory resources → model demand → identify gaps → recommend allocation**—applies broadly:

| Role | Application |
|------|-------------|
| **Engineering Managers** | Sprint and quarterly planning |
| **Project Managers** | Project staffing and timeline planning |
| **Operations** | Workforce planning and scheduling |
| **Finance** | Budget allocation modeling |
| **Sales Ops** | Territory and quota planning |
| **Any Manager** | Team workload management |

---

## Next Steps

1. **This planning cycle:** Use this recipe for your next capacity analysis
2. **Start tracking:** Begin capturing effort actuals to improve estimates
3. **Build your template:** Customize prompts for your team's specific context
4. **Train your intuition:** Compare Claude's analysis to your gut feel—learn where they differ

---

*Recipe #15 of 100 in the Claude Code Knowledge Worker Recipe Collection*
