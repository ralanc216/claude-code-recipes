# Task and Project List Organization

**Recipe #8: From Scattered Tasks to Prioritized Action**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 5 minutes (first time) / 2 minutes (repeat) | 30-60 minutes per week | Beginner | Anyone managing multiple workstreams |

---

## The Problem

Your tasks live everywhere—in your head, sticky notes, multiple apps, email threads, Slack messages, and meeting notes. You know you're forgetting things. You aren't sure what's most important. You spend mental energy remembering instead of doing. When someone asks "what are you working on?" you can't give a clear answer.

**Pain Points:**
- Tasks scattered across 5+ locations
- No clear sense of priority
- Mental overhead of remembering everything
- Dropping balls on important items
- Unable to see the full picture of your commitments
- Weekly planning takes forever (or doesn't happen)

---

## The Outcome

A consolidated, prioritized task list organized by project, deadline, and importance. Dependencies identified. Clear view of your week. Mental clarity from capturing everything in one place. The ability to say "here's what I'm working on" with confidence.

**What You'll Have When Done:**
- Comprehensive task list capturing all commitments
- Priority ranking based on impact and urgency
- Project grouping showing related work
- Dependencies and blockers identified
- Realistic weekly plan based on available time
- Feeling of control over your work

---

## When to Use This Recipe

**Good Fit:**
- Weekly planning sessions
- When feeling overwhelmed by competing demands
- Starting a new role or project with many unknowns
- After returning from vacation to a pile of tasks
- Quarterly or monthly planning and prioritization
- Before high-demand periods to get organized

**Not a Good Fit:**
- Day-to-day task management (use your normal tools)
- Simple weeks with obvious priorities
- When you already have a well-functioning system

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You've brain-dumped all your tasks (messy is fine)
- [ ] You can access your various task sources (email, notes, apps)
- [ ] You know your goals/priorities for the current period
- [ ] You have 15-30 minutes for organization and planning

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Processes messy, unstructured task lists
- Identifies duplicates and related items
- Groups tasks by project or theme
- Suggests prioritization based on criteria you provide
- Flags dependencies and blockers
- Creates time-blocked plans

**Where Human Judgment Is Essential:**
- Deciding actual importance vs. perceived urgency
- Understanding political/relationship priorities
- Knowing effort level for tasks (you know your work)
- Making hard choices when everything can't get done
- Committing to the plan

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Brain dump | Random list of things you need to do | Raw task capture |
| Email to-dos | Copied from flagged emails | Committed obligations |
| Meeting notes | Action items from recent meetings | Extracted tasks |
| App exports | Todoist, Asana, etc. exports | Existing task lists |
| Calendar | Upcoming deadlines | Time constraints |
| Goals | Current quarter priorities | Prioritization context |

**Sample Brain Dump (What You Might Have):**
```
BRAIN DUMP - Everything on my mind:

- finish Q4 planning deck
- respond to Sarah's email about the vendor
- hire senior engineer - need to review resumes
- annual review for Tom - due Friday!!
- fix bug in reporting dashboard
- prepare for board meeting next week
- renew AWS contract before it expires
- write blog post (told marketing I would)
- 1:1 with new team member
- follow up with customer about renewal
- book travel for conference
- update team OKRs
- that thing I promised my manager 2 weeks ago (what was it?)
- dentist appointment
- process expense reports
- review PR from James
- strategic planning offsite - need to prepare
- mom's birthday gift
- security training (overdue)
- read the industry report Sarah sent
```

---

## Step-by-Step Implementation

### Step 1: Brain Dump Everything
**Time: 5-10 minutes**

Get everything out of your head and scattered locations:

- Scan email for flagged items and commitments
- Check Slack for things you said you'd do
- Review meeting notes from the past week
- Look at any existing task lists or apps
- Add anything floating in your head

Don't organize—just capture. Messy is perfect.

**Pro Tip:** Set a 10-minute timer. Capture quickly. You'll organize in the next step.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Task Organization Prompt
**Time: 2-3 minutes for Claude to process**

---

**PRIMARY PROMPT: Task List Organization**

```
Please help me organize my scattered tasks into a prioritized, actionable system.

MY RAW TASK DUMP:
"""
[PASTE YOUR BRAIN DUMP HERE]
"""

MY CONTEXT:
- Role: [e.g., Engineering Manager]
- Current priorities: [e.g., Q4 planning, hiring, team development]
- Available hours this week for focused work: [e.g., ~15 hours]
- Key deadlines I know about: [e.g., Board meeting Jan 25, reviews due Jan 19]

PLEASE PROVIDE:

1. CLEANED TASK LIST
   - Remove duplicates and consolidate related items
   - Clarify vague items (suggest specific next actions)
   - Separate true tasks from "someday/maybe" items
   - Flag any items that need more definition

2. PROJECT GROUPING
   - Group tasks by project or area of responsibility
   - Identify which tasks are standalone vs. part of larger efforts
   - Note any hidden projects (multiple related tasks that form a bigger initiative)

3. PRIORITY RANKING
   Using this framework:
   - P1: Urgent AND important (do this week, can't slip)
   - P2: Important, not urgent (schedule this week)
   - P3: Urgent, less important (delegate or quick-handle)
   - P4: Neither (schedule later or drop)

   Rank each task with rationale.

4. DEPENDENCIES & BLOCKERS
   - Which tasks are blocked by others?
   - Which tasks block other work?
   - Any external dependencies (waiting on someone)?

5. WEEKLY PLAN RECOMMENDATION
   Based on my ~[X] available hours:
   - Recommended focus for this week
   - What realistically fits
   - What should explicitly wait until next week
   - Suggested daily distribution if helpful

6. ITEMS NEEDING ATTENTION
   - Overdue or at-risk items
   - Items that need clarification (ask someone)
   - Items that might be delegable
   - Items that could be declined/dropped
```

---

### Step 4: Review and Adjust
**Time: 5-10 minutes**

Review Claude's organization:

**Check prioritization:**
- Do the P1s feel right? Would you actually do these first?
- Any important items ranked too low?
- Any low-importance items ranked too high?

**Check grouping:**
- Are the project groupings logical?
- Any tasks that should be connected that aren't?

**Check realism:**
- Does the weekly plan fit your actual capacity?
- Any overcommitment?

---

### Step 5: Refine and Decide
**Time: 5 minutes**

**To adjust priorities:**
```
The customer renewal follow-up should be P1, not P2. It's a $500K account at risk. Please re-rank and adjust the weekly plan.
```

**To get more specific:**
```
"Prepare for board meeting" is too vague. Break this down into specific sub-tasks with time estimates.
```

**To handle overcommitment:**
```
I have 15 hours but you've suggested 25 hours of work. What should I explicitly defer or delegate to make this realistic?
```

**To identify quick wins:**
```
Which of these tasks could I complete in under 15 minutes each? Give me a list for when I have small time blocks.
```

**To get delegation suggestions:**
```
Which of these tasks could reasonably be delegated, and to whom (I have a team of 6 engineers and 1 project manager)?
```

---

### Step 6: Export and Transfer
**Time: 2 minutes**

Save your organized list:
```
Save this as my weekly task plan: "Week-Jan-15-Task-Plan.md"
```

Transfer to your system:
```
Format the P1 and P2 tasks for import into Todoist/Asana/etc.
```

Or for a visual board:
```
Create a simple Kanban view with columns: This Week, Next Week, Blocked, Delegated
```

---

## Example Output

Below is abbreviated example output:

---

> **CLEANED TASK LIST**
>
> *Clarified and consolidated from 21 items to 18 distinct tasks:*
>
> | Task | Clarified Next Action |
> |------|----------------------|
> | "Finish Q4 planning deck" | Complete slides 8-15 and add financial projections |
> | "That thing for manager" | ⚠️ Needs clarification - ask manager what this was |
> | "Hire senior engineer" | Review 5 resumes in queue, decide who to phone screen |
> | "Mom's birthday gift" | Order gift online (moved to personal list) |
>
> ---
>
> **PROJECT GROUPING**
>
> **Q4 Planning (4 tasks)**
> - Complete planning deck
> - Update team OKRs
> - Prepare for strategic planning offsite
> - Review industry report (input for planning)
>
> **Hiring (2 tasks)**
> - Review 5 resumes
> - 1:1 with new team member
>
> **Team Management (3 tasks)**
> - Annual review for Tom
> - Security training (overdue)
> - 1:1 with new team member
>
> **Customer/Business (3 tasks)**
> - Follow up with customer about renewal
> - Board meeting prep
> - Renew AWS contract
>
> **Operational/Admin (4 tasks)**
> - Review PR from James
> - Fix reporting dashboard bug
> - Process expense reports
> - Book conference travel
>
> ---
>
> **PRIORITY RANKING**
>
> **P1 - Must Do This Week**
> | Task | Deadline | Rationale |
> |------|----------|-----------|
> | Annual review for Tom | Fri Jan 19 | Hard deadline, impacts his timeline |
> | Complete Q4 planning deck | Mon Jan 22 | Presenting Monday, no buffer |
> | Customer renewal follow-up | None stated | High-value account, time-sensitive |
>
> **P2 - Should Do This Week**
> | Task | Rationale |
> |------|-----------|
> | Review resumes | Blocking hiring pipeline |
> | Board meeting prep | Jan 25 - need lead time |
> | AWS contract renewal | Expires soon, needs attention |
>
> **P3 - If Time Allows**
> - Review PR from James (can unblock him)
> - 1:1 with new team member (important but can flex)
> - Fix dashboard bug (annoying but not critical)
>
> **P4 - Defer or Drop**
> - Blog post (apologize to marketing, defer to Feb)
> - Industry report (skim only, full read later)
>
> ---
>
> **WEEKLY PLAN (15 hours available)**
>
> *Realistic scope: 12-14 hours of tasks, 1-3 hours buffer*
>
> | Day | Focus | Est. Hours |
> |-----|-------|------------|
> | Mon | Q4 deck completion | 3 |
> | Tue | Tom's review + customer follow-up | 3 |
> | Wed | Board prep + resume review | 3 |
> | Thu | AWS contract + 1:1 | 2 |
> | Fri | Buffer + quick wins | 2 |
>
> **Explicitly Deferred to Next Week:**
> - Blog post (communicate to marketing)
> - Dashboard bug fix
> - Strategic offsite prep (Jan 28 offsite)

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Still feels overwhelming | Too many P1s | Be honest: "Force rank these P1s. If I could only do 3 this week, which 3?" |
| Tasks too vague | Not clarified to next action | Ask: "Break down each vague task into the specific next physical action" |
| Can't estimate time | Tasks poorly defined | Ask: "Estimate time for each task. Flag any that need more scoping" |
| Keep adding new tasks | Didn't capture everything initially | Add new items, re-run prioritization: "Here are 5 more things. Re-rank the full list" |
| Nothing feels droppable | Everything seems important | Ask: "If I could only keep 50% of these tasks, which 50% has the most impact?" |
| Personal tasks mixed in | Work/life blended | Ask Claude to separate into work vs. personal lists |

---

## Tips from Experience

1. **Do this weekly.** 20 minutes every Monday morning transforms your week. Make it a ritual.

2. **Be honest about capacity.** If you have 15 hours of focused work time, don't plan 30 hours of tasks. Build in buffer.

3. **Distinguish projects from tasks.** "Launch new feature" is a project. "Draft feature spec" is a task. Break projects into tasks.

4. **Accept that some things won't happen.** Better to consciously defer than unconsciously drop. The list helps you make explicit choices.

5. **Capture "waiting for" items.** Things blocked on others still need tracking. "Waiting for Sarah's vendor response" is a valid item.

6. **Review at end of week.** What got done? What didn't? Why? This learning improves future planning.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] You have one source of truth for your tasks
- [ ] Weekly planning takes under 30 minutes
- [ ] You rarely forget committed tasks
- [ ] You can answer "what are you working on?" clearly
- [ ] You feel in control rather than overwhelmed

**Track over time:**
- Tasks completed vs. planned each week
- Number of "dropped balls" or forgotten commitments
- Feeling of control/overwhelm (simple 1-10 weekly rating)

---

## Variations

### Quarterly Planning
For longer-horizon planning:
```
Help me plan my quarter. Here are:
- My goals for Q1: [list]
- Major projects: [list]
- Known deadlines: [list]
- Recurring commitments: [list]

Please create:
1. Project breakdown with milestones
2. Monthly themes/focuses
3. Resource/time allocation by area
4. Risks to the plan
5. Recommended first two weeks in detail
```

### Project Planning
For organizing a specific project:
```
Help me plan this project: [project description]

Current status: [where things stand]
Deadline: [if any]
Resources: [who's involved]

Create:
1. Work breakdown structure (all tasks)
2. Dependencies and sequence
3. Timeline/schedule
4. Risk register
5. First 10 tasks in priority order
```

### Delegation Planning
When you need to offload work:
```
I'm overcommitted. Here's my full task list: [list]
I have these team members who could help: [list with brief capabilities]

Help me:
1. Identify which tasks are delegable
2. Match tasks to team members
3. Create delegation briefs for each (what, context, deadline, support needed)
4. Determine what only I can do
```

### Catch-Up Organization
After vacation or absence:
```
I've been out for [X days/weeks]. Here's what accumulated:
- [Email summary]
- [Slack highlights]
- [Meeting notes]
- [New requests]

Help me:
1. Triage everything by urgency
2. Identify anything truly overdue or at-risk
3. Create a catch-up plan for the first 3 days back
4. Draft any needed "I'm back, here's status" messages
```

---

## Building Your Repeatable System

After using this recipe, establish your weekly system:

1. **Capture everywhere, process once.** Quick-capture to inbox throughout week, organize weekly
2. **Weekly planning session.** Same time each week, 20-30 minutes
3. **Daily review.** 5 minutes each morning to look at today's plan
4. **Weekly review.** What worked? What didn't? Lessons?
5. **Quarterly reset.** Full brain dump and reorg quarterly

**Sample Setup:**
```
task-management/
├── templates/
│   └── weekly-planning-prompt.txt
├── weekly-plans/
│   ├── 2024-W03.md
│   ├── 2024-W04.md
│   └── ...
├── projects/
│   ├── q4-planning.md
│   └── hiring.md
└── inbox.md                       # Quick capture throughout week
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**brain dump chaos → structured organization → prioritized plan**—applies broadly:

| Role | Application |
|------|-------------|
| **Executives** | Strategic priority management across initiatives |
| **Managers** | Team workload and delegation planning |
| **Project Managers** | Project breakdown and task sequencing |
| **Individual Contributors** | Personal productivity and focus |
| **Students** | Assignment and study planning |
| **Anyone** | Personal life task management |

---

## Next Steps

1. **Today:** Brain dump everything on your mind
2. **Run this recipe:** Get organized for this week
3. **Weekly ritual:** Schedule 30 minutes every Monday
4. **Review and improve:** Each week, refine what works

---

*Recipe #8 of 100 in the Claude Code Knowledge Worker Recipe Collection*
