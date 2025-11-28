# Email Drafting and Response Management

**Recipe #3: From Inbox Overload to Efficient Communication**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 5 minutes (first time) / 1 minute (repeat) | 1-2 hours per day | Beginner | All professionals with high email volume |

---

## The Problem

Email is essential but overwhelming. Complex responses require careful thought and multiple drafts. Simple responses pile up. Striking the right tone—especially for sensitive topics—takes time. You spend hours crafting messages when you should be doing actual work, or you let emails pile up because responding feels like a chore.

**Pain Points:**
- Complex emails require multiple drafts to get tone right
- Simple replies still take mental energy to compose
- Sensitive topics require careful wordsmithing
- Pile-up creates anxiety and missed responses
- Different audiences require different communication styles

---

## The Outcome

Polished email drafts generated in seconds that you refine and send. Complex responses that would take 20 minutes now take 3. Your communication is clearer, more professional, and consistent—without the mental drain of composing everything from scratch.

**What You'll Have When Done:**
- Ready-to-send email drafts requiring only light editing
- Appropriate tone for each recipient and context
- Consistent professional communication quality
- Time back for work that matters
- Reduced email anxiety and backlog

---

## When to Use This Recipe

**Good Fit:**
- Complex replies requiring careful framing
- Sensitive communications (feedback, escalations, apologies)
- Formal emails to executives, clients, or partners
- Batch processing multiple similar responses
- Emails you've been procrastinating on because they're hard to write

**Not a Good Fit:**
- Quick "Got it, thanks!" responses (just type them)
- Highly personal messages to close relationships
- Messages where your unique voice is the point
- Confidential information you don't want in any system

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have the email context (original email, thread, or situation description)
- [ ] You know your intended outcome (what do you want to happen after they read this?)
- [ ] You know the relationship context (boss, client, peer, direct report)
- [ ] You have 2-3 minutes per email

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Generates professional, polished prose quickly
- Adapts tone for different relationships and situations
- Structures complex messages logically
- Maintains consistent voice across communications
- Suggests diplomatic phrasings for sensitive topics

**Where Human Judgment Is Essential:**
- Final review of tone appropriateness
- Confirming factual accuracy
- Adding personal touches that matter
- Deciding what to include vs. omit
- Ensuring message achieves your actual goal

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Original email | The email you're responding to | Context for relevant response |
| Thread history | Previous messages in chain | Maintains continuity |
| Relationship context | "This is a client I've worked with for 2 years" | Calibrates tone |
| Your goal | "I need to decline but keep the door open" | Shapes message strategy |
| Key points | Bullet points of what to convey | Ensures completeness |

**Sample Context (What You Might Provide):**
```
Need to respond to:

"Hi - I wanted to follow up on the proposal we discussed last week.
Our team is eager to move forward but we'd like to understand the
pricing better. Can we get on a call this week?"

Context:
- This is a prospective client we want to win
- Our pricing is firm - not much room to negotiate
- I'm available Thursday or Friday
- Want to seem enthusiastic without being pushy
```

---

## Step-by-Step Implementation

### Step 1: Gather Email Context
**Time: 1 minute**

Copy or summarize:
- The email you're responding to (or describe the situation)
- Any relevant thread history
- Who the recipient is and your relationship
- What you want to achieve

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Email Drafting Prompt
**Time: 1-2 minutes for Claude to process**

---

**PRIMARY PROMPT: Email Response Generator**

```
Please draft an email response for me.

ORIGINAL EMAIL / CONTEXT:
"""
[PASTE THE EMAIL YOU'RE RESPONDING TO, OR DESCRIBE THE SITUATION]
"""

RECIPIENT CONTEXT:
- Who: [e.g., prospective client, my manager, a vendor, colleague in another department]
- Relationship: [e.g., we've worked together 2 years, first interaction, they're senior to me]
- Tone needed: [e.g., professional and warm, formal, friendly but firm, apologetic]

MY GOAL:
[What do you want to happen after they read this? e.g., "Accept the meeting, understand our pricing is firm, feel valued as a prospect"]

KEY POINTS TO INCLUDE:
- [Point 1]
- [Point 2]
- [Point 3]

CONSTRAINTS:
- Length: [Brief (2-3 sentences) / Standard (1 paragraph) / Detailed (multiple paragraphs)]
- Things to avoid: [e.g., don't apologize too much, don't commit to specific dates, don't mention X]

Please draft the email with an appropriate subject line (if new email) or just the body (if reply).
```

---

### Step 4: Review the Draft
**Time: 1-2 minutes**

Read through Claude's draft and check:

**Tone:**
- Does it sound like you?
- Is it appropriate for this recipient?
- Would you be comfortable with this being forwarded?

**Content:**
- Are all your key points included?
- Is anything mischaracterized?
- Does it achieve your stated goal?

**Length:**
- Is it appropriately concise?
- Is anything important missing?

---

### Step 5: Refine as Needed
**Time: 1-2 minutes**

**To adjust tone:**
```
Make this warmer and more enthusiastic. This is a client we really want.
```

**To add specificity:**
```
Add that I'm available Thursday 2-4pm or Friday morning. Also mention we can do video or phone.
```

**To soften a decline:**
```
This feels too blunt. Make the "no" softer while keeping it clear we can't reduce pricing.
```

**To adjust length:**
```
This is too long. Condense to 3 sentences maximum while keeping the key points.
```

**To match your voice:**
```
I never say "I hope this email finds you well." Remove that and make the opening more direct.
```

---

### Step 6: Copy, Final Edit, Send
**Time: 30 seconds**

Copy the draft to your email client, make any final personal tweaks, and send.

---

## Example Output

Below is an example of a well-crafted response:

