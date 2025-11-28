# Performance Review Writing Assistance

**Recipe #13: From Scattered Notes to Comprehensive Reviews**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 10 minutes (first time) / 5 minutes (repeat) | 1-2 hours per review | Beginner | All managers with direct reports |

---

## The Problem

Performance review season arrives and you face a stack of reviews to write. For each employee, you need to recall months of work, provide specific examples, balance honest feedback with encouragement, and follow your organization's format. You know you should give thoughtful, detailed reviews, but the time pressure leads to rushed, generic feedback that doesn't serve your employees well.

**Pain Points:**
- Remembering 6-12 months of accomplishments and challenges
- Writing specific, meaningful feedback (not generic praise)
- Balancing positive and constructive feedback appropriately
- Following required format while being genuine
- Writing 5-15 reviews in a compressed timeline
- Making each review feel personalized, not templated
- Avoiding recency bias (overweighting recent events)

---

## The Outcome

Well-structured, specific performance reviews that accurately capture each employee's contributions and growth areas. Reviews are comprehensive yet efficient to produce, with balanced feedback and clear development recommendations that actually help employees grow.

**What You'll Have When Done:**
- Complete performance review following your format
- Specific examples supporting each assessment
- Balanced feedback (strengths and growth areas)
- Clear, actionable development recommendations
- Consistent quality across all reviews
- Confidence that each employee gets fair, thoughtful feedback

---

## When to Use This Recipe

**Good Fit:**
- Annual or semi-annual performance reviews
- Quarterly check-in documentation
- Promotion justification writing
- 360-degree feedback compilation
- New manager review writing (learning the skill)
- High volume of reviews due in short timeframe

**Not a Good Fit:**
- Real-time performance conversations (these should be verbal)
- Initial feedback that hasn't been discussed with employee first
- Situations requiring HR/legal involvement (get guidance first)
- Reviews for employees you've managed less than 3 months

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have notes, observations, or documentation on the employee
- [ ] You know your organization's review format and rating scale
- [ ] You've had regular feedback conversations (no surprises in review)
- [ ] You know the employee's goals/OKRs from the review period
- [ ] You have 20-30 minutes per review

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Structures feedback according to your format
- Generates specific language from your bullet points
- Balances positive and constructive feedback
- Creates actionable development recommendations
- Maintains consistent quality across multiple reviews
- Reduces writer's block and blank page syndrome

**Where Human Judgment Is Essential:**
- Accuracy of the assessment (you know their actual performance)
- Relationship and political context
- Calibrating ratings against team and organization norms
- Deciding what's appropriate to document vs. discuss verbally
- Final review—your name is on this document

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Your observations | Bullet points of what you noticed | Core feedback content |
| Goal/OKR status | Which goals were met/missed | Objective assessment |
| Project outcomes | Key deliverables and impact | Specific examples |
| Feedback from others | 360 input, peer comments | Broader perspective |
| Previous review | Last period's review | Continuity and progress |
| Competency model | Company's skill framework | Framework alignment |

**Sample Input (What You Might Provide):**
```
Employee: Sarah Chen
Role: Senior Software Engineer
Review Period: Jan-Dec 2024

My observations and notes:
- Led the API redesign project - delivered on time, reduced latency 40%
- Became go-to person for architecture decisions
- Mentored 2 junior engineers, both are now independent
- Sometimes takes on too much, missed a few deadlines in Q3
- Communication with product team improved significantly mid-year
- Wants to move toward tech lead role
- Strong technically but needs more practice with stakeholder management
- Got great feedback from the QA team on her documentation

Goals from beginning of year:
1. Lead API redesign (Met - exceeded expectations)
2. Improve system reliability to 99.9% (Met - achieved 99.95%)
3. Develop mentoring skills (Met)
4. Improve cross-functional communication (Partially met - improved but still developing)

Rating I'm thinking: "Exceeds Expectations" overall
```

---

## Step-by-Step Implementation

### Step 1: Gather Your Notes
**Time: 5-10 minutes**

