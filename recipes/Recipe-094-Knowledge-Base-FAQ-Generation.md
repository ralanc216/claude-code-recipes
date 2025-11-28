# Knowledge Base and FAQ Generation

**Recipe #94: From Support Tickets to Self-Service Knowledge Base**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 10 minutes (first time) / 5 minutes (repeat) | 3-6 hours per KB section | Beginner | Support Managers, Technical Writers, Product Managers |

---

## The Problem

Support teams answer the same questions repeatedly. Every ticket about "how do I reset my password" or "why isn't X working" consumes agent time that could be spent on complex issues. Knowledge bases exist in theory, but they're often outdated, incomplete, poorly organized, or written in a style that users can't understand—so customers contact support anyway.

**Pain Points:**
- Same questions answered hundreds of times via individual tickets
- Knowledge base exists but customers can't find answers
- Articles written in technical jargon users don't understand
- Documentation outdated and doesn't match current product
- Users email support instead of searching because search never works
- Support agents give different answers to the same question
- Article creation backlog grows while ticket volume increases

---

## The Outcome

A comprehensive, searchable knowledge base with clear answers to common questions, organized logically, written at the appropriate level for the target audience, and structured for both self-service browsing and support agent reference.

**What You'll Have When Done:**
- User-friendly articles answering top support questions
- Clear step-by-step instructions with screenshots
- Troubleshooting guides for common issues
- Logically organized category structure
- Search-optimized content using terms users actually use
- Internal playbooks for support agents

---

## When to Use This Recipe

**Good Fit:**
- Building new knowledge base from scratch
- Updating outdated help documentation
- Extracting FAQ from support tickets
- Creating internal support playbooks
- Launching new features requiring documentation
- Consolidating scattered documentation

**Not a Good Fit:**
- Real-time chat responses (too slow)
- Technical API documentation (different format)
- Legal or compliance documentation (requires legal review)
- Highly personalized customer issues

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] Support ticket data available (common questions)
- [ ] Existing documentation gathered (however scattered)
- [ ] Product/service feature list compiled
- [ ] Known issues and workarounds documented
- [ ] Target audience clearly defined
- [ ] Common search terms users use identified
- [ ] Product screenshots available (if applicable)
- [ ] Subject matter expert access confirmed
- [ ] You have 30-45 minutes for KB article creation

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Analyzes support tickets to identify question patterns
- Transforms technical answers into user-friendly language
- Organizes content logically by category and user journey
- Ensures consistent style and format across articles
- Identifies gaps in documentation coverage
- Creates troubleshooting decision trees from scattered notes
- Generates search-optimized titles and descriptions

**Where Human Judgment Is Essential:**
- Validating technical accuracy of solutions
- Testing instructions actually work as written
- Determining appropriate detail level for audience
- Deciding article priority based on business impact
- Reviewing for brand voice and tone consistency
- Identifying when to escalate vs. self-service

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Support ticket analysis | Top 20 questions by volume | Article prioritization and topic identification |
| Existing documentation | Internal wikis, old articles, Slack | Technical accuracy and current solutions |
| Product context | Feature descriptions, workflows | User-facing explanations and use cases |
| Known issues | Bug tracker, workarounds | Troubleshooting sections and limitations |
| Search analytics | What users search for but don't find | Title optimization and content gaps |

**Sample Input:** *(Support ticket analysis)*
```
TOP SUPPORT TICKETS (Last 90 days):

1. "Can't log in" - 450 tickets
   Common causes: Wrong email, expired password, account locked, browser cache
   Resolution: Password reset, clear cache, unlock account

2. "How do I export data?" - 320 tickets
   Questions: Format options, size limits, export schedule
   Resolution: Guide to export feature in Settings

3. "Integration not working" - 280 tickets
   Types: Slack not connecting, API errors, webhook failures
   Resolution: Various troubleshooting steps by integration
```

---

## Step-by-Step Implementation

### Step 1: Analyze Support Data
**Time: 10 minutes**

Gather your support intelligence:
- Export top 20-30 tickets by volume from past 90 days
- Review support agent notes for common resolution paths
- Collect screenshots showing where users get confused
- List known product limitations and workarounds
- Identify what users search for but can't find

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Support Analysis Prompt
**Time: 10-15 minutes for Claude to process**

---

**PRIMARY PROMPT: Analyze Support Patterns**

```
Claude, I need to build a knowledge base from support data.

Here's our ticket analysis:
[Paste top ticket categories with volumes, common causes, resolutions]

Help me:
1. Group tickets into logical categories for users
2. Prioritize which articles to create first (by volume and impact)
3. Identify variations of the same question (e.g., "can't login" vs "forgot password")
4. Note which questions need single vs multiple articles
5. List common search terms for each topic
```

