# Interview Question Banks and Scorecards

**Recipe #62: Build Structured Interviews That Predict Success**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 5 minutes (first time) / 2 minutes (repeat) | 2-3 hours per role | Beginner | HR, Recruiters, Hiring Managers, Interviewers |

---

## The Problem

Interviews are inconsistent. Different interviewers ask different questions. Some candidates get softballs; others get grilled. Evaluations are based on "gut feeling" rather than evidence. Bias creeps in because there's no structure. After a full interview loop, the team can't compare notes because everyone assessed different things. And without proper questions, you learn what candidates rehearsed, not whether they can do the job.

**Pain Points:**
- Interviewers make up questions on the fly
- No consistency across candidates
- "Gut feeling" evaluations with no evidence
- Bias in unstructured interviews
- Can't compare candidates fairly
- Miss critical competencies
- Strong interviewers mask weak candidates

---

## The Outcome

Comprehensive interview question banks organized by competency, with follow-up probes and evaluation criteria. Structured scorecards that enable consistent, fair, evidence-based hiring decisions. Interview guides that help any interviewer assess candidates effectively.

**What You'll Have When Done:**
- Question bank by competency
- Behavioral questions with follow-ups
- Technical/functional questions
- Evaluation scorecards
- Interviewer guides
- Debrief frameworks

---

## When to Use This Recipe

**Good Fit:**
- Setting up structured interviews
- Standardizing hiring across teams
- Training new interviewers
- Preparing for high-volume hiring
- Improving interview quality
- Reducing bias in hiring

**Not a Good Fit:**
- Highly specialized technical assessments (need SME)
- Executive conversations (different format)
- Casual networking conversations
- Reference checks (different approach)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have defined the competencies for the role
- [ ] You know the interview format (rounds, interviewers)
- [ ] You understand what success looks like in the role
- [ ] You have 20-30 minutes for complete kit development

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Generates behavioral questions (STAR format)
- Creates follow-up probes
- Develops evaluation criteria
- Builds consistent scorecards
- Organizes questions by competency
- Suggests red flags to watch for

**Where Human Judgment Is Essential:**
- Validating competency relevance
- Adjusting for role specifics
- Ensuring legal compliance
- Calibrating evaluation standards
- Final hiring decisions
- Context-specific follow-ups

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Role requirements | Job description | Competency identification |
| Success criteria | What top performers do | Question targeting |
| Interview format | Who interviews, for what | Assignment distribution |
| Level | Junior, senior, lead | Calibration |
| Culture | Values, behaviors | Culture fit questions |

**Sample Input:**
```
Interview Question Bank Request

ROLE: Senior Product Manager, Enterprise
LEVEL: Senior (5+ years experience)

KEY COMPETENCIES TO ASSESS:

1. Customer Insight
   - Ability to deeply understand customer needs
   - Conducts effective user research
   - Translates insights into product decisions

2. Strategic Thinking
   - Develops product vision and roadmap
   - Makes prioritization trade-offs
   - Balances short-term and long-term

3. Technical Fluency
   - Understands technical architecture
   - Can communicate with engineering
   - Makes informed technical trade-offs

4. Execution
   - Ships products on time
   - Manages cross-functional stakeholders
   - Handles ambiguity and pivots

5. Communication
   - Writes clear specs
   - Presents to executives
   - Influences without authority

6. Culture Fit
   - Customer obsession
   - Data-driven decision making
   - Direct communication
   - Ownership mindset

INTERVIEW STRUCTURE:
- Round 1: Hiring Manager (45 min) - Overall fit, experience
- Round 2: Product Case (60 min) - Strategic thinking, problem-solving
- Round 3: Engineering (30 min) - Technical fluency, collaboration
- Round 4: Design (30 min) - Customer insight, collaboration
- Round 5: Sales (30 min) - Business acumen, communication
- Round 6: VP Product + CEO (60 min) - Culture, leadership

WHAT TOP PERFORMERS DO:
- Make decisions with incomplete data confidently
- Build strong relationships with engineering
- Can explain complex problems simply
- Push back respectfully when they disagree
- Own outcomes, not just outputs

RED FLAGS FROM PAST HIRES:
- Couldn't prioritize—everything was urgent
- Blamed engineering for missed deadlines
- Couldn't articulate why decisions were made
- Avoided customer contact
- Only talked about features, not outcomes
```

---

## Step-by-Step Implementation

### Step 1: Define Competencies
**Time: 5-10 minutes**

