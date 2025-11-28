# Board & Leadership Meeting Prep Automation

**Recipe #11: From Scattered Inputs to Executive-Ready Briefings**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 30-45 minutes (first time) / 10 minutes (repeat) | 4-8 hours per meeting | Beginner | Executives, Directors, Senior Managers |

---

## The Problem

Board meetings, quarterly business reviews, and leadership updates require synthesizing information from multiple sources: financial reports in spreadsheets, project status updates in various documents, customer metrics from dashboards, and strategic context from emails and meeting notes. Professionals spend hours manually gathering, reading, and distilling this information into coherent briefing documents.

**Pain Points:**
- Information scattered across 5-15 different files and sources
- Manual synthesis takes 4-8 hours per major meeting
- Important details get lost or overlooked under time pressure
- Briefing quality varies based on available prep time
- Last-minute updates require re-doing significant work

---

## The Outcome

With Claude Code, you point to a folder containing your source materials and receive a comprehensive, executive-ready briefing document in 15-30 minutes. The document includes an executive summary, key decisions required, supporting data highlights, risk flags, and recommended talking points—all formatted professionally and ready to use.

**What You'll Have When Done:**
- A 3-4 page briefing document ready for distribution
- Clear decision items with recommendations
- Anticipated questions with suggested responses
- Confidence that nothing major was missed

---

## When to Use This Recipe

**Good Fit:**
- Quarterly board meetings or investor updates
- Leadership team business reviews (QBRs)
- Department-level status presentations to executives
- Annual planning kickoff summaries
- Any meeting requiring synthesis of multiple data sources

**Not a Good Fit:**
- Highly confidential M&A discussions (sensitive data concerns)
- Situations where you have only 1-2 simple source documents (overkill)
- Meetings where the narrative is already clear and you just need formatting
- Real-time meeting situations (this is for prep, not live use)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working (run `claude` in terminal to verify)
- [ ] You have at least 3-5 source documents ready
- [ ] Source files are in readable formats (PDF, Word, Excel, CSV, TXT, MD)
- [ ] No password-protected or encrypted files in the batch
- [ ] You have 30-45 minutes for first-time setup (10 min for repeat use)
- [ ] You know the meeting date, audience, and key topics expected

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Reads and processes multiple file types simultaneously
- Identifies key themes, metrics, and decisions across disparate sources
- Generates structured output with consistent formatting
- Creates Word documents or presentations directly
- Spots patterns and connections you might miss when reading sequentially

**Where Human Judgment Is Essential:**
- Verify accuracy of extracted financial figures (always spot-check numbers)
- Add political context or sensitive dynamics Claude doesn't know
- Adjust emphasis based on what you know about your audience's priorities
- Include verbal updates or context not captured in documents
- Make final calls on recommendations and framing

---

## Input Examples

**Ideal Source Materials (aim for 5-15 files):**

| File Type | Example | What Claude Extracts |
|-----------|---------|---------------------|
| Financial Report (PDF/Excel) | `Q3-Financial-Summary.xlsx` | Revenue, margins, variance vs. plan |
| Project Status (Word/PDF) | `Engineering-Status-Oct.docx` | Milestones, blockers, timeline updates |
| Customer Metrics (CSV/Excel) | `Customer-Health-Dashboard.csv` | Retention rates, NPS, churn risks |
| Sales Pipeline (Excel) | `Pipeline-Report-Oct.xlsx` | Pipeline value, close rates, forecast |
| Meeting Notes (TXT/Word) | `Leadership-Sync-Notes.txt` | Decisions made, open items, concerns raised |
| Strategic Memo (Word/PDF) | `Market-Analysis-Q3.pdf` | Competitive moves, market trends |
| Email Thread (saved as PDF) | `Customer-Escalation-Thread.pdf` | Issue context, resolution status |

