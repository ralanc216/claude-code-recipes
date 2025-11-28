# Customer Communication Templates

**Recipe #38: From Blank Page to Consistent, Professional Customer Messages**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 15 minutes (first time) / 3 minutes (repeat) | 1-2 hours per communication | Beginner | Customer Success, Support, Account Management |

---

## The Problem

Every customer interaction requires a slightly different message, but starting from scratch each time is inefficient. Your team sends inconsistent communications—different tones, varying quality, missing key information. Critical customer moments (onboarding, renewals, escalations) deserve polished communications, but there's no time to craft them perfectly. Templates exist somewhere, but they're outdated or too rigid.

**Pain Points:**
- Inconsistent quality across customer communications
- Time wasted rewriting similar messages
- Missing key information in important moments
- Tone varies by who's writing
- Templates too rigid for real situations
- Delayed responses while crafting messages
- No standard for critical customer touchpoints

---

## The Outcome

A library of adaptable, professional customer communication templates. Messages that maintain brand voice while being genuinely personalized. Faster response times without sacrificing quality. Consistent customer experience across all touchpoints.

**What You'll Have When Done:**
- Professional templates for key scenarios
- Customization framework for each
- Consistent brand voice across communications
- Reduced time to respond
- Higher quality customer interactions

---

## When to Use This Recipe

**Good Fit:**
- Onboarding communications
- Renewal and upsell conversations
- Support escalation responses
- Service disruption notifications
- Account review communications
- Win-back campaigns
- Milestone acknowledgments
- Difficult conversation templates

**Not a Good Fit:**
- Completely unique situations
- Legal/contractual communications
- Highly personalized relationship messages
- Crisis situations requiring executive involvement

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You know the scenario/communication type
- [ ] You have customer context and details
- [ ] You know your brand voice guidelines
- [ ] You have 30-45 minutes for template creation

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Creates professional, polished templates
- Adapts tone for different scenarios
- Identifies customization points
- Maintains consistency across templates
- Suggests variations for different situations
- Ensures key information is included

**Where Human Judgment Is Essential:**
- Customer relationship nuance
- Sensitive situation handling
- When to deviate from templates
- Approval of difficult communications
- Brand voice calibration
- Strategic account decisions

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Scenario | Onboarding, renewal, etc. | Template structure |
| Customer context | Company, role, history | Personalization |
| Brand voice | Tone guidelines | Style consistency |
| Key messages | What must be communicated | Content framework |
| Examples | Past successful communications | Style matching |

**Sample Input:**
```
Customer Communication Template Request

SCENARIO: Service Disruption Notification

CONTEXT:
- We had a 2-hour outage affecting our API
- Root cause: Database failover issue
- Affected: ~30% of customers
- Timeline: Started 2:15 PM ET, resolved 4:22 PM ET
- Impact: API calls failed or timed out during this window

COMMUNICATION NEEDS:
1. Initial notification (during outage)
2. Update notification (when resolved)
3. Post-incident summary (next day)

AUDIENCE SEGMENTS:
- Enterprise customers (need detailed technical info)
- SMB customers (need simpler explanation)
- Affected vs. not affected (different levels of detail)

BRAND VOICE:
- Professional but human
- Take responsibility, don't make excuses
- Technical without being jargon-heavy
- Empathetic to customer impact
- Action-oriented

WHAT CUSTOMERS NEED TO KNOW:
- What happened
- How it affected them
- What we're doing about it
- What they need to do (if anything)
- How we're preventing recurrence

TONE:
- Apologetic but confident
- Transparent about the issue
- Focused on resolution and prevention

CUSTOMIZATION POINTS:
- Customer name
- Whether they were affected
- Specific impact to their usage
- SLA implications (enterprise only)
```

---

## Step-by-Step Implementation

### Step 1: Define the Communication Scenario
**Time: 5-10 minutes**

Clarify:
- What's the situation?
- Who's the audience?
- What must be communicated?
- What outcome do you want?
- What's the right tone?

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Template Generation Prompt
**Time: 5-7 minutes for Claude to process**

---

**PRIMARY PROMPT: Customer Communication Templates**

