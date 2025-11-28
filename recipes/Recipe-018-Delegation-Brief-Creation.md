# Delegation Brief Creation

**Recipe #18: From Quick Handoff to Comprehensive Delegation**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 10 minutes (first time) / 5 minutes (repeat) | 30-60 minutes per delegation | Beginner | All managers, Executives, Senior ICs |

---

## The Problem

You delegate a task and the result comes back wrong—not because the person is incapable, but because the handoff was incomplete. You said "handle the vendor review" but didn't specify the criteria, timeline, or authority level. The person made reasonable decisions that didn't match your unstated expectations. Now you're doing rework, they're frustrated, and future delegations become harder.

**Pain Points:**
- Vague handoffs leading to wrong outcomes
- Time spent on rework after poor delegation
- Direct reports hesitant to take ownership
- "I thought you meant..." conversations
- Difficulty scaling yourself through others
- Critical context staying in your head

---

## The Outcome

Clear, comprehensive delegation briefs that set others up for success. Every handoff includes context, objectives, constraints, authority level, and success criteria. Your team can execute with confidence because they know exactly what's expected. You multiply your capacity by delegating effectively.

**What You'll Have When Done:**
- Complete delegation brief for any task
- Clear success criteria and expectations
- Explicit authority level and decision rights
- Support structure and check-in points
- Reduced rework and better outcomes
- Team members who feel empowered

---

## When to Use This Recipe

**Good Fit:**
- Complex tasks requiring significant autonomy
- Delegating to someone unfamiliar with the domain
- High-stakes assignments where failure is costly
- Cross-functional work with multiple stakeholders
- Any time you've experienced delegation failures before

**Not a Good Fit:**
- Simple, routine tasks (overkill)
- Tasks the person has done many times successfully
- Situations requiring real-time collaboration (just work together)
- True emergencies (brief verbally, document later)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You're clear on what you're delegating
- [ ] You know who you're delegating to
- [ ] You've thought about timeline and constraints
- [ ] You know the decision authority level
- [ ] You have 10-15 minutes to create the brief

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Structures comprehensive delegation briefs
- Identifies information gaps you might miss
- Generates clear success criteria
- Creates appropriate check-in structures
- Tailors briefs to the delegate's experience level
- Produces consistent delegation documentation

**Where Human Judgment Is Essential:**
- Deciding what to delegate and to whom
- Knowing the delegate's capabilities
- Setting appropriate authority levels
- Providing organizational context
- Being available for questions
- Actually following up

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Task description | What needs to be done | Core brief content |
| Background context | Why this matters, history | Context for decision-making |
| Who you're delegating to | Their role, experience | Tailors detail level |
| Constraints | Budget, timeline, authority | Explicit guardrails |
| Success criteria | What "done well" looks like | Clear evaluation standard |

**Sample Input:**
```
Need to delegate: Lead the vendor selection for our new CRM system

Delegating to: Sarah (Project Manager, 2 years at company, hasn't led vendor selection before)

Background:
- Our current CRM contract expires in 90 days
- Budget is $150K annually
- Key stakeholders: Sales VP, Customer Success VP, IT Security
- We've shortlisted 3 vendors from initial research
- CEO wants a recommendation by end of month

What I care about:
- Fair evaluation process
- Stakeholder buy-in (especially Sales)
- Security requirements met
- On-time decision (can't miss contract deadline)

What I don't want:
- A decision driven purely by cost
- Stakeholders surprised at the end
- Security doing a last-minute veto
```

---

## Step-by-Step Implementation

### Step 1: Clarify the Delegation
**Time: 5 minutes**

Before creating the brief, answer:
- What exactly am I delegating? (specific outcomes)
- Why am I delegating this to this person?
- What's the timeline and any hard constraints?
- What decisions can they make vs. need to check with me?
- What does success look like?

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Delegation Brief Prompt
**Time: 2-3 minutes for Claude to process**

---

**PRIMARY PROMPT: Delegation Brief Generator**

