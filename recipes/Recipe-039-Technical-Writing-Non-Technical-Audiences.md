# Technical Writing for Non-Technical Audiences

**Recipe #39: From Complex to Clear Without Losing Accuracy**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 10 minutes (first time) / 5 minutes (repeat) | 2-4 hours per document | Intermediate | Technical Writers, Product Managers, Engineers, Consultants |

---

## The Problem

You understand the technical details, but your audience doesn't—and they don't need to. Executives want the business impact, not the architecture. Customers want to know what it does, not how it works. Sales needs to explain features without a CS degree. But every time you simplify, something gets lost in translation or becomes technically inaccurate. The result is either content that's too complex or content that's so dumbed down it's misleading.

**Pain Points:**
- Technical accuracy vs. accessibility tension
- "Explain it like I'm five" goes too far
- Key nuance gets lost in simplification
- Different audiences need different depths
- SMEs can't write for non-experts
- Non-experts can't verify technical accuracy
- Content takes forever to get right

---

## The Outcome

Clear, accessible technical content that remains accurate. Documents that non-technical readers can understand and act on, while technical reviewers confirm nothing is wrong. Multiple versions calibrated for different audience technical levels.

**What You'll Have When Done:**
- Simplified but accurate technical explanation
- Appropriate analogies and examples
- Content calibrated to audience level
- Key concepts explained without jargon
- Technical accuracy preserved
- Multiple versions for different audiences

---

## When to Use This Recipe

**Good Fit:**
- Product documentation for end users
- Executive briefings on technical topics
- Sales enablement materials
- Customer-facing feature explanations
- Board presentations on technical initiatives
- Training materials for non-technical staff
- Technical blog posts for general audiences

**Not a Good Fit:**
- Developer documentation (needs technical depth)
- API references (technical audience)
- Engineering specs (wrong audience)
- Compliance documentation (has specific requirements)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have the technical content to simplify
- [ ] You know your target audience's technical level
- [ ] You understand what decisions/actions the audience needs to make
- [ ] You have 1-2 hours for content development

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Identifies jargon and technical terms
- Suggests accessible analogies
- Calibrates explanation depth
- Maintains technical accuracy while simplifying
- Creates multiple versions for different audiences
- Structures information for clarity

**Where Human Judgment Is Essential:**
- Technical accuracy verification
- Audience understanding assessment
- What level of simplification is appropriate
- Which nuances matter vs. can be omitted
- Analogy appropriateness
- Final approval

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Technical content | Specs, docs, explanations | Source material |
| Audience profile | Who's reading, their background | Calibration |
| Purpose | What reader needs to do/decide | Focus |
| Current docs | Existing materials | Style matching |
| Problem examples | Where current docs fail | Gap identification |

**Sample Input:**
```
Technical Writing Request

TECHNICAL CONTENT TO SIMPLIFY:

Our new authentication system uses OAuth 2.0 with PKCE (Proof Key for Code Exchange)
for mobile applications. This eliminates the need for client secrets in native apps
while maintaining security against authorization code interception attacks. The flow
involves generating a cryptographically random code verifier, creating a code challenge
using SHA-256 hashing, and including this challenge in the authorization request.
When exchanging the authorization code for tokens, the original code verifier is sent,
allowing the authorization server to verify the challenge matches.

Key features:
- Supports both S256 and plain challenge methods (S256 recommended)
- Refresh tokens use rotation with automatic revocation of compromised tokens
- Access tokens are JWTs with configurable expiration (default 1 hour)
- Supports OIDC for identity verification alongside OAuth for authorization

AUDIENCE: Sales team preparing for customer conversations

AUDIENCE TECHNICAL LEVEL: Low - comfortable with basic concepts like "login" and
"security" but don't understand cryptography, tokens, or authentication protocols

WHAT AUDIENCE NEEDS TO DO:
- Explain to customers why our mobile app login is secure
- Answer basic customer security questions
- Know when to bring in technical resources
- Differentiate our approach from competitors (some use less secure methods)

WHAT THEY DON'T NEED TO KNOW:
- How to implement it
- The cryptographic details
- Protocol specifications

OUTPUT NEEDED:
1. One-pager explanation for sales team
2. Customer-facing talking points
3. FAQ for common customer questions
4. Competitive differentiation points
```

---

## Step-by-Step Implementation

### Step 1: Define Audience and Purpose
**Time: 5-10 minutes**

