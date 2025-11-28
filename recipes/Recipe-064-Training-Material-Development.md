# Training Material Development

**Recipe #64: Transform Expertise into Effective Learning Experiences**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 10 minutes (first time) / 5 minutes (repeat) | 10-20 hours per course | Intermediate | L&D, HR, Trainers, Subject Matter Experts |

---

## The Problem

The expert knows everything but can't explain it simply. The trainer creates slides but they're boring. The content is good but there's no structure for learning. People sit through training and forget everything a week later. Creating effective training materials takes forever—so much that most internal training is thrown together at the last minute. And measuring whether anyone actually learned anything? Nobody has time for that.

**Pain Points:**
- Subject matter experts can't teach effectively
- Training materials take weeks to create
- Content is either too detailed or too superficial
- No assessment of whether learning happened
- Boring slides that people zone out during
- No connection between modules
- Materials that quickly become outdated

---

## The Outcome

Complete training curricula with learning objectives, structured content, engaging activities, assessments, and facilitator guides. Materials that transform expertise into effective learning experiences that people actually retain.

**What You'll Have When Done:**
- Learning objectives (measurable)
- Course outline and structure
- Module content
- Activities and exercises
- Assessment questions
- Facilitator guide
- Participant materials

---

## When to Use This Recipe

**Good Fit:**
- New employee onboarding
- Skills training programs
- Process and system training
- Compliance training
- Leadership development modules
- Knowledge transfer from experts

**Not a Good Fit:**
- Highly technical certification prep (specialized)
- External professional courses (different standards)
- Pure self-paced e-learning development (need tools)
- Legally mandated content (requires specific approach)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have subject matter content or SME access
- [ ] You know the target audience
- [ ] You understand the delivery format (live, virtual, self-paced)
- [ ] You have 60-120 minutes for course development

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Structures content for learning
- Creates learning objectives
- Develops assessment questions
- Writes facilitator guides
- Generates activities and exercises
- Organizes modules logically

**Where Human Judgment Is Essential:**
- Validating subject matter accuracy
- Adapting to audience needs
- Choosing appropriate activities
- Assessing cultural fit
- Testing and iterating
- Delivering the training

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Raw content | Expert knowledge, docs | Core material |
| Audience | Who will learn | Calibration |
| Format | Live, virtual, self-paced | Structure design |
| Duration | Time available | Scope planning |
| Outcomes | What they should do after | Objective setting |

**Sample Input:**
```
Training Development Request

TRAINING TOPIC: Product Knowledge for Sales Team
COMPANY: CloudSync Pro (B2B SaaS collaboration platform)

AUDIENCE:
- New sales reps (0-90 days tenure)
- 10-15 people per cohort
- Mixed experience (some B2B SaaS veterans, some new to tech)
- Need to demo product and answer customer questions

DELIVERY FORMAT:
- Live virtual sessions (Zoom)
- 3 sessions x 2 hours each
- Supplemental self-paced materials for reference

DESIRED OUTCOMES:
After this training, sales reps should be able to:
- Explain CloudSync's value proposition clearly
- Navigate the product to demo key features
- Answer common customer questions accurately
- Position against top 3 competitors
- Identify upsell/cross-sell opportunities

SUBJECT MATTER CONTENT:

Product Overview:
- CloudSync is a real-time collaboration platform
- Target customers: 50-5,000 employee companies
- Core use cases: document collaboration, project management, team communication
- Key differentiators: real-time sync, enterprise security, integrations ecosystem

Key Features:
- Document collaboration (real-time editing, version history, comments)
- Project spaces (folders, permissions, workflows)
- Team chat (channels, DMs, threads)
- Integrations (200+ apps, including Salesforce, Slack, Google)
- Enterprise features (SSO, admin controls, audit logs)

Pricing:
- Starter: $8/user/month (basic features)
- Professional: $15/user/month (advanced features)
- Business: $25/user/month (enterprise features)
- Enterprise: Custom pricing (full features + support)

Common Customer Questions:
- How does security work?
- What's the implementation timeline?
- How does it compare to [Competitor]?
- Can it integrate with our existing tools?
- What support is included?

Competitors:
- RivalSync: Lower price, fewer features
- WorkSpace Pro: More features, complex to use
- TeamFlow: Good for small teams, doesn't scale

CONSTRAINTS:
- Keep it interactive—no lectures
- Include practice time (demos, role plays)
- Create reference materials for ongoing use
- Assessments should be practical, not trivia
- Account for mixed experience levels
```