```
Create a comprehensive delegation brief for the following assignment.

TASK TO DELEGATE:
[Describe what you're delegating]

DELEGATING TO:
- Name/Role: [Who]
- Experience level: [Their background with this type of work]
- Time available: [Full-time on this? Partial?]

BACKGROUND & CONTEXT:
"""
[Why this matters, history, anything they need to know]
"""

TIMELINE:
- Start: [Date]
- Key milestones: [Any interim deadlines]
- Final deadline: [End date]

CONSTRAINTS:
- Budget: [If applicable]
- Resources: [What they have to work with]
- Other limitations: [Anything they can't do]

KEY STAKEHOLDERS:
- [Stakeholder 1]: [Their interest/role]
- [Stakeholder 2]: [Their interest/role]

WHAT SUCCESS LOOKS LIKE:
[Your criteria for a job well done]

WHAT I WANT TO AVOID:
[Failure modes or outcomes you don't want]

PLEASE CREATE A DELEGATION BRIEF WITH:

1. ASSIGNMENT OVERVIEW
   - Clear one-paragraph description of what's being delegated
   - Why this matters (business context)
   - Their ownership and accountability

2. OBJECTIVES AND SUCCESS CRITERIA
   - Specific, measurable outcomes expected
   - How we'll evaluate success
   - Quality standards

3. SCOPE AND BOUNDARIES
   - What's included in this delegation
   - What's explicitly NOT included
   - Adjacent responsibilities that remain with others

4. AUTHORITY LEVEL
   - Decisions they CAN make independently
   - Decisions that need my input
   - Decisions that need my approval
   - Budget/spending authority

5. KEY INFORMATION
   - Background they need
   - Key stakeholders and how to engage them
   - Known risks or challenges
   - Resources available to them

6. TIMELINE AND CHECK-INS
   - Key milestones and dates
   - Check-in cadence (how often we'll sync)
   - What I need to see at each check-in
   - Escalation triggers (when to come to me immediately)

7. SUPPORT STRUCTURE
   - How I'll support them
   - Who else can help
   - Where to find resources/information
   - Standing meetings or access

8. POTENTIAL PITFALLS
   - Common mistakes to avoid
   - Risks specific to this assignment
   - Things that have gone wrong before

Format as a document they can reference throughout the assignment.
```

---

### Step 4: Review and Customize
**Time: 5-10 minutes**

Review the brief for:

**Completeness:**
- Is anything missing that they'll need?
- Are there implicit expectations you haven't stated?

**Clarity:**
- Would they understand this without verbal explanation?
- Is the authority level crystal clear?

**Appropriateness:**
- Is the detail level right for this person?
- Are you over-specifying (micromanaging in writing)?

---

### Step 5: Refine the Brief
**Time: 3-5 minutes**

**To adjust authority level:**
```
I want Sarah to have more autonomy. Change the vendor recommendation from "needs my approval" to "needs my input on final recommendation, but she makes the call."
```

**To add context:**
```
Add this political context: Sales VP has a strong preference for Vendor A based on past experience. Sarah should understand this but not let it bias the evaluation.
```

**To simplify:**
```
This is too detailed for Sarah's experience level—she might feel micromanaged. Shorten the potential pitfalls section and trust her more.
```

**To add guardrails:**
```
Add a guardrail: If any vendor's security assessment raises red flags, she should pause and check with IT Security AND me before proceeding.
```

---

### Step 6: Deliver and Set Up for Success
**Time: 5 minutes with the person**

Don't just send the brief—have a handoff conversation:

1. Walk through the brief together
2. Ask what questions they have
3. Confirm understanding of authority level
4. Schedule the first check-in
5. Express confidence in them

```
Create a short summary (3-5 bullets) I can use to walk Sarah through this in a 10-minute conversation.
```

---

## Example Output

Below is an abbreviated delegation brief example:

---

