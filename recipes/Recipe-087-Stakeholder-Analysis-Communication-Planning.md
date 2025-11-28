# Stakeholder Analysis and Communication Planning

**Recipe #87: From Unmanaged Stakeholders to Strategic Engagement**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 30 minutes (first time) / 15 minutes (repeat) | 2-4 hours per project | Intermediate | Project Managers, Change Managers, Program Managers |

---

## The Problem

Projects succeed or fail based on stakeholder engagement, yet stakeholder analysis is often done superficially—a quick list of names without real understanding of interests, influence, or communication needs. When stakeholders feel uninformed or unheard, they become obstacles. When they're engaged appropriately, they become advocates. The challenge is understanding dozens of stakeholders with different needs and creating a communication approach that reaches each one effectively.

**Pain Points:**
- Superficial stakeholder lists with names but no understanding of their interests or power
- Important stakeholders discovered mid-project when they block progress
- One-size-fits-all communication that misses different stakeholder needs
- Resistance from stakeholders who feel blindsided or uninformed
- Time wasted managing conflicts that could have been prevented
- Lack of champions because supporters weren't cultivated early
- Critical decisions delayed because key influencers weren't engaged

---

## The Outcome

A comprehensive stakeholder map with influence/interest analysis, tailored communication strategies for each stakeholder segment, and a concrete communication plan that ensures the right people receive the right information at the right time through the right channels.

**What You'll Have When Done:**
- Complete stakeholder register with influence, interest, and attitude assessments
- Stakeholder matrix mapping engagement strategy for each segment
- Detailed profiles for high-priority stakeholders with specific engagement plans
- Communication plan matrix showing who gets what, when, and how
- 90-day communication calendar with specific activities
- Key message frameworks tailored to each audience

---

## When to Use This Recipe

**Good Fit:**
- Project kickoffs and planning phases
- Organizational change initiatives
- Product launches affecting multiple groups
- Cross-functional program management
- Merger/acquisition integration
- Process transformation projects
- New system implementations

**Not a Good Fit:**
- Small team projects with 5-10 people who all know each other
- Projects entirely within your direct control
- Short-duration tasks (under 2 weeks)
- Situations where stakeholders are already well-aligned and engaged

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] Project scope and objectives documented
- [ ] Organizational chart or team structure
- [ ] List of potentially affected groups
- [ ] Known supporters and detractors
- [ ] Historical context on stakeholder relationships
- [ ] Communication channel inventory (email, meetings, Slack, etc.)
- [ ] Project timeline and key milestones
- [ ] You have 45-60 minutes for initial analysis

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Systematically analyzes stakeholder information across multiple dimensions
- Identifies patterns in influence and interest across stakeholder groups
- Recommends engagement strategies based on stakeholder profiles
- Generates tailored communication plans with appropriate frequency and channels
- Creates communication calendars aligned with project milestones
- Ensures no critical stakeholder segments are overlooked

**Where Human Judgment Is Essential:**
- Assessing political dynamics and informal power structures
- Determining who truly has influence vs. who has title
- Reading stakeholder attitudes and likely reactions
- Deciding what information to share and what to withhold
- Navigating sensitive relationships and organizational history
- Choosing when to escalate or when to manage independently

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Project context | "ERP migration, 18 months, impacts all employees" | Understanding scope and stakeholder breadth |
| Stakeholder list | "CFO (sponsor), VP Finance (skeptical), 30 Finance staff" | Categorizing and prioritizing stakeholders |
| Org relationships | "VP Finance had bad ERP experience before" | Assessing attitudes and concerns |
| Communication channels | "Monthly all-hands, weekly dept meetings, Slack, email" | Matching messages to appropriate channels |
| Known concerns | "Finance worried about year-end timing" | Tailoring engagement strategies |

**Sample Input:**
```
PROJECT: ERP System Migration
SCOPE: Replace legacy finance and HR systems with cloud-based ERP
TIMELINE: 18 months
IMPACT: All employees will use new system; major process changes
for Finance (30 people), HR (15 people), IT (20 people)

BUSINESS DRIVERS:
- Current system end-of-life in 24 months
- Compliance requirements not met by legacy system
- Manual processes costing $500K/year in inefficiencies

KNOWN STAKEHOLDERS:
EXECUTIVES:
- CEO: Sarah Chen - Strong sponsor, championing the initiative
- CFO: Michael Brown - Project sponsor, accountable for success
- COO: David Lee - Concerned about operational disruption
- CIO: Jennifer Wu - Technical authority, cautiously supportive

DEPARTMENT HEADS:
- VP Finance: Amanda White - Skeptical, had bad ERP experience before
- Controller: Lisa Anderson - Key user, worried about audit compliance
- IT Director: Karen Davis - Technical owner, resource constrained

END USERS:
- Finance Staff (25): Primary users, varying tech comfort levels
- HR Staff (12): Secondary users, focused on employee data
- All Employees (500): Self-service portal users

KNOWN CONCERNS:
- Finance team worried about learning new system during year-end
- IT concerned about integration with other systems
- HR worried about data migration accuracy
```