**File Organization Example:**
```
Q4-Board-Prep/
├── financials/
│   ├── Q3-Financial-Summary.xlsx
│   └── Q3-vs-Q2-Comparison.pdf
├── operations/
│   ├── Engineering-Status-Oct.docx
│   └── Product-Roadmap-Update.pdf
├── sales/
│   ├── Pipeline-Report-Oct.xlsx
│   └── Win-Loss-Summary.pdf
├── customer/
│   ├── Customer-Health-Dashboard.csv
│   └── NPS-Survey-Results.pdf
└── context/
    ├── Leadership-Sync-Notes.txt
    └── Previous-Board-Action-Items.docx
```

---

## Step-by-Step Implementation

### Step 1: Prepare Your Source Folder
**Time: 10-20 minutes (first time) / 5 minutes (repeat)**

Create a dedicated folder for your meeting prep materials. Use a clear naming convention.

```bash
mkdir ~/Documents/Board-Prep-2024-Q4
```

Gather your source documents into this folder. Prioritize:
1. Financial reports and dashboards
2. Operational/project status updates
3. Customer and sales metrics
4. Previous meeting notes and action items
5. Any strategic memos or context documents

**Pro Tip:** Create subfolders by category (financials/, operations/, sales/) to help Claude organize its analysis, but this isn't required.

---

### Step 2: Launch Claude Code
**Time: 1 minute**

Open your terminal and navigate to your prep folder:

```bash
cd ~/Documents/Board-Prep-2024-Q4
```

Start Claude Code:

```bash
claude
```

---

### Step 3: Run the Briefing Prompt
**Time: 5-10 minutes for Claude to process**

Copy and customize the prompt below. Replace bracketed sections with your specifics.

---

**PRIMARY PROMPT: Board Meeting Briefing Generator**

```
I need to prepare a briefing document for our [Q4 Board Meeting on December 15th].

The audience is [our board of directors, who focus primarily on financial performance, strategic progress, and risk management].

Please analyze all documents in this folder and create a comprehensive briefing document with these sections:

1. EXECUTIVE SUMMARY (1 paragraph, 4-5 sentences max)
   - Overall business health assessment (clear positive/negative/mixed signal)
   - 2-3 key headline metrics vs. targets
   - Single most critical item requiring board attention

2. KEY DECISIONS REQUIRED
   - List each decision needing board approval
   - For each: context (2-3 sentences), options considered, recommended action, and urgency level

3. PERFORMANCE HIGHLIGHTS
   - Top 3-5 wins and achievements this period
   - Include specific metrics and comparisons where available
   - Note any records broken or exceptional performance

4. RISKS AND CHALLENGES
   - Active risks with severity (High/Medium/Low) and likelihood
   - Current mitigation status
   - What we're asking the board to note or approve regarding each risk

5. FINANCIAL SUMMARY
   - Key financial metrics vs. plan and vs. prior period
   - Notable variances with explanations
   - Forward-looking indicators

6. OPERATIONAL UPDATES BY FUNCTION (2-3 sentences each)
   - Organize by: Finance, Operations, Product/Engineering, Sales/Revenue, People/HR
   - Focus on: status vs. plan, key metrics, notable items

7. STRATEGIC INITIATIVE PROGRESS
   - Status of major strategic priorities
   - Milestones achieved and upcoming
   - Any course corrections needed

8. RECOMMENDED TALKING POINTS
   - 3-5 key messages I should emphasize
   - Anticipated tough questions with suggested responses
   - Topics to potentially defer or minimize

9. APPENDIX RECOMMENDATIONS
   - List any detailed data that should be available as backup
   - Note any documents board members should review in advance

Format as a professional document with clear headers and consistent formatting. Target 3-4 pages for the main document (excluding appendices). Use bullet points for readability. Bold key numbers and decisions.

Company context for reference: [We are a B2B software company with 200 employees, $50M ARR, serving enterprise customers in the financial services sector.]
```

---

### Step 4: Review Initial Output
**Time: 10-15 minutes**

Claude will read all source documents and generate the briefing. As you review:

**Check immediately:**
- Did Claude read all the files? (It will typically mention what it found)
- Are the key topics from your sources represented?
- Do the numbers look right at first glance?

