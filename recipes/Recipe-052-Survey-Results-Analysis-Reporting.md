# Survey Results Analysis and Reporting

**Recipe #52: From Raw Responses to Actionable Insights**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 10 minutes (first time) / 5 minutes (repeat) | 4-8 hours per survey | Intermediate | HR, Marketing, Product, Researchers |

---

## The Problem

You ran a survey and got responses—now what? Raw data sits in exports while stakeholders wait for insights. Analyzing open-ended responses takes forever. Quantitative data needs context to be meaningful. Different stakeholders want different cuts of the data. By the time you've written the report, the moment for action has passed. And the same manual analysis process awaits next quarter.

**Pain Points:**
- Hours spent analyzing open-ended responses
- Quantitative data without meaningful interpretation
- No systematic approach to theme identification
- Reports that present data without actionable insights
- Stakeholders waiting while analysis drags on
- Same manual process every survey cycle
- Difficulty comparing across survey waves

---

## The Outcome

Comprehensive survey analysis with quantitative summaries, qualitative theme identification, and actionable recommendations. Reports that tell a clear story and drive decisions, delivered in a fraction of the time.

**What You'll Have When Done:**
- Executive summary of key findings
- Quantitative analysis with statistical context
- Theme analysis of open-ended responses
- Segment comparisons
- Trend analysis (vs. prior surveys)
- Prioritized recommendations
- Presentation-ready visualizations

---

## When to Use This Recipe

**Good Fit:**
- Employee engagement surveys
- Customer satisfaction surveys (CSAT, NPS)
- Market research surveys
- Product feedback surveys
- Event feedback surveys
- 360 feedback compilations
- Any structured survey with 50+ responses

**Not a Good Fit:**
- Surveys with <50 responses (too small for themes)
- Highly sensitive surveys requiring special handling
- Complex statistical analysis (need specialized tools)
- Surveys still collecting responses

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] Survey is closed and data exported
- [ ] You have the survey questions for context
- [ ] You know the target audience for results
- [ ] You have 2-4 hours for analysis

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Analyzes open-ended responses for themes
- Identifies sentiment patterns
- Summarizes quantitative findings
- Creates segment comparisons
- Generates narrative reports
- Suggests action items

**Where Human Judgment Is Essential:**
- Statistical significance assessment
- Business context interpretation
- Sensitive topic handling
- Action prioritization
- Presentation to stakeholders
- Follow-up planning

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Survey data | Exported responses | Core analysis |
| Questions | Survey instrument | Context for responses |
| Prior surveys | Historical data | Trend comparison |
| Segments | Department, tenure, etc. | Segment analysis |
| Context | What prompted the survey | Interpretation |

**Sample Input:**
```
Survey Analysis Request

SURVEY: Q4 2024 Employee Engagement Survey

SURVEY CONTEXT:
- Population: All employees (~500)
- Responses: 387 (77% response rate)
- Prior survey: Q2 2024 (372 responses)
- Purpose: Quarterly pulse check on engagement
- Recent events: Leadership change in Q3, new benefits in October

QUANTITATIVE DATA:
Overall engagement score: 7.2/10 (prior: 6.8/10)

By category:
- Leadership & direction: 7.5 (prior: 6.5)
- Career development: 6.4 (prior: 6.2)
- Work-life balance: 7.8 (prior: 7.6)
- Compensation & benefits: 6.9 (prior: 6.1)
- Manager relationship: 7.6 (prior: 7.4)
- Team collaboration: 7.4 (prior: 7.5)
- Resources & tools: 6.8 (prior: 6.6)

eNPS: +22 (prior: +12)

BY DEPARTMENT:
- Engineering: 7.5 (prior: 7.2)
- Sales: 6.8 (prior: 6.5)
- Marketing: 7.0 (prior: 7.1)
- Operations: 7.4 (prior: 6.4)
- Customer Success: 6.9 (prior: 7.0)
- Finance/Admin: 7.6 (prior: 6.8)

BY TENURE:
- <1 year: 7.8
- 1-3 years: 7.0
- 3-5 years: 6.6
- 5+ years: 6.9

OPEN-ENDED RESPONSES (sample):

Q: "What is working well at the company?"
[Paste 50-100 sample responses]

Q: "What could be improved?"
[Paste 50-100 sample responses]

Q: "Any additional comments?"
[Paste responses]

TARGET AUDIENCE: Executive team and HR leadership

DELIVERABLES NEEDED:
- Executive summary (1 page)
- Full analysis report
- Department-specific summaries
- Action recommendations
```

