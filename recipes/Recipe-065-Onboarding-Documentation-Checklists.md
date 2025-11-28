# Onboarding Documentation and Checklists

**Recipe #65: Design New Hire Experiences That Set People Up for Success**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 5 minutes (first time) / 2 minutes (repeat) | 4-6 hours per program | Beginner | HR, Managers, People Operations |

---

## The Problem

New hires show up excited and leave confused. There's no consistent onboarding—each manager does something different. Critical tasks fall through cracks. New employees don't know who to talk to, where to find things, or what success looks like. Managers are too busy to properly onboard, so people figure it out themselves (or don't). The first 90 days determine retention, yet onboarding is often an afterthought.

**Pain Points:**
- No standard onboarding process
- New hires feel lost and unproductive
- Critical setup tasks forgotten
- Inconsistent experience across teams
- Managers don't know what to do
- No accountability for onboarding quality
- Early turnover attributed to "bad fit"

---

## The Outcome

Comprehensive onboarding programs with day-by-day schedules, checklists, meeting guides, and resource links. Clear accountability for each task. An experience that gets new hires productive faster while making them feel welcome and supported.

**What You'll Have When Done:**
- Onboarding timeline and schedule
- Task checklists (new hire, manager, HR, IT)
- First day/week/month guides
- Meeting templates and talking points
- Resource directory
- 30/60/90-day milestones

---

## When to Use This Recipe

**Good Fit:**
- Creating new onboarding programs
- Standardizing onboarding across teams
- Improving existing onboarding
- Role-specific onboarding plans
- Remote onboarding programs
- Scaling rapidly (high-volume hiring)

**Not a Good Fit:**
- Executive onboarding (different needs)
- Merger integration (larger scope)
- Contractor/temp onboarding (simpler)
- When there's no clarity on the role

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You know the role or role type
- [ ] You understand team structure and key relationships
- [ ] You know available resources and systems
- [ ] You have 30-45 minutes for complete program design

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Structures comprehensive onboarding plans
- Creates detailed checklists
- Designs meeting agendas
- Builds resource directories
- Sets appropriate milestones
- Ensures nothing is forgotten

**Where Human Judgment Is Essential:**
- Validating relevance to your company
- Adding company-specific resources
- Confirming stakeholder availability
- Adapting for culture
- Assigning ownership
- Approving final plan

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Role info | Title, team, level | Program customization |
| Company context | Culture, tools, structure | Resource planning |
| Timeline | Start date, key dates | Scheduling |
| Stakeholders | Key people to meet | Meeting design |
| Success criteria | What makes someone effective | Milestone setting |

**Sample Input:**
```
Onboarding Program Request

NEW HIRE: Senior Product Manager
DEPARTMENT: Product
REPORTS TO: VP of Product
START DATE: January 6, 2025
WORK LOCATION: Remote (US-based), occasional travel to SF HQ

COMPANY CONTEXT:
- CloudSync Pro, 150 employees
- B2B SaaS collaboration platform
- Remote-first company
- Values: customer obsession, data-driven, ownership, radical candor
- Growing 50% YoY, Series B

TEAM STRUCTURE:
- Product team: 8 people (1 VP, 3 PMs, 4 designers)
- This PM will own the enterprise product line
- Works closely with: Enterprise Engineering (12 people), Sales (5 enterprise reps), Customer Success (3 enterprise CSMs)

KEY STAKEHOLDERS TO MEET:
- VP Product (manager)
- Fellow PMs (Sarah, Mike)
- Lead Designer (Jamie)
- Enterprise Engineering Lead (Alex)
- VP Sales (Chris)
- VP Customer Success (Pat)
- CEO (Jordan) - typically meets all new hires
- Current PM transitioning out (Taylor) - knowledge transfer critical

CRITICAL SYSTEMS:
- Jira (project management)
- Figma (design)
- Notion (documentation)
- Slack (communication)
- Gong (customer call recordings)
- Salesforce (customer data)
- CloudSync (our own product!)

KEY RESOURCES:
- Product wiki in Notion
- Customer research repository
- Competitive analysis docs
- Previous roadmap presentations
- Enterprise customer list and health scores

SUCCESS CRITERIA:
- 30 days: Understand product, customers, and team. Can answer "what does CloudSync do for enterprise?"
- 60 days: Own the roadmap, shipping first small improvement
- 90 days: Full ownership, trusted partner to engineering and sales

CONSTRAINTS:
- First week should include HQ visit for in-person meetings
- Customer calls can start week 2
- Taylor (transitioning PM) leaves January 31 - overlap critical
- VP Product travels Jan 13-17

CULTURE NOTES:
- We move fast—don't wait for permission
- Ask for help—no one expects you to know everything
- Customers are accessible—talk to them early
- Documentation is valued—leave things better than you found them
```

---

## Step-by-Step Implementation

### Step 1: Gather Context
**Time: 5-10 minutes**

Collect:
- Role and team information
- Key stakeholders
- Systems and resources
- Success criteria
- Any constraints or timing

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Onboarding Design Prompt
**Time: 3-5 minutes for Claude to process**

---

**PRIMARY PROMPT: Onboarding Program Design**

```
Please design a comprehensive onboarding program for this new hire.

ROLE: [Title and level]
REPORTS TO: [Manager]
START DATE: [Date]
WORK LOCATION: [Office/Remote/Hybrid]

COMPANY CONTEXT:
[Company info, culture, size]

TEAM STRUCTURE:
[Who they work with]

KEY STAKEHOLDERS:
[People they need to meet]

SYSTEMS AND TOOLS:
[What they need access to]

KEY RESOURCES:
[Documentation, knowledge bases]

SUCCESS CRITERIA:
[30/60/90 day expectations]

CONSTRAINTS:
[Any timing or availability issues]

CREATE THE FOLLOWING:

1. ONBOARDING OVERVIEW

   **Program Goals:**
   - By day 30: [Goal]
   - By day 60: [Goal]
   - By day 90: [Goal]

   **Key Principles:**
   [Guiding principles for this onboarding]

   **Success Metrics:**
   [How we know onboarding worked]

2. PRE-BOARDING CHECKLIST (Before Day 1)

   **HR Tasks:**
   - [ ] [Task with owner and deadline]

   **IT Tasks:**
   - [ ] [Task with owner and deadline]

   **Manager Tasks:**
   - [ ] [Task with owner and deadline]

3. WEEK 1: ORIENTATION & FOUNDATIONS

   **Day 1:**
   | Time | Activity | With | Purpose | Location |
   |------|----------|------|---------|----------|
   [Hour-by-hour schedule]

   **Day 2:**
   [Schedule]

   **Day 3-5:**
   [Schedule]

   **Week 1 Outcomes:**
   - [ ] [What should be accomplished]

4. WEEK 2-4: LEARNING & OBSERVING

   **Week 2 Focus:** [Theme]
   - Key activities: [List]
   - Meetings to schedule: [List]
   - Deliverable: [What they should produce]

   **Week 3 Focus:** [Theme]
   [Same structure]

   **Week 4 Focus:** [Theme]
   [Same structure]

5. MONTH 2: CONTRIBUTING

   **Focus:** [Theme]

   **Key Activities:**
   - [Activity 1]
   - [Activity 2]

   **Milestones:**
   - [ ] [Milestone 1]
   - [ ] [Milestone 2]

6. MONTH 3: OWNING

   **Focus:** [Theme]

   **Key Activities:**
   - [Activity 1]

   **Milestones:**
   - [ ] [Milestone 1]

7. STAKEHOLDER MEETING GUIDE

   For each key stakeholder:

   **Meeting with [Name], [Role]**
   - Purpose: [Why this meeting]
   - Suggested timing: [When]
   - Duration: [Time]
   - Discussion topics:
     - [Topic 1]
     - [Topic 2]
   - Questions to ask:
     - [Question 1]
   - Desired outcome: [What to learn/achieve]

8. MANAGER CHECKLIST

   **Before Start:**
   - [ ] [Task]

   **Week 1:**
   - [ ] [Task]

   **Ongoing:**
   - [ ] [Task]

9. NEW HIRE CHECKLIST

   **Day 1:**
   - [ ] [Task]

   **Week 1:**
   - [ ] [Task]

   **Month 1:**
   - [ ] [Task]

10. 1:1 AGENDA TEMPLATES

    **First 1:1 (Day 1 or 2):**
    Topics:
    - [Topic 1]
    - [Topic 2]

    **Week 1 Check-in:**
    Topics:
    - [Topic 1]

    **30-Day Review:**
    Topics:
    - [Topic 1]

11. RESOURCE DIRECTORY

    **Getting Started:**
    - [Resource]: [Location/Link]

    **Key Documentation:**
    - [Resource]: [Location/Link]

    **People to Know:**
    - [Name]: [Role] — [What they help with]

12. FAQ FOR NEW HIRES

    **Q: [Common question]**
    A: [Answer]

Design an onboarding that builds confidence and competence progressively.
```

---

### Step 4: Customize for Your Context
**Time: 10-15 minutes**

```
Adjust the onboarding plan for these specifics:

SCHEDULE CHANGES:
- Week 1 must include: [Specific requirement]
- Avoid scheduling on: [Dates]

ADDITIONAL MEETINGS:
- Add meeting with: [Person, purpose]

RESOURCES TO ADD:
- [Resource name]: [Location]

CULTURAL ELEMENTS:
- Our tradition is: [Onboarding ritual]
```

---

### Step 5: Generate Final Package
**Time: 5 minutes**

```
Create the final onboarding package:

1. NEW HIRE GUIDE (for the new employee)
2. MANAGER GUIDE (for the manager)
3. HR CHECKLIST (for HR)
4. IT CHECKLIST (for IT)
5. STAKEHOLDER CALENDAR INVITES (pre-written)
6. 30/60/90 REVIEW TEMPLATES
```

---

## Example Output

Below is an abbreviated onboarding program example:

---

> **ONBOARDING PROGRAM**
>
> **Senior Product Manager, Enterprise**
> **Start Date: January 6, 2025**
>
> ---
>
> ## Program Goals
>
> **By Day 30:** Understand the product, customers, and team deeply enough to answer "what does CloudSync do for enterprise?" with confidence.
>
> **By Day 60:** Own the enterprise roadmap, ship first improvement, and be a trusted partner to engineering.
>
> **By Day 90:** Full ownership of enterprise product with demonstrated impact. Taylor (transitioning PM) can fully exit.
>
> ---
>
> ## Pre-Boarding Checklist (Before January 6)
>
> **HR Tasks (Complete by Jan 3):**
> - [ ] Send offer letter and new hire paperwork — HR
> - [ ] Order laptop and equipment — HR/IT
> - [ ] Schedule Day 1 orientation — HR
> - [ ] Send welcome email with first day details — HR
> - [ ] Add to company directory — HR
>
> **IT Tasks (Complete by Jan 3):**
> - [ ] Create email and Slack accounts — IT
> - [ ] Set up Jira, Figma, Notion, Gong access — IT
> - [ ] Configure laptop with required software — IT
> - [ ] Add to CloudSync demo environment — IT
> - [ ] Grant Salesforce read access — IT
>
> **Manager Tasks (Complete by Jan 3):**
> - [ ] Send personal welcome message — VP Product
> - [ ] Schedule Week 1 1:1s — VP Product
> - [ ] Notify team of new hire start date — VP Product
> - [ ] Prepare Day 1 team intro — VP Product
> - [ ] Brief Taylor on knowledge transfer plan — VP Product
> - [ ] Book HQ conference room for Week 1 meetings — VP Product
>
> **Taylor (Transitioning PM) Tasks:**
> - [ ] Prepare enterprise product overview doc — Taylor
> - [ ] Document top 10 enterprise customers and their needs — Taylor
> - [ ] List open issues and ongoing projects — Taylor
> - [ ] Identify key stakeholder relationships to transfer — Taylor
>
> ---
>
> ## Week 1: Orientation & Foundations
>
> *Location: San Francisco HQ (Mon-Fri)*
>
> ---
>
> ### Day 1 (Monday, January 6)
>
> | Time | Activity | With | Purpose |
> |------|----------|------|---------|
> | 9:00 AM | Arrive at HQ, welcome coffee | VP Product | Personal welcome |
> | 9:30 AM | HR orientation | HR | Paperwork, benefits, policies |
> | 10:30 AM | IT setup | IT | Laptop, accounts, access |
> | 11:30 AM | Team introduction | Product team | Meet the team |
> | 12:00 PM | Welcome lunch | VP Product + team | Build relationships |
> | 1:30 PM | Company overview | VP Product | CloudSync strategy, vision |
> | 3:00 PM | Product tour | Taylor | High-level product walkthrough |
> | 4:00 PM | Office tour, meet people | Team buddy | Get oriented |
> | 4:30 PM | First 1:1 with manager | VP Product | Expectations, questions |
>
> **Day 1 Outcomes:**
> - [ ] All accounts working
> - [ ] Met the immediate team
> - [ ] Understand company context
> - [ ] Clear on Week 1 plan
>
> ---
>
> ### Day 2 (Tuesday, January 7)
>
> | Time | Activity | With | Purpose |
> |------|----------|------|---------|
> | 9:00 AM | Enterprise product deep dive | Taylor | Understand the product line |
> | 10:30 AM | Customer overview | Taylor | Who are enterprise customers |
> | 12:00 PM | Lunch with engineering | Alex (Eng Lead) | Build relationship |
> | 1:30 PM | Engineering team overview | Alex | Understand how product works |
> | 3:00 PM | Review product wiki | Self-study | Read key documentation |
> | 4:00 PM | Questions session | Taylor | Clarify what you've learned |
>
> ---
>
> ### Day 3 (Wednesday, January 8)
>
> | Time | Activity | With | Purpose |
> |------|----------|------|---------|
> | 9:00 AM | Sales overview | VP Sales (Chris) | Understand go-to-market |
> | 10:30 AM | Listen to Gong calls | Self-study | Hear real customer conversations |
> | 12:00 PM | Lunch with design | Jamie (Design Lead) | Build relationship |
> | 1:30 PM | Design process overview | Jamie | How product and design work together |
> | 3:00 PM | Competitive landscape | Taylor | Understand market positioning |
> | 4:00 PM | Daily check-in | VP Product | Questions, observations |
>
> ---
>
> ### Day 4 (Thursday, January 9)
>
> | Time | Activity | With | Purpose |
> |------|----------|------|---------|
> | 9:00 AM | Customer Success overview | VP CS (Pat) | Understand customer lifecycle |
> | 10:30 AM | Review customer health scores | Self-study | Understand current customer state |
> | 12:00 PM | Team lunch | Full product team | Bond with team |
> | 1:30 PM | Current roadmap review | Taylor | What's planned and why |
> | 3:00 PM | Open issues and priorities | Taylor | What needs attention |
> | 4:00 PM | Prepare Week 1 summary | Self | Synthesize learning |
>
> ---
>
> ### Day 5 (Friday, January 10)
>
> | Time | Activity | With | Purpose |
> |------|----------|------|---------|
> | 9:00 AM | CEO meet & greet | Jordan (CEO) | Company vision, culture |
> | 10:00 AM | Week 1 synthesis | VP Product | Share observations, get feedback |
> | 11:00 AM | Peer PM conversations | Sarah, Mike | Learn from peers |
> | 12:00 PM | Farewell lunch at HQ | Team | Wrap up HQ visit |
> | 1:30 PM | Travel back / WFH setup | — | Set up remote workspace |
> | 3:00 PM | Plan Week 2 | Self | Organize next steps |
>
> **Week 1 Outcomes:**
> - [ ] Understand product at high level
> - [ ] Met all key stakeholders
> - [ ] Have context on enterprise customers
> - [ ] Can explain what CloudSync does
> - [ ] Remote setup complete
>
> ---
>
> ## Week 2-4: Learning & Observing
>
> *Location: Remote*
>
> ---
>
> ### Week 2: Customers & Market (Jan 13-17)
>
> *Note: VP Product traveling—async updates*
>
> **Focus:** Deep customer understanding
>
> **Key Activities:**
> - Shadow 3-4 customer calls (Gong recordings or live)
> - Review top 10 enterprise customer accounts in Salesforce
> - Talk to 2 enterprise CSMs about customer patterns
> - Review recent win/loss analysis
>
> **Meetings to Schedule:**
> - Daily sync with Taylor (30 min) — Knowledge transfer
> - CSM deep dives (2 x 30 min) — Customer insights
> - Sales rep conversations (2 x 30 min) — Deal dynamics
>
> **Deliverable:** One-page summary of "Top 5 things enterprise customers need" based on your learning. Share with VP Product.
>
> ---
>
> ### Week 3: Product & Process (Jan 20-24)
>
> **Focus:** How things get done
>
> **Key Activities:**
> - Participate in sprint planning and standup
> - Review last 3 months of shipped features
> - Understand roadmap process and tools (Jira, Notion)
> - Begin drafting questions for customer interviews
>
> **Meetings to Schedule:**
> - Engineering deep dive (1 hr) — Technical architecture
> - Sprint ceremonies — Observe team process
> - Weekly 1:1 with VP Product — Check-in
>
> **Deliverable:** Draft interview guide for customer research you'll start in Week 4.
>
> ---
>
> ### Week 4: Taking Over (Jan 27-31)
>
> **Focus:** Transition from Taylor
>
> *Critical: Taylor's last week*
>
> **Key Activities:**
> - Co-lead sprint planning with Taylor
> - Take ownership of active customer issues
> - Conduct 2 customer interviews (Taylor shadows)
> - Prepare 30-day summary presentation
>
> **Meetings to Schedule:**
> - Daily Taylor sync — Final knowledge transfer
> - Customer interviews (2 x 30 min) — Direct customer contact
> - 30-day review with VP Product — Formal check-in
>
> **Deliverable:** 30-day summary: What you've learned, what questions remain, your initial priorities.
>
> **Taylor Transition Complete:**
> - [ ] All active projects handed over
> - [ ] Customer relationships introduced
> - [ ] Engineering relationships established
> - [ ] Documentation updated
> - [ ] Taylor's last day (Jan 31)
>
> ---
>
> ## Stakeholder Meeting Guide
>
> ### Meeting with Chris, VP Sales
>
> **Purpose:** Understand how enterprise sales works, what product needs from you
> **Timing:** Day 3 (Week 1)
> **Duration:** 60 minutes
>
> **Discussion Topics:**
> - How the enterprise sales process works
> - What product can do to help close deals
> - Common customer objections
> - Product gaps that cost us deals
> - How to stay connected as partners
>
> **Questions to Ask:**
> - What's the #1 thing product could do to help sales?
> - Which deals are stuck because of product gaps?
> - How should I engage on strategic deals?
> - What do customers love that we should protect?
>
> **Desired Outcome:** Clear understanding of sales priorities; establish communication rhythm.
>
> ---
>
> ### Meeting with Jordan, CEO
>
> **Purpose:** Understand company vision, make personal connection
> **Timing:** Day 5 (Week 1)
> **Duration:** 30 minutes
>
> **Discussion Topics:**
> - Company vision and where we're headed
> - How enterprise fits in that vision
> - What success looks like for this role
> - Company culture—what's important here
>
> **Questions to Ask:**
> - What made you excited about the enterprise opportunity?
> - What's the biggest challenge facing CloudSync?
> - What should I know about the culture that isn't in the handbook?
> - What does great look like in 6 months for this role?
>
> **Desired Outcome:** Feel connected to company mission; understand CEO's perspective.
>
> ---
>
> ## Manager Checklist
>
> **Before Start:**
> - [ ] Send personal welcome message
> - [ ] Ensure all access is ready
> - [ ] Brief team on new hire
> - [ ] Book Week 1 in-person meetings
> - [ ] Prepare Taylor for knowledge transfer
>
> **Week 1:**
> - [ ] Be present for Day 1 welcome
> - [ ] Have daily check-ins
> - [ ] Introduce to key stakeholders
> - [ ] Set initial 1:1 rhythm
> - [ ] Share expectations clearly
>
> **Month 1:**
> - [ ] Weekly 1:1s (don't skip!)
> - [ ] Regular feedback on observations
> - [ ] Connect to projects gradually
> - [ ] Ensure Taylor transition is working
> - [ ] Conduct 30-day review
>
> **Month 2-3:**
> - [ ] Begin delegating real ownership
> - [ ] Provide stretch opportunities
> - [ ] 60-day and 90-day reviews
> - [ ] Solicit stakeholder feedback
>
> ---
>
> ## 30-Day Review Template
>
> **Date:** [Date]
> **Attendees:** New Hire, VP Product
>
> **Agenda:**
>
> 1. **How are you feeling?** (10 min)
>    - What's going well?
>    - What's challenging?
>    - Any surprises?
>
> 2. **What you've learned** (15 min)
>    - New hire presents summary
>    - Manager provides feedback
>
> 3. **Progress against goals** (10 min)
>    - Review 30-day milestones
>    - What's on track vs. needs attention
>
> 4. **Questions and gaps** (10 min)
>    - What do you still need to understand?
>    - What support do you need?
>
> 5. **Next 30 days** (10 min)
>    - Key priorities for Month 2
>    - Any adjustments to plan
>
> **After the meeting:**
> - Document outcomes and action items
> - Update onboarding tracker
> - Share feedback with HR (if applicable)

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Too many meetings | Over-scheduled | Limit to 3-4 substantial meetings per day; leave processing time |
| Information overload | Too much too fast | Spread learning; prioritize must-knows vs nice-to-knows |
| Manager too busy | No accountability | Make manager tasks explicit; involve HR in tracking |
| Missing critical people | Not identified | Ask: "Who will this person need relationships with to succeed?" |
| No clear deliverables | Passive learning | Add output: "What should they produce by end of Week 1?" |

---

## Tips from Experience

1. **First day is for feeling, not learning.** Focus on welcome, connection, and making them feel they belong.

2. **Front-load relationships.** People remember who they met more than what they read.

3. **Build in processing time.** Back-to-back meetings prevent absorption.

4. **Make the manager accountable.** Great onboarding requires manager engagement—make it explicit.

5. **Assign a buddy.** Someone who's not the manager, for "stupid questions."

6. **Check in frequently early.** Daily in Week 1, then dial back.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] New hire feels welcomed and supported
- [ ] Time to productivity improves
- [ ] 30/60/90 milestones are achieved
- [ ] Early turnover decreases
- [ ] Manager satisfaction increases
- [ ] New hire feedback is positive

**Track over time:**
- Time to first contribution
- 30/60/90-day milestone achievement
- New hire satisfaction (survey)
- Manager satisfaction (survey)
- 90-day and 1-year retention
- Performance at first review

---

## Variations

### Remote Onboarding
For fully remote hires:
```
Adapt for remote:
- Virtual coffee chats instead of in-person
- Video-first meetings (cameras on)
- Ship equipment early with setup guide
- Assign remote buddy
- Over-communicate in Slack
- Plan in-person meetup within 60 days

Include: Remote work guide, virtual social events
```

### High-Volume Onboarding
For scaling teams:
```
Design for cohorts:
- Group orientation sessions
- Peer cohort connections
- Standardized training modules
- Cohort Slack channel
- Group Q&A sessions
- Buddy program from previous cohort

Include: Cohort schedule, peer activities
```

### Technical Role Onboarding
For engineers, developers:
```
Add technical components:
- Development environment setup
- Codebase walkthrough
- First commit timeline
- Architecture documentation
- On-call shadowing
- Technical mentorship

Include: Technical onboarding checklist, first ticket guide
```

### Manager Onboarding
For people joining as managers:
```
Additional components:
- Team member 1:1s
- Team dynamics assessment
- Previous manager handoff
- Performance history review
- Leadership principles alignment
- 30-day "listening tour"

Include: Team transition plan, leadership expectations
```

---

## Building Your Repeatable System

After several onboardings, establish:

1. **Template library** by role family
2. **Standard checklists** (HR, IT, manager)
3. **Resource directory** (maintained)
4. **Feedback loop** to improve
5. **Onboarding metrics** dashboard

**Sample Setup:**
```
onboarding/
├── templates/
│   ├── general-onboarding.md
│   ├── engineering-onboarding.md
│   ├── sales-onboarding.md
│   └── manager-onboarding.md
├── checklists/
│   ├── hr-checklist.md
│   ├── it-checklist.md
│   └── manager-checklist.md
├── active/
│   ├── [new-hire-name]-jan-2025/
│   │   ├── onboarding-plan.md
│   │   └── progress-tracker.md
│   └── [new hires]
├── resources/
│   ├── company-overview.md
│   ├── systems-guide.md
│   └── people-directory.md
└── feedback/
    ├── new-hire-survey.md
    └── improvements-log.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**structured timeline → clear ownership → progressive milestones → regular check-ins**—applies broadly:

| Role | Application |
|------|-------------|
| **HR** | All employee onboarding |
| **Managers** | Team member onboarding |
| **Customer Success** | Customer onboarding |
| **Partners** | Partner onboarding |
| **Vendors** | Vendor orientation |
| **Projects** | New team member integration |

---

## Next Steps

1. **Identify the hire:** Who is starting soon?
2. **Gather context:** Role, team, stakeholders, resources
3. **Design the program:** Use this recipe
4. **Assign ownership:** Who does what?
5. **Execute and track:** Follow the plan, check in frequently
6. **Improve:** Collect feedback, iterate for next time

---

*Recipe #65 of 100 in the Claude Code Knowledge Worker Recipe Collection*