**Spot-check 3-5 specific facts:**
- Pick a financial number and verify against the source
- Check that a quoted metric matches the original
- Confirm a date or milestone is accurate

---

### Step 5: Refine with Follow-up Prompts
**Time: 10-20 minutes**

Use conversational follow-ups to improve the output. Here are effective refinement patterns:

**To expand a section:**
```
Expand the Operations section. Pull in more specific details from the Engineering-Status-Oct.docx file, particularly around the platform migration timeline.
```

**To add comparisons:**
```
Add Q3 vs Q2 comparisons for all financial metrics. Also include year-over-year where that data is available.
```

**To adjust tone or emphasis:**
```
The executive summary feels too positive given the revenue miss. Reframe it to lead with the challenge while maintaining confidence in the recovery plan.
```

**To add missing context:**
```
I need to add context that isn't in these documents: We lost two key engineering leaders last month, which is contributing to the timeline delays. Please incorporate this into the Operations section and Risks section appropriately.
```

**To prepare for tough questions:**
```
The board will likely challenge us on customer churn. Generate 3 additional tough questions they might ask about churn and retention, with detailed suggested responses.
```

**To create a shorter version:**
```
Create a 1-page executive summary version I can use as a leave-behind or pre-read.
```

---

### Step 6: Export Final Document
**Time: 2 minutes**

Once satisfied with the content:

```
Save this briefing as a Word document named "Board-Briefing-Q4-2024-Final.docx"
```

Or for a presentation format:
```
Convert this briefing into a 10-slide PowerPoint presentation with speaker notes. Save as "Board-Presentation-Q4-2024.pptx"
```

---

## Example Output

Below is an abbreviated example of what a well-executed briefing looks like:

---

> **EXECUTIVE SUMMARY**
>
> Q3 performance was **mixed**, with revenue of $12.4M (94% of plan) offset by stronger-than-expected gross margins of 72% (vs. 68% plan). Customer retention improved to 94% from 91% in Q2, though new logo acquisition remains below target. **The board's primary attention is needed on** the proposed Series C timeline acceleration, given favorable market conditions and increased competitive pressure. Overall, we are well-positioned for Q4 but require board approval on two time-sensitive decisions.
>
> **KEY DECISIONS REQUIRED**
>
> **1. Series C Timeline Acceleration** | URGENCY: High
> - Context: Market conditions favor raising now vs. Q1. Two tier-1 VCs have expressed interest following our recent product launch.
> - Options: (A) Accelerate to December close, (B) Maintain Q1 timeline, (C) Delay to Q2 for better metrics
> - Recommendation: Option A—Accelerate to December
> - Board action needed: Approve engagement of investment bank and authorize management to proceed
>
> **2. Engineering Team Expansion** | URGENCY: Medium
> - Context: Platform migration requires 4 additional senior engineers to maintain timeline. Current market allows favorable hiring.
> - Budget impact: $800K annually ($200K in Q4)
> - Recommendation: Approve hiring plan
> - Board action needed: Approve budget amendment
>
> [Document continues with Highlights, Risks, Financial Summary, etc.]

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Claude says "I don't see any files" | Wrong directory or files not readable | Verify you're in the right folder with `ls` or `dir`. Check file permissions. |
| Output is too generic/vague | Not enough specific data in source files | Add more detailed source documents, or explicitly point Claude to specific files: "Focus especially on the data in Q3-Financial-Summary.xlsx" |
| Numbers seem wrong | Claude may have misread or combined figures | Always spot-check. Ask Claude: "Show me exactly where you found the $12.4M revenue figure" |
| Missing a major topic | Source document may not have been processed | Ask: "Did you review the Customer-Health-Dashboard.csv? I don't see customer metrics in your output." |
| Output is too long | Default is comprehensive | Ask for a shorter version: "Condense this to 2 pages maximum, keeping only the most critical items" |
| Tone doesn't match your style | Claude defaults to neutral professional | Provide a sample: "Here's an example of how I typically write for this board: [paste sample]. Match this tone." |
| Sensitive data concerns | Confidential content in files | Review output before sharing. Ask Claude to remove or generalize specific details if needed. |