---

## Step-by-Step Implementation

### Step 1: Prepare Survey Data
**Time: 15-20 minutes**

- Export survey data from survey tool
- Organize quantitative data by question/category
- Gather all open-ended responses
- Collect comparison data (prior surveys, benchmarks)

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Survey Analysis Prompt
**Time: 10-15 minutes for Claude to process**

---

**PRIMARY PROMPT: Survey Results Analysis**

```
Please analyze this survey data and generate a comprehensive report.

SURVEY INFORMATION:
- Survey name: [Name]
- Purpose: [Why this survey was conducted]
- Population: [Who was surveyed]
- Responses: [Number and response rate]
- Prior survey: [If applicable, for comparison]
- Context: [Recent events, business situation]

QUANTITATIVE DATA:
[Paste quantitative results]

SEGMENT BREAKDOWNS:
[Paste by department, tenure, location, etc.]

OPEN-ENDED RESPONSES:

Question 1: "[Question text]"
Responses:
[Paste responses]

Question 2: "[Question text]"
Responses:
[Paste responses]

[Continue for all open-ended questions]

TARGET AUDIENCE: [Who will read this]

PLEASE CREATE:

1. EXECUTIVE SUMMARY (1 page)
   - Overall findings (2-3 sentences)
   - Key wins (what's working)
   - Key concerns (what needs attention)
   - Critical recommendations (top 3)
   - Comparison to prior survey (if applicable)

2. QUANTITATIVE ANALYSIS

   A. Overall Scores
   - Summary table with all scores
   - Comparison to prior survey (change +/-)
   - Trend assessment

   B. Score Distribution
   - What's strong (above benchmark/expectation)
   - What's average
   - What's concerning (below benchmark/expectation)

   C. Statistical Notes
   - Response rate and confidence
   - Changes that are likely significant
   - Changes that may be noise

3. SEGMENT ANALYSIS

   For each segment dimension:
   - Highest scoring segments
   - Lowest scoring segments
   - Notable differences
   - Segments needing attention

4. OPEN-ENDED THEME ANALYSIS

   For each open-ended question:

   **[Question]**

   Top Themes (by frequency):
   | Theme | Frequency | Sentiment | Representative Quote |

   Sub-themes:
   - [Sub-theme 1]
   - [Sub-theme 2]

   Notable Outliers:
   - [Unique perspectives worth highlighting]

   Sentiment Analysis:
   - Overall: [Positive/Neutral/Negative %]
   - Key sentiment drivers

5. CROSS-TABULATION INSIGHTS

   Interesting relationships in the data:
   - [Finding 1: e.g., "Employees with 3-5 years tenure have lowest scores across all categories"]
   - [Finding 2]

6. TREND ANALYSIS (if prior survey available)

   | Category | Prior | Current | Change | Assessment |

   What improved:
   - [Area 1] — [Why it likely improved]

   What declined:
   - [Area 1] — [Why it may have declined]

   What stayed stable:
   - [Areas that didn't change significantly]

7. KEY FINDINGS

   Finding 1: [Clear statement]
   - Evidence: [Supporting data]
   - Implication: [Why it matters]
   - Suggested action: [What to do]

   [Continue for top 5-7 findings]

8. RECOMMENDATIONS

   Priority 1: [Recommendation]
   - Rationale: [Why]
   - Proposed action: [Specific steps]
   - Expected impact: [What will improve]

   [Continue for 4-5 recommendations]

9. QUESTIONS FOR FOLLOW-UP

   Issues needing further investigation:
   - [Question 1]
   - [Question 2]

10. APPENDICES

    - Full score tables
    - All themes identified
    - Methodology notes
    - Response demographics

Write for clarity and action. Focus on insights that drive decisions, not just data presentation.
```