---

## Step-by-Step Implementation

### Step 1: Gather Content and Context
**Time: 10-15 minutes**

Collect:
- Subject matter content
- Audience profile
- Delivery constraints
- Desired outcomes
- Any existing materials

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Training Development Prompt
**Time: 5-10 minutes for Claude to process**

---

**PRIMARY PROMPT: Training Material Development**

```
Please develop comprehensive training materials for this program.

TOPIC: [Training topic]
AUDIENCE: [Who will learn]
FORMAT: [Delivery method and duration]

CONTENT:
[Paste subject matter content]

DESIRED OUTCOMES:
[What learners should be able to do after]

CONSTRAINTS:
[Any requirements or limitations]

CREATE THE FOLLOWING:

1. LEARNING OBJECTIVES

   **Terminal Objective:**
   [What learners will be able to do at course completion]

   **Enabling Objectives:**
   By the end of this training, participants will be able to:
   - [Objective 1 - measurable verb + content + condition]
   - [Objective 2]
   - [Objective 3]
   [5-8 objectives using Bloom's taxonomy verbs]

2. COURSE STRUCTURE

   **Course Overview:**
   | Module | Topic | Duration | Key Outcome |
   |--------|-------|----------|-------------|

   **Prerequisites:**
   - [What they need before starting]

   **Learning Path:**
   [Logical progression through modules]

3. MODULE CONTENT

   For each module:

   ---
   **MODULE [X]: [Title]**

   Duration: [Time]
   Objectives: [Specific to this module]

   **Content Outline:**
   1. [Topic 1]
      - Key points
      - Examples
   2. [Topic 2]
      - Key points
      - Examples

   **Key Concepts:**
   - [Concept 1]: [Definition/explanation]
   - [Concept 2]: [Definition/explanation]

   **Activity: [Activity Name]**
   - Type: [Discussion/practice/role-play/etc.]
   - Duration: [Time]
   - Instructions: [How to run it]
   - Debrief questions: [What to discuss after]

   **Transition to Next Module:**
   [How this connects to what's next]
   ---

4. FACILITATOR GUIDE

   **Before the Session:**
   - Materials needed: [List]
   - Technology setup: [Requirements]
   - Pre-work for participants: [If any]

   **Session Flow:**
   | Time | Activity | Facilitator Actions | Materials |
   |------|----------|---------------------|-----------|
   [Minute-by-minute guide]

   **Facilitation Tips:**
   - [Tip 1]
   - [Tip 2]

   **Common Challenges:**
   - [Challenge]: [How to handle]

   **Energy Management:**
   [When to take breaks, change activities]

5. PARTICIPANT MATERIALS

   **Pre-Work (if any):**
   [What to do before attending]

   **Handouts:**
   - [Handout 1]: [Description]
   - [Handout 2]: [Description]

   **Reference Guide:**
   [Quick reference for after training]

   **Job Aid:**
   [Tool for applying learning on the job]

6. ACTIVITIES AND EXERCISES

   **Activity 1: [Name]**
   Type: [Type]
   Duration: [Time]
   Materials: [What's needed]
   Setup: [How to prepare]
   Instructions:
   1. [Step 1]
   2. [Step 2]
   Debrief: [Questions to ask]
   Virtual Adaptation: [How to do remotely]

   [Repeat for each activity]

7. ASSESSMENTS

   **Knowledge Check Questions:**
   [Mix of formats - multiple choice, true/false, scenario-based]

   Question 1: [Question]
   A) [Option A]
   B) [Option B]
   C) [Option C]
   D) [Option D]
   Correct: [Answer] — Rationale: [Why]

   **Skill Assessment:**
   [Practical demonstration or role-play assessment]

   **Post-Training Assessment:**
   [How to measure if learning transferred to job]

8. SUPPLEMENTAL MATERIALS

   **Quick Reference Card:**
   [One-page summary of key points]

   **Glossary:**
   - [Term]: [Definition]

   **Additional Resources:**
   - [Resource 1]: [Where to find more]

9. EVALUATION

   **Reaction (Level 1):**
   Post-session survey questions

   **Learning (Level 2):**
   Assessment approach

   **Behavior (Level 3):**
   How to measure application on job

   **Results (Level 4):**
   Business metrics to track

Create engaging, practical content that leads to behavior change, not just information transfer.
```