Before writing, collect:
- Your running notes on this employee (you kept those, right?)
- Their goals/OKRs and status
- Key projects and outcomes
- Feedback from others (peers, stakeholders)
- Previous review for context
- Any recognition, awards, or notable moments

Don't worry about organization—just gather the raw material.

**Pro Tip:** If you don't have running notes, spend 10 minutes brainstorming specific examples before starting. Vague reviews are useless reviews.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Performance Review Prompt
**Time: 3-5 minutes for Claude to process**

---

**PRIMARY PROMPT: Performance Review Generator**

```
Please help me write a performance review based on my notes and observations.

EMPLOYEE INFORMATION:
- Name: [Name]
- Role: [Title]
- Review period: [Start date - End date]
- Time in role: [Duration]
- My overall assessment: [Exceeds/Meets/Below expectations or your rating scale]

MY NOTES AND OBSERVATIONS:
"""
[PASTE YOUR OBSERVATIONS, ACCOMPLISHMENTS, CHALLENGES, FEEDBACK]
"""

GOALS/OKRS STATUS:
"""
[LIST THEIR GOALS AND WHETHER MET/NOT MET]
"""

OUR REVIEW FORMAT REQUIREMENTS:
[Describe your company's format, or use this default structure]:
1. Overall summary (2-3 sentences)
2. Key accomplishments (3-5 specific examples with impact)
3. Strengths demonstrated (2-3 with examples)
4. Areas for development (2-3 with specific, actionable guidance)
5. Goal achievement summary
6. Development recommendations for next period
7. Overall rating with justification

ADDITIONAL CONTEXT:
- Their career aspirations: [What they want to develop toward]
- Team/company context: [Any relevant organizational factors]
- Things to be sensitive about: [If any]

PLEASE GENERATE:

1. COMPLETE PERFORMANCE REVIEW
   Following our format, with:
   - Specific examples (not generic praise)
   - Balanced feedback (strengths AND development areas)
   - Forward-looking development recommendations
   - Professional tone appropriate for HR documentation

2. RATING JUSTIFICATION
   - Why this rating is appropriate
   - Evidence supporting the rating
   - How this compares to role expectations

3. DEVELOPMENT CONVERSATION TALKING POINTS
   - Key themes to discuss in the review meeting
   - How to frame development areas constructively
   - Questions to ask them

4. SUGGESTED 30/60/90 DAY FOCUS
   - Specific actions for their development
   - How you can support them
```

---

### Step 4: Review for Accuracy
**Time: 5-10 minutes**

This step is critical—you're putting your name on this:

**Fact check:**
- Are the specific examples accurate?
- Are dates and outcomes correct?
- Did Claude invent anything not in your notes?

**Fairness check:**
- Does the overall assessment match your rating?
- Is the feedback balanced and fair?
- Would the employee recognize themselves in this?

**Tone check:**
- Is development feedback constructive, not punitive?
- Are strengths genuinely celebrated?
- Does it read as supportive of their growth?

---

### Step 5: Refine the Review
**Time: 5-10 minutes**

**To strengthen specific examples:**
```
The API redesign accomplishment needs more specifics. Add that it serves 2M daily requests and the team completed it 2 weeks ahead of schedule despite losing a team member mid-project.
```

**To adjust the balance:**
```
The development section feels too heavy. This is a strong performer. Reduce from 3 development areas to 2, and frame them more as "opportunities" than "gaps."
```

**To add context:**
```
Add context that she took on the API project mid-year when the original lead left unexpectedly. This makes the on-time delivery even more impressive.
```

**To soften feedback:**
```
The comment about "missed deadlines" is accurate but harsh. Reframe it as "learning to manage scope and say no" - that's the actual skill she needs to develop.
```

**To align with career goals:**
```
She wants to become a tech lead. Make sure the development recommendations are clearly connected to that aspiration.
```

---

### Step 6: Finalize and Document
**Time: 2 minutes**

Save the review:
```
Save this performance review as "Sarah-Chen-2024-Annual-Review.md"
```

For your records:
```
Create a brief summary of key points for my 1:1 notes - what to emphasize in our review conversation.
```