---

### Step 4: Validate Theme Analysis
**Time: 15-20 minutes**

Review the open-ended theme analysis:
- Do the themes ring true?
- Are quotes representative?
- Any themes missed?
- Sentiment assessment accurate?

---

### Step 5: Add Context and Interpretation
**Time: 10-15 minutes**

**To add business context:**
```
Add context for these findings:
- The leadership score increase likely relates to [new CEO hiring in Q3]
- The career development concern aligns with [recent promotion freeze]
- Add this context to make the analysis more actionable
```

**To refine recommendations:**
```
Make recommendations more specific and actionable:
- Who should own each recommendation?
- What's the timeline?
- What does success look like?
```

**To create segment summaries:**
```
Create a 1-page summary specifically for [Engineering/Sales/etc.]:
- Their scores vs. company average
- Their specific concerns (from open-ended)
- Recommended actions for their leadership
```

---

### Step 6: Create Final Deliverables
**Time: 15 minutes**

```
Create the final survey analysis package:

1. EXECUTIVE SUMMARY (1 page)
   For leadership quick read

2. FULL ANALYSIS REPORT
   Complete analysis with all sections

3. PRESENTATION DECK OUTLINE
   Slides for all-hands or leadership presentation:
   - Key findings (3-4 slides)
   - What's working (1 slide)
   - What needs attention (1 slide)
   - Recommendations (1-2 slides)
   - Next steps (1 slide)

4. DEPARTMENT SUMMARIES
   One-pager for each department head

5. ACTION PLANNING TEMPLATE
   For turning insights into initiatives

6. COMMUNICATION DRAFT
   For sharing results with all employees
```

---

## Example Output

Below is an abbreviated survey analysis example:

---