Get crystal clear on:
- Who's reading this?
- What's their technical background?
- What do they need to DO with this information?
- What decisions do they need to make?
- What can be safely omitted vs. must be included?

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Technical Simplification Prompt
**Time: 5-7 minutes for Claude to process**

---

**PRIMARY PROMPT: Technical Writing for Non-Technical Audiences**

```
Please help me translate technical content for a non-technical audience.

TECHNICAL CONTENT:
"""
[PASTE YOUR TECHNICAL CONTENT HERE]
"""

AUDIENCE:
- Who: [Who will read this]
- Technical level: [None / Basic / Some / Moderate]
- Background: [What they already understand]
- Role: [Their job/context]

PURPOSE:
- What they need to DO with this information: [Actions/decisions]
- What they need to UNDERSTAND: [Key concepts]
- What they DON'T need to know: [Can be omitted]

OUTPUT FORMAT: [One-pager / FAQ / Presentation / Training material]

PLEASE CREATE:

1. SIMPLIFIED EXPLANATION
   Rewrite the technical content for this audience:
   - Replace jargon with plain language
   - Use analogies where helpful
   - Focus on "what it does" and "why it matters"
   - Preserve technical accuracy
   - Keep only what audience needs to know

2. KEY CONCEPTS GLOSSARY
   For any technical terms that must be used:
   - Term: Plain-language definition
   - Why it matters to the reader

3. ANALOGIES AND EXAMPLES
   Provide 2-3 relatable analogies that explain core concepts
   - Analogy
   - What it explains
   - Limitations of the analogy (where it breaks down)

4. WHAT THIS MEANS FOR [AUDIENCE]
   Translate into their context:
   - Impact on their work
   - What they can tell others
   - What to watch out for

5. COMMON QUESTIONS
   FAQ with non-technical questions this audience might ask:
   - Question (in their words)
   - Answer (in plain language)

6. ACCURACY CHECK
   Note any simplifications that trade precision for clarity:
   - What was simplified
   - What's technically more nuanced
   - Whether this matters for this audience

7. ESCALATION TRIGGERS
   When this audience should bring in technical experts:
   - Questions they shouldn't try to answer
   - Situations requiring technical depth

Keep it accurate but accessible. The goal is understanding, not expertise.
```

---

### Step 4: Verify Technical Accuracy
**Time: 10-15 minutes**

Review the simplified version:
- Is anything technically wrong?
- Are the analogies accurate enough?
- Does the simplification introduce misconceptions?
- Are the right things emphasized?

---

### Step 5: Refine for Audience
**Time: 10-15 minutes**

**To adjust complexity level:**
```
This is still too technical. The audience won't know what "tokens" means. Replace with something more familiar like "temporary access passes" and explain further.
```

**To improve analogies:**
```
The key analogy isn't quite right—it implies [misconception]. Can you find a better analogy that avoids this, or clarify the limitation?
```

**To add missing context:**
```
Add a section on why this matters for customer trust. The sales team needs to explain the "so what" to customers who ask about security.
```

**To check accuracy:**
```
Double-check: Is it accurate to say [simplified statement]? Or does that oversimplify in a misleading way?
```

---

### Step 6: Create Audience-Specific Versions
**Time: 10 minutes**

```
Create versions for different audiences:

1. EXECUTIVE VERSION (1 paragraph)
   - Business impact only
   - No technical details
   - Focus on: secure, competitive, trustworthy

2. SALES TEAM VERSION (1 page)
   - What to tell customers
   - How to answer questions
   - When to escalate

3. CUSTOMER-FACING VERSION (FAQ format)
   - Questions customers actually ask
   - Answers that build confidence
   - No unnecessary complexity

4. INTERNAL TRAINING VERSION (detailed)
   - More context for internal teams
   - Background on why we chose this approach
   - How it compares to alternatives

For each version, maintain accuracy while adjusting depth.
```

---

## Example Output

Below is an abbreviated technical simplification example:

---

