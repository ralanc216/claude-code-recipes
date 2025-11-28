# Meeting Facilitation Planning

**Recipe #19: From Chaotic Meetings to Productive Sessions**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 10 minutes (first time) / 5 minutes (repeat) | 30-45 minutes per meeting | Beginner | Anyone who runs meetings |

---

## The Problem

You're responsible for running a meeting, but you haven't thought through how to actually facilitate it. You start with "so, what should we discuss?" and the meeting meanders. Important topics get rushed at the end. The loudest voices dominate. You leave without clear decisions or next steps. The meeting was held, but nothing was really accomplished.

**Pain Points:**
- Meetings without clear purpose or outcomes
- Important topics rushed or skipped
- Dominant voices crowding out others
- No clear decisions by meeting end
- Running over time consistently
- Participants feeling like meetings are a waste

---

## The Outcome

A complete facilitation plan with timed agenda, discussion questions, decision frameworks, and techniques for managing participation. Your meetings have clear outcomes, stay on time, and everyone contributes. Participants leave knowing what was decided and what's next.

**What You'll Have When Done:**
- Clear meeting objective and success criteria
- Timed agenda with facilitation notes
- Discussion questions that drive progress
- Techniques for managing the room
- Decision frameworks for reaching conclusions
- Clear next steps and accountability

---

## When to Use This Recipe

**Good Fit:**
- Strategy or planning sessions
- Decision-making meetings
- Workshops and working sessions
- Team retrospectives
- Cross-functional alignment meetings
- Any meeting you're facilitating (not just attending)

**Not a Good Fit:**
- Simple status updates (just share async)
- 1:1 conversations (different dynamic)
- Meetings you're not facilitating
- Informal brainstorming (can be too structured)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You know the meeting's purpose and desired outcome
- [ ] You know who's attending and their roles
- [ ] You know how much time you have
- [ ] You have any pre-work or materials to reference
- [ ] You have 10-15 minutes for planning

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Structures agendas with appropriate time allocation
- Generates discussion questions that drive outcomes
- Suggests facilitation techniques for different situations
- Creates decision frameworks
- Anticipates challenges and suggests mitigations
- Produces meeting materials ready to use

**Where Human Judgment Is Essential:**
- Knowing the actual dynamics in the room
- Reading energy and adjusting in real-time
- Managing difficult personalities
- Making judgment calls on when to go deeper or move on
- Being present in the meeting itself

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Meeting purpose | "Decide on Q2 priorities" | Outcome focus |
| Attendees | List with roles | Participation planning |
| Time available | 60 minutes | Time allocation |
| Pre-work | Materials sent in advance | Building on preparation |
| Past context | Previous meetings, history | Continuity |

**Sample Input:**
```
Meeting to plan: Q2 Product Roadmap Prioritization

Purpose: Decide which features to include in Q2 (we have 10 candidates, can do ~5)

Attendees:
- Me (VP Product) - facilitating
- Sarah (Head of Engineering) - capacity perspective
- Mike (VP Sales) - customer/revenue perspective
- Lisa (Head of Customer Success) - user feedback perspective
- Tom (CEO) - strategic alignment

Time: 90 minutes
Where: Conference room, hybrid (Tom is remote)

Pre-work: Everyone has seen the feature candidates list with effort estimates

Challenges:
- Mike tends to push for whatever customers are asking for NOW
- Sarah and Mike often clash on priorities
- Tom sometimes takes over the meeting
- We've struggled to actually decide in past meetings (end up deferring)
```

---

## Step-by-Step Implementation

### Step 1: Clarify the Meeting Outcome
**Time: 3 minutes**

Before planning the agenda, get clear on:
- What's the ONE outcome we must achieve?
- What does success look like at meeting end?
- What will we have decided or produced?

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Facilitation Planning Prompt
**Time: 3-5 minutes for Claude to process**

---

**PRIMARY PROMPT: Meeting Facilitation Planning**