---

**Prompt context:** Responding to a client asking about pricing, want to seem enthusiastic but pricing is firm.

---

> **Subject: Re: Proposal Follow-up - Happy to Connect This Week**
>
> Hi Sarah,
>
> Thanks for reaching out—I'm glad the team is excited to move forward!
>
> I'd be happy to jump on a call to walk through the pricing structure in detail. I can share the thinking behind our approach and answer any questions your team has. I'm available Thursday between 2-4pm or Friday morning—let me know what works best for you, and I'll send over a calendar invite.
>
> Looking forward to connecting.
>
> Best,
> [Your name]

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Sounds too formal/stiff | Default professional tone | Specify: "Make this casual and conversational—this is a colleague I work with daily" |
| Too long | Claude defaulting to comprehensive | Specify word count: "Keep this under 75 words" |
| Wrong tone for situation | Context wasn't clear | Add relationship detail: "This person is upset about a mistake we made" |
| Missing key points | Points weren't explicit | List them explicitly: "Must include: apology, timeline for fix, escalation contact" |
| Generic feeling | No personalization input | Add context: "Reference the coffee we had last week" or "They mentioned their daughter's soccer game" |
| Sounds like AI | Too polished, no personality | Ask for adjustment: "Add some personality—I'm known for being direct and occasionally using humor" |

---

## Tips from Experience

1. **Include your goal, not just the reply request.** "I want them to feel heard but understand we can't do this" is more useful than "reply to this email."

2. **Share your actual voice.** If you have a signature phrase or style, mention it. "I always end with 'Cheers' not 'Best regards'" helps Claude match you.

3. **For sensitive emails, do two passes.** First draft for content, then refine specifically for tone. "Now make this 20% softer" works well.

4. **Use this for emails you're avoiding.** That difficult response you've been procrastinating on? This removes the activation energy barrier.

5. **Build a personal style guide.** After using this a few times, note what refinements you always make. Include them upfront in future prompts.

6. **Batch similar emails.** If you have 5 similar vendor outreach emails, do them in one session. "Now write a similar email for [next vendor] with these differences..."

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Email response time has decreased significantly
- [ ] You send more polished, professional emails
- [ ] Difficult emails no longer sit in drafts for days
- [ ] Recipients respond positively to your communication
- [ ] You have less email anxiety at the end of the day

**Track over time:**
- Number of emails lingering as drafts
- Time spent on email composition
- Response quality (based on feedback and outcomes)

---

## Variations

### Difficult Conversation Email
For delivering bad news, feedback, or uncomfortable messages:
```
This is a difficult email. I need to [decline their request / give negative feedback / deliver bad news].

Please draft an email that:
- Leads with empathy and acknowledgment
- Delivers the message clearly but kindly
- Doesn't over-apologize or be defensive
- Offers what I CAN do (if applicable)
- Maintains the relationship for future interaction

The recipient is [relationship context] and they will likely feel [disappointed / frustrated / etc.].
```

### Executive Communication
For emails to senior leadership:
```
This email is going to [C-level exec / Board member / Senior VP]. Please draft it to be:
- Concise and scannable (they're busy)
- Leading with the bottom line / ask
- Professional and polished
- Appropriately deferential without being obsequious
- Clear about what action (if any) is needed from them

Key message: [what you need them to know/do]
```

### Apology / Recovery Email
For fixing mistakes or service failures:
```
I need to apologize for [situation]. Please draft an email that:
- Takes clear responsibility without excessive groveling
- Explains what happened (briefly, no excuses)
- States what we're doing to fix it
- Offers appropriate make-good (if applicable)
- Rebuilds confidence in our reliability

The recipient is [relationship context] and this impacts them by [specific impact].
```

### Follow-up / Reminder Email
For following up without being annoying:
```
I need to follow up on [previous email/request] sent [timeframe] ago. Please draft a message that:
- Politely reminds without being pushy
- Acknowledges they're busy
- Makes it easy for them to respond
- Provides any needed context refresh
- Includes a clear ask or next step

I've followed up [0/1/2] times before on this.
```

---

## Building Your Repeatable System

After using this recipe for a week, establish your system:

1. **Create a "voice guide"** documenting your email style preferences
2. **Save prompt snippets** for common email types (declines, follow-ups, client responses)
3. **Keep a "relationship context" note** for key recurring correspondents
4. **Set up quick access** to Claude Code from your email workflow
5. **Build templates** for your most common email scenarios

**Sample Setup:**
```
email-helpers/
├── voice-guide.txt              # Your personal style notes
├── prompts/
│   ├── difficult-conversation.txt
│   ├── executive-update.txt
│   ├── client-response.txt
│   └── follow-up-reminder.txt
└── contacts/
    └── key-contacts.txt         # Context for important correspondents
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**provide context and goal → generate appropriate communication → refine to your voice**—applies broadly:

| Role | Application |
|------|-------------|
| **Sales** | Prospect outreach, proposal follow-ups, objection handling |
| **Customer Success** | Account updates, escalation responses, renewal discussions |
| **Managers** | Team communications, skip-level updates, cross-functional requests |
| **Executives** | Board communications, investor updates, company announcements |
| **HR** | Candidate communications, policy announcements, sensitive situations |
| **Consultants** | Client updates, scope discussions, deliverable handoffs |

---

## Next Steps

1. **Today:** Use this for your next complex email that would normally take 10+ minutes
2. **This week:** Try it on an email you've been avoiding
3. **Refine your style:** Note what adjustments you always make and build them into your prompts
4. **Expand:** Try the variations for specific email types you send frequently

---

*Recipe #3 of 100 in the Claude Code Knowledge Worker Recipe Collection*