```
Please help me create customer communication templates.

SCENARIO:
[Describe the situation requiring communication]

AUDIENCE:
- Primary: [Who's receiving this]
- Segments: [Any variations needed]

KEY INFORMATION TO COMMUNICATE:
1. [Required element 1]
2. [Required element 2]
3. [Required element 3]
(etc.)

BRAND VOICE:
[Describe your communication style]
[Any voice guidelines or samples]

DESIRED OUTCOME:
[What you want the customer to think/feel/do]

TONE REQUIREMENTS:
- [Primary tone]
- [What to avoid]

PLEASE CREATE:

1. PRIMARY TEMPLATE
   Complete communication template with:
   - Subject line (if email)
   - Opening that addresses the situation directly
   - Body with all key information
   - Clear next steps or call to action
   - Professional closing
   - [CUSTOMIZATION POINTS] clearly marked

2. VARIATIONS
   Adapted versions for different:
   - Customer segments (if applicable)
   - Levels of impact (if applicable)
   - Communication channels (email, in-app, etc.)

3. CUSTOMIZATION GUIDE
   For each template:
   - What to personalize
   - What NOT to change (key messages)
   - Tone adjustments for different situations

4. SUBJECT LINE OPTIONS
   5 subject line variations (if email)

5. RESPONSE FRAMEWORKS
   If customers might reply:
   - Common questions and suggested responses
   - Escalation triggers

6. QUALITY CHECKLIST
   What to verify before sending

Make templates professional but human. Avoid corporate jargon. Sound like a real person who cares.
```

---

### Step 4: Review for Completeness and Tone
**Time: 10 minutes**

Check each template:
- Does it cover all required information?
- Is the tone appropriate?
- Are customization points clear?
- Is it easy to adapt?
- Does it sound like your brand?

---

### Step 5: Customize for Your Context
**Time: 10-15 minutes**

**To adjust tone:**
```
This sounds too formal. Make it warmer and more conversational while keeping it professional. We want customers to feel supported, not processed.
```

**To add specific elements:**
```
Add a section specifically addressing SLA implications for enterprise customers. They'll want to know if this affects their SLA credits.
```

**To simplify:**
```
The technical explanation is too detailed for our SMB segment. Create a simpler version that explains the impact without the technical details.
```

**To strengthen empathy:**
```
The apology feels hollow. Make it more genuine—acknowledge the specific impact on their business, not just that "we're sorry for any inconvenience."
```

---

### Step 6: Create Final Template Library
**Time: 10 minutes**

```
Create the final template package:

1. TEMPLATE LIBRARY
   Organized by scenario type:
   - Each template clearly named
   - Version for each segment/variation
   - Customization points highlighted

2. USAGE GUIDE
   - When to use each template
   - Required customizations
   - Approval requirements
   - Do's and don'ts

3. QUICK REFERENCE
   - One-pager showing all templates
   - Which to use when
   - Escalation triggers

4. EXAMPLE FILLED-IN VERSIONS
   Show each template with sample customer data filled in
```

---

## Example Output

Below is an abbreviated template library example:

---