List:
- Core competencies for the role
- What good looks like for each
- What bad looks like (red flags)

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Interview Kit Prompt
**Time: 5-8 minutes for Claude to process**

---

**PRIMARY PROMPT: Interview Question Bank and Scorecards**

```
Please create a comprehensive interview kit for this role.

ROLE: [Title and level]

COMPETENCIES TO ASSESS:
[List competencies with descriptions]

INTERVIEW STRUCTURE:
[Who interviews for what]

SUCCESS INDICATORS:
[What top performers do]

RED FLAGS:
[What to watch for]

CREATE THE FOLLOWING:

1. COMPETENCY-BASED QUESTION BANK

   For each competency:

   **[COMPETENCY NAME]**

   Definition: [What this competency means]

   **Behavioral Questions (STAR format):**

   Question 1: "[Question]"
   - Follow-up probes:
     - [Probe 1]
     - [Probe 2]
   - What good looks like: [Answer indicators]
   - Red flags: [Warning signs]

   Question 2: "[Question]"
   [Same structure]

   Question 3: "[Question]"
   [Same structure]

   **Situational Questions:**

   Question 1: "[Hypothetical scenario question]"
   - What good looks like: [Expected approach]
   - Red flags: [Warning signs]

2. INTERVIEW GUIDES BY ROUND

   For each interview round:

   **[Round Name] — [Interviewer Role] — [Duration]**

   Purpose: [What this round assesses]

   Competencies to Focus On:
   - [Competency 1]
   - [Competency 2]

   Suggested Questions:
   [Selected from question bank]

   Time Allocation:
   - Intro: X min
   - Questions: X min
   - Candidate questions: X min
   - Wrap-up: X min

   Notes for Interviewer:
   [Specific guidance for this round]

3. EVALUATION SCORECARD

   **Candidate:** ________________
   **Interviewer:** ________________
   **Date:** ________________
   **Round:** ________________

   | Competency | 1-Weak | 2-Below | 3-Meets | 4-Exceeds | 5-Strong | Notes |
   |------------|--------|---------|---------|-----------|----------|-------|
   [Row for each competency]

   **Scoring Guide:**
   1 - Weak: [Definition]
   2 - Below expectations: [Definition]
   3 - Meets expectations: [Definition]
   4 - Exceeds expectations: [Definition]
   5 - Strong: [Definition]

   **Evidence Requirements:**
   For each score, provide specific example from interview

   **Overall Recommendation:**
   [ ] Strong Hire — Would advocate for this candidate
   [ ] Hire — Meets bar, no concerns
   [ ] No Hire — Does not meet bar
   [ ] Strong No Hire — Significant concerns

   **Key Strengths:**

   **Key Concerns:**

   **Additional Notes:**

4. DEBRIEF FRAMEWORK

   **Pre-Debrief:**
   - All interviewers submit scorecards before debrief
   - No discussion before submission (avoid anchoring)

   **Debrief Agenda:**
   1. Each interviewer shares recommendation (no explanation yet)
   2. Round-robin: Key evidence for each competency
   3. Discussion of concerns and counterarguments
   4. Final recommendation discussion

   **Questions to Address:**
   - Where do we have strong evidence?
   - Where are we missing data?
   - What concerns need resolution?
   - How does candidate compare to our bar?

5. CANDIDATE QUESTIONS TO EXPECT

   Candidates will likely ask:
   - [Question] — Good answer: [Response]
   [5-10 expected questions with answers]

6. RED FLAG REFERENCE

   **Immediate Concerns:**
   - [Red flag]: Why it matters

   **Yellow Flags (Probe Deeper):**
   - [Yellow flag]: What to explore

7. CALIBRATION EXAMPLES

   **Strong Hire Example:**
   [What a strong candidate response looks like]

   **No Hire Example:**
   [What an insufficient response looks like]

Create questions that reveal capability, not rehearsed answers.
```

---

### Step 4: Customize for Your Context
**Time: 5-10 minutes**

```
Refine the interview kit:

ADJUSTMENTS NEEDED:
- [Competency X] should focus more on: [Specific aspect]
- Add questions about: [Topic]
- Remove questions about: [Topic]

COMPANY-SPECIFIC:
- Our values are: [Values]
- Our challenges are: [Challenges]
- Candidates should know: [Context]

LEGAL CONSIDERATIONS:
- Ensure all questions are job-related
- Avoid questions about: [Protected categories]
```

---

### Step 5: Assign to Interviewers
**Time: 5 minutes**