> **SIMPLIFIED EXPLANATION: Mobile App Security (For Sales Team)**
>
> ---
>
> ## What It Is (One Sentence)
>
> Our mobile app uses an industry-standard security system that protects customer logins even if someone intercepts the connection.
>
> ---
>
> ## How It Works (No Technical Jargon)
>
> When a customer logs in on their phone:
>
> 1. **The app creates a unique "key"** — Think of this like a one-time secret code that only your app and our servers know.
>
> 2. **The login happens with that key** — The customer enters their username and password, but there's also this invisible key protecting everything.
>
> 3. **Even if someone intercepts the login, they can't use it** — Without the original key (which never leaves the phone), intercepted data is useless.
>
> The result: Customer credentials stay safe, even on public WiFi or compromised networks.
>
> ---
>
> ## Why This Matters to Customers
>
> **"Is my data safe on your app?"**
>
> Yes. We use the same security standard that Google, Microsoft, and major banks use for their mobile apps. It's called OAuth 2.0 with something called PKCE (you don't need to remember that—just know it's the current best practice for mobile security).
>
> **What makes it better than older methods:**
> - Older apps stored a "secret password" in the app itself — if someone reverse-engineered the app, they could steal it
> - Our approach doesn't store any secrets in the app — there's nothing to steal
>
> ---
>
> ## The Analogy: Hotel Key Cards
>
> Think of it like a hotel key card system:
>
> - Your room key only works for YOUR room, during YOUR stay
> - If someone copies your key card, it stops working (we detect the copy and invalidate it)
> - The hotel never gives you the master key — just temporary access to what you need
>
> Our login works the same way: temporary, limited, and automatically revoked if something seems wrong.
>
> **Where this analogy breaks down:** Unlike a physical key card, our system also verifies WHO is using it, not just whether the key is valid.
>
> ---
>
> ## What Sales Needs to Know
>
> **Say this to customers:**
> - "We use the same mobile security standard as Google and major banks"
> - "Your credentials are protected even on public WiFi"
> - "We follow industry best practices—no shortcuts on security"
>
> **Don't say this (it's wrong or misleading):**
> - "It's impossible to hack" (nothing is impossible—it's just very, very hard)
> - "We invented a new security system" (we use proven standards, which is actually better)
>
> **When to bring in a technical resource:**
> - Customer has a dedicated security team with detailed questions
> - Customer asks about compliance certifications (SOC 2, etc.)
> - Customer wants to see documentation or audit our approach
> - Anything about "encryption algorithms" or "key lengths"
>
> ---
>
> ## FAQ: Questions Customers Actually Ask
>
> **Q: "What happens if my phone is stolen?"**
> A: "The thief can't access your account without your login credentials. And if you report the phone lost, we can immediately revoke any active sessions—they're locked out even if they somehow had your password."
>
> **Q: "Is this more secure than [competitor]?"**
> A: "Many competitors still use older methods that store secrets in the app itself. We use the current best practice that doesn't require storing any secrets. It's the same approach Google and Microsoft use for their mobile apps."
>
> **Q: "Can you explain how the encryption works?"**
> A: "I'd be happy to connect you with our security team for the technical details. The short version: we use industry-standard encryption that's verified by third-party security audits."
>
> **Q: "What about if someone hacks your servers?"**
> A: "Our security is designed with that scenario in mind. We don't store passwords—we store encrypted versions that can't be reversed. And the mobile login system has additional layers that protect even if a breach occurred."
>
> ---
>
> ## Accuracy Notes
>
> **Simplifications made:**
>
> | What we said | What's technically true | Does it matter here? |
> |--------------|------------------------|---------------------|
> | "Key that never leaves the phone" | The code verifier is sent during token exchange | No—the point is it's never exposed to interception |
> | "Same as Google uses" | Google uses OAuth 2.0 + PKCE | Accurate enough for credibility |
> | "Automatically revoked if something seems wrong" | Refresh token rotation with revocation | No—the outcome is what matters |
>
> These simplifications are appropriate for sales conversations. For technical customers, bring in engineering.
>
> ---
>
> ## Competitive Differentiation
>
> | Us | Many Competitors |
> |----|------------------|
> | PKCE flow (no secrets in app) | Client secrets embedded in app |
> | Refresh token rotation | Static refresh tokens |
> | Current OAuth 2.0 best practices | Older OAuth implementations |
>
> **Plain English:** "We use the newest, most secure approach. Some competitors cut corners with older methods because they're easier to implement."

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Still too technical | Jargon remains | Ask: "A reader with zero technical background should understand this. Remove all jargon" |
| Oversimplified to inaccuracy | Went too far | Ask: "Is [statement] accurate enough, or does it mislead? Find the simplest accurate version" |
| Analogies don't land | Wrong domain | Ask: "Find an analogy from [audience's field] instead of [current domain]" |
| Missing the "so what" | Focus on mechanism | Ask: "Why should the reader care? Lead with impact, not how it works" |
| Too long | Over-explaining | Ask: "What's the minimum they need to know? Cut everything else" |
| Different versions inconsistent | Independent creation | Ask: "Ensure all versions are consistent—same core facts, different depth" |