> **SERVICE DISRUPTION TEMPLATES**
>
> ---
>
> ## Template 1: Initial Outage Notification
>
> **Use when:** An outage is in progress and customers need to know
>
> **Subject Line Options:**
> 1. Service Update: [Product Name] API experiencing issues
> 2. ⚠️ Current service disruption affecting [Product Name]
> 3. We're investigating issues with [Product Name]
>
> ---
>
> **TEMPLATE (Affected Enterprise Customers):**
>
> Subject: Service Update: [Product Name] API experiencing issues
>
> Hi [Customer First Name],
>
> We're currently experiencing issues with our API that may be affecting your integration. We wanted to let you know immediately.
>
> **What's happening:**
> Starting at [TIME] [TIMEZONE], some API calls are failing or timing out. Our team is actively investigating.
>
> **Impact to [Customer Company]:**
> [CUSTOMIZE: Describe specific impact based on their usage]
>
> **What we're doing:**
> Our engineering team is working to resolve this as quickly as possible. We'll send updates every 30 minutes until resolved.
>
> **What you may need to do:**
> [CUSTOMIZE: Any actions they should take, or "No action needed on your end"]
>
> Track real-time status at: [status page link]
>
> I'm personally monitoring this and will update you as soon as we have more information.
>
> [Your name]
> [Title]
> Direct: [phone] | [email]
>
> ---
>
> **Customization Guide:**
> - [Customer First Name]: Use first name for warm relationship, "Team" if no primary contact
> - [TIME] [TIMEZONE]: Always use customer's timezone if known
> - [Impact description]: Be specific—"Your nightly sync jobs may have failed" is better than "you may experience issues"
> - [Actions]: Most outages need no customer action—say so clearly
>
> ---
>
> ## Template 2: Resolution Notification
>
> **Use when:** The issue is resolved
>
> **Subject Line Options:**
> 1. ✅ Resolved: [Product Name] API issue
> 2. Service restored: [Product Name] back to normal
> 3. Update: [Product Name] issue resolved at [TIME]
>
> ---
>
> **TEMPLATE:**
>
> Subject: ✅ Resolved: [Product Name] API issue
>
> Hi [Customer First Name],
>
> Good news—the API issue we notified you about earlier has been resolved.
>
> **Summary:**
> - Issue started: [START TIME]
> - Issue resolved: [END TIME]
> - Duration: [X hours/minutes]
>
> **What happened:**
> [BRIEF EXPLANATION—technical enough to be credible, simple enough to understand]
>
> **Impact to your account:**
> [CUSTOMIZE: What specifically was affected]
> [CUSTOMIZE: Any data recovery or retry needed]
>
> **What we're doing to prevent this:**
> We're conducting a full post-incident review. I'll share what we learn and what we're changing within [TIMEFRAME, typically 48-72 hours].
>
> If you notice any ongoing issues or have questions, please reply to this email or call me directly.
>
> Thank you for your patience.
>
> [Your name]
>
> ---
>
> ## Template 3: Post-Incident Summary (Enterprise)
>
> **Use when:** 24-48 hours after resolution, for enterprise customers
>
> **Subject:** Post-Incident Report: [Date] API Disruption
>
> ---
>
> **TEMPLATE:**
>
> Hi [Customer First Name],
>
> As promised, here's our full post-incident report on the API disruption that occurred on [DATE].
>
> **Incident Summary**
> - Duration: [START TIME] to [END TIME] ([DURATION])
> - Services affected: [SERVICES]
> - Root cause: [BRIEF EXPLANATION]
>
> **Timeline of Events**
> - [TIME]: Issue first detected by monitoring
> - [TIME]: Engineering team engaged
> - [TIME]: Root cause identified
> - [TIME]: Fix deployed
> - [TIME]: Service fully restored
>
> **Impact to [Customer Company]**
> [CUSTOMIZE with specific details]:
> - API calls affected: [NUMBER or PERCENTAGE]
> - [Specific impact to their use case]
>
> **Root Cause**
> [CLEAR EXPLANATION—be honest about what went wrong]
>
> **Corrective Actions**
> We're implementing the following changes to prevent recurrence:
>
> 1. [ACTION 1] - [STATUS: Complete/In progress/Planned]
> 2. [ACTION 2] - [STATUS]
> 3. [ACTION 3] - [STATUS]
>
> **SLA Impact**
> [CUSTOMIZE for enterprise customers]:
> This incident [did/did not] affect your SLA. [If affected: You're entitled to X credit. Our account team will apply this to your next invoice automatically.]
>
> I'm happy to walk through this report in more detail. Would a call be helpful?
>
> [Your name]
>
> ---
>
> ## Quick Reference: When to Use Which Template
>
> | Situation | Template | Segments |
> |-----------|----------|----------|
> | Outage in progress | Initial Notification | All affected |
> | Outage resolved | Resolution Notification | All affected |
> | 24-48 hours later | Post-Incident Summary | Enterprise only |
> | Customer asks for details | Direct to Post-Incident or schedule call | Case by case |
>
> ---
>
> ## Response Framework: Common Customer Questions
>
> **"What caused this?"**
> During outage: "Our team is still investigating. Once we understand the root cause, I'll share details."
> After resolution: Refer to Post-Incident Summary or share brief explanation.
>
> **"How do I know this won't happen again?"**
> "I understand the concern. Here's what we're changing: [list specific actions]. I'll share our full corrective action plan within [timeframe]."
>
> **"What about my SLA?"**
> "Let me check your specific agreement and get back to you today with details on any credits."
>
> **"This is unacceptable"**
> Acknowledge, don't defend. "You're right to be frustrated. This fell short of the reliability you expect from us. Here's what we're doing..." [Then offer call with account manager or escalation path]
>
> ---
>
> ## Quality Checklist Before Sending
>
> - [ ] Customer name and company are correct
> - [ ] Times are in correct timezone
> - [ ] Impact description is accurate and specific to their usage
> - [ ] No placeholder text remaining
> - [ ] Tone matches severity (not too casual for serious issue)
> - [ ] Clear next steps or "no action needed"
> - [ ] Contact information included
> - [ ] Links work
> - [ ] Approved for sending (if required)

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Templates too rigid | Over-structured | Ask: "Make templates more flexible—show what's required vs. optional to customize" |
| Tone feels cold | Too formal | Ask: "Warm this up. Sound like a helpful person, not a company" |
| Missing key info | Requirements not clear | Add: "Must include: [specific elements]. Flag clearly if missing" |
| Hard to customize | Unclear markers | Ask: "Use [BRACKETS] clearly for all customization points with brief guidance" |
| Different for segments | One-size-fits-all | Ask: "Create separate versions for [segment 1] and [segment 2]" |
| Too long | Over-explaining | Ask: "Shorten to essential information only. Customers want answers, not essays" |

---

## Tips from Experience

1. **Lead with what customers care about.** They want to know: Am I affected? What do I need to do? Lead with that.

2. **Be specific about impact.** "You may experience issues" is useless. "Your automated reports may have been delayed" is helpful.

3. **Include clear next steps.** Even if the next step is "no action needed," say so explicitly.

4. **Time zones matter.** Always communicate in the customer's timezone when possible.

5. **Apologies should be specific.** "Sorry for the inconvenience" is hollow. "Sorry you had to reschedule your demo because of our outage" is real.

6. **Templates are starting points.** The best customer communication sounds like it was written just for them, even when it wasn't.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Response time to customers improves
- [ ] Communication quality is consistent across team
- [ ] Fewer escalations due to poor communication
- [ ] Positive customer feedback on communications
- [ ] Team confidence in handling difficult situations

**Track over time:**
- Average response time
- Customer satisfaction with communications
- Escalation rate
- Template usage and adaptations
- Time saved per communication

---

## Variations

### Onboarding Communication Sequence
For new customer welcome:
```
Create an onboarding communication sequence.

Customer profile: [Type of customer]
Product: [What they purchased]
Onboarding milestones: [Key steps]

Create templates for:
1. Welcome email (immediately after purchase)
2. Getting started guide (Day 1)
3. First milestone check-in (Day 3-5)
4. Feature introduction (Day 7)
5. Success check-in (Day 14)
6. Review/feedback request (Day 30)

Include: Personalization points, success metrics to reference
```

### Renewal Communication Templates
For contract renewals:
```
Create renewal communication templates.

Scenario types:
1. Proactive renewal outreach (60 days before)
2. Renewal proposal with upsell
3. Renewal proposal (flat renewal)
4. At-risk customer renewal approach
5. Renewal confirmation

Include: Customization for usage data, success metrics, pricing
```

### Escalation Response Templates
For handling escalations:
```
Create escalation response templates.

Scenarios:
1. Initial escalation acknowledgment
2. Investigation update
3. Resolution with explanation
4. Resolution with compensation offer
5. Executive involvement (serious escalation)

Tone: Apologetic, action-oriented, specific
Include: What to escalate internally
```

### Win-Back Campaign Templates
For re-engaging churned customers:
```
Create win-back communication templates.

Churn reasons to address:
1. Price/budget concerns
2. Feature gaps (now addressed)
3. Usage declined/forgot about us
4. Competitor switch

Sequence: Initial outreach, follow-up, final attempt
Include: Incentive options, personalization based on past usage
```

---

## Building Your Repeatable System

After creating templates, build your system:

1. **Organize templates by scenario** for easy access
2. **Create a template request process** for new scenarios
3. **Establish review and update cadence**
4. **Track which templates are used most**
5. **Collect feedback for improvements**

**Sample Setup:**
```
customer-templates/
├── by-scenario/
│   ├── onboarding/
│   │   ├── welcome-email.md
│   │   ├── getting-started.md
│   │   └── milestone-checkins.md
│   ├── incidents/
│   │   ├── outage-notification.md
│   │   ├── resolution-notification.md
│   │   └── post-incident-summary.md
│   ├── renewals/
│   │   ├── proactive-outreach.md
│   │   ├── renewal-proposal.md
│   │   └── at-risk-approach.md
│   └── escalations/
│       ├── acknowledgment.md
│       ├── investigation-update.md
│       └── resolution.md
├── by-segment/
│   ├── enterprise/
│   └── smb/
├── guides/
│   ├── brand-voice.md
│   ├── when-to-use.md
│   └── customization-guide.md
└── feedback/
    ├── template-requests.md
    └── improvement-log.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**identify scenario → create adaptable template → define customization points → maintain consistency**—applies broadly:

| Role | Application |
|------|-------------|
| **Customer Success** | All customer touchpoints |
| **Support** | Ticket responses, escalations |
| **Account Management** | Renewal and upsell communications |
| **Sales** | Outreach and follow-up templates |
| **Onboarding** | New customer communications |
| **Marketing** | Customer lifecycle emails |

---

## Next Steps

1. **Identify priority scenarios:** Which communications need templates most urgently?
2. **Gather voice guidelines:** Document your brand voice
3. **Create first template set:** Start with highest-volume scenario
4. **Test with team:** Get feedback from people who'll use them
5. **Iterate and expand:** Refine based on usage, add new scenarios

---

*Recipe #38 of 100 in the Claude Code Knowledge Worker Recipe Collection*