```
Create interviewer assignments:

For each interviewer, provide:
1. Which competencies they're assessing
2. Which questions to ask
3. What to look for
4. How long to spend on each area
5. How their round fits with others
```

---

### Step 6: Generate Final Kit
**Time: 2 minutes**

```
Create the final interview kit package:

1. QUESTION BANK (master document)
2. INTERVIEW GUIDES (one per round)
3. SCORECARDS (printable/digital)
4. INTERVIEWER TRAINING (how to use the kit)
5. DEBRIEF TEMPLATE
```

---

## Example Output

Below is an abbreviated interview question bank example:

---

> **INTERVIEW KIT**
>
> **Senior Product Manager, Enterprise**
>
> ---
>
> ## Customer Insight Questions
>
> **Definition:** Ability to deeply understand customer needs through research, empathy, and analysis; translates insights into product decisions.
>
> ---
>
> ### Behavioral Question 1
>
> **"Tell me about a time when customer research led you to change your product direction."**
>
> **Follow-up probes:**
> - What research methods did you use?
> - How did you validate the insights?
> - What was the original direction and why did you think it was right?
> - Who did you have to convince to change course?
> - What was the outcome?
>
> **What good looks like:**
> - Describes specific research methodology (not just "we talked to customers")
> - Shows how they synthesized multiple data points
> - Demonstrates willingness to be wrong
> - Quantifies outcome where possible
> - Shows influence skills in changing direction
>
> **Red flags:**
> - Vague about methodology ("I have good intuition")
> - Only talked to friendly customers
> - Couldn't explain why original direction was wrong
> - Took credit for team decisions
> - No measurable outcome
>
> ---
>
> ### Behavioral Question 2
>
> **"Describe your process for understanding a new customer segment you hadn't worked with before."**
>
> **Follow-up probes:**
> - How did you identify who to talk to?
> - What questions did you ask?
> - How did you know when you understood enough?
> - What surprised you?
> - How did you share learnings with the team?
>
> **What good looks like:**
> - Systematic approach to customer discovery
> - Mix of qualitative and quantitative methods
> - Intellectual curiosity evident
> - Identifies assumptions and validates them
> - Creates shareable artifacts
>
> **Red flags:**
> - Relied solely on Sales for customer understanding
> - Didn't actually talk to customers
> - Made assumptions without validation
> - Couldn't articulate customer pain points
>
> ---
>
> ### Situational Question
>
> **"You're hearing conflicting feedback from customers: Enterprise customers want more customization while SMB customers want simplicity. How would you approach this?"**
>
> **What good looks like:**
> - Asks clarifying questions (segment size, revenue, strategy)
> - Suggests segmentation approach
> - Considers platform vs product tradeoffs
> - Proposes validation steps before deciding
> - Acknowledges tradeoffs, doesn't pretend there's easy answer
>
> **Red flags:**
> - Immediately picks a side without investigation
> - Proposes building everything for everyone
> - Doesn't consider business strategy
> - Can't articulate the tradeoffs
>
> ---
>
> ## Strategic Thinking Questions
>
> **Definition:** Develops compelling product vision, makes smart prioritization tradeoffs, balances short-term and long-term considerations.
>
> ---
>
> ### Behavioral Question 1
>
> **"Tell me about the most difficult prioritization decision you've made. Walk me through how you approached it."**
>
> **Follow-up probes:**
> - What were the options you were choosing between?
> - What framework did you use?
> - Who was involved in the decision?
> - What did you have to say no to?
> - How did stakeholders react to what got deprioritized?
>
> **What good looks like:**
> - Clear framework for prioritization (impact, effort, strategic alignment)
> - Considers multiple dimensions, not just one
> - Shows ability to make hard calls
> - Communicates decisions effectively to losers
> - Outcome-oriented, not just process-oriented
>
> **Red flags:**
> - Everything was high priority
> - Let stakeholders dictate priorities
> - Avoided making decisions
> - Couldn't articulate why chosen items won
> - Only focused on short-term
>
> ---
>
> ### Behavioral Question 2
>
> **"Describe a time when you had to balance a quick win against a more strategic long-term investment."**
>
> **Follow-up probes:**
> - What was the tradeoff specifically?
> - How did you evaluate the long-term value?
> - Who pushed for the quick win?
> - What did you decide and why?
> - In hindsight, was it the right call?
>
> **What good looks like:**
> - Demonstrates both types of thinking
> - Has a framework for these decisions
> - Can quantify or articulate long-term value
> - Willing to make unpopular calls
> - Reflects honestly on outcomes
>
> **Red flags:**
> - Only optimizes for short-term
> - Can't articulate long-term strategy
> - Always defers to stakeholder pressure
> - No framework for these decisions
>
> ---
>
> ## Technical Fluency Questions
>
> **Definition:** Understands technical concepts well enough to have substantive conversations with engineering, make informed technical tradeoffs, and write specs that engineers respect.
>
> ---
>
> ### Behavioral Question 1
>
> **"Tell me about a time you had to make a product decision that had significant technical implications. How did you approach it?"**
>
> **Follow-up probes:**
> - What were the technical constraints or tradeoffs?
> - How did you work with engineering to understand the options?
> - What was your role in the decision vs. engineering's role?
> - How did you communicate the decision to stakeholders?
> - What would you do differently?
>
> **What good looks like:**
> - Demonstrates understanding of technical concepts (not just vocabulary)
> - Shows collaboration with engineering, not deference or conflict
> - Can explain technical concepts in business terms
> - Took ownership of decision while respecting engineering expertise
> - Learned from the experience
>
> **Red flags:**
> - Completely deferred to engineering
> - Made technical decisions without engineering input
> - Can't explain the technical concepts involved
> - Blames engineering when things went wrong
> - Uses jargon without understanding
>
> ---
>
> ## Evaluation Scorecard
>
> **Candidate:** _________________ **Date:** _________
>
> | Competency | 1 | 2 | 3 | 4 | 5 | Evidence |
> |------------|---|---|---|---|---|----------|
> | Customer Insight | | | | | | |
> | Strategic Thinking | | | | | | |
> | Technical Fluency | | | | | | |
> | Execution | | | | | | |
> | Communication | | | | | | |
> | Culture Fit | | | | | | |
>
> **Scoring Guide:**
>
> **1 - Weak:** Clear evidence of deficiency. Would not succeed in role.
>
> **2 - Below:** Some positive signals but significant gaps. Below our bar.
>
> **3 - Meets:** Solid evidence of competency. Meets expectations for role.
>
> **4 - Exceeds:** Strong evidence. Better than most candidates at this level.
>
> **5 - Strong:** Exceptional. Top 10% of candidates we've seen.
>
> ---
>
> **Overall Recommendation:**
>
> [ ] **Strong Hire** — I would advocate for this candidate
> [ ] **Hire** — Meets our bar, no concerns
> [ ] **No Hire** — Does not meet our bar
> [ ] **Strong No Hire** — Significant concerns
>
> **Key Strengths:**
>
>
> **Key Concerns:**
>
>
> **Evidence Summary:**
>
>
> ---
>
> ## Interview Round: Engineering (30 min)
>
> **Purpose:** Assess technical fluency and engineering collaboration
>
> **Competencies to Focus On:**
> - Technical Fluency (primary)
> - Execution (secondary)
>
> **Time Allocation:**
> - Intro and rapport: 3 min
> - Technical questions: 15 min
> - Collaboration questions: 8 min
> - Candidate questions: 4 min
>
> **Suggested Questions:**
>
> 1. "Tell me about a time you had to make a product decision that had significant technical implications."
>
> 2. "Describe how you typically work with engineering to scope and estimate work."
>
> 3. "Tell me about a time you and an engineer disagreed about an approach. How did you resolve it?"
>
> **Notes for Interviewer:**
> - You're not looking for them to be an engineer
> - Can they have a substantive technical conversation?
> - Do they respect engineering while still owning product?
> - Would you want to work with this person?
>
> ---
>
> ## Debrief Framework
>
> **Before Debrief:**
> - All scorecards submitted (no peeking at others)
> - Review all feedback individually
>
> **Debrief Agenda (30 min):**
>
> 1. **Blind vote** (2 min)
>    - Each interviewer states recommendation without explanation
>    - Record: ___ Strong Hire, ___ Hire, ___ No Hire, ___ Strong No
>
> 2. **Evidence round-robin** (15 min)
>    - Each interviewer: 2 min on key evidence
>    - Focus on specific examples, not impressions
>
> 3. **Concerns discussion** (8 min)
>    - What concerns were raised?
>    - Is there counter-evidence?
>    - Can concerns be mitigated?
>
> 4. **Final decision** (5 min)
>    - Where's the bar?
>    - Final recommendation
>    - Next steps
>
> **Decision Criteria:**
> - Strong Hire from hiring manager: proceed
> - Majority hire with no strong concerns: proceed
> - Any Strong No Hire: must be discussed and resolved
> - Mixed signals: dig deeper before deciding

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Questions too easy | Not probing deep enough | Add: "Include follow-up probes that test depth. Push beyond prepared answers." |
| All candidates sound the same | Questions too generic | Ask: "Make questions specific to our context. What would differentiate strong from average?" |
| Interviewers not using kit | Too complicated | Simplify: "Create a 1-page cheat sheet per round with just the essentials" |
| Can't calibrate scores | No examples | Add: "Provide calibration examples of what 3 vs 5 looks like for each competency" |
| Missing critical areas | Incomplete competencies | Ask: "What competencies separate top performers from average? Add questions for those." |