---

### Step 4: Review and Customize
**Time: 15-20 minutes**

Review generated materials:
- Is content accurate?
- Are activities appropriate?
- Do assessments match objectives?
- Is timing realistic?

---

### Step 5: Adapt for Your Audience
**Time: 10 minutes**

```
Customize the training for these specifics:

AUDIENCE ADJUSTMENTS:
- Some attendees have X background, so: [Adjustment]
- Need more/less depth on: [Topic]

ACTIVITY MODIFICATIONS:
- Activity X should be changed to: [Modification]
- Add an activity for: [Topic]

ASSESSMENT CHANGES:
- Add questions about: [Topic]
- Make assessment more practical by: [Change]
```

---

### Step 6: Generate Final Package
**Time: 5 minutes**

```
Create the final training package:

1. FACILITATOR GUIDE (complete)
2. PARTICIPANT WORKBOOK
3. PRESENTATION SLIDES (outline)
4. ACTIVITY INSTRUCTIONS
5. ASSESSMENT PACKAGE
6. QUICK REFERENCE CARD
7. EVALUATION FORMS
```

---

## Example Output

Below is an abbreviated training development example:

---

> **PRODUCT KNOWLEDGE FOR SALES**
>
> **CloudSync Pro | New Sales Rep Training**
>
> ---
>
> ## Learning Objectives
>
> **Terminal Objective:**
> After completing this training, sales reps will be able to conduct effective CloudSync product demonstrations and answer customer questions accurately, demonstrating proficiency through a live demo assessment.
>
> **Enabling Objectives:**
>
> By the end of this training, participants will be able to:
>
> 1. **Explain** CloudSync's value proposition in terms of customer outcomes
> 2. **Navigate** the CloudSync interface to demonstrate key features
> 3. **Demonstrate** the top 5 use cases customers care about most
> 4. **Answer** the 10 most common customer questions accurately
> 5. **Differentiate** CloudSync from top 3 competitors with specific proof points
> 6. **Identify** upsell and cross-sell opportunities within customer conversations
> 7. **Handle** objections using the problem-agitate-solve framework
>
> ---
>
> ## Course Structure
>
> | Session | Topic | Duration | Key Outcome |
> |---------|-------|----------|-------------|
> | Session 1 | Value Proposition & Platform Overview | 2 hours | Explain CloudSync's value |
> | Session 2 | Product Deep Dive & Demo Skills | 2 hours | Demo key features |
> | Session 3 | Competitive Positioning & Practice | 2 hours | Handle real conversations |
>
> **Total:** 6 hours live training + 1 hour self-paced materials
>
> **Prerequisites:**
> - Completed company onboarding
> - Access to CloudSync demo environment
> - Reviewed competitor websites (30 min pre-work)
>
> ---
>
> ## Module 1: Value Proposition & Platform Overview
>
> **Duration:** 2 hours
> **Objectives:** Explain CloudSync's value; navigate the platform; understand target customers
>
> ---
>
> ### 1.1 Why CloudSync Exists (20 min)
>
> **Key Concepts:**
>
> - **The Collaboration Problem:** Teams waste 20% of time on version control, finding files, and communication gaps
> - **The CloudSync Solution:** Real-time collaboration that brings documents, projects, and communication together
> - **The Result:** Teams ship faster with fewer errors and less frustration
>
> **Key Message Framework:**
>
> "CloudSync helps [company type] teams [do what] so they can [achieve what outcome]."
>
> Example: "CloudSync helps growing marketing teams collaborate on campaigns in real-time so they can launch faster with fewer errors."
>
> **Activity: Value Proposition Practice** (10 min)
>
> - Type: Pair exercise
> - Instructions:
>   1. Pair up with a partner
>   2. Each person practices the value proposition for a different customer type
>   3. Partner provides feedback: Was it clear? Compelling? Customer-focused?
> - Debrief: What made some statements more compelling than others?
>
> ---
>
> ### 1.2 Target Customers & Use Cases (25 min)
>
> **Ideal Customer Profile:**
> - Company size: 50-5,000 employees
> - Multiple teams or locations
> - Document-heavy work
> - Outgrown basic file sharing
> - Budget authority at department or company level
>
> **Top 5 Use Cases:**
>
> 1. **Document Collaboration:** Multiple people editing the same document without version confusion
> 2. **Project Spaces:** Organizing work by project with the right people having the right access
> 3. **Team Communication:** Chat that's connected to documents and projects
> 4. **External Sharing:** Working with clients or partners securely
> 5. **Enterprise Control:** IT/Admin visibility and security controls
>
> **Activity: Use Case Matching** (10 min)
>
> - Type: Small group exercise
> - Instructions:
>   1. Each group gets 3 customer scenarios (on cards)
>   2. Match each scenario to the primary use case it represents
>   3. Discuss: What questions would you ask to uncover this need?
> - Debrief: Share the best discovery questions
>
> ---
>
> ### 1.3 Platform Navigation (30 min)
>
> **Demo Environment Tour:**
>
> Live walkthrough of key areas:
> - Dashboard and navigation
> - Creating and organizing spaces
> - Document creation and collaboration
> - Chat and communication
> - Admin console basics
>
> **Activity: Scavenger Hunt** (15 min)
>
> - Type: Individual hands-on
> - Instructions:
>   1. Complete the 10-task scavenger hunt in the demo environment
>   2. Tasks include: Create a space, invite a user, share a document, start a chat
>   3. First 3 to complete all tasks wins CloudSync swag
> - Purpose: Ensure everyone can navigate the basics
>
> ---
>
> ### 1.4 Session 1 Wrap-Up (15 min)
>
> **Key Takeaways:**
> 1. Lead with customer outcomes, not features
> 2. Know which use cases match which customer types
> 3. Be comfortable navigating the platform before you demo
>
> **Knowledge Check:** (5 min quiz in chat)
>
> **Pre-Work for Session 2:**
> - Complete the demo environment certification (30 min)
> - Review the "Top 10 Customer Questions" document
>
> ---
>
> ## Module 2: Product Deep Dive & Demo Skills
>
> **Duration:** 2 hours
> **Objectives:** Demo key features; answer common questions; handle the "show me" moments
>
> ---
>
> ### 2.1 Demo Best Practices (15 min)
>
> **The SELL Demo Framework:**
>
> - **S - Situation:** Start with customer's situation (not product features)
> - **E - Explain:** Explain what you'll show and why it matters to them
> - **L - Live Demo:** Show the feature in action
> - **L - Link:** Link back to their specific situation/pain
>
> **Demo Don'ts:**
> - Don't show everything—show what matters to THIS customer
> - Don't click around aimlessly—know your path
> - Don't talk about features—talk about outcomes
> - Don't ignore questions—address them, then return to flow
>
> ---
>
> ### 2.2 Feature Deep Dives (45 min)
>
> **For each key feature:**
>
> **Document Collaboration:**
> - What it does: Real-time co-editing with presence indicators
> - Customer problem it solves: "Which version is latest?" confusion
> - Demo path: Create doc → invite user → show simultaneous editing → version history
> - Wow moment: "See how you can see Sarah's cursor moving in real-time?"
> - Common questions: How does it work offline? How many people can edit at once?
>
> **[Similar breakdown for other features...]**
>
> **Activity: Demo Practice Rounds** (25 min)
>
> - Type: Triads (3 people)
> - Instructions:
>   1. Person A demos document collaboration (5 min)
>   2. Person B plays customer, asks questions
>   3. Person C observes and provides feedback
>   4. Rotate until everyone has demoed
> - Feedback focus: Did they use SELL framework? Were they confident? Did they handle questions?
>
> ---
>
> ### 2.3 Common Customer Questions (30 min)
>
> **Top 10 Questions & Answers:**
>
> 1. **"How does security work?"**
>    - Answer: "CloudSync is SOC 2 Type II certified with bank-grade encryption. Your data is encrypted in transit and at rest. For enterprise, we also support SSO and detailed audit logs."
>    - If they probe deeper: Offer to connect them with security team for detailed review
>
> 2. **"What's the implementation timeline?"**
>    - Answer: "Most teams are up and running in a day. For enterprise with SSO and integrations, plan for 2-4 weeks. We provide dedicated onboarding support."
>    - Key point: Quick to value, thorough for complex needs
>
> **[Continue for all 10 questions...]**
>
> **Activity: Question Rapid Fire** (10 min)
>
> - Type: Game
> - Instructions:
>   1. Facilitator asks questions rapid-fire (15 seconds per answer)
>   2. Popcorn-style: anyone can answer
>   3. Group validates if answer was accurate and complete
> - Purpose: Build confidence in handling common questions
>
> ---
>
> ## Assessments
>
> ### Knowledge Check (Post-Session 2)
>
> **Multiple Choice:**
>
> 1. What is the primary differentiator of CloudSync vs. competitors?
>    A) Lower price
>    B) Real-time sync with enterprise security
>    C) More features
>    D) Better customer support
>    **Correct: B** — This is our positioning and core value prop.
>
> 2. A customer asks: "How does CloudSync compare to RivalSync?" The best response is:
>    A) "RivalSync is cheaper but has fewer features"
>    B) "Let me understand what's most important to you first, then I can explain the differences that matter"
>    C) "CloudSync is better in every way"
>    D) "I don't know much about RivalSync"
>    **Correct: B** — Always qualify before positioning; focus on what matters to them.
>
> **Scenario-Based:**
>
> 3. A prospect says: "We're using Google Docs and it's free. Why would we pay for CloudSync?"
>
>    Write your response: _______________________
>
>    **Good answer includes:** Acknowledging Google Docs works for basics, asking about their pain points (permissions, organization, enterprise control), positioning CloudSync for growing teams that need more structure and security.
>
> ---
>
> ### Practical Assessment: Live Demo
>
> **Assessment Scenario:**
>
> You're meeting with a Marketing Director at a 200-person company. They're frustrated because:
> - Campaign assets live in multiple places
> - External agencies need access but IT worries about security
> - They can't track who changed what
>
> **Task:** Deliver a 10-minute demo that addresses their needs.
>
> **Evaluation Criteria:**
>
> | Criterion | 1-Needs Work | 3-Meets | 5-Exceeds |
> |-----------|--------------|---------|-----------|
> | Customer Focus | Showed generic demo | Customized to stated needs | Anticipated unstated needs |
> | Product Knowledge | Struggled with navigation | Confident navigation | Smooth, natural demo |
> | SELL Framework | Didn't use structure | Used framework | Framework + personalization |
> | Question Handling | Couldn't answer questions | Answered accurately | Answered and pivoted well |
> | Overall Impact | Wouldn't advance deal | Would advance deal | Would create urgency |
>
> **Pass Threshold:** Average of 3 or higher across all criteria
>
> ---
>
> ## Facilitator Guide: Session 1
>
> **Before Session:**
> - [ ] Demo environment access confirmed for all participants
> - [ ] Breakout rooms set up (pairs and triads)
> - [ ] Scavenger hunt tasks prepared
> - [ ] Knowledge check poll ready
>
> **Session Flow:**
>
> | Time | Activity | Facilitator Actions | Materials |
> |------|----------|---------------------|-----------|
> | 0:00 | Welcome | Intro, objectives, icebreaker | Slides 1-3 |
> | 0:10 | Why CloudSync | Present problem/solution | Slides 4-8 |
> | 0:25 | Value Prop Practice | Assign pairs, monitor, debrief | Pair assignment |
> | 0:40 | Target Customers | Present ICP and use cases | Slides 9-15 |
> | 1:00 | Use Case Matching | Distribute scenarios, group work | Scenario cards |
> | 1:15 | Platform Navigation | Live demo walkthrough | Demo environment |
> | 1:35 | Scavenger Hunt | Release tasks, support, recognize winners | Task sheet |
> | 1:50 | Wrap-Up | Key takeaways, pre-work, Q&A | Slides 16-18 |
>
> **Facilitation Tips:**
> - Energy dips around 1:00—that's why the group activity is there
> - If someone struggles in pair exercise, partner them with a stronger participant
> - For the scavenger hunt, have a leaderboard visible to create excitement
>
> **Common Challenges:**
> - Demo environment is slow: Have backup screenshots ready
> - Mix of experience levels: Pair veterans with newbies in activities
> - Questions going off-track: Park for later, "Great question—we'll cover that in Session 3"

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Content too dense | Too much information | Ask: "Prioritize the 20% of content that delivers 80% of value. What can be reference material instead?" |
| Activities feel forced | Not connected to objectives | Ask: "Each activity should practice a specific skill. What skill does this activity build?" |
| Assessment doesn't match objectives | Disconnect between design | Ask: "For each objective, what would evidence of mastery look like? Design assessment from there." |
| Timing unrealistic | Too much content | Ask: "What's the minimum viable version? What can be cut or moved to self-paced?" |
| Boring delivery | Lecture-heavy | Ask: "Maximum 10 minutes of presentation before an interaction. Add more activities." |