---

## Step-by-Step Implementation

### Step 1: Prepare Your Project Context
**Time: 10 minutes**

Gather your project information, stakeholder list, organizational chart, and any known concerns or relationships. Don't worry if the list isn't complete—you'll identify gaps through the analysis.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Stakeholder Identification Prompt
**Time: 5 minutes for Claude to process**

---

**PRIMARY PROMPT: Stakeholder Identification and Categorization**

```
Claude, I'm starting stakeholder analysis for a project.

Project context:
[Paste project description, scope, timeline, business drivers]

Known stakeholders:
[Paste stakeholder list with roles, relationships, known attitudes]

Help me:
1. Ensure the stakeholder list is complete - identify any missing stakeholder groups
2. Categorize stakeholders by type (executive, management, end users, external)
3. Identify any obvious conflicts, alliances, or political dynamics
4. Suggest which stakeholders require deep analysis vs. basic tracking

Format this as a comprehensive stakeholder register.
```

---

### Step 4: Analyze Influence and Interest
**Time: 10 minutes**

```
For each stakeholder in the register, assess their position:

Stakeholder list: [Paste from Step 3]
Project context: [Paste project details]

Rate each stakeholder on:
1. INFLUENCE (High/Medium/Low) - Power to impact project success
2. INTEREST (High/Medium/Low) - How much they care about outcomes
3. CURRENT ATTITUDE (Champion/Supporter/Neutral/Resistant)
4. DESIRED ATTITUDE (What we need from them for success)

Create a stakeholder matrix mapping these dimensions and recommend
engagement strategies for each quadrant:
- Manage Closely (High Influence, High Interest)
- Keep Satisfied (High Influence, Low Interest)
- Keep Informed (Low Influence, High Interest)
- Monitor (Low Influence, Low Interest)
```

---

### Step 5: Develop Engagement Strategies
**Time: 10 minutes**

```
For high-priority stakeholders (those requiring close management or special attention):

Stakeholders: [List high-priority stakeholders from analysis]
Project context: [Paste]

For each stakeholder, create a detailed profile:
1. What they care about most (their priorities)
2. What concerns or fears they have
3. What information they need to feel confident
4. How they prefer to receive information
5. Who influences them
6. What would make them a champion vs. what would make them resist
7. Specific engagement strategy with tactics and timing

Focus especially on resistant or skeptical stakeholders.
```

---

### Step 6: Create Communication Plan
**Time: 10 minutes**

```
Create a detailed communication plan:

Stakeholder analysis: [Paste from previous steps]
Project milestones: [Paste timeline and key dates]
Available channels: [Paste communication options and constraints]

Generate:
1. Communication matrix (who gets what information, through which channel, how often)
2. Key message framework for each major audience segment
3. Communication calendar for first 90 days with specific activities
4. Feedback and escalation mechanisms
5. RACI for who creates and delivers communications

Make this actionable and specific.
```

---

### Step 7: Review and Validate
**Time: 10-15 minutes**

**Check immediately:**
- All affected groups are represented
- High-influence stakeholders have specific strategies
- Communication frequency matches stakeholder needs
- Message frameworks address known concerns

**Spot-check specifics:**
- Resistant stakeholders have concrete engagement tactics
- External stakeholders (auditors, vendors, board) included
- Communication calendar is realistic given resource constraints
- Escalation paths are clear

---

### Step 8: Refine and Iterate
**Time: 5-10 minutes**

**To add stakeholder details:**
```
Create a detailed engagement strategy for [Stakeholder Name]:
- Current position: [Resistant/Neutral/Supportive]
- Key concerns: [List]
- Desired outcome: [What we need from them]

Provide specific tactics, timeline, and success criteria.
```

**To adjust communication frequency:**
```
The Finance team needs more frequent communication than weekly.
Update the communication matrix to show bi-weekly department meetings
and a dedicated Slack channel for questions.
```