```
Help me plan and facilitate an effective meeting.

MEETING BASICS:
- Purpose: [What's this meeting for?]
- Desired outcome: [What must we achieve?]
- Duration: [How long?]
- Format: [In-person / Hybrid / Virtual]

ATTENDEES:
- [Name, Role, Their perspective/interest]
- [Name, Role, Their perspective/interest]
- ...

PRE-WORK:
[What have attendees already received/prepared?]

KNOWN CHALLENGES:
[Any dynamics, personalities, or patterns to manage]

PLEASE CREATE:

1. MEETING DESIGN
   - Clear objective (one sentence)
   - Success criteria (how we know the meeting worked)
   - Meeting type/approach (decision-making, brainstorming, alignment, etc.)

2. TIMED AGENDA
   For each segment:
   | Time | Topic | Purpose | Facilitation approach |
   Include buffer time and realistic timing

3. FACILITATION GUIDE
   For key segments, provide:
   - How to open/frame the discussion
   - Questions to ask
   - How to drive toward conclusion
   - Techniques for managing participation

4. DISCUSSION QUESTIONS
   - Opening question to get engagement
   - Probing questions to go deeper
   - Decision-framing questions to drive closure
   - Questions to surface unstated concerns

5. DECISION FRAMEWORK
   - How we'll actually make the decision
   - Criteria for evaluation (if applicable)
   - What to do if we can't reach consensus
   - How to document and communicate the decision

6. PARTICIPATION MANAGEMENT
   - How to draw out quieter voices
   - How to manage dominant participants
   - Specific techniques for [known challenges you mentioned]

7. BACKUP PLANS
   - If discussion runs long: what to cut
   - If we can't decide: what's the fallback
   - If key person dominates: intervention approach

8. MEETING MATERIALS
   - Agenda to share with attendees
   - Any frameworks or templates to use in the meeting
```

---

### Step 4: Review and Customize
**Time: 5-10 minutes**

Review the facilitation plan for:

**Timing:**
- Is the time allocation realistic?
- Where's the buffer for inevitable overrun?

**Flow:**
- Does the agenda build logically?
- Is there warm-up before hard decisions?

**Dynamics:**
- Does the plan address the specific challenges you mentioned?
- Are there participation strategies for known personalities?

---

### Step 5: Refine for Your Context
**Time: 5 minutes**

**To address specific dynamics:**
```
Tom (CEO) tends to take over discussions. Add specific techniques for respectfully containing his input while still honoring his perspective as CEO.
```

**To strengthen decision-making:**
```
We always end up deferring decisions. Make the decision framework stronger—add a "must decide today" forcing function and specify what happens if we don't agree.
```

**To improve participation:**
```
Lisa is quiet but has valuable CS insights. Add a segment where she specifically presents the customer perspective before open discussion.
```

**To adjust timing:**
```
The prioritization discussion feels too short. Reduce the opening from 15 minutes to 10 and give prioritization an extra 10 minutes.
```

---

### Step 6: Prepare Final Materials
**Time: 3 minutes**

```
Create the final deliverables:
1. Clean agenda I can share with attendees (just time/topic/purpose)
2. My facilitation notes (detailed, for my eyes only)
3. Decision capture template I can fill in during the meeting
4. Follow-up email template for after the meeting
```

---

## Example Output

Below is an abbreviated facilitation plan example:

---

