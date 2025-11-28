# Job Descriptions and Role Documentation

**Recipe #61: Create Comprehensive Role Definitions That Attract the Right Talent**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 5 minutes (first time) / 2 minutes (repeat) | 2-3 hours per role | Beginner | HR, Recruiters, Hiring Managers |

---

## The Problem

Job descriptions are either too vague to attract qualified candidates or so detailed they scare everyone away. Hiring managers describe what they want but struggle to articulate it in a job posting. Requirements lists become wishlists. The same role looks completely different across departments. Candidates can't tell if they're qualified. And writing good job descriptions takes hours—time that hiring managers don't have.

**Pain Points:**
- Hours spent wordsmithing job postings
- Inconsistent format across the organization
- Requirements bloat ("10 years experience for entry role")
- Missing context about the actual work
- Can't articulate culture and team dynamics
- Qualified candidates self-select out
- Unqualified candidates flood the pipeline

---

## The Outcome

Clear, compelling job descriptions that accurately represent roles and attract qualified candidates. Comprehensive role documentation including screening criteria, interview questions, and evaluation rubrics. Consistency across hiring that improves quality and reduces bias.

**What You'll Have When Done:**
- Professional job posting
- Complete role documentation
- Screening criteria
- Interview question bank
- Evaluation rubric
- Hiring manager prep materials

---

## When to Use This Recipe

**Good Fit:**
- Opening a new position
- Updating outdated job descriptions
- Creating roles from scratch
- Standardizing JD format across organization
- Preparing for rapid hiring
- Building role libraries

**Not a Good Fit:**
- Executive search (needs specialized approach)
- Highly technical roles requiring SME input
- Roles where you're not clear on requirements
- Confidential searches with sensitivity concerns

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You understand the role's purpose and context
- [ ] You know the team structure and reporting
- [ ] You have compensation range (rough is fine)
- [ ] You have 20-30 minutes for complete documentation

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Structures job descriptions professionally
- Identifies essential vs nice-to-have requirements
- Generates inclusive language
- Creates screening criteria
- Develops interview questions
- Builds evaluation frameworks

**Where Human Judgment Is Essential:**
- Validating requirements accuracy
- Confirming team culture fit description
- Approving compensation range
- Ensuring legal compliance
- Final review and approval
- Customizing for specific situations

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Role summary | What the job is | Core description |
| Requirements | Skills and experience needed | Requirements structuring |
| Team context | Who they work with | Team/culture section |
| Company info | Values, mission | Company positioning |
| Specifics | Location, comp, benefits | Practical details |

**Sample Input:**
```
Job Description Request

ROLE TITLE: Senior Product Manager
DEPARTMENT: Product
REPORTS TO: VP of Product
LOCATION: Remote (US-based) or San Francisco HQ
COMPENSATION: $150K-$180K base + equity

ABOUT THE COMPANY:
CloudSync Pro is a B2B SaaS company with 150 employees. We make collaboration software for distributed teams. Series B funded ($40M), growing 50% YoY, aiming for profitability in 18 months. Values: customer obsession, data-driven decisions, radical candor, ownership mindset.

TEAM CONTEXT:
- Product team is 8 people (1 VP, 3 PMs, 4 designers)
- This PM will own our enterprise product line
- Work closely with 2 engineering teams (~12 engineers)
- Customers range from 50 to 5,000 employees
- Major enterprise customers include 3 Fortune 500 companies

WHY WE'RE HIRING:
- Enterprise segment growing 80% YoY
- Need dedicated PM focus on enterprise features
- Current PM (who's moving to a new product line) built the enterprise product from scratch
- Backlog is significant—lots of opportunity

WHAT THEY'LL ACTUALLY DO:
- Own enterprise product roadmap end-to-end
- Conduct customer research (calls, visits, analysis)
- Write detailed specs and PRDs
- Partner with engineering on execution
- Work with sales on enterprise deals
- Present to executive team monthly
- Define and track product metrics

MUST HAVE:
- 5+ years product management experience
- B2B SaaS background
- Enterprise customer experience
- Strong technical fluency (can speak to APIs, integrations)
- Excellent communication skills

NICE TO HAVE:
- Collaboration software experience
- Experience with SOC 2, compliance features
- Previous startup experience
- SQL skills

WHAT SUCCESS LOOKS LIKE:
- 6 months: Owns the roadmap, shipped first major feature
- 12 months: Enterprise NPS improved, revenue impact visible
- 18 months: Enterprise product is a competitive differentiator

CULTURE FIT:
- Self-starters who don't wait for direction
- Data-oriented but willing to make judgment calls
- Comfortable with ambiguity
- Direct communicators
- Customer-focused

INTERVIEW PROCESS:
- Recruiter screen (30 min)
- Hiring manager call (45 min)
- Product case presentation (1 hr)
- Cross-functional interviews (3 x 30 min: Eng, Design, Sales)
- Final: VP Product + CEO (1 hr)

BENEFITS:
- Competitive salary + equity
- Unlimited PTO (actually used)
- Health/dental/vision (100% covered)
- 401k with 4% match
- $2,000 annual learning budget
- Remote-first with optional SF office
```