---

## Tips from Experience

1. **Tell them, show them, let them practice.** The ratio should be 30% content, 70% application.

2. **Start with the job.** What will they actually DO? Design backward from that.

3. **Small chunks beat big ones.** 15-20 minute segments with transitions work better than hour-long lectures.

4. **Practice trumps theory.** People remember what they did, not what they heard.

5. **Make failure safe.** Practice environments should encourage mistakes.

6. **Follow up matters.** Training without reinforcement has 10% retention. Build in follow-up.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Learners can demonstrate competency
- [ ] Skills transfer to the job
- [ ] Business metrics improve
- [ ] Training development time decreases
- [ ] Facilitator feedback is positive
- [ ] Learner satisfaction is high

**Track over time:**
- Assessment pass rates
- Time to competency
- Manager feedback on skill application
- Business metrics (e.g., sales conversion)
- Training satisfaction scores
- Time to develop new trainings

---

## Variations

### Compliance Training
For required training:
```
Focus on:
- Regulatory requirements coverage
- Documentation and attestation
- Knowledge checks for compliance
- Scenario-based ethical decisions
- Record keeping

Include: Completion tracking, audit trail
```

### Leadership Development
For management training:
```
Focus on:
- Self-reflection and assessment
- Case studies and discussions
- Role-play for difficult conversations
- Action planning and commitments
- Peer learning and feedback

Include: Pre-work assessments, coaching integration
```

