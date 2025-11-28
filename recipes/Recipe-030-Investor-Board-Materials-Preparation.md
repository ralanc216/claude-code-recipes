# Investor/Board Materials Preparation

**Recipe #30: From Data to Compelling Board Narrative**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 20 minutes (first time) / 15 minutes (repeat) | 8-15 hours per package | Advanced | Executives, Investor Relations, Finance, Board Secretaries |

---

## The Problem

Board meetings and investor updates require comprehensive materials that synthesize financial performance, strategic progress, market context, and forward-looking outlook into a compelling narrative. Creating these materials is time-intensive—pulling data from multiple sources, crafting appropriate messaging, ensuring consistency, and packaging it all professionally. The stakes are high, and the deadline is always tight.

**Pain Points:**
- Multiple data sources to consolidate
- Time pressure before board meetings
- Balancing transparency with narrative control
- Ensuring consistency across slides and documents
- Answering "so what?" for every metric
- Anticipating board member questions
- Same process repeated quarterly

---

## The Outcome

Comprehensive, professional board and investor materials that tell a clear story. Financial results presented in context, strategic progress communicated effectively, and forward outlook articulated clearly. Materials that generate productive board discussions rather than confusion.

**What You'll Have When Done:**
- Board deck with executive summary and sections
- Financial performance summary with narrative
- Strategic progress update
- Forward outlook and key decisions
- Supporting appendices
- Pre-read materials if needed

---

## When to Use This Recipe

**Good Fit:**
- Quarterly board meetings
- Annual investor updates
- Fundraising materials
- Annual reports
- Strategic reviews
- Special situation communications