> # DELEGATION BRIEF
> ## CRM Vendor Selection Project
> ### Assigned to: Sarah Chen, Project Manager
> ### Date: January 10, 2024
>
> ---
>
> ## Assignment Overview
>
> You are leading the vendor selection process for our new CRM system. This is a high-visibility project affecting Sales and Customer Success teams daily operations. Our current contract expires in 90 days, making timely completion critical. You have full ownership of the evaluation process and stakeholder management, with the final vendor recommendation being yours to make.
>
> **Why this matters:** The CRM is the backbone of our customer relationships. The right choice improves sales productivity and customer retention; the wrong choice creates friction for 50+ daily users.
>
> ---
>
> ## Objectives and Success Criteria
>
> **Primary Objective:** Recommend a CRM vendor that meets our functional, technical, and budgetary requirements by January 31.
>
> **Success looks like:**
> - ✅ All three stakeholder groups (Sales, CS, IT Security) support the recommendation
> - ✅ Clear rationale documented for the decision
> - ✅ Security requirements formally validated
> - ✅ Recommendation delivered by January 31 (no extensions)
> - ✅ Smooth handoff to contract negotiation phase
>
> **Quality standards:**
> - Evaluation criteria documented and agreed before scoring
> - Each stakeholder has participated in at least one demo
> - Security assessment completed for finalist vendor
>
> ---
>
> ## Authority Level
>
> | Decision Type | Your Authority |
> |---------------|----------------|
> | Evaluation criteria and weighting | ✅ You decide |
> | Demo scheduling and logistics | ✅ You decide |
> | Stakeholder meeting facilitation | ✅ You decide |
> | Reference check questions and approach | ✅ You decide |
> | Requesting vendor pricing/proposals | ✅ You decide |
> | Final vendor recommendation | ✅ **You decide** (inform me) |
> | Contract terms and negotiation | ❌ Handoff to Procurement |
> | Spending on evaluation activities | ✅ Up to $2K without approval |
>
> ---
>
> ## Timeline and Check-ins
>
> | Milestone | Date | Deliverable |
> |-----------|------|-------------|
> | Evaluation criteria finalized | Jan 15 | Documented scorecard |
> | Demos complete | Jan 22 | Demo notes + initial scores |
> | Security assessment | Jan 26 | IT Security sign-off |
> | Recommendation ready | Jan 31 | Written recommendation |
>
> **Check-in cadence:** Weekly 30-minute sync (Thursdays 2pm)
>
> **What I need at each check-in:**
> - Status vs. timeline
> - Stakeholder temperature
> - Any blockers or risks
> - Decisions you need input on
>
> **Escalate immediately if:**
> - Any stakeholder is actively blocking progress
> - Security assessment reveals showstoppers
> - Timeline is at risk
>
> ---
>
> ## Potential Pitfalls
>
> **Watch out for:**
> 1. **Sales VP's vendor preference** — He likes Vendor A from past experience. Give it fair consideration but don't let it bias the evaluation.
> 2. **Security last-minute veto** — Engage IT Security early. A late "no" derails everything.
> 3. **Feature checklist blindness** — The best CRM isn't the one with the most features; it's the one people will actually use.
>
> ---
>
> ## My Commitment to You
>
> - I'll be available for questions within 24 hours (usually faster)
> - I'll clear blockers with my peers if needed
> - I won't second-guess your process or swoop in to take over
> - I'll give you honest feedback at check-ins, not surprises at the end
>
> I'm confident you'll do great work on this. Own it.

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| They keep checking everything | Authority level unclear or trust not established | Clarify: "You have permission to make these decisions without asking me" |
| Outcome was different than expected | Unstated expectations | Add to future briefs; use this as learning |
| They felt micromanaged | Too much detail | Reduce specificity; delegate the "how" not just the "what" |
| They hit blockers and got stuck | Escalation triggers unclear | Make explicit: "Come to me immediately if X happens" |
| Stakeholders weren't aligned | Didn't emphasize stakeholder management | Add: "Your job includes building stakeholder buy-in" |
| They missed the deadline | Didn't have enough context on criticality | Make timeline non-negotiability explicit |