---

### Step 4: Review and Validate
**Time: 5 minutes**

**Check immediately:**
- Category groupings make sense from user perspective
- Prioritization aligns with business impact
- Search terms match what users actually type

**Spot-check specifics:**
- No jargon in article titles
- Related topics are grouped together
- Navigation paths are intuitive

---

### Step 5: Create Knowledge Base Structure
**Time: 10 minutes**

```
Design a knowledge base structure for these topics:

Topics identified: [Paste from previous analysis]
Target audience: [End users (non-technical) / Administrators / Support agents]
Platform: [Zendesk / Confluence / SharePoint / etc.]

Create:
1. Top-level categories (4-6 max for easy navigation)
2. Subcategories within each
3. Suggested article titles using user language
4. Logical navigation path for common user journeys
```

---

### Step 6: Write Individual Articles
**Time: 15-20 minutes per article**

**For How-To Articles:**
```
Write a knowledge base article on this topic:

Topic: [Specific topic, e.g., "Resetting your password"]
Common questions: [List variations users ask]
Technical answer: [Paste internal knowledge / existing docs]
Target audience: [Non-technical end users]

Requirements:
- Lead with user's problem/goal ("Can't log in? Reset your password.")
- Step-by-step format with numbered lists
- Plain language (no jargon or assume nothing)
- Include troubleshooting for common issues ("What if I don't get the reset email?")
- Add "Related articles" section
- Include search keywords users would use
```

**For Troubleshooting Guides:**
```
Create a troubleshooting article for this issue:

Issue: [Problem users experience, e.g., "Slack integration not working"]
Common causes: [List from ticket analysis]
Solutions for each cause: [Technical details]

Format as:
1. Symptom description (what the user sees)
2. Quick fixes to try first (restart, check settings)
3. Detailed troubleshooting by cause
4. When to contact support (escalation criteria)
5. Prevention tips
```

---

### Step 7: Review and Optimize
**Time: 10 minutes**

```
Review this knowledge base article for publication:

Article draft: [Paste]
Target audience: [User type and technical level]

Check for:
1. Clarity and appropriate readability level
2. Completeness (does it fully answer the question?)
3. Accuracy of steps (can someone follow this successfully?)
4. Search optimization (includes keywords users search for)
5. Consistency with other articles (terminology, style)
6. Appropriate links to related content
```

---

### Step 8: Export and Publish
**Time: 5 minutes**

```
Format this article for [Zendesk Guide / Confluence / etc.]. Include:
- Proper formatting (headers, lists, callouts)
- "Was this helpful?" feedback mechanism
- Related articles section
- Last updated date
- Appropriate tags for search and categorization
```

---

## Example Output

Below is an abbreviated example of what well-executed knowledge base content looks like:

---