---

## Step-by-Step Implementation

### Step 1: Gather Role Information
**Time: 5-10 minutes**

Collect:
- Role purpose and responsibilities
- Requirements (must-have vs nice-to-have)
- Team and company context
- Compensation and benefits
- Success metrics

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Job Description Prompt
**Time: 3-5 minutes for Claude to process**

---

**PRIMARY PROMPT: Job Description Generation**

```
Please create comprehensive job documentation for this role.

ROLE INFORMATION:
[Paste all role details from Step 1]

CREATE THE FOLLOWING:

1. JOB POSTING
   Format for job boards and career page:

   **About Us**
   [Company description - compelling, not boilerplate]

   **About the Role**
   [What makes this role exciting and impactful]

   **What You'll Do**
   [Responsibilities as action-oriented bullets]

   **What You Bring**
   [Requirements - be specific about what's truly required]

   **Nice to Have**
   [Additional qualifications that would be valuable]

   **What Success Looks Like**
   [Clear expectations for the first year]

   **What We Offer**
   [Compensation, benefits, culture highlights]

   **How to Apply**
   [Process and what to include]

   Write in engaging, inclusive language. Avoid jargon and clichés.

2. ROLE DOCUMENTATION (Internal)

   **Role Overview:**
   - Title and level
   - Department and reporting structure
   - Direct reports (if any)
   - Key relationships

   **Core Responsibilities:**
   [Detailed list with % time allocation]

   **Success Metrics:**
   [How performance will be measured]

   **Growth Path:**
   [Where this role can lead]

3. SCREENING CRITERIA

   **Resume Screen:**
   | Criteria | Must Have | Strong | Nice to Have | Red Flag |
   |----------|-----------|--------|--------------|----------|

   **Initial Screen Questions:**
   [Questions for recruiter to ask]

   **Knockout Factors:**
   [What automatically disqualifies]

4. INTERVIEW QUESTION BANK

   **Background/Experience:**
   - [Question] — [What good looks like]

   **Technical/Functional:**
   - [Question] — [What good looks like]

   **Behavioral (STAR format):**
   - [Question] — [Competency assessed]

   **Culture Fit:**
   - [Question] — [What good looks like]

   **Candidate Questions:**
   [Potential questions from candidates and good answers]

5. EVALUATION RUBRIC

   | Competency | Definition | 1-Poor | 3-Good | 5-Excellent |
   |------------|------------|--------|--------|-------------|
   [For each key competency]

   **Overall Recommendation:**
   - Strong Hire: [Criteria]
   - Hire: [Criteria]
   - No Hire: [Criteria]

6. HIRING MANAGER PREP

   **Key Selling Points:**
   - [What makes this role attractive]

   **Anticipated Objections:**
   - [Objection] → [Response]

   **Competitive Positioning:**
   - How this compares to similar roles elsewhere

Make the job posting compelling and accurate. Make the internal documentation practical and usable.
```