> **MEETING DESIGN**
>
> **Objective:** Decide which 5 of the 10 feature candidates will be in the Q2 product roadmap.
>
> **Success criteria:**
> - We leave with an agreed, prioritized list of 5 features
> - Engineering has validated capacity fit
> - Sales/CS perspectives have been heard and incorporated
> - CEO has blessed the direction
> - Everyone understands the "why" behind priorities
>
> ---
>
> **TIMED AGENDA**
>
> | Time | Min | Topic | Purpose |
> |------|-----|-------|---------|
> | 0:00 | 5 | Opening | Set context, confirm outcome |
> | 0:05 | 10 | Stakeholder perspectives | Each voice shares priorities |
> | 0:15 | 30 | Feature scoring | Apply criteria to candidates |
> | 0:45 | 25 | Prioritization discussion | Debate and decide |
> | 1:10 | 10 | Capacity validation | Engineering confirms feasibility |
> | 1:20 | 10 | Decisions and next steps | Document and assign |
>
> ---
>
> **FACILITATION GUIDE: Key Segments**
>
> **Stakeholder Perspectives (5:00-15:00)**
>
> *Purpose:* Get all perspectives on the table before discussion, ensuring quieter voices are heard.
>
> *Technique:* Round-robin, 2 minutes each
>
> *Frame it as:*
> "Before we dig into the list, I'd like each of you to share your top priority and why. This helps us understand what we're optimizing for. Mike, you're closest to revenue—start us off. Two minutes, then I'll move to Lisa."
>
> *Containment for Tom:*
> "Tom, you'll go last so you can reflect on what you've heard. I'll give you a bit more time to react and add strategic context."
>
> ---
>
> **DISCUSSION QUESTIONS**
>
> *Opening (to get engagement):*
> "Looking at this list, what's the one feature you think is most obviously a Q2 priority—and why?"
>
> *Probing (to go deeper):*
> "Mike, when you say customers are asking for this—how many customers, and what's the revenue at risk if we don't do it?"
>
> *Decision-framing (to drive closure):*
> "We've heard strong cases for both Feature A and Feature E, but we can only do one. What would change your mind on this?"
>
> *Surfacing concerns (for unstated issues):*
> "Before we lock this in—what's the thing we might regret about this list in June?"
>
> ---
>
> **DECISION FRAMEWORK**
>
> **How we'll decide:**
> 1. Score each feature on: Revenue impact / Customer value / Strategic fit / Effort
> 2. Stack-rank based on scores
> 3. Engineering validates top 5 fit capacity
> 4. Adjust if capacity doesn't work
> 5. CEO blesses or raises concerns
> 6. Final list is DECIDED in this meeting
>
> **If we can't agree:**
> - Reduce to the features everyone agrees on (probably 3-4)
> - VP Product makes call on remaining 1-2 with input heard
> - We do NOT leave without a decided list
>
> ---
>
> **PARTICIPATION MANAGEMENT**
>
> **For Mike (tends to push current customer asks):**
> "Mike, I hear the urgency from customers. Help us understand—is this 'nice to have' or 'lose the deal'? Let's separate the urgent from the critical."
>
> **For Tom (CEO may dominate):**
> Structure has Tom going last in round-robin. If he starts taking over:
> "Tom, great point. Let me make sure we get the other perspectives before we converge—Lisa, how does that square with what you're hearing from customers?"
>
> **For Lisa (quiet but valuable):**
> Give her dedicated time: "Lisa, you have the pulse on how customers actually use the product. What would make the biggest difference in their daily experience?"

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Meeting ran over time | Over-ambitious agenda | Build in 20% buffer; know what to cut |
| Didn't reach decision | No forcing mechanism | Add: "We will decide today. Here's the tiebreaker if needed." |
| One person dominated | No participation structure | Use round-robin, time limits, and redirect techniques |
| Quiet people didn't speak | Open discussion favors talkers | Call on them specifically; use written input before verbal |
| Discussion meandered | Weak facilitation | Use questions to redirect: "How does this relate to our decision?" |
| People left unclear | No explicit closure | End with: "Let me confirm what we decided..." |

---

## Tips from Experience

1. **Name the outcome upfront.** Start with "We're here to decide X. At 2:30, we'll have decided." This sets expectations.

2. **Silence is your friend.** After asking a question, wait. Count to 10 in your head. Someone will fill the silence.