---

## Example Output

Below is an abbreviated example review:

---

> **PERFORMANCE REVIEW**
> **Sarah Chen | Senior Software Engineer | January - December 2024**
>
> ---
>
> **Overall Summary**
>
> Sarah delivered exceptional results in 2024, most notably leading the API redesign project to successful completion while serving as a technical mentor to junior team members. She has grown significantly in cross-functional collaboration and is ready to take on expanded technical leadership responsibilities. Her overall rating is **Exceeds Expectations**.
>
> ---
>
> **Key Accomplishments**
>
> 1. **API Redesign Project Leadership** — Led the complete redesign of our core API infrastructure, delivering 2 weeks ahead of schedule despite taking over the project mid-year when the original lead departed. The new architecture serves 2M+ daily requests with 40% improved latency, directly impacting customer satisfaction scores.
>
> 2. **System Reliability Achievement** — Drove system reliability from 99.7% to 99.95%, exceeding the 99.9% target. Implemented proactive monitoring and automated recovery procedures that have prevented 3 potential outages.
>
> 3. **Engineering Mentorship** — Mentored two junior engineers (Alex and Jordan), both of whom have progressed to independent contributors. Created documentation and onboarding materials that have reduced new engineer ramp time by 30%.
>
> ---
>
> **Strengths Demonstrated**
>
> - **Technical Excellence:** Deep expertise in system architecture and ability to make sound technical decisions under pressure. The QA team specifically recognized her documentation quality.
>
> - **Leadership Initiative:** Naturally stepped up when the team needed direction, earning trust from both peers and stakeholders.
>
> ---
>
> **Areas for Development**
>
> - **Scope Management:** Sarah's dedication sometimes leads to overcommitment. Developing the skill to push back on scope and negotiate timelines will be important as she takes on larger leadership responsibilities. We saw this impact Q3 delivery when multiple commitments competed for her time.
>
> - **Stakeholder Communication:** Significant improvement mid-year, with proactive updates to product team becoming the norm. Next level is developing executive communication skills for broader visibility.
>
> ---
>
> **Development Recommendations**
>
> Given Sarah's aspiration toward a Tech Lead role:
>
> 1. **Lead Q1 planning process** for the platform team—practice in priority-setting and cross-team coordination
> 2. **Shadow VP Engineering** in 2-3 stakeholder meetings to develop executive communication
> 3. **Attend leadership training** (recommend: internal Tech Lead cohort starting February)
>
> ---
>
> **Rating: Exceeds Expectations**
>
> Sarah consistently performed above the expectations for a Senior Software Engineer, particularly in technical leadership and mentorship. She is ready for expanded responsibilities and should be considered for Tech Lead opportunities in 2025.

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Review sounds generic | Input lacked specific examples | Add concrete details: projects, metrics, dates, impact |
| Tone is too critical | Development areas overweighted | Ask: "Rebalance to 70% strengths, 30% development" |
| Feedback not actionable | Vague improvement suggestions | Ask: "Make each development area include a specific action they can take" |
| Doesn't match rating | Disconnect between narrative and assessment | Ask: "Adjust the narrative to support a [rating] - what evidence should be emphasized?" |
| Invented examples | Claude filled gaps creatively | Review carefully; remove anything you can't verify |
| Doesn't fit company format | Format wasn't specified clearly | Provide exact template or section headers required |

---

## Tips from Experience

1. **Keep running notes throughout the year.** 10 minutes per month beats 2 hours of archaeology at review time. Even just a few bullets per month in a 1:1 doc helps immensely.

2. **No surprises in reviews.** If development areas haven't been discussed in 1:1s, discuss them BEFORE putting them in writing. Reviews document ongoing feedback, not reveal new issues.

3. **Be specific or don't bother.** "Great job this year" helps no one. "Led API redesign, reducing latency 40%" is meaningful feedback they can build on.

4. **Development areas should be actionable.** "Improve communication" is useless. "Practice presenting technical decisions to non-technical stakeholders in weekly product syncs" is actionable.