> **EMPLOYEE ENGAGEMENT SURVEY ANALYSIS**
>
> **Q4 2024 | Executive Summary**
>
> ---
>
> ## Executive Summary
>
> Employee engagement improved meaningfully this quarter. Overall engagement score rose from 6.8 to 7.2, with eNPS jumping from +12 to +22—our highest since tracking began. The leadership transition is landing well (leadership scores up 1.0 point), and new benefits are resonating (compensation scores up 0.8). However, career development remains a persistent concern, and mid-tenure employees (3-5 years) show the lowest engagement across all dimensions.
>
> **Key Wins:**
> - Leadership & direction scores significantly improved (+1.0)
> - New benefits program received positively (+0.8 on compensation)
> - Operations team saw largest improvement (+1.0 overall)
>
> **Key Concerns:**
> - Career development remains lowest category (6.4)
> - Mid-tenure employees are disengaging (6.6 vs. 7.2 average)
> - Customer Success team declined slightly (-0.1)
>
> **Top 3 Recommendations:**
> 1. Launch career pathing initiative targeting mid-tenure employees
> 2. Investigate Customer Success decline—likely related to recent restructuring
> 3. Capitalize on leadership momentum with increased visibility and communication
>
> ---
>
> ## Quantitative Analysis
>
> ### Overall Scores
>
> | Category | Q2 2024 | Q4 2024 | Change |
> |----------|---------|---------|--------|
> | **Overall Engagement** | 6.8 | 7.2 | +0.4 ⬆️ |
> | Leadership & direction | 6.5 | 7.5 | +1.0 ⬆️ |
> | Career development | 6.2 | 6.4 | +0.2 |
> | Work-life balance | 7.6 | 7.8 | +0.2 |
> | Compensation & benefits | 6.1 | 6.9 | +0.8 ⬆️ |
> | Manager relationship | 7.4 | 7.6 | +0.2 |
> | Team collaboration | 7.5 | 7.4 | -0.1 |
> | Resources & tools | 6.6 | 6.8 | +0.2 |
> | **eNPS** | +12 | +22 | +10 ⬆️ |
>
> ### Score Assessment
>
> **Strong (≥7.5):**
> - Work-life balance (7.8) — Consistently our strength
> - Manager relationship (7.6) — Managers remain valued
> - Leadership & direction (7.5) — Significant improvement
>
> **Moderate (6.5-7.4):**
> - Team collaboration (7.4) — Slight decline worth monitoring
> - Compensation & benefits (6.9) — New benefits well received
> - Resources & tools (6.8) — Modest improvement
>
> **Needs Attention (<6.5):**
> - Career development (6.4) — Persistent weakness
>
> ---
>
> ## Segment Analysis
>
> ### By Department
>
> | Department | Q2 | Q4 | Change | Flag |
> |------------|-----|-----|--------|------|
> | Finance/Admin | 6.8 | 7.6 | +0.8 | ✅ Improved |
> | Engineering | 7.2 | 7.5 | +0.3 | ✅ |
> | Operations | 6.4 | 7.4 | +1.0 | ✅ Most improved |
> | Marketing | 7.1 | 7.0 | -0.1 | |
> | Customer Success | 7.0 | 6.9 | -0.1 | ⚠️ Monitor |
> | Sales | 6.5 | 6.8 | +0.3 | |
>
> **Note:** Operations saw the largest improvement (+1.0). The new operations manager (hired Q2) appears to be having positive impact. Customer Success slight decline warrants attention—may be related to Q3 team restructuring.
>
> ### By Tenure
>
> | Tenure | Score | vs. Average | Flag |
> |--------|-------|-------------|------|
> | <1 year | 7.8 | +0.6 | ✅ New hires engaged |
> | 1-3 years | 7.0 | -0.2 | |
> | 3-5 years | 6.6 | -0.6 | 🔴 Needs attention |
> | 5+ years | 6.9 | -0.3 | |
>
> **Concerning pattern:** Mid-tenure employees (3-5 years) show the lowest engagement. This is typically when career progression questions become urgent. Without clear paths, this cohort may be the highest attrition risk.
>
> ---
>
> ## Open-Ended Theme Analysis
>
> ### "What is working well?"
>
> **Top Themes:**
>
> | Theme | Mentions | Representative Quote |
> |-------|----------|---------------------|
> | Leadership/direction | 42% | "New CEO brings clarity and energy. For the first time in a while, I feel like we know where we're going." |
> | Team/colleagues | 38% | "The people here are amazing. My team is collaborative and supportive." |
> | Flexibility | 28% | "Work from home policy is genuinely flexible—not just on paper." |
> | New benefits | 24% | "The new parental leave policy shows the company cares about life outside work." |
> | Manager support | 19% | "My manager goes to bat for me and gives me room to grow." |
>
> **Sentiment:** 78% positive, 15% neutral, 7% negative
>
> ---
>
> ### "What could be improved?"
>
> **Top Themes:**
>
> | Theme | Mentions | Sentiment | Representative Quote |
> |-------|----------|-----------|---------------------|
> | Career growth/paths | 34% | Frustrated | "No clear path for advancement. People leave because they can't see a future here." |
> | Communication/transparency | 22% | Concerned | "Decisions are made and announced without context. Would help to understand the 'why.'" |
> | Compensation | 18% | Mixed | "Benefits improved, but base comp is still below market for my role." |
> | Workload | 15% | Stressed | "We keep adding priorities but nothing comes off the list." |
> | Cross-team coordination | 12% | Frustrated | "Departments don't talk to each other. Too many silos." |
>
> **Sentiment:** 23% positive, 31% neutral, 46% negative (expected for improvement question)
>
> **Notable:** Career development concerns appeared in 34% of responses—the dominant theme by a significant margin. This is consistent with the lowest quantitative score (6.4) and represents a genuine organizational gap.
>
> ---
>
> ## Key Findings
>
> ### Finding 1: Leadership Transition is Working
>
> **Evidence:** Leadership & direction scores jumped 1.0 point (6.5 → 7.5). Open-ended responses explicitly cite new CEO with 42% mentioning leadership as "what's working well."
>
> **Implication:** Initial leadership skepticism has given way to optimism. This is a foundation to build on.
>
> **Action:** Continue high leadership visibility. Don't let communication frequency drop now that the "new leader" period has passed.
>
> ---
>
> ### Finding 2: Career Development is a Critical Gap
>
> **Evidence:** Lowest quantitative score (6.4), top open-ended concern (34% of improvement comments). Mid-tenure employees (3-5 years) show lowest engagement (6.6), likely related.
>
> **Implication:** Career path ambiguity is driving disengagement and is a likely driver of attrition. This cohort represents experienced employees you can't easily replace.
>
> **Action:** Prioritize career framework development. Create visible career paths, especially for mid-level roles. Address in Q1.
>
> ---
>
> ### Finding 3: New Benefits are Resonating
>
> **Evidence:** Compensation score improved 0.8 points. 24% of "what's working" responses mention benefits specifically.
>
> **Implication:** The investment is paying off in employee perception. Benefits matter beyond just compensation.
>
> **Action:** Continue communicating benefits value. Consider annual total compensation statements to reinforce.
>
> ---
>
> ### Finding 4: Mid-Tenure Employees Need Attention
>
> **Evidence:** Employees with 3-5 years tenure score 6.6 vs. 7.2 company average—the lowest of any segment.
>
> **Implication:** This is typically when employees expect advancement and, if they don't see it, start looking elsewhere. This cohort represents your experienced individual contributors and emerging leaders.
>
> **Action:** Targeted focus on 3-5 year employees. Career conversations, development opportunities, retention risk assessment.
>
> ---
>
> ## Recommendations
>
> ### Priority 1: Launch Career Pathing Initiative
>
> **Rationale:** Career development is the lowest score and top open-ended concern. Mid-tenure employees are disengaging, creating retention risk.
>
> **Proposed Action:**
> - Create visible career ladders for all roles
> - Manager training on career conversations
> - Quarterly career discussions (add to 1:1 templates)
> - Pilot internal mobility program
>
> **Timeline:** Initiative launch Q1; full rollout by Q2
>
> **Owner:** HR with department head partnership
>
> ---
>
> ### Priority 2: Investigate Customer Success Decline
>
> **Rationale:** Only department showing decline. May be early warning of broader issues.
>
> **Proposed Action:**
> - Focus group with CS team
> - 1:1s with CS leadership
> - Review recent changes (restructuring impact?)
> - Action plan based on findings
>
> **Timeline:** Investigation in next 2 weeks; action plan by month-end
>
> **Owner:** CHRO with CS VP
>
> ---
>
> ### Priority 3: Maintain Leadership Momentum
>
> **Rationale:** Leadership scores improved dramatically. Don't let this become "new car smell" that fades.
>
> **Proposed Action:**
> - Continue all-hands cadence
> - Executive Q&A sessions
> - Leader visibility in different offices/teams
> - Communication of strategic progress
>
> **Timeline:** Ongoing
>
> **Owner:** CEO and leadership team
>
> ---
>
> ## Employee Communication Draft
>
> Subject: Your Voice Matters: Q4 Engagement Survey Results
>
> Team,
>
> Thank you to the 77% of you who completed our Q4 engagement survey. Your feedback matters, and I want to share what we heard and what we're doing about it.
>
> **What we learned:**
>
> ✅ **What's working:** Leadership and direction scores improved significantly. You're feeling more confident about where we're headed. The new benefits are resonating—thank you for that feedback; it confirms we made the right investments.
>
> ⚠️ **What needs work:** Career development is your top concern. You're telling us you want clearer paths to grow here. We hear you, and this is our top priority for Q1.
>
> **What we're doing:**
>
> 1. **Career pathing initiative** — We're building clear career ladders for every role and training managers on career conversations. More details coming in January.
>
> 2. **Continued leadership visibility** — We'll keep our all-hands rhythm and add more opportunities for Q&A.
>
> 3. **Department-specific actions** — Each department head received their team's results and is developing specific action plans.
>
> Engagement doesn't improve because we run surveys—it improves because we act on what we learn. Thank you for helping us get better.
>
> [CEO Name]

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Themes too generic | Not enough responses analyzed | Include more responses, or ask: "What specific sub-themes exist within [theme]?" |
| Quantitative and qualitative don't align | Different things measured | Ask: "How do we reconcile [quantitative finding] with [qualitative finding]?" |
| No actionable insights | Analysis too descriptive | Ask: "For each finding, what should we DO about it?" |
| Segment analysis shallow | Not enough data per segment | Acknowledge limitations; combine small segments |
| Report too long | Over-detailed | Ask: "Prioritize for executive audience. What's essential?" |
| Trends not meaningful | Small sample or changes | Add: "Note which changes are likely significant vs. within margin of error" |