---

## Tips from Experience

1. **Start with more files than you think you need.** Claude can ignore irrelevant content, but it can't invent data that isn't there.

2. **Name files descriptively.** `Q3-Financial-Summary.xlsx` helps Claude more than `Report-Final-v2.xlsx`.

3. **Include previous meeting notes.** Claude can track action items and show progress, which boards love.

4. **Run this 2-3 days before the meeting**, not the night before. You want time to refine and add verbal context.

5. **Save your best prompts.** After a few iterations, you'll have a customized prompt that matches your board's preferences. Save it for reuse.

6. **Create a "standing context" file.** A simple text file with company overview, board member bios, and standing topics to always address. Include it in every prep folder.

7. **Don't over-automate the narrative.** The best briefings combine Claude's synthesis with your strategic judgment. Use Claude for assembly; you provide the interpretation.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Prep time dropped from 4-8 hours to under 1 hour
- [ ] No major topics were missed that a board member raised
- [ ] Numbers in the document matched source data when checked
- [ ] You felt more prepared, not less, than manual prep
- [ ] You could handle follow-up questions because you'd anticipated them

**Track over time:**
- Time spent on meeting prep (before vs. after adoption)
- Number of "surprises" in meetings you didn't anticipate
- Feedback from board/leadership on briefing quality

---

## Variations

### Investor Update
Modify the prompt to emphasize:
```
Focus heavily on: ARR growth, net retention, burn rate and runway, key milestones achieved, and competitive positioning. Frame everything through an investor lens—they care about growth trajectory and capital efficiency.
```

### Quarterly Business Review (Internal)
Modify the prompt to emphasize:
```
This is for our internal leadership team, so be more candid about challenges. Include department-level accountability, resource requests, and cross-functional dependencies. Less polish, more actionable detail.
```

### Annual Planning Kickoff
Modify the prompt to emphasize:
```
Frame this as backward-looking assessment AND forward-looking setup. Include: what worked this year, what didn't, market changes we need to respond to, and preliminary thinking on next year's priorities. End with discussion questions, not conclusions.
```

### Audit Committee
Modify the prompt to emphasize:
```
Focus on: compliance status, control findings, risk register updates, regulatory changes, and any financial reporting concerns. This audience wants detail and documentation, not high-level narrative.
```

---

## Building Your Repeatable System

After using this recipe 2-3 times, establish your system:

1. **Create a template folder structure** you copy for each meeting cycle
2. **Save your refined prompt** as a text file in a "prompts" folder
3. **Maintain a "standing context" document** with evergreen company information
4. **Build a checklist of source documents** you gather each cycle
5. **Set a calendar reminder** 3-4 days before each major meeting to start prep

**Sample Recurring Setup:**
```
Board-Meeting-Template/
├── 00-standing-context.txt      # Company overview, board bios, standing topics
├── 00-prompt-template.txt       # Your refined prompt
├── financials/                  # Empty folder, ready for this quarter's files
├── operations/
├── sales/
├── customer/
└── previous-meeting/            # Last meeting's notes and action items
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**aggregate scattered inputs → synthesize with AI → refine through conversation → export professional output**—applies broadly:

| Role | Application |
|------|-------------|
| **Directors/Managers** | Team status updates, leadership reviews |
| **Project Managers** | Project status briefings, steering committee prep |
| **Customer Success** | QBR prep, account review presentations |
| **Sales Leaders** | Pipeline reviews, forecast presentations |
| **Product Managers** | Roadmap reviews, stakeholder updates |
| **Finance** | Budget reviews, variance analysis presentations |

---

## Next Steps

1. **This week:** Try this recipe for your next meeting that requires multi-source synthesis
2. **Track your time:** Note how long prep takes with vs. without Claude Code
3. **Iterate your prompt:** After each use, refine based on what worked
4. **Share results:** Tell a colleague about your time savings

---

*Recipe #11 of 100 in the Claude Code Knowledge Worker Recipe Collection*