### Technical Skills Training
For system or tool training:
```
Focus on:
- Hands-on lab exercises
- Step-by-step procedures
- Troubleshooting scenarios
- Reference documentation
- Sandbox environments

Include: Checklists, job aids, troubleshooting guides
```

### Blended Learning Program
For multi-modal delivery:
```
Design for:
- Pre-work (self-paced)
- Live session (instructor-led)
- Practice (on the job)
- Reinforcement (follow-up)
- Assessment (demonstration)

Include: Learning path, touchpoint schedule
```

---

## Building Your Repeatable System

After several training programs, establish:

1. **Template library** by training type
2. **Activity bank** for reuse
3. **Assessment question pool**
4. **Facilitator certification process**
5. **Evaluation framework**

**Sample Setup:**
```
training-development/
├── programs/
│   ├── product-knowledge-sales/
│   │   ├── facilitator-guide.md
│   │   ├── participant-materials.md
│   │   ├── assessments.md
│   │   └── slides/
│   └── [by program]
├── templates/
│   ├── module-template.md
│   ├── activity-template.md
│   └── assessment-template.md
├── resources/
│   ├── activity-bank.md
│   ├── icebreakers.md
│   └── debrief-questions.md
├── evaluation/
│   ├── survey-templates.md
│   └── metrics-tracking.md
└── facilitator-resources/
    ├── facilitation-tips.md
    └── certification-checklist.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**define outcomes → structure content → build practice → assess mastery**—applies broadly:

| Role | Application |
|------|-------------|
| **L&D** | All training development |
| **Managers** | Team skill building |
| **SMEs** | Knowledge transfer |
| **Onboarding** | New hire programs |
| **Customer Success** | Customer training |
| **Partners** | Channel enablement |

---

## Next Steps

1. **Identify the need:** What skill gap are you addressing?
2. **Gather content:** Get SME input, existing materials
3. **Define outcomes:** What should learners DO after?
4. **Develop materials:** Use this recipe
5. **Pilot and iterate:** Test with a small group, refine
6. **Roll out and measure:** Deploy, track results

---

*Recipe #64 of 100 in the Claude Code Knowledge Worker Recipe Collection*