---

## Tips from Experience

1. **Lead with the story, not the data.** Start with "Here's what we learned" not "Here are the numbers."

2. **Quote liberally.** Stakeholders connect with employee voices more than statistics.

3. **Separate observation from recommendation.** State what the data shows, then what to do about it.

4. **Acknowledge limitations.** Small samples, low response rates, and recent events all affect interpretation.

5. **Create segment-specific summaries.** Department heads want their data, not the company overview.

6. **Plan the communication.** Survey results without communication erode trust. Always close the loop.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Analysis delivered within target timeline
- [ ] Stakeholders understand the findings
- [ ] Actions are identified and assigned
- [ ] Results are communicated to participants
- [ ] Engagement scores improve over time
- [ ] Trust in the survey process increases

**Track over time:**
- Time from survey close to report delivery
- Stakeholder satisfaction with analysis
- Action item completion rate
- Engagement trend across surveys
- Survey participation rate

---

## Variations

### NPS/Customer Survey
For customer feedback:
```
Analyze customer satisfaction survey.

Focus on:
- NPS score and drivers
- Promoter themes vs. detractor themes
- Product/service specific feedback
- Competitive mentions
- Churn risk indicators

Include: Segment analysis by customer type, tenure, spend
```

### 360 Feedback Compilation
For leadership feedback:
```
Compile 360 feedback for [leader name].

Responses: [Multiple rater perspectives]

Create:
- Strength themes
- Development themes
- Blind spots (self vs. others)
- Specific examples
- Development recommendations

Tone: Constructive, specific, actionable
```