---

### Step 4: Review and Refine
**Time: 10-15 minutes**

Check:
- Are requirements accurate?
- Is language inclusive?
- Does it represent the culture honestly?
- Are interview questions appropriate?
- Is the rubric fair and useful?

---

### Step 5: Customize for Channels
**Time: 5 minutes**

```
Create versions for different channels:

1. LINKEDIN POSTING
   - Character limit: 3,000
   - Include: Company snapshot, key responsibilities, requirements, apply link
   - Tone: Professional but engaging

2. CAREER PAGE VERSION
   - Full detail
   - Include: All sections, team photos mention, growth path

3. RECRUITER OUTREACH
   - Brief version for sourcing messages
   - Key hooks to attract passive candidates
   - 150 words max

4. INTERNAL REFERRAL
   - Version for employee sharing
   - Highlights why someone would want this job
   - Referral bonus mention
```

---

### Step 6: Generate Final Package
**Time: 2 minutes**

```
Create the final hiring package:

1. Job posting (external)
2. Role documentation (internal)
3. Screening guide (recruiter)
4. Interview kit (interviewers)
5. Offer talking points (hiring manager)
```

---

## Example Output

Below is an abbreviated job description example:

---

> **SENIOR PRODUCT MANAGER, ENTERPRISE**
>
> **CloudSync Pro | Remote (US) or San Francisco**
>
> ---
>
> ## About Us
>
> CloudSync Pro helps distributed teams collaborate without friction. Our software powers teamwork at 2,000+ companies, from fast-growing startups to Fortune 500 enterprises. We're 150 people, Series B funded, growing 50% year-over-year, and building toward profitability while still investing in product.
>
> We're a company where PMs have real ownership, decisions are made with data, and everyone is expected to be customer-obsessed. We value directness—you'll know where you stand and we'll want to know what you really think.
>
> ---
>
> ## About the Role
>
> We're looking for a Senior Product Manager to own our enterprise product line. Enterprise is our fastest-growing segment (80% YoY) and our largest customers are pushing us to build features that make CloudSync Pro the system of record for their organizations.
>
> This isn't a role where you'll be executing someone else's vision. You'll define what enterprise means for CloudSync Pro—working directly with Fortune 500 CIOs, partnering with our engineering teams, and shaping a product that handles the complexity of large organizations.
>
> The foundation is solid (our current enterprise PM built something customers love), but there's a significant roadmap ahead and real opportunity to make your mark.
>
> ---
>
> ## What You'll Do
>
> - **Own the enterprise roadmap:** Define priorities, make trade-offs, and ship features that drive enterprise revenue and retention
> - **Understand customers deeply:** Regular calls with enterprise customers, on-site visits, analysis of usage data—you'll be the expert on what large organizations need
> - **Write specs that engineers want to build:** Clear PRDs with context, not just requirements. You'll partner with engineering, not throw things over the wall
> - **Work cross-functionally:** Sales needs you on strategic deals. Customer Success needs you on retention. Leadership needs you in strategy discussions
> - **Track what matters:** Define metrics, build dashboards, and hold yourself accountable to outcomes, not outputs
>
> ---
>
> ## What You Bring
>
> **Required:**
> - 5+ years of product management experience, with at least 2 years in B2B SaaS
> - Experience building products for enterprise customers (understanding procurement, security requirements, and stakeholder complexity)
> - Technical fluency—you can have substantive conversations about APIs, integrations, and architecture (you don't need to code, but you need to understand)
> - Excellent communication skills—you'll write specs, present to executives, and negotiate priorities
> - Track record of shipping products that drove measurable business results
>
> **Nice to Have:**
> - Experience in collaboration, productivity, or workflow software
> - Familiarity with SOC 2, compliance features, and enterprise security requirements
> - Startup experience (you're comfortable with ambiguity and moving fast)
> - SQL skills (we're a data-driven team)
>
> ---
>
> ## What Success Looks Like
>
> **First 6 months:** You've taken full ownership of the enterprise roadmap, built relationships with key customers, and shipped your first major feature. You're the go-to expert on enterprise.
>
> **First year:** Enterprise NPS has improved. Revenue impact from features you've shipped is visible and measurable. Sales references your work in deals.
>
> **18 months:** The enterprise product is a competitive differentiator. You've helped define what "enterprise-grade" means for CloudSync Pro.
>
> ---
>
> ## What We Offer
>
> - **Compensation:** $150K-$180K base + equity (meaningful, not nominal)
> - **Benefits:** 100% covered health/dental/vision, 401k with 4% match
> - **Flexibility:** Remote-first (US-based) with optional SF office access
> - **Growth:** $2,000 annual learning budget, clear career paths
> - **Culture:** Unlimited PTO that people actually use, transparent communication, no politics
>
> ---
>
> ## Interview Process
>
> We respect your time. Here's what to expect:
>
> 1. **Recruiter screen** (30 min) — Tell us your story
> 2. **Hiring manager call** (45 min) — Deeper dive into experience
> 3. **Product case** (1 hr) — Present your thinking on a realistic problem
> 4. **Team interviews** (3 × 30 min) — Meet Engineering, Design, and Sales
> 5. **Final round** (1 hr) — VP Product + CEO
>
> We move quickly and communicate clearly throughout.
>
> ---
>
> ## Screening Criteria
>
> | Criteria | Must Have | Strong | Nice to Have |
> |----------|-----------|--------|--------------|
> | B2B SaaS PM experience | 2+ years | 4+ years | — |
> | Enterprise customer work | Some exposure | Primary focus | Fortune 500 |
> | Technical fluency | API/integration understanding | Technical background | Engineering degree |
> | Shipped products | Identifiable launches | Revenue impact | 0→1 experience |
>
> **Knockout Factors:**
> - No B2B experience (pure consumer background)
> - Cannot articulate product decisions with data
> - Poor communication in initial screens
>
> ---
>
> ## Interview Questions (Sample)
>
> **Experience:**
> - "Walk me through a product you shipped from concept to launch. What was your specific contribution?"
> - *Good answer: Specific role, data-driven decisions, measurable outcomes*
>
> **Technical:**
> - "One of our enterprise customers wants to integrate CloudSync with their existing SSO provider. Walk me through how you'd approach the requirements gathering and spec writing."
> - *Good answer: Asks clarifying questions, considers edge cases, thinks about user experience and technical constraints*
>
> **Behavioral:**
> - "Tell me about a time you had to make a product decision with incomplete data."
> - *Looking for: Framework for decision-making, comfort with ambiguity, learning from outcomes*
>
> **Culture:**
> - "Describe a situation where you disagreed with a stakeholder. How did you handle it?"
> - *Looking for: Directness, data-driven persuasion, ability to disagree and commit*
>
> ---
>
> ## Evaluation Rubric
>
> | Competency | 1-Poor | 3-Good | 5-Excellent |
> |------------|--------|--------|-------------|
> | Customer Insight | Can't articulate customer needs | Understands customer problems | Deep empathy, predicts needs |
> | Strategic Thinking | Tactical only | Balances short/long term | Clear vision, convincing |
> | Technical Fluency | Can't discuss technical topics | Conversant | Can go deep, credible with eng |
> | Communication | Unclear, unfocused | Clear and organized | Compelling, adapts to audience |
> | Execution | Describes, doesn't deliver | Ships regularly | Ships fast, high quality |
> | Culture Fit | Doesn't match values | Matches most values | Strong alignment, will thrive |

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Too many requirements | Wishlist instead of requirements | Ask: "Separate into must-have vs nice-to-have. What would truly disqualify someone?" |
| Generic description | Missing specifics | Add: "Include specific projects, tools, or outcomes. What will they actually do day-to-day?" |
| Boring posting | Corporate language | Ask: "Write conversationally. What would make someone excited about this role?" |
| Biased language | Unconscious bias | Ask: "Review for inclusive language. Remove gendered terms, aggressive language" |
| Unclear success criteria | No outcomes defined | Add: "What does success look like at 6, 12, and 18 months?" |

---

## Tips from Experience

1. **Separate requirements from preferences.** Ten "requirements" usually means two requirements and eight nice-to-haves.

2. **Show the work, not just the title.** "You'll lead enterprise strategy" beats "Senior Product Manager."

3. **Be honest about culture.** "Fast-paced" means different things—describe what it actually looks like.

4. **Include the hard parts.** Candidates appreciate knowing challenges; it builds trust.

5. **Make the process clear.** Ambiguity about next steps loses good candidates.

6. **Write for the candidate you want.** The best candidates have options—give them reasons to choose you.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Job posting attracts qualified applicants
- [ ] Hiring managers find documentation useful
- [ ] Interview process is consistent
- [ ] Time to create job descriptions decreases
- [ ] Quality of hire improves
- [ ] Candidate experience is positive

**Track over time:**
- Qualified applicant ratio
- Time to fill
- Offer acceptance rate
- New hire 90-day retention
- Hiring manager satisfaction
- Candidate feedback scores

---

## Variations

### Technical Role Job Description
For engineering, data, etc.:
```
Add emphasis on:
- Technical environment (stack, tools)
- Technical challenges and problems to solve
- Code review and technical quality expectations
- Career growth in technical track
- Interview format (take-home vs live coding)

Include: Day-in-the-life technical activities
```

### Executive Role Job Description
For VP/C-level positions:
```
Adjust for executive search:
- Strategic impact over task list
- P&L or team size context
- Board/investor interaction
- Leadership philosophy fit
- Compensation structure (base + bonus + equity)

Tone: More strategic, less tactical
```

### Entry-Level Job Description
For junior roles:
```
Adjust for early career:
- Emphasize growth and learning
- Reduce experience requirements
- Focus on potential indicators
- Describe mentorship and training
- Clarify what "entry-level" means

Avoid: Unrealistic experience requirements
```

### Internal Transfer Description
For internal mobility:
```
Adjust for internal candidates:
- What's different from current role
- How this advances their career
- Transferable skills valued
- Onboarding and transition support
- How to express interest

Include: Why consider this move
```

---

## Building Your Repeatable System

After several role descriptions, establish:

1. **Template library** by role family
2. **Standard competency frameworks**
3. **Interview question bank** by skill
4. **Evaluation rubrics** by level
5. **Channel-specific formatting**

**Sample Setup:**
```
job-descriptions/
├── templates/
│   ├── product-manager.md
│   ├── software-engineer.md
│   ├── sales-rep.md
│   └── [by role family]
├── active-roles/
│   ├── senior-pm-enterprise.md
│   └── [current openings]
├── interview-kits/
│   ├── competency-questions.md
│   ├── behavioral-questions.md
│   └── evaluation-rubrics.md
├── reference/
│   ├── inclusive-language-guide.md
│   ├── compensation-bands.md
│   └── benefits-summary.md
└── archive/
    └── [filled roles]
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**define requirements → structure documentation → create evaluation criteria**—applies broadly:

| Role | Application |
|------|-------------|
| **HR** | All hiring documentation |
| **Managers** | Team role definitions |
| **Consultants** | Engagement scoping |
| **Vendors** | RFP requirements |
| **Project Managers** | Resource requirements |
| **L&D** | Competency frameworks |

---

## Next Steps

1. **Identify the role:** What position needs documentation?
2. **Gather inputs:** Talk to hiring manager, review existing JDs
3. **Generate documentation:** Use this recipe
4. **Review for accuracy:** Validate with stakeholders
5. **Post and source:** Get it in front of candidates
6. **Iterate:** Improve based on applicant quality

---

*Recipe #61 of 100 in the Claude Code Knowledge Worker Recipe Collection*
