# 1:1 Meeting Preparation and Documentation

**Recipe #14: From Scattered Context to Productive Conversations**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 5 minutes (first time) / 3 minutes (repeat) | 30-45 minutes per meeting | Beginner | All managers with direct reports |

---

## The Problem

You have back-to-back 1:1 meetings but haven't had time to prepare for any of them. You scramble to remember what you discussed last time, what action items were pending, and what's actually going on with each person. Conversations end up reactive rather than developmental, and important topics get pushed to "next time" repeatedly.

**Pain Points:**
- No time to prepare between meetings
- Forgetting what was discussed or committed last time
- Action items fall through the cracks
- Same issues discussed repeatedly without resolution
- Developmental conversations crowded out by status updates
- Different quality of attention for different team members

---

## The Outcome

A prepared agenda for each 1:1 with context from previous meetings, pending action items surfaced, and thoughtful discussion topics queued. After the meeting, organized notes capture decisions and next steps. Your 1:1s become consistent, productive, and truly developmental.

**What You'll Have When Done:**
- Pre-meeting agenda with context and priorities
- Previous action items and commitments surfaced
- Suggested discussion topics based on history
- Post-meeting documentation of decisions and next steps
- Running history that makes each conversation build on the last

---

## When to Use This Recipe

**Good Fit:**
- Regular 1:1 meetings with direct reports
- Skip-level meetings
- Mentor/mentee check-ins
- Regular stakeholder touchpoints
- Any recurring meeting where continuity matters

**Not a Good Fit:**
- First meetings (no history to draw from)
- Ad-hoc crisis conversations (just have the conversation)
- Large group meetings (different dynamic)
- Meetings where the other person drives the agenda entirely

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have notes from previous 1:1s (or remember key points)
- [ ] You know what's happened since last meeting (projects, issues)
- [ ] You have any feedback or topics you need to address
- [ ] You have 5-10 minutes before the meeting

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Synthesizes history from previous meeting notes
- Identifies patterns and recurring themes
- Generates relevant discussion topics
- Tracks action items and commitments
- Creates consistent documentation format
- Surfaces items that have been pending too long

**Where Human Judgment Is Essential:**
- Knowing what's really important to discuss
- Reading the room and adjusting in the moment
- Providing personal support and coaching
- Making judgment calls on sensitive topics
- Being present in the actual conversation

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Previous 1:1 notes | Last 2-4 meeting notes | Continuity and follow-up |
| Action items | Pending commitments | Accountability tracking |
| Project status | Current work context | Relevant topics |
| Feedback received | Input from others | Discussion points |
| Development goals | Their growth objectives | Developmental focus |

**Sample Previous Notes:**
```
1:1 Notes - Sarah Chen - Dec 15

Discussed:
- API project is on track, demo next week
- She's frustrated with product team response time
- Interested in tech lead opportunities
- Mentioned feeling burned out from Q4 push

Action items:
- Sarah: Send me the architecture doc by Friday
- Me: Talk to Product manager about response time
- Me: Share tech lead role description

Next time:
- Follow up on burnout - how is she recovering?
- Discuss conference attendance
```

---

## Step-by-Step Implementation

### Step 1: Gather Context
**Time: 2-3 minutes**

Pull together:
- Notes from the last 1-2 meetings
- Any pending action items
- What you know has happened since (projects, wins, issues)
- Any feedback or topics you need to raise

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Generate Pre-Meeting Agenda
**Time: 2-3 minutes for Claude to process**

---

**PRIMARY PROMPT: 1:1 Pre-Meeting Preparation**

```
Help me prepare for my 1:1 with [NAME].

CONTEXT:
- Their role: [Role/title]
- Reporting relationship: [Direct report / skip-level / etc.]
- Meeting frequency: [Weekly / bi-weekly / etc.]
- Today's meeting time: [Duration]

PREVIOUS MEETING NOTES:
"""
[PASTE NOTES FROM LAST 1-2 MEETINGS]
"""

PENDING ACTION ITEMS:
- From them: [List any commitments they made]
- From me: [List any commitments I made]

WHAT'S HAPPENED SINCE LAST MEETING:
- [Notable events, project updates, any issues]

TOPICS I NEED TO ADDRESS:
- [Any specific feedback or topics from your side]

PLEASE GENERATE:

1. AGENDA FOR TODAY'S 1:1
   - Suggested time allocation
   - Priority order of topics
   - Mix of: check-in, updates, development, and their agenda

2. ACTION ITEM FOLLOW-UP
   - Status check questions for each pending item
   - Any items that have been pending too long (flag these)

3. SUGGESTED DISCUSSION TOPICS
   - Based on patterns from previous meetings
   - Development-focused questions
   - Topics that have been deferred too long

4. QUESTIONS TO ASK
   - Check-in questions (how are they doing)
   - Project-specific questions
   - Growth/development questions

5. THINGS TO REMEMBER
   - Personal context (things they mentioned previously)
   - Sensitivities to be aware of
   - Recognition or positive feedback due

Keep the agenda flexible—this is a conversation, not a checklist.
```