---

### Step 9: Export Final Documentation
**Time: 5 minutes**

```
Format the stakeholder analysis and communication plan as:
1. Executive summary (1 page overview for sponsor)
2. Detailed stakeholder register (spreadsheet format)
3. Communication calendar (first 90 days)
4. High-priority stakeholder profiles (detailed engagement strategies)
```

---

## Example Output

Below is an abbreviated example of what a well-executed stakeholder analysis looks like:

---

> **STAKEHOLDER ANALYSIS AND COMMUNICATION PLAN**
> **ERP System Migration Project**
>
> ---
>
> #### Executive Summary
>
> This document maps 47 stakeholders across 8 categories for the ERP Migration project. Analysis reveals strong executive sponsorship but significant concern at the middle management level, particularly in Finance. The communication strategy focuses on building confidence through transparency, early wins, and heavy support for the most impacted groups.
>
> **Key Findings:**
> - 4 stakeholders require close management (high influence, high interest)
> - Finance department needs intensive change management support
> - External stakeholders (auditors, board) need formal milestone communications
> - 70% of end users have low ERP experience—training is critical
>
> ---
>
> #### Stakeholder Matrix
>
> ```
>                     INTEREST
>                     Low         High
>                 ┌───────────┬───────────┐
>            High │  KEEP     │  MANAGE   │
>                 │ SATISFIED │  CLOSELY  │
>     INFLUENCE   │           │           │
>                 │ S01, S03  │ S02, S04  │
>                 │ S19       │ S06, S10  │
>                 ├───────────┼───────────┤
>            Low  │  MONITOR  │   KEEP    │
>                 │           │ INFORMED  │
>                 │           │           │
>                 │ S16       │ S08, S09  │
>                 │           │ S11, S14  │
>                 └───────────┴───────────┘
> ```
>
> **Manage Closely:** CFO Michael Brown, CIO Jennifer Wu, VP Finance Amanda White, IT Director Karen Davis
>
> **Keep Satisfied:** CEO Sarah Chen, COO David Lee, Board
>
> **Keep Informed:** Controller, HR Director, Finance Managers, Finance Staff
>
> **Monitor:** General employee population
>
> ---
>
> #### S06: Amanda White, VP Finance — HIGH PRIORITY
>
> | Attribute | Assessment |
> |-----------|------------|
> | **Current Position** | Resistant |
> | **Target Position** | Neutral → Supportive |
> | **Influence Level** | High (controls Finance adoption) |
> | **Key Concerns** | Previous ERP failure; Year-end timing; Team capacity |
> | **Information Needs** | Proof points, risk mitigation plans, training schedule |
> | **Preferred Channel** | 1:1 meetings with CFO and PM |
>
> **Engagement Strategy:**
> 1. CFO to have direct conversation about her concerns (Week 1)
> 2. Connect her with peer at company that successfully migrated (Week 2)
> 3. Give her team "early look" access to demonstrate ease of use (Week 4)
> 4. Ensure her input shapes Finance module configuration
> 5. Public recognition of Finance team contributions
> 6. Guaranteed no go-live during year-end close period
>
> ---
>
> #### Communication Plan Matrix
>
> | Audience | Communication | Channel | Frequency | Owner | Start |
> |----------|---------------|---------|-----------|-------|-------|
> | Steering Committee | Project status, decisions | Meeting | Monthly | PM | M1 |
> | CFO (Sponsor) | Detailed progress, risks | 1:1 | Weekly | PM | M1 |
> | VP Finance | Progress, concerns | 1:1 | Bi-weekly | PM | M1 |
> | Finance Staff | What's changing, support | Training + Slack | Weekly | Change Mgr | M3 |
> | All Employees | Awareness, timeline | All-hands + email | Monthly | PM | M3 |

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Important stakeholders discovered mid-project | Incomplete initial identification | Use multiple methods: org charts, process maps, ask "who else cares?"; validate with sponsor |
| Stakeholder has more/less power than assumed | Influence misjudged | Validate assessments with colleagues who know the organization; adjust strategy quickly |
| Stakeholders complain about too many messages | Communication overload | Consolidate messages; use "need to know" vs "nice to know" filter; respect preferences |
| Key stakeholder won't engage | Resistant stakeholder avoiding you | Engage through their trusted colleagues; address root concerns; escalate if blocking |
| Communication plan not being followed | Too complex or unrealistic | Simplify to what you can actually execute; assign clear owners; track compliance |
| Stakeholder positions change unexpectedly | Static analysis in dynamic environment | Reassess regularly (monthly); adapt strategies based on feedback and behavior |

