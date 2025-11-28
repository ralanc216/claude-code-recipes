# High-Stakes Communication Drafting

**Recipe #12: From Difficult Messages to Polished Delivery**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 5 minutes (first time) / 2 minutes (repeat) | 1-3 hours per message | Intermediate | Executives, HR, Legal, Communications, Managers |

---

## The Problem

Some communications carry significant weight—layoff announcements, customer escalation responses, regulatory correspondence, investor updates, crisis communications, or sensitive feedback. These require careful wordsmithing: clear enough to be understood, diplomatic enough to maintain relationships, and precise enough to avoid misinterpretation. You agonize over every sentence, often through multiple drafts and reviewers.

**Pain Points:**
- High stakes create writer's block and procrastination
- Multiple drafts consume hours
- Finding the right tone is challenging
- Legal, HR, and leadership all have different concerns
- Rushing leads to costly mistakes
- The emotional weight makes objective writing difficult

---

## The Outcome

Polished draft communications that hit the right tone, address multiple stakeholder concerns, and maintain appropriate formality—produced in minutes instead of hours. You review and refine rather than write from scratch, reducing both time and emotional burden.

**What You'll Have When Done:**
- Well-crafted initial draft for any sensitive communication
- Multiple tone variations to choose from
- Anticipated objections and responses addressed
- Version history for iteration
- Confidence in your message before sending

---

## When to Use This Recipe

**Good Fit:**
- Personnel changes (layoffs, terminations, role changes)
- Customer escalations requiring executive response
- Regulatory or legal correspondence
- Crisis communications
- Investor relations updates
- Difficult feedback delivery
- Apologies and service recovery
- Change announcements (policy, org structure, benefits)

**Not a Good Fit:**
- Routine communications (overkill)
- Personal messages where authentic voice matters most
- Situations requiring real-time verbal communication
- Content requiring legal review before drafting (get input first)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You know the key message you need to deliver
- [ ] You know the audience and their likely concerns
- [ ] You understand any legal or compliance constraints
- [ ] You have any required messaging points or restrictions
- [ ] You have 15-30 minutes for drafting and refinement

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Generates diplomatic language for difficult messages
- Balances clarity with sensitivity
- Creates multiple tone variations
- Anticipates reader reactions and concerns
- Maintains consistency across drafts
- Identifies potentially problematic phrasing

**Where Human Judgment Is Essential:**
- Final approval of messaging and tone
- Adding personal touches that convey authenticity
- Understanding political and relationship nuances
- Deciding what can/cannot be said (legal, policy)
- Timing and delivery method decisions
- Verifying factual accuracy

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Key facts | What happened, what's changing | Core message content |
| Audience info | Who's receiving, their concerns | Tone calibration |
| Constraints | What can't be said, legal limits | Guardrails |
| Desired outcome | What you want reader to feel/do | Message shaping |
| Examples | Previous communications, style samples | Voice matching |

**Sample Context (What You Might Provide):**
```
Need to communicate: We're eliminating the QA team (6 people) due to shift to automated testing.

Facts:
- Effective date: March 1
- Severance: 3 months + benefits continuation
- Outplacement services provided
- This decision is final, not open for discussion

Audience: The 6 affected employees (individual meetings), then broader engineering team

Concerns I need to address:
- Why them, why now
- Is this the start of broader layoffs (no)
- What support they'll receive
- How to handle transition

Tone: Compassionate but clear. Not apologetic to the point of undermining the decision.
```

---

## Step-by-Step Implementation

### Step 1: Clarify Your Message
**Time: 5 minutes**

Before drafting, write down:
- What are the key facts?
- What is the audience's likely emotional response?
- What do you want them to understand/feel/do?
- What can't you say? (legal, policy, premature)
- What must you say? (required disclosures, policy language)

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the High-Stakes Communication Prompt
**Time: 3-5 minutes for Claude to process**

---

**PRIMARY PROMPT: High-Stakes Communication Generator**

```
Please help me draft a sensitive communication.

SITUATION:
[Describe what happened or what you need to communicate]

AUDIENCE:
- Who: [e.g., Affected employees, all staff, customers, investors]
- Their likely concerns: [List what they'll worry about]
- Relationship context: [e.g., Long-tenured team members, key customer]

KEY MESSAGES THAT MUST BE CONVEYED:
- [Message 1]
- [Message 2]
- [Message 3]

TONE REQUIREMENTS:
- Primary tone: [e.g., Compassionate but clear, Professional and direct, Apologetic but confident]
- Must avoid: [e.g., Blame, excessive apology, vague language]
- Formality level: [Formal / Professional / Conversational]

CONSTRAINTS:
- Cannot say: [Any messaging restrictions]
- Must include: [Any required language or disclosures]
- Legal/policy considerations: [Note any]

DESIRED OUTCOME:
After reading this, the recipient should:
- Understand: [What facts should be clear]
- Feel: [What emotional response is appropriate]
- Do: [What action, if any, should they take]

PLEASE PROVIDE:

1. RECOMMENDED STRUCTURE
   - Opening approach
   - Key message sequence
   - Closing approach

2. DRAFT COMMUNICATION
   - Complete draft ready for review
   - Clear paragraphs with logical flow
   - Appropriate length for the medium [email / letter / announcement / script]

3. TONE VARIATIONS (brief alternatives)
   - Version A: [More direct]
   - Version B: [More empathetic]
   - Note which you recommend and why

4. ANTICIPATED QUESTIONS/REACTIONS
   - What questions might this generate?
   - Suggested responses for each

5. RED FLAGS TO WATCH
   - Any phrases that could be misinterpreted
   - Areas that might need legal review
   - Potential emotional triggers
```