> ### Can't Log In? Here's How to Fix It
>
> **Category:** Troubleshooting > Login Issues
> **Search Keywords:** can't log in, login problem, forgot password, account locked
>
> ---
>
> #### Quick Answer
>
> If you can't log in, try these fixes:
> 1. **Wrong password?** [Reset your password](#reset-password)
> 2. **Wrong email?** Try other email addresses you use
> 3. **Account locked?** Wait 30 minutes or [contact support](#contact-support)
>
> ---
>
> #### Detailed Troubleshooting
>
> ##### Problem: "Invalid email or password"
>
> **Try these steps:**
>
> 1. **Check for typos** in your email address
> 2. **Try other email addresses** you might have used to sign up
> 3. **Reset your password:**
>    - Go to the [login page](link)
>    - Click "Forgot password?"
>    - Enter your email
>    - Check your inbox (and spam folder) for the reset link
>    - Create a new password (minimum 8 characters)
>
> > **Tip:** The reset link expires after 24 hours. If it's expired, request a new one.
>
> ---
>
> ##### Problem: "Account locked"
>
> After 5 failed login attempts, your account locks for 30 minutes.
>
> **To unlock your account:**
> - **Option 1:** Wait 30 minutes, then try again
> - **Option 2:** Reset your password (this unlocks immediately)
> - **Option 3:** [Contact support](#contact-support) if you're still locked out
>
> ---
>
> ##### Problem: "No reset email received"
>
> If you don't receive the password reset email:
>
> 1. **Check your spam/junk folder**
> 2. **Wait a few minutes** — emails can be delayed
> 3. **Try a different email** — you may have signed up with another address
> 4. **Contact support** — we can look up your account by name
>
> ---
>
> **Related Articles:**
> - [How to reset your password](#)
> - [Setting up two-factor authentication](#)
> - [Managing your account email](#)
>
> ---
>
> *Was this article helpful?* 👍 Yes | 👎 No
>
> *Last updated: January 15, 2025*

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Articles too technical | Written from internal perspective | Write for lowest common denominator; define all technical terms; use "you" language; test with actual users |
| Hard to find right article | Poor search optimization or organization | Add multiple search keywords; use common phrasing in titles; link related articles heavily; test search |
| Articles go out of date | No update process | Include "last updated" date prominently; set review cycle; add user feedback flags; trigger updates on product changes |
| KB doesn't match agent answers | No single source of truth | Agents should contribute to KB; regular sync meetings; KB should be agent training resource |
| Low deflection rate | Users prefer contacting support | Promote KB in product, email signatures; measure and improve findability; make KB easier than email |
| Inconsistent style/quality | Multiple authors, no standards | Create style guide; use templates; single reviewer/editor role; regular quality audits |

---

## Tips from Experience

1. **Answer the question first.** Don't make users scroll past context and background. Lead with the solution, then provide details.

2. **Use their words.** Title articles with the exact phrases users search for, not internal product names or technical terms.

3. **Show don't tell.** Screenshots and GIFs are worth a thousand words. Show the button to click, don't describe where it is.

4. **Progressive disclosure.** Provide a quick answer upfront, then detailed steps for those who need them. Most users want the quick fix.

5. **Keep it current.** An outdated knowledge base is worse than no knowledge base. Build updates into your product release process.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Support ticket volume decreases for documented topics
- [ ] Article helpfulness ratings are consistently positive (>80%)
- [ ] Search success rate improves (users find answers)
- [ ] Support agents reference KB articles regularly
- [ ] Time to resolution decreases for common issues

**Track over time:**
- Article views and search queries leading to views
- Support ticket deflection rate
- "Was this helpful?" feedback scores

---

## Variations

### Internal IT Knowledge Base
**When to use:** Documentation for internal systems and procedures
```
Focus on internal systems and institutional knowledge:
- Access procedures for internal systems
- Standard operating procedures
- IT troubleshooting for common employee issues
- Software installation guides
- Hardware setup and configuration
- Security best practices for employees
```

### Developer Documentation FAQ
**When to use:** Technical audience with API/integration questions
```
Technical guides for developer audiences:
- Common API integration issues
- Code examples for frequent patterns
- Authentication troubleshooting
- Rate limiting and best practices
- SDK-specific guidance
- Webhook debugging
```

### Chatbot Training Data
**When to use:** Building conversational AI responses
```
Structured Q&A pairs for bot training:
- Question variations for same intent
- Concise answers suitable for chat
- Follow-up question handling
- Escalation triggers to human support
- Confidence scoring based on question clarity
```

---

## Building Your Repeatable System

After using this recipe 2-3 times, establish your system:

1. **Create article templates** for common types: how-to articles, troubleshooting guides, FAQ format, reference tables. This ensures consistency and speeds creation.

2. **Link ticket system to KB** so support agents can suggest relevant articles during ticket creation. Agents should also flag articles needing updates.

3. **Integrate with product updates** where new features automatically trigger KB article creation. No feature ships without documentation.

4. **Establish review cadence** (quarterly) for all articles. Check accuracy, update screenshots, remove outdated content.

**Sample Folder Structure:**
```
knowledge-base/
├── getting-started/
│   ├── account-setup.md
│   ├── first-steps.md
│   └── quick-start-guide.md
├── account-billing/
│   ├── account-settings/
│   ├── team-management/
│   └── billing-plans/
├── features-how-to/
│   ├── data-management/
│   ├── integrations/
│   └── reports-analytics/
├── troubleshooting/
│   ├── login-issues.md
│   ├── integration-problems.md
│   └── common-errors.md
└── templates/
    ├── how-to-template.md
    ├── troubleshooting-template.md
    └── faq-template.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**transforming repeated questions into self-service documentation**—applies broadly:

| Role | Application |
|------|-------------|
| **HR Teams** | Employee self-service for benefits, leave, policies, onboarding |
| **IT Support** | Internal support documentation for common tech issues |
| **Sales Teams** | Prospect FAQ, objection handling, product comparison docs |
| **Legal** | Policy FAQ, compliance guidance, contract templates |
| **Education** | Course FAQ, learning resources, student support documentation |

---

## Next Steps

1. **This week:** Publish initial articles for your top 3 support topics by volume. Measure baseline ticket volume.

2. **Track your results:** Monitor ticket volume for documented topics. Set deflection rate goals (aim for 30-50% reduction).

3. **Iterate:** Collect feedback via "Was this helpful?" buttons. Update articles based on negative feedback and new questions.

4. **Share:** Promote KB in email signatures, in-app help, onboarding flows. Make it easier to find than support contact.

---

*Recipe #94 of 100 in the Claude Code Knowledge Worker Recipe Collection*