5. **Calibrate across your team.** Before finalizing, review all your reviews together. Ensure your "Exceeds" performers are consistently differentiated from your "Meets" performers.

6. **Write for multiple audiences.** The employee reads it, but so does HR, future managers, and potentially executives during promotion discussions. Write accordingly.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Reviews are completed on time without last-minute scrambling
- [ ] Employees recognize themselves in the feedback
- [ ] Each review has specific, verifiable examples
- [ ] Development areas feel constructive, not punitive
- [ ] Reviews enable productive development conversations
- [ ] Quality is consistent across all your direct reports

**Track over time:**
- Time spent per review
- Employee feedback on review usefulness
- Correlation between review feedback and actual development

---

## Variations

### Promotion Justification
For supporting a promotion case:
```
I need to write a promotion justification for [name] to [new level].

Current role: [role and level]
Proposed role: [new role and level]

Evidence of readiness:
[Your notes on why they're ready]

Our promotion criteria for [new level]:
[Company's level expectations]

Please create a promotion justification that:
1. Maps their performance to the new level's expectations
2. Provides specific examples for each criterion
3. Addresses the "stretch" they're demonstrating
4. Anticipates questions the promotion committee might ask
```

### Mid-Year Check-in
For lighter-weight periodic feedback:
```
I need to document a mid-year check-in, not a full review.

Focus on:
- Progress on annual goals
- Any adjustments needed
- Key wins to recognize
- Development progress
- Look-ahead to remainder of year

Keep it to 1 page maximum. Less formal than annual review.
```

### 360 Feedback Synthesis
For compiling multi-source feedback:
```
Help me synthesize 360 feedback for [name].

Feedback from:
- Peers: [paste or summarize]
- Direct reports: [paste or summarize]
- Stakeholders: [paste or summarize]
- My observations: [your notes]

Create a synthesized view that:
- Identifies common themes across sources
- Notes any significant differences in perception
- Highlights blind spots (things they may not see in themselves)
- Provides balanced overall picture
```

### Performance Improvement Documentation
For struggling performers (proceed carefully):
```
I need to document performance concerns for [name]. This is not a formal PIP yet, but documentation of specific concerns.

Issues:
[Specific concerns with examples]

Context:
[Any mitigating factors]

Previous feedback given:
[What's already been communicated]

Create documentation that:
- States concerns factually and specifically
- Includes dates and examples
- Notes feedback already provided
- Sets clear expectations going forward
- Is appropriate for HR review

Tone: Direct and clear, not punitive. Focus on facts and expectations.
```

---

## Building Your Repeatable System

After completing one review cycle, establish your system:

1. **Create a running notes habit** — Add observations after each 1:1
2. **Build a review template** with your organization's format pre-loaded
3. **Save your best prompts** customized to your team's roles
4. **Maintain a "calibration notes" doc** to ensure consistency
5. **Schedule prep time** before review season begins

**Sample Setup:**
```
performance-reviews/
├── templates/
│   └── review-prompt-template.txt
├── team-notes/
│   ├── sarah-chen-running-notes.md
│   ├── alex-jones-running-notes.md
│   └── ...
├── 2024-reviews/
│   ├── sarah-chen-2024-review.md
│   └── ...
└── calibration-notes.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**gather observations → structure into format → generate specific feedback**—applies broadly:

| Role | Application |
|------|-------------|
| **Executives** | Leadership team assessments, board member feedback |
| **Managers** | Any employee evaluation or feedback documentation |
| **HR** | Performance documentation, talent review preparation |
| **Mentors** | Mentee progress documentation |
| **Project Managers** | Team member contribution assessments |
| **Educators** | Student evaluations, recommendation letters |

---

## Next Steps

1. **Start running notes now** — Don't wait for review season
2. **Try on your next review** — Use this recipe for your next performance review
3. **Calibrate with peers** — Compare your reviews with other managers for consistency
4. **Build your template** — Customize the prompt for your organization's format

---

*Recipe #13 of 100 in the Claude Code Knowledge Worker Recipe Collection*