---

### Step 4: Review for Fit
**Time: 5-10 minutes**

Review Claude's draft against your needs:

**Message accuracy:**
- Are all key facts correct?
- Is anything said that shouldn't be?
- Is anything missing that must be included?

**Tone check:**
- Read it aloud—does it sound like something you'd say?
- Is it appropriately warm/direct for this audience?
- Are there any phrases that feel wrong?

**Reaction prediction:**
- How would YOU feel receiving this?
- What follow-up questions would you have?

---

### Step 5: Refine Iteratively
**Time: 5-15 minutes**

**To soften the message:**
```
The second paragraph feels too harsh. Soften the language while keeping the message clear. Acknowledge the emotional impact more directly.
```

**To strengthen the message:**
```
This is too wishy-washy. Make it clear that this decision is final and not open for negotiation, while remaining respectful.
```

**To add personal touches:**
```
Add a sentence acknowledging the specific contributions this team has made. I want them to know their work mattered.
```

**To address concerns preemptively:**
```
People will wonder if more layoffs are coming. Add a sentence that honestly addresses broader job security without making promises we can't keep.
```

**To adjust for different audiences:**
```
Now create a version of this announcement for the broader company. They need to understand what's happening without the personal details.
```

---

### Step 6: Finalize and Route
**Time: 2-5 minutes**

Save your drafts:
```
Save this as "QA-Team-Communication-Draft-v1.md"
```

For review process:
```
Create a summary of this communication with key messages and sensitive areas flagged, suitable for sending to Legal/HR for review.
```

---

## Example Output

Below is an abbreviated example for a team restructuring:

---

> **RECOMMENDED STRUCTURE**
>
> 1. Open with respect and direct statement of news
> 2. Explain the "why" (business context)
> 3. Acknowledge the personal impact
> 4. Detail the support being provided
> 5. Set clear next steps
> 6. Close with genuine appreciation
>
> ---
>
> **DRAFT COMMUNICATION**
>
> Subject: Important Update Regarding Your Role
>
> [Name],
>
> I want to speak with you directly about a difficult decision that affects your position at [Company]. Effective March 1, we are eliminating the Quality Assurance team as part of our transition to automated testing infrastructure. This means your role will be ending on that date.
>
> I want to be clear: this decision reflects a fundamental change in how we approach quality engineering, not a reflection of your work or contributions. Our move to test automation reduces the need for manual QA resources, and we've made the difficult decision to restructure accordingly.
>
> I know this news is hard to receive, and I don't want to minimize its impact. You've contributed meaningful work during your time here, and this transition doesn't change that.
>
> We are committed to supporting you through this change:
> - Severance: 3 months of base salary
> - Benefits: Medical and dental continuation through June 1
> - Outplacement: Professional career transition services through [Provider]
> - Reference: Strong professional references from leadership
>
> [HR Contact] will meet with you this afternoon to review all details and answer questions about logistics. I'm also available to speak with you directly about anything you'd like to discuss.
>
> I'm sorry to deliver this news and genuinely grateful for your contributions to the team.
>
> [Your name]
>
> ---
>
> **TONE VARIATIONS**
>
> *Version A (More Direct):* Opens with "I have difficult news to share" - gets to the point faster, appropriate for direct-communicator audiences.
>
> *Version B (More Empathetic):* Adds more acknowledgment of emotions upfront - "I know you'll have many feelings about this news, and I want you to know they're valid."
>
> *Recommendation:* The primary draft balances both. Choose Version A for employees who prefer directness; Version B for longer-tenured or more emotionally expressive team members.
>
> ---
>
> **ANTICIPATED QUESTIONS**
>
> *Q: Is this the start of larger layoffs?*
> A: "This change is specific to the QA function and our shift to automated testing. We don't anticipate broader workforce reductions as a result of this initiative."
>
> *Q: Why wasn't I offered another role?*
> A: "We explored internal placement options but don't currently have open roles that match your experience. If something opens up during your notice period, we'll absolutely consider you."
>
> *Q: What if I find a new job before March 1?*
> A: "We'll work with you on transition timing. Your severance is guaranteed regardless of your end date."

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Too formal/corporate | Default professional tone | Ask: "Make this sound more human and less like HR boilerplate" |
| Too soft, lacks clarity | Over-indexed on empathy | Ask: "The core message is getting lost. Make it clearer while staying compassionate" |
| Missing required language | Constraints weren't specified | Add: "We must include this exact severance language: [paste required text]" |
| Doesn't sound like you | No voice sample provided | Provide: "Here's how I typically write: [example]. Match this voice" |
| Raises more questions than answers | Gaps in the information | Ask: "What questions would this leave unanswered? Add content to address them" |
| Legal concern | Potentially problematic phrasing | Ask: "Flag any language that might create legal risk and suggest safer alternatives" |