**Not a Good Fit:**
- Informal investor calls (overkill)
- Day-to-day investor relations
- Technical financial filings (need specialists)
- Legal documents (require legal review)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You have financial data and metrics
- [ ] You have strategic updates and progress data
- [ ] You know the board agenda and focus areas
- [ ] You understand your audience (who's on the board)
- [ ] You have 4-6 hours for comprehensive preparation

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Synthesizes multiple data sources
- Generates narrative from numbers
- Creates consistent structure
- Produces executive summaries
- Identifies discussion topics
- Ensures comprehensive coverage

**Where Human Judgment Is Essential:**
- Sensitive information handling
- Board member relationships
- Political considerations
- Strategic framing choices
- What to emphasize or de-emphasize
- Final approval of all materials

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Financial data | P&L, metrics, KPIs | Performance section |
| Strategic updates | Initiative progress | Strategic section |
| Market context | Industry developments | Context setting |
| Forward outlook | Projections, risks | Outlook section |
| Prior board materials | Last meeting's deck | Continuity |
| Agenda items | What board wants to discuss | Content focus |

**Sample Input:**
```
Board Meeting Prep: Q3 2024 Board Meeting (October 15)

COMPANY: CloudScale (Enterprise SaaS)
Board composition:
- 2 Founders (CEO, CTO)
- 2 VCs (lead investor, follow-on)
- 1 Independent (former public company CFO)

AGENDA:
1. Q3 Performance Review
2. 2024 Forecast Update
3. Product Strategy Discussion
4. 2025 Planning Preview
5. Operational Items

FINANCIAL DATA (Q3):
- Revenue: $12.2M (vs $11.0M budget, vs $10.1M Q3 LY)
- ARR: $52M (vs $50M target)
- Gross Margin: 74% (vs 72% budget)
- Operating Expenses: $11.8M (vs $11.5M budget)
- Cash: $28M (down from $32M Q2)
- Burn: $3.8M/month

KEY METRICS:
- New ARR: $3.8M (vs $3.5M target)
- Net Retention: 115% (vs 112% Q2)
- Customer Count: 285 (+ 18 Q3)
- Churn: 3 customers ($180K ARR)
- Sales Pipeline: $18M (vs $15M Q2)

STRATEGIC UPDATES:
- Product: AI features launched on schedule, early adoption strong
- Sales: Enterprise motion gaining traction, 2 $500K+ deals won
- Ops: Data center migration 60% complete
- People: 3 senior hires made (VP Sales, VP Eng, VP CS)

CONCERNS:
- Cash runway discussions (18 months)
- Competitive pressure on pricing
- Q4 pipeline conversion
- 2025 planning assumptions

PRIOR BOARD FEEDBACK:
- Want more market context
- Requested customer case studies
- Asked for competitive update
- Want clarity on path to profitability
```

---

## Step-by-Step Implementation

### Step 1: Gather All Inputs
**Time: 30-45 minutes**

Collect:
- Financial statements and metrics
- Strategic initiative updates
- Market and competitive information
- Prior board materials (for continuity)
- Agenda and expected discussion topics
- Any specific requests from board members

Organize chronologically and by section.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
cd ~/Documents/board-materials
claude
```

---

### Step 3: Run the Board Materials Prompt
**Time: 10-15 minutes for Claude to process**

---

**PRIMARY PROMPT: Board Materials Preparation**

```
Please help me prepare comprehensive board meeting materials.

MEETING CONTEXT:
- Company: [Name]
- Meeting date: [Date]
- Meeting type: [Quarterly / Annual / Special]
- Board composition: [Who's on the board]

AGENDA:
1. [Agenda item 1]
2. [Agenda item 2]
3. [etc.]

FINANCIAL DATA:
"""
[PASTE YOUR FINANCIAL DATA AND METRICS]
"""

STRATEGIC UPDATES:
"""
[PASTE YOUR STRATEGIC AND OPERATIONAL UPDATES]
"""

MARKET CONTEXT:
"""
[PASTE RELEVANT MARKET AND COMPETITIVE INFORMATION]
"""

CONCERNS AND TOPICS:
"""
[PASTE KEY CONCERNS, DISCUSSION TOPICS, BOARD REQUESTS]
"""

PRIOR BOARD FEEDBACK:
"""
[PASTE FEEDBACK FROM PREVIOUS MEETINGS]
"""

PLEASE CREATE:

1. EXECUTIVE SUMMARY (1-2 pages)
   - Quarter/Period headline
   - Key accomplishments
   - Key challenges
   - Critical decisions for board
   - Outlook summary

2. FINANCIAL PERFORMANCE SECTION
   - Performance summary table
   - Variance analysis narrative
   - Key metrics dashboard
   - Cash and runway
   - Trends and implications
   - Commentary addressing likely questions

3. STRATEGIC PROGRESS SECTION
   - Progress against strategic priorities
   - Key initiative updates
   - Milestones achieved and missed
   - Resource allocation
   - Risks and issues

4. MARKET AND COMPETITIVE UPDATE
   - Market dynamics
   - Competitive developments
   - Customer insights
   - Implications for strategy

5. FORWARD OUTLOOK SECTION
   - Updated projections
   - Key assumptions
   - Scenarios (bull/base/bear)
   - Major risks and opportunities
   - Resource needs

6. DISCUSSION ITEMS
   - Topics requiring board input
   - Decisions needed
   - Options and recommendations
   - Discussion questions

7. APPENDIX MATERIALS
   - Detailed financials
   - Customer metrics
   - Product roadmap summary
   - Org chart updates
   - Key performance indicators detail

8. SLIDE STRUCTURE
   Suggested board deck outline:
   - Cover and agenda (1 slide)
   - Executive summary (1-2 slides)
   - Financial performance (3-4 slides)
   - Strategic progress (3-4 slides)
   - Market update (1-2 slides)
   - Forward outlook (2-3 slides)
   - Discussion items (1-2 slides)
   - Appendix (as needed)

9. ANTICIPATED QUESTIONS
   - Questions board members will likely ask
   - Prepared responses/data points

10. PRE-READ SUMMARY
    If sending materials in advance:
    - 1-page summary highlighting key points
    - Call-outs for areas requiring attention
```

---

### Step 4: Develop Each Section
**Time: 45-60 minutes**

Work through each section, refining as needed:

**For executive summary:**
```
Refine the executive summary to:
1. Lead with the headline (good quarter or challenging quarter)
2. Include exactly 3 accomplishments and 2 challenges
3. Make the board's required decisions clear
4. End with a forward-looking statement
```

**For financial narrative:**
```
Enhance the financial narrative to:
1. Explain why we beat/missed each line item
2. Address the cash burn and runway question proactively
3. Connect financial results to strategic initiatives
4. Anticipate CFO board member's detailed questions
```

**For strategic section:**
```
Strengthen the strategic progress section to:
1. Show clear RAG status for each priority
2. Include specific metrics, not just narrative
3. Address the items called out as concerns
4. Connect to competitive dynamics
```

---

### Step 5: Prepare for Discussion
**Time: 20-30 minutes**

**For discussion items:**
```
For the 2025 planning discussion item:
1. Frame the decision we need from the board
2. Present 3 options with pros/cons
3. Include our recommendation
4. Provide key discussion questions
5. Anticipate pushback and prepare responses
```

**For Q&A preparation:**
```
Based on this board composition and materials, generate:
1. 10 most likely questions by board member
2. Data points needed to answer each
3. Prepared response for sensitive questions about cash runway
4. Bridge to key messages we want to reinforce
```

---

### Step 6: Create Final Deliverables
**Time: 30 minutes**

```
Create these final outputs:

1. BOARD DECK (PowerPoint structure)
   - Slide-by-slide content
   - Key data points for each slide
   - Suggested visualizations
   - Speaker notes

2. PRE-READ DOCUMENT (Word format)
   - 2-3 page summary
   - Key data tables
   - Executive summary

3. APPENDIX PACKAGE
   - Detailed financial schedules
   - Metric definitions
   - Supporting analysis

4. CEO TALKING POINTS
   - Key messages per section
   - Transition language
   - Difficult question responses

5. FOLLOW-UP ITEMS TEMPLATE
   - Placeholder for board requests
   - Action item tracking format
```

---

## Example Output

Below is an abbreviated board materials example:

---

> **CLOUDSCALE Q3 2024 BOARD MEETING**
> **October 15, 2024**
>
> ---
>
> **EXECUTIVE SUMMARY**
>
> **Headline: Strong Q3 with Revenue and ARR Ahead of Plan**
>
> Q3 delivered $12.2M revenue (11% above budget, 21% YoY growth) and $52M ARR, exceeding our $50M target. This performance reflects successful execution of our enterprise strategy and strong AI feature adoption.
>
> **Key Accomplishments:**
> 1. ✅ **ARR beat:** $52M ARR vs. $50M plan (+4%)
> 2. ✅ **Enterprise traction:** 2 deals >$500K closed; enterprise mix now 35%
> 3. ✅ **AI launch:** On-time delivery with 40% customer adoption in first month
>
> **Key Challenges:**
> 1. ⚠️ **Cash consumption:** Burn at $3.8M/month vs. $3.5M plan (18-month runway)
> 2. ⚠️ **Competitive pricing:** Seeing 10-15% discount pressure in mid-market
>
> **Board Input Requested:**
> - 2025 planning investment level (aggressive vs. measured growth)
> - Fundraising timing (proactive vs. wait for metrics)
>
> ---
>
> **FINANCIAL PERFORMANCE**
>
> | Metric | Q3 Actual | Q3 Budget | Q3 LY | vs Budget | vs LY |
> |--------|-----------|-----------|-------|-----------|-------|
> | Revenue | $12.2M | $11.0M | $10.1M | +11% | +21% |
> | Gross Profit | $9.0M | $7.9M | $7.1M | +14% | +27% |
> | Gross Margin | 74% | 72% | 70% | +200bps | +400bps |
> | Operating Expenses | $11.8M | $11.5M | $9.8M | +3% | +20% |
> | Operating Income | $(2.8M) | $(3.6M) | $(2.7M) | +22% | -4% |
> | Cash | $28M | $29M | $35M | -3% | -20% |
>
> **Key Takeaways:**
>
> 1. **Revenue beat:** $1.2M above budget driven by enterprise deal timing (2 large deals closed early) and strong net retention (115% vs. 112% budget).
>
> 2. **Margin improvement:** Gross margin at 74% reflects infrastructure optimization and higher enterprise mix. Expect this level to sustain.
>
> 3. **OpEx overage:** $300K above plan primarily from accelerated hiring (VP Sales, VP Eng both started in Q3 vs. Q4 plan). This is intentional investment.
>
> 4. **Cash:** Burn of $3.8M/month vs. $3.5M plan. 18-month runway at current burn. Key discussion topic for 2025 planning.
>
> ---
>
> **KEY METRICS DASHBOARD**
>
> | Metric | Q3 | Q2 | Q1 | YoY | Target | Status |
> |--------|-----|-----|-----|-----|--------|--------|
> | ARR | $52M | $48M | $44M | +30% | $50M | ✅ |
> | Net Retention | 115% | 112% | 110% | +5pts | 115% | ✅ |
> | New ARR | $3.8M | $3.5M | $3.2M | +25% | $3.5M | ✅ |
> | Customer Count | 285 | 267 | 248 | +22% | 280 | ✅ |
> | Churn ($) | $180K | $210K | $250K | -35% | <$200K | ✅ |
> | Sales Pipeline | $18M | $15M | $14M | +40% | $16M | ✅ |
> | Win Rate | 28% | 25% | 24% | +4pts | 25% | ✅ |
> | CAC Payback | 16mo | 17mo | 18mo | -2mo | 18mo | ✅ |
>
> ---
>
> **STRATEGIC PROGRESS**
>
> | Priority | Status | Q3 Milestone | Achieved? | Commentary |
> |----------|--------|--------------|-----------|------------|
> | Enterprise Sales | 🟢 On Track | 2 $500K+ deals | ✅ Yes | Exceeded—closed 2 |
> | AI Product | 🟢 On Track | Launch by Sept | ✅ Yes | 40% adoption Month 1 |
> | Ops Efficiency | 🟡 Watch | DC migration 50% | ⚠️ 60% | Slightly ahead |
> | Team Build | 🟢 On Track | 3 VPs hired | ✅ Yes | All started |
>
> **Enterprise Sales Momentum:**
> - Closed: Acme Corp ($600K), GlobalTech ($520K)
> - Pipeline: 4 additional $300K+ opportunities for Q4
> - Enterprise mix: Now 35% of new ARR (vs. 25% Q3 LY)
> - Sales cycle: 75 days enterprise (improving from 90)
>
> **AI Features Adoption:**
> - 40% of customers activated AI features (Month 1)
> - NPS for AI users: 72 (vs. 58 for non-AI)
> - Expansion revenue from AI: $220K incremental ARR
> - Competitive differentiator in 3 enterprise wins
>
> ---
>
> **FORWARD OUTLOOK**
>
> **Q4 2024 Guidance:**
>
> | Metric | Q4 Guidance | Q4 Budget | Confidence |
> |--------|-------------|-----------|------------|
> | Revenue | $13.0-13.5M | $12.5M | High |
> | ARR Exit | $56-58M | $55M | Medium-High |
> | Cash Exit | $24-25M | $25M | Medium |
>
> **Key Q4 Drivers:**
> - Enterprise pipeline conversion (4 large opportunities)
> - AI upsell to existing base
> - Seasonal Q4 strength
>
> **Key Q4 Risks:**
> - Pipeline slip if enterprise deals push to Q1
> - Competitive pricing pressure
> - Year-end budget freezes at prospects
>
> ---
>
> **DISCUSSION: 2025 Investment Level**
>
> **Decision Required:** Board input on 2025 growth vs. efficiency trade-off
>
> **Context:**
> - 18-month runway at current burn
> - Strong market opportunity, competitive window
> - Team ready to scale
> - Macro uncertainty for fundraising
>
> **Options:**
>
> | Scenario | Growth Target | Investment | Cash at YE'25 | Trade-off |
> |----------|---------------|------------|---------------|-----------|
> | A: Aggressive | 50% growth | +$5M | $15M | High growth, narrow runway |
> | B: Balanced | 40% growth | +$2M | $22M | Good growth, safer runway |
> | C: Efficient | 30% growth | Flat | $28M | Preserve cash, slower growth |
>
> **Management Recommendation:** Option B (Balanced)
>
> **Discussion Questions:**
> 1. What runway level is board comfortable with?
> 2. Appetite for proactive fundraising in H1 2025?
> 3. Trade-off between growth rate and profitability timeline?
>
> ---
>
> **ANTICIPATED BOARD QUESTIONS**
>
> | Question | Prepared Response |
> |----------|-------------------|
> | "What's the path to profitability?" | At current trajectory, cash flow positive in 24 months. With Scenario B, 18 months. Ready to share detailed model. |
> | "Why is burn higher than plan?" | Accelerated VP hires (intentional). Q4 burn normalizing. Full year will be within 5% of plan. |
> | "How sustainable is this growth?" | Pipeline visibility is 4+ months. Enterprise motion working. AI differentiation provides 12-18 month window. |
> | "What if fundraising market stays closed?" | Scenario C gets us to profitability with existing cash. We can pivot if needed by Q2 decision point. |

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Materials feel too long | Too much detail | Ask: "Summarize to executive level—what are the 5 things the board needs to know?" |
| Story isn't clear | Missing narrative thread | Ask: "What's the single headline for this quarter? Build all sections to support that." |
| Numbers don't tie | Inconsistency across sections | Ask: "Reconcile all financial figures—ensure consistency throughout" |
| Missing context | Not enough explanation | Add: "For each metric, include 'why' and 'so what'" |
| Board member concerns unaddressed | Not anticipating questions | Ask: "What will [board member type] ask? Prepare responses." |
| Too rosy | Avoiding difficult topics | Add: "Be direct about challenges—boards value transparency" |

---

## Tips from Experience

1. **Lead with the headline.** Don't make board members work to figure out if it was a good quarter or bad quarter. Tell them.

2. **Anticipate, don't react.** Answer the hard questions before they're asked. It builds credibility.

3. **Consistency matters.** Numbers must tie across all documents. Inconsistencies destroy confidence.

4. **Less is more.** Boards have limited attention. Prioritize ruthlessly. Move detail to appendix.

5. **Know your audience.** Different board members care about different things. Address each.

6. **Send pre-reads.** Give board members time to digest materials before the meeting.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Board discussions are strategic, not clarifying
- [ ] Questions are answered in the materials
- [ ] No surprises emerge in the meeting
- [ ] Board members feel informed
- [ ] Decisions are made efficiently

**Track over time:**
- Board meeting time spent on clarifications
- Follow-up questions after meetings
- Board feedback on materials quality
- Time to prepare materials (should decrease)

---

## Variations

### Investor Update
For regular investor communications:
```
Create an investor update for our quarterly letter.

Financial and strategic data: [Paste]

Include:
1. Opening paragraph (quarter summary)
2. Key highlights (3-5 bullets)
3. Financial summary (table)
4. Strategic progress
5. What we're focused on next
6. Closing note

Tone: Transparent, confident, forward-looking
Length: 1-2 pages
```

### Fundraising Deck
For pitch preparation:
```
Create a fundraising deck structure.

Company info: [Paste]
Round: [Series X]
Raise amount: [$XM]
Use of funds: [Description]

Create:
1. Deck outline (12-15 slides)
2. Key message per slide
3. Data points needed
4. Anticipated investor questions
5. Follow-up materials checklist
```

### Annual Report
For comprehensive annual reporting:
```
Help prepare materials for our annual report.

Data: [Financial and strategic data for the year]

Create:
1. Letter from CEO
2. Year in review highlights
3. Financial summary
4. Strategic accomplishments
5. Team and culture section
6. Forward outlook
7. Key metrics dashboard
```

### Crisis/Special Situation Board Update
For urgent communications:
```
Help prepare an urgent board update.

Situation: [Description of issue/event]
Impact: [Known and potential impact]
Actions: [What we're doing]

Create:
1. Situation summary (factual)
2. Impact assessment
3. Actions taken
4. Support requested
5. Timeline for updates
6. Q&A preparation

Tone: Direct, factual, action-oriented
```

---

## Building Your Repeatable System

After several board cycles, establish your system:

1. **Create standard templates** for each section
2. **Build a data collection checklist** for consistent gathering
3. **Maintain a questions library** of board member concerns
4. **Establish timeline** for materials preparation
5. **Document lessons learned** from each meeting

**Sample Setup:**
```
board-materials/
├── templates/
│   ├── board-deck-template.pptx
│   ├── pre-read-template.docx
│   ├── financials-template.xlsx
│   └── content-prompts.txt
├── meetings/
│   ├── 2024-Q3/
│   │   ├── deck/
│   │   ├── pre-read/
│   │   ├── appendix/
│   │   └── follow-up.md
│   └── archive/
├── reference/
│   ├── board-member-profiles.md
│   ├── common-questions.md
│   └── metric-definitions.md
└── checklists/
    ├── data-collection.md
    ├── timeline.md
    └── quality-review.md
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**gather data → synthesize narrative → anticipate questions → create materials → prepare for discussion**—applies broadly:

| Role | Application |
|------|-------------|
| **Executives** | All board communications |
| **Finance** | Investor relations, financial reviews |
| **Investor Relations** | Shareholder communications |
| **Strategy** | Strategic reviews, planning presentations |
| **Board Secretaries** | Meeting preparation |
| **Consultants** | Client board presentations |

---

## Next Steps

1. **Review your timeline:** When is your next board meeting?
2. **Start early:** Begin gathering data 2+ weeks ahead
3. **Use the template:** Apply this recipe systematically
4. **Get feedback:** Ask board members what they'd like improved
5. **Iterate:** Refine based on meeting outcomes

---

*Recipe #30 of 100 in the Claude Code Knowledge Worker Recipe Collection*