---

## Tips from Experience

1. **Start early.** Stakeholder analysis in the planning phase prevents problems during execution. Trying to fix stakeholder issues mid-project is 10x harder.

2. **Validate assumptions.** Your assessments of influence and interest might be wrong. Test them with people who know the organization and stakeholders personally.

3. **Focus energy ruthlessly.** You cannot deeply engage everyone. Prioritize the high-influence stakeholders and those whose resistance could derail you.

4. **Listen more than talk.** Understand concerns before pushing messages. The best engagement comes from addressing what they actually care about, not what you think they should care about.

5. **Adapt continuously.** Stakeholder positions change as projects evolve. A supporter can become resistant, a skeptic can become a champion. Reassess regularly.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] 95%+ stakeholder awareness of project existence (survey at Month 3)
- [ ] 70%+ of key stakeholders are positive or neutral (based on interviews)
- [ ] Communication effectiveness rated useful by 80%+ of recipients
- [ ] No major stakeholder surprises or blockers from unanticipated resistance
- [ ] Champions actively advocating for the project without prompting

**Track over time:**
- Stakeholder sentiment shift (measure quarterly)
- Engagement rates in feedback channels
- Adoption rates among key stakeholder groups

---

## Variations

### Change Management Focus
**When to use:** Transformational initiatives requiring significant behavior change
```
Emphasize resistance management, readiness assessment, and adoption planning.
Add stakeholder readiness scoring and change impact analysis.
Focus communication on "what's in it for me" and capability building.
```

### Executive Stakeholder Map
**When to use:** High-visibility strategic initiatives with C-suite and board
```
Focus on C-suite dynamics, informal power structures, board member concerns.
Communication is highly curated, formal, and focused on business outcomes.
Include board presentation calendar and executive briefing materials.
```

### External Stakeholder Analysis
**When to use:** Projects with significant customer, partner, or vendor impact
```
Map customer segments, partner ecosystem, regulatory bodies, media.
Communication focuses on competitive positioning, market messaging.
Include PR and external communications strategies.
```

---

## Building Your Repeatable System

After using this recipe 2-3 times, establish your system:

1. **Create standard templates** - Stakeholder register template, analysis matrix template, communication plan template, stakeholder profile template for deep-dive analysis.

2. **Build process integration** - Include stakeholder analysis in all project initiation checklists. Review stakeholder map at steering committee meetings. Update assessments monthly or at phase gates.

3. **Establish feedback loops** - Regular pulse checks on stakeholder sentiment. Conduct formal stakeholder feedback surveys at project close. Track what engagement strategies worked.

4. **Build organizational knowledge** - Archive stakeholder analyses for future projects. Document stakeholder preferences that persist across initiatives. Build relationship history for repeat stakeholders.

**Sample Folder Structure:**
```
stakeholder-management/
├── templates/
│   ├── stakeholder-register-template.xlsx
│   ├── communication-plan-template.md
│   └── stakeholder-profile-template.md
├── current-projects/
│   ├── erp-migration/
│   │   ├── stakeholder-analysis.md
│   │   ├── communication-calendar.xlsx
│   │   └── high-priority-profiles/
│   └── portal-redesign/
└── reference/
    ├── engagement-strategies-that-worked.md
    └── stakeholder-preferences.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**mapping influence and interest to tailor engagement strategies**—applies broadly:

| Role | Application |
|------|-------------|
| **Product Management** | Customer and market stakeholder mapping for feature prioritization |
| **Policy/Compliance** | Affected party identification and engagement for regulatory changes |
| **HR/Org Design** | Employee and leadership alignment for organizational changes |
| **Sales** | Decision maker and influencer mapping for complex enterprise deals |
| **Partnerships** | Partner ecosystem stakeholder analysis for joint initiatives |

---

## Next Steps

1. **This week:** Complete stakeholder analysis for your current project and identify your top 5 high-priority stakeholders.

2. **Track your results:** Monitor stakeholder sentiment monthly and adjust strategies based on feedback.

3. **Iterate:** Refine your engagement tactics based on what works with different stakeholder personalities.

4. **Share:** Brief your project team on stakeholder analysis so everyone understands the landscape and communication responsibilities.

---

*Recipe #87 of 100 in the Claude Code Knowledge Worker Recipe Collection*