---

## Tips from Experience

1. **The brief is a conversation starter, not a replacement for conversation.** Walk through it together; don't just send and expect.

2. **Match detail level to the person.** Experienced people need less; new people need more. Adjust accordingly.

3. **Be explicit about authority.** "Use your judgment" sounds empowering but creates anxiety. Tell them what they can decide.

4. **Build in early check-ins.** Catch misalignment in week 1, not at the deadline.

5. **Own your failures.** If delegation goes wrong, first question is whether YOUR handoff was complete. Usually it wasn't.

6. **Celebrate when it works.** Public recognition for successful delegation encourages others to step up.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Delegated tasks come back done correctly first time
- [ ] Team members feel empowered, not constrained
- [ ] You're able to scale yourself through others
- [ ] Check-ins are informative, not revealing surprises
- [ ] Others are willing to take on more responsibility

**Track over time:**
- Rework rate on delegated tasks
- Team confidence in taking on new responsibilities
- Your capacity freed up through effective delegation

---

## Variations

### Delegation to Peer or Cross-Functional Partner
For delegating to someone who doesn't report to you:
```
This delegation is to a peer, not a direct report. Adjust the brief to:
- Frame as a request/collaboration, not an assignment
- Be explicit about what you're asking vs. offering
- Clarify what's in it for them
- Acknowledge their other priorities
- Define how decisions will be made jointly
```

### Delegating Up (Managing Up)
For asking your manager to take something on:
```
I need to delegate something to my manager. Create a brief that:
- Clearly explains what I need from them
- Justifies why they're the right person (influence, access)
- Is respectful of their time
- Provides everything they need to act
- Minimizes their effort while still getting the outcome
```

### Delegating to a Contractor/Vendor
For external resources:
```
This delegation is to an external contractor/vendor. Adjust to:
- Be more formal and complete (they have less context)
- Include explicit acceptance criteria
- Define communication protocols
- Specify deliverables and format requirements
- Include IP and confidentiality expectations
- Define payment/approval milestones
```

### Quick Delegation (Time-Sensitive)
When you don't have time for a full brief:
```
I need to delegate quickly. Create a minimal brief that covers:
1. What (in one sentence)
2. Why it matters
3. By when
4. Authority level (one line)
5. Single most important thing to get right
6. Who to ask if stuck

Keep it under 200 words total.
```

---

## Building Your Repeatable System

After several delegations, establish your system:

1. **Create a delegation template** for consistent handoffs
2. **Build a delegation log** tracking what's out and when to check in
3. **Document lessons learned** from delegation successes and failures
4. **Develop standard authority levels** for common delegation types
5. **Create a "delegation retrospective" habit** after major assignments

**Sample Setup:**
```
delegation/
├── templates/
│   ├── full-delegation-brief.txt
│   └── quick-delegation.txt
├── active/
│   ├── sarah-crm-vendor/
│   │   ├── brief.md
│   │   └── check-in-notes.md
│   └── alex-budget-analysis/
├── completed/
│   └── [archived delegations]
└── lessons-learned.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**clarify expectations → document thoroughly → set up for success**—applies broadly:

| Role | Application |
|------|-------------|
| **Executives** | Delegating strategic initiatives |
| **Managers** | All levels of task assignment |
| **Project Managers** | Work package delegation |
| **Senior ICs** | Handing off work to others |
| **Consultants** | Client handoffs and transitions |
| **Anyone** | Getting help effectively |

---

## Next Steps

1. **Next delegation:** Use this recipe instead of a quick verbal handoff
2. **Review past failures:** What would a better brief have included?
3. **Build your template:** Customize for your common delegation types
4. **Practice the conversation:** The brief is just the start; the conversation seals it

---

*Recipe #18 of 100 in the Claude Code Knowledge Worker Recipe Collection*