---

## Tips from Experience

1. **Lead with "why it matters," not "how it works."** Non-technical readers care about impact first.

2. **Use their vocabulary.** If your audience says "login" not "authentication," use "login."

3. **Analogies are powerful but dangerous.** Always note where they break down, so readers don't over-extend them.

4. **Technical accuracy ≠ technical completeness.** You can be accurate without including everything.

5. **Test with a real non-technical person.** Read it to someone outside your field. Where they look confused, simplify more.

6. **Create escalation paths.** It's okay for simplified content to say "ask a technical expert for details."

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Non-technical audience understands the content
- [ ] Technical reviewers confirm accuracy
- [ ] Audience can take appropriate action
- [ ] Questions to technical team decrease for covered topics
- [ ] Content is used and referenced

**Track over time:**
- Reader comprehension (can they explain it back?)
- Technical accuracy feedback
- Reduction in clarifying questions
- Usage of simplified materials
- Time saved vs. custom explanations

---

## Variations

### Executive Briefing
For C-level technical summaries:
```
Translate this technical topic for an executive briefing.

Technical content:
[Paste content]

Executive audience:
- Time: 2-3 minutes to read
- Focus: Business impact, risk, investment needed
- No interest in: Implementation details

Create:
1. One-paragraph summary (what and why it matters)
2. Business impact statement
3. Risk summary (what could go wrong)
4. Investment/decision needed
5. One slide if presenting
```

### Customer Documentation
For end-user guides:
```
Translate this technical feature for customer documentation.

Technical content:
[Feature specification]

Customer audience:
- End users of the product
- Varied technical levels
- Need to USE, not understand deeply

Create:
1. Feature overview (what it does)
2. Step-by-step how to use it
3. Common questions
4. Troubleshooting basics
5. When to contact support
```

### Training Material
For internal non-technical staff:
```
Create training material from this technical content.

Technical content:
[Paste content]

Training audience: [Department/role]
Learning objective: [What they should be able to do after]

Create:
1. Key concepts (5-7 bullet points)
2. Common scenarios and how to handle
3. Practice questions/scenarios
4. Quick reference card
5. Knowledge check questions
```

### Sales Enablement
For sales team technical prep:
```
Create sales enablement content from this technical material.

Technical content:
[Paste content]

Sales needs:
- Customer-facing talking points
- Competitive differentiation
- Objection handling
- When to bring in technical resources

Create:
1. One-pager for sales
2. Customer FAQ
3. Competitive positioning
4. Demo talking points
5. Technical escalation triggers
```

---

## Building Your Repeatable System

After several translations, build your system:

1. **Create audience profiles** for common targets
2. **Build analogy library** of proven explanations
3. **Document accuracy guidelines** for different contexts
4. **Maintain glossary** of approved simplifications
5. **Track what works** with different audiences

**Sample Setup:**
```
technical-writing/
├── audience-profiles/
│   ├── executives.md
│   ├── sales-team.md
│   ├── customers.md
│   └── non-technical-staff.md
├── translations/
│   ├── security-features/
│   │   ├── oauth-explanation.md
│   │   ├── encryption-basics.md
│   │   └── compliance-overview.md
│   └── product-features/
│       ├── [feature-translations]/
├── resources/
│   ├── analogy-library.md
│   ├── approved-simplifications.md
│   └── glossary.md
└── templates/
    ├── executive-briefing.txt
    ├── customer-doc.txt
    └── sales-enablement.txt
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**understand audience level → translate to appropriate depth → preserve accuracy → calibrate for action**—applies broadly:

| Role | Application |
|------|-------------|
| **Technical Writers** | All user-facing documentation |
| **Product Managers** | Stakeholder communications |
| **Engineers** | Explaining work to non-technical teams |
| **Consultants** | Client deliverables |
| **Sales Engineers** | Customer-facing technical content |
| **Trainers** | Technical onboarding |

---

## Next Steps

1. **Identify your audience:** Who needs to understand this?
2. **Gather technical content:** What needs translation?
3. **Define purpose:** What will they DO with this understanding?
4. **Generate simplified version:** Use this recipe
5. **Verify accuracy:** Have technical reviewer confirm
6. **Test with real audience:** Does it actually work?

---

*Recipe #39 of 100 in the Claude Code Knowledge Worker Recipe Collection*