---

### Step 4: During the Meeting
**Time: The meeting duration**

Use the agenda as a guide, not a script:
- Start with genuine check-in
- Let them drive topics where appropriate
- Cover the priority items
- Leave space for what emerges
- Note any new action items

**Quick Capture:** Jot notes as you go, or immediately after.

---

### Step 5: Post-Meeting Documentation
**Time: 3-5 minutes**

Immediately after (or within an hour), document:

---

**POST-MEETING PROMPT: 1:1 Documentation**

```
Please help me document today's 1:1 with [NAME].

WHAT WE DISCUSSED:
"""
[YOUR RAW NOTES FROM THE MEETING - can be messy]
"""

Please organize into:

1. MEETING SUMMARY (2-3 sentences)
   - Key themes discussed
   - Overall tone/vibe of the conversation

2. ACTION ITEMS
   - For them: [Task] - [Due date if set]
   - For me: [Task] - [Due date if set]

3. KEY DECISIONS/AGREEMENTS
   - What was decided
   - What was agreed to

4. FOLLOW-UP TOPICS
   - What to check on next time
   - Topics to continue

5. NOTES TO SELF
   - Important context to remember
   - Development areas to support
   - Concerns to monitor

Save to my running notes for [NAME].
```

---

### Step 6: Maintain Running Notes
**Time: 1 minute**

Append to a running document for each person:

```
Add today's notes to the running 1:1 log for [NAME]. Keep the last 6 meetings accessible; archive older ones.
```

---

## Example Output

Below is an abbreviated pre-meeting agenda example:

---