---

## Tips from Experience

1. **Behavioral over hypothetical.** Past behavior predicts future behavior better than "what would you do."

2. **Follow up relentlessly.** The gold is in the follow-ups. Prepared answers crumble under probing.

3. **Evidence over impressions.** "They seemed smart" isn't evidence. "They explained X specifically" is.

4. **Assign competencies to interviewers.** Don't have everyone assess everything.

5. **Calibrate your bar.** What does "3" mean for your company? Get interviewers aligned.

6. **Debrief before deciding.** Individual votes submitted before group discussion reduces bias.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Interviews are consistent across candidates
- [ ] Interviewers feel prepared and confident
- [ ] Debriefs are evidence-based
- [ ] Hiring decisions improve (quality of hire)
- [ ] Bias indicators decrease
- [ ] Candidate experience improves

**Track over time:**
- Interviewer feedback on kit usefulness
- Score calibration across interviewers
- Correlation between interview scores and job performance
- Candidate satisfaction with process
- Time from interview to decision

---

## Variations

### Technical Interview Kit
For engineering roles:
```
Include:
- Coding question rubrics
- System design evaluation criteria
- Code review assessment
- Architecture discussion guides
- Technical depth vs breadth balance

Focus on: Can they solve problems, not just explain concepts
```

### Executive Interview Kit
For senior leadership:
```
Include:
- Leadership philosophy questions
- Strategic vision assessment
- Board presentation evaluation
- Reference check framework
- Executive presence criteria

Focus on: Pattern matching to successful executives
```