### Market Research Survey
For market/competitive research:
```
Analyze market research survey.

Focus on:
- Market awareness
- Brand perception
- Purchase drivers
- Competitive positioning
- Segment preferences

Include: Opportunity identification, positioning recommendations
```

### Event Feedback
For post-event surveys:
```
Analyze event feedback survey.

Focus on:
- Overall satisfaction
- Content quality
- Logistics feedback
- Speaker ratings
- Suggestions for improvement

Include: What to repeat, what to change for next event
```

---

## Building Your Repeatable System

After several survey analyses, build your system:

1. **Create survey analysis templates** by survey type
2. **Maintain theme codebook** for consistent categorization
3. **Track trend data** across survey waves
4. **Build benchmark library** for comparison
5. **Establish reporting calendar** and workflow

**Sample Setup:**
```
survey-analysis/
├── templates/
│   ├── engagement-survey.md
│   ├── nps-survey.md
│   ├── market-research.md
│   └── event-feedback.md
├── analyses/
│   ├── engagement/
│   │   ├── 2024-Q4/
│   │   │   ├── raw-data/
│   │   │   ├── analysis.md
│   │   │   ├── executive-summary.md
│   │   │   └── department-summaries/
│   │   └── [prior quarters]/
│   └── [other surveys]/
├── reference/
│   ├── theme-codebook.md
│   ├── benchmarks.md
│   └── historical-trends.xlsx
└── communications/
    ├── templates/
    └── archive/
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**collect data → identify themes → compare to benchmarks → recommend actions**—applies broadly:

| Role | Application |
|------|-------------|
| **HR** | Engagement, culture, exit surveys |
| **Marketing** | Customer research, brand studies |
| **Product** | User feedback, feature research |
| **CX** | NPS, CSAT, customer feedback |
| **Events** | Post-event evaluation |
| **Research** | Any survey-based research |

---

## Next Steps

1. **Prepare data:** Export survey results
2. **Gather context:** What's the business situation?
3. **Generate analysis:** Use this recipe
4. **Validate findings:** Check theme accuracy
5. **Add interpretation:** Your knowledge and judgment
6. **Communicate results:** Close the loop with participants

---

*Recipe #52 of 100 in the Claude Code Knowledge Worker Recipe Collection*