---

## Tips from Experience

1. **Get the facts nailed down first.** Sensitive communications suffer when facts are fuzzy. Clarify what's true before crafting how to say it.

2. **Write for the angriest reader.** Assume your most skeptical, upset recipient. If the message works for them, it works for everyone.

3. **Read it aloud.** High-stakes communications must flow naturally. If you stumble reading it, rewrite.

4. **Don't over-apologize.** One clear acknowledgment of impact is more powerful than repeated apologies that dilute the message.

5. **Plan for the Q&A.** The communication itself is half the work. Prepare for the questions it will generate.

6. **Sleep on major communications.** If time allows, draft today, finalize tomorrow. Fresh eyes catch issues.

7. **Have the right reviewers.** Know who must see it (legal, HR, leadership) vs. who might wordsmith it to death.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] First draft captures 80%+ of the final message
- [ ] Revision cycles decrease significantly
- [ ] Recipients respond as anticipated
- [ ] No significant miscommunications or backlash
- [ ] You feel confident before hitting send

**Track over time:**
- Time from "need to write" to "ready to send"
- Number of revision cycles
- Post-communication feedback and reactions

---

## Variations

### Crisis Communication
For urgent situations requiring immediate response:
```
This is a crisis situation. [Describe what happened]

I need to communicate to [audience] within [timeframe].

Key constraints:
- We don't yet know: [what's still unclear]
- We can confirm: [what's verified]
- We're doing: [actions being taken]

Create a holding statement that:
- Acknowledges the situation
- Shows we're taking it seriously
- Commits to follow-up communication
- Doesn't speculate or admit fault prematurely
```

### Apology/Service Recovery
For apologizing to customers or stakeholders:
```
We need to apologize for [what went wrong].

Context:
- What happened: [facts]
- Impact on them: [how they were affected]
- What we're doing about it: [remediation]

Tone: Genuine apology without excessive groveling. Own it, fix it, rebuild trust.

Include: What we're doing to prevent recurrence. Don't include: Excuses or blame-shifting.
```

### Org Change Announcement
For communicating restructuring or changes:
```
We're announcing [org change/new structure/new leadership].

Audience needs to understand:
- What's changing
- Why (honest business rationale)
- How it affects them
- Timeline
- Who to ask questions

Create versions for:
1. All-company announcement
2. Direct manager talking points
3. FAQ document
```

### Negative Feedback/Performance Communication
For difficult performance conversations:
```
I need to communicate performance concerns to [employee].

The issues:
- [Specific behavior/performance gap 1]
- [Specific behavior/performance gap 2]

What I need them to understand:
- This is serious but not (yet) terminal
- Specific expectations going forward
- Support available
- Consequences if no improvement

Tone: Direct and clear, but not punitive. Focus on future improvement, not past failures.
```

---

## Building Your Repeatable System

After using this for several sensitive communications, establish your system:

1. **Create a communication template library** for common scenarios
2. **Document your organization's required language** (severance terms, legal disclaimers, etc.)
3. **Build an approval workflow** knowing who reviews what
4. **Maintain a "lessons learned" doc** from past communications
5. **Save successful communications** as examples for future reference

**Sample Setup:**
```
high-stakes-comms/
├── templates/
│   ├── personnel-change.txt
│   ├── crisis-response.txt
│   ├── customer-apology.txt
│   └── org-announcement.txt
├── required-language/
│   ├── severance-terms.txt
│   └── legal-disclaimers.txt
├── examples/
│   ├── successful-comms/
│   └── lessons-learned.md
└── review-checklist.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**define constraints → generate calibrated draft → refine through iteration**—applies broadly:

| Role | Application |
|------|-------------|
| **HR** | Performance communications, policy rollouts, terminations |
| **Legal** | Settlement communications, regulatory responses |
| **Executives** | Investor updates, board communications, company announcements |
| **Customer Success** | Escalation responses, contract negotiations |
| **PR/Comms** | Media statements, crisis response, public announcements |
| **Managers** | Difficult feedback, team restructuring, change communication |

---

## Next Steps

1. **Next difficult message:** Use this recipe instead of staring at a blank screen
2. **Build your template library:** Save prompts for communications you send repeatedly
3. **Document required language:** Create a file with any standard verbiage your org requires
4. **Practice on medium-stakes:** Build confidence before using on highest-stakes situations

---

*Recipe #12 of 100 in the Claude Code Knowledge Worker Recipe Collection*