> **1:1 PREP: Sarah Chen | January 8, 2024 | 30 minutes**
>
> ---
>
> **SUGGESTED AGENDA**
>
> | Time | Topic | Type |
> |------|-------|------|
> | 0-5 min | Check-in: How are you doing? | Connection |
> | 5-10 min | Action item follow-up | Accountability |
> | 10-20 min | API project demo prep + tech lead discussion | Substance |
> | 20-25 min | Her topics | Their agenda |
> | 25-30 min | Wrap-up + action items | Closure |
>
> ---
>
> **ACTION ITEM FOLLOW-UP**
>
> *From Sarah:*
> - [ ] Architecture doc was due Friday Dec 15 — **Needs follow-up** (hasn't been received)
>
> *From Me:*
> - [ ] Talk to Product manager about response time — **Done** (update her on outcome)
> - [ ] Share tech lead role description — **Not done** (apologize, commit to date)
>
> ---
>
> **SUGGESTED DISCUSSION TOPICS**
>
> Based on previous meetings:
> 1. **Burnout recovery** — She mentioned feeling burned out Dec 15. Check in on how holidays went and current energy levels. This is important—she's a high performer at risk.
>
> 2. **Tech lead aspirations** — She's expressed interest twice now. Time to have a substantive conversation about timeline and development areas.
>
> 3. **Product team friction** — This has come up 3 times. Worth exploring if there's a systemic issue or specific relationship to address.
>
> ---
>
> **QUESTIONS TO ASK**
>
> Check-in:
> - "How are you feeling coming back from the holidays?"
> - "What's your energy level like right now?"
>
> Project:
> - "How did the API demo prep go?"
> - "Any surprises or blockers?"
>
> Development:
> - "You've mentioned tech lead a couple times. Can we talk about what that path might look like?"
> - "What skills do you feel you'd want to develop to get there?"
>
> ---
>
> **REMEMBER**
>
> - She mentioned being burned out last time—take this seriously
> - Conference attendance was a topic for "next time" (Dec 15)—bring it up
> - She appreciates direct feedback—don't sugarcoat
> - Outstanding work on API project—make sure to recognize this

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| No previous notes to reference | Starting fresh | Create simple template; commit to noting 3-5 points after each 1:1 |
| Action items always lost | Not documented clearly | End each 1:1 by verbally confirming action items; document immediately |
| Same topics repeat endlessly | Not resolving underlying issues | Ask Claude to flag items discussed 3+ times; make them priority to actually resolve |
| Too much status, not enough development | Agenda imbalance | Explicitly block "development" time in agenda; status can be async |
| Feels too formal/scripted | Over-reliance on agenda | Use prep as input, not script; be present in actual conversation |
| Notes too detailed/burdensome | Over-documenting | Keep notes to action items + 3-5 key points; not a transcript |

---

## Tips from Experience

1. **Prepare, but don't over-script.** The agenda is a starting point. Be present enough to follow what matters in the moment.

2. **Their agenda first.** Ask "What's on your mind?" and let them start. Your items can wait; theirs can't.

3. **Document immediately.** Notes from 30 minutes ago are accurate. Notes from "later today" are fiction.

4. **Action items are sacred.** If you commit to something, do it. If you don't, apologize and recommit. Credibility is built here.

5. **Watch for patterns.** Claude can help you see themes you miss: "This is the 4th time Sarah has mentioned product team friction."

6. **Development should be intentional.** If every 1:1 is status updates, you're not developing your people. Block time for growth conversations.

7. **Share your notes (selectively).** Consider sharing a summary with your report after each 1:1. It builds accountability both ways.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Every 1:1 has clear action items that actually get done
- [ ] Conversations build on previous discussions (continuity)
- [ ] Development topics get regular airtime, not just crisis management
- [ ] Your direct reports feel heard and supported
- [ ] You can recall key context without scrambling

**Track over time:**
- Action item completion rate (yours and theirs)
- Balance of topic types (status vs. development vs. their agenda)
- Direct report feedback on 1:1 quality

---

## Variations

### Skip-Level 1:1 Prep
For meetings with your reports' reports:
```
This is a skip-level 1:1 with [name], who reports to [their manager].

Goals for skip-levels:
- Ensure they have visibility to senior leadership
- Get unfiltered perspective on team dynamics
- Identify issues their manager might not surface
- Discuss career and growth from broader perspective

Previous skip-level notes: [paste]

Generate an agenda that:
- Opens with genuine interest in their experience
- Includes questions about team health and their manager
- Explores career development
- Avoids undermining their direct manager
- Creates psychological safety for honest feedback
```

### First 1:1 with New Report
For establishing the relationship:
```
This is my first 1:1 with [name]. They are a [new hire / transferred from X].

My goals for this first meeting:
- Begin building trust and relationship
- Understand their working style and preferences
- Set expectations for our 1:1s
- Learn about their background and aspirations

Create an agenda and question list for a "get to know you" 1:1 that establishes a strong foundation.
```

### Difficult Conversation Prep
When you need to address a serious issue:
```
I need to have a difficult conversation in today's 1:1 about [issue].

Context:
- What happened: [specific situation]
- Impact: [why it matters]
- Previous feedback on this: [if any]
- Outcome I need: [what needs to change]

Help me prepare:
1. Opening that's direct but not attacking
2. Key points to make clearly
3. Questions to understand their perspective
4. Path forward I can propose
5. How to handle likely reactions

This should be supportive and developmental, not punitive.
```

### Career Development Focus
For dedicated growth conversations:
```
This 1:1 is focused on [name]'s career development.

Their current role: [role]
Time in role: [duration]
Stated aspirations: [what they've said they want]
My assessment of their readiness: [your view]

Create a career development conversation guide that:
- Explores their aspirations deeply
- Assesses their self-awareness of strengths/gaps
- Discusses realistic timelines and paths
- Identifies concrete development actions
- Creates mutual accountability
```

---

## Building Your Repeatable System

After a few weeks of consistent 1:1s, establish your system:

1. **Create a running doc per person** that accumulates over time
2. **Set a prep reminder** 30 minutes before each 1:1
3. **Build a post-meeting habit** of documenting within 1 hour
4. **Review patterns quarterly** using the accumulated notes
5. **Share summaries appropriately** to build mutual accountability

**Sample Setup:**
```
one-on-ones/
├── templates/
│   ├── prep-prompt.txt
│   └── post-meeting-prompt.txt
├── sarah-chen/
│   ├── running-notes.md
│   └── career-discussion-oct-2024.md
├── alex-jones/
│   └── running-notes.md
└── skip-levels/
    └── [name]/
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**gather context → prepare thoughtfully → document outcomes → build continuity**—applies broadly:

| Role | Application |
|------|-------------|
| **Managers** | All direct report 1:1s |
| **Executives** | Leadership team check-ins, board member conversations |
| **Account Managers** | Regular client touchpoints |
| **Mentors** | Mentee sessions |
| **Project Leads** | Stakeholder check-ins |
| **Anyone** | Regular meetings where continuity matters |

---

## Next Steps

1. **This week:** Use this recipe for one 1:1—see the difference preparation makes
2. **Create your running docs:** Start maintaining notes for each direct report
3. **Build the habit:** Set calendar reminders for prep and documentation
4. **Check your balance:** After a month, review if development gets enough time vs. status

---

*Recipe #14 of 100 in the Claude Code Knowledge Worker Recipe Collection*