3. **Write things down visibly.** Use a whiteboard or shared doc. Writing forces clarity and creates shared record.

4. **Time-box ruthlessly.** "We have 5 more minutes on this topic" is a powerful phrase.

5. **Park tangents visibly.** When discussion goes off-track, say "Important point—adding to the parking lot. Let's return to X."

6. **Check for commitment.** "Can everyone support this decision?" is different from "Does anyone object?"

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Meetings end with clear decisions
- [ ] All voices are heard, not just the loudest
- [ ] Participants feel their time was well-spent
- [ ] Action items have owners and deadlines
- [ ] Meetings end on time (or early!)

**Track over time:**
- Decision rate (% of decision meetings that actually decide)
- Participant feedback on meeting effectiveness
- Time spent in meetings vs. outcomes achieved

---

## Variations

### Strategy Workshop
For longer strategic sessions:
```
Design a 3-hour strategy workshop for:
[Topic and attendees]

Include:
- Multiple segments with different modalities (individual, small group, full group)
- Energy management (when to break, when to change pace)
- Visual outputs/artifacts we'll create
- Synthesis and decision points
- Both divergent (explore options) and convergent (make choices) phases
```

### Retrospective Facilitation
For team retros:
```
Design a team retrospective for:
- Team size: [X people]
- Duration: [time]
- Focus: [sprint/project/period]

Include:
- Safe space creation
- Data gathering (what happened)
- Insight generation (why did it happen)
- Decision making (what to change)
- Specific techniques to surface issues without blame
```

### Conflict Resolution Meeting
For addressing team conflict:
```
Design a meeting to address conflict between [parties].

The issue: [description]
Stakes: [what happens if unresolved]

Include:
- Ground rules for productive dialogue
- Structure for each party to share perspective
- Questions that seek to understand, not assign blame
- Framework for finding common ground
- Path to resolution or next steps

Tone: Constructive, not judicial.
```

### Executive Decision Meeting
For high-stakes decisions with senior leaders:
```
Design an executive decision meeting for:
- Decision: [what we're deciding]
- Attendees: [C-suite members]
- Duration: [time]
- Pre-work: [what they've already seen]

These executives are time-constrained and impatient with process.
Include:
- Minimal process, maximum substance
- Clear recommendation with options
- Efficient path to decision
- Appropriate authority acknowledgment
- Clear outcome documentation
```

---

## Building Your Repeatable System

After facilitating several meetings, establish your system:

1. **Create meeting type templates** for your common meeting types
2. **Build a facilitation technique library** with go-to approaches
3. **Develop standard agendas** for recurring meetings
4. **Create a pre-meeting checklist** to ensure consistent prep
5. **Document lessons learned** from successful and failed meetings

**Sample Setup:**
```
meeting-facilitation/
├── templates/
│   ├── decision-meeting.txt
│   ├── strategy-workshop.txt
│   ├── retrospective.txt
│   └── alignment-meeting.txt
├── techniques/
│   ├── participation-techniques.md
│   └── decision-frameworks.md
├── past-meetings/
│   └── [meeting notes and learnings]
└── checklists/
    └── pre-meeting-prep.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**clarify outcome → design structure → plan facilitation → prepare materials**—applies broadly:

| Role | Application |
|------|-------------|
| **Executives** | Board meetings, leadership offsites |
| **Managers** | Team meetings, planning sessions |
| **Product** | Sprint planning, stakeholder reviews |
| **Consultants** | Client workshops, discovery sessions |
| **HR** | Training sessions, focus groups |
| **Anyone** | Any meeting you're responsible for running |

---

## Next Steps

1. **Next meeting you run:** Use this recipe to prepare
2. **Try one new technique:** Pick a participation technique you haven't used
3. **Solicit feedback:** After the meeting, ask participants how it went
4. **Iterate:** Adjust your approach based on what worked

---

*Recipe #19 of 100 in the Claude Code Knowledge Worker Recipe Collection*