### High-Volume Interview Kit
For rapid hiring (sales, support):
```
Include:
- Phone screen script
- Rapid assessment scorecard
- Group interview format
- Role-play scenarios
- Quick calibration guide

Focus on: Efficiency and consistency at scale
```

### Culture Add Interview
For diversity and inclusion:
```
Include:
- Questions about different perspectives
- How they handle disagreement
- Examples of challenging status quo
- Inclusion behaviors assessment
- Avoiding "culture fit" as exclusion

Focus on: What do they add, not are they like us
```

---

## Building Your Repeatable System

After several interview kits, establish:

1. **Master question bank** by competency
2. **Standard competency definitions**
3. **Level calibration guides**
4. **Interviewer training materials**
5. **Continuous improvement process**

**Sample Setup:**
```
interview-kits/
├── question-bank/
│   ├── competencies/
│   │   ├── leadership.md
│   │   ├── technical-fluency.md
│   │   ├── communication.md
│   │   └── [by competency]
│   └── master-bank.md
├── roles/
│   ├── senior-pm-enterprise/
│   │   ├── interview-kit.md
│   │   ├── scorecard.md
│   │   └── round-guides/
│   └── [by role]
├── training/
│   ├── interviewer-guide.md
│   ├── calibration-examples.md
│   └── bias-awareness.md
├── templates/
│   ├── scorecard-template.md
│   └── debrief-template.md
└── analytics/
    └── hiring-metrics.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**define criteria → create structured assessment → evaluate consistently**—applies broadly:

| Role | Application |
|------|-------------|
| **HR** | All structured interviewing |
| **Managers** | Performance conversations |
| **L&D** | Training assessments |
| **Sales** | Discovery call frameworks |
| **Customer Success** | QBR preparation |
| **Consulting** | Client qualification |

---

## Next Steps

1. **Define competencies:** What really matters for this role?
2. **Design the loop:** Who interviews for what?
3. **Generate the kit:** Use this recipe
4. **Train interviewers:** Ensure consistent use
5. **Run and calibrate:** Adjust based on results
6. **Iterate:** Improve questions based on outcomes

---

*Recipe #62 of 100 in the Claude Code Knowledge Worker Recipe Collection*
