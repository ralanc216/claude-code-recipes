# Rapid Presentation Development

**Recipe #5: From Blank Slide to Complete Deck**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 15 minutes (first time) / 5 minutes (repeat) | 3-6 hours per deck | Beginner | All professionals who create presentations |

---

## The Problem

Creating presentations is time-consuming and often dreaded. You start with a blank deck, struggle to organize your thoughts, spend hours on structure before even getting to content, then wrestle with each slide. The result: hours of work, often the night before, for a deck that might still lack clear narrative flow.

**Pain Points:**
- Blank slide paralysis—where do you even start?
- Organizing complex information into slide format
- Creating consistent, professional slide content
- Writing effective speaker notes
- Iterating on structure takes forever
- Night-before scrambles for presentations

---

## The Outcome

A complete presentation draft—outline, slide-by-slide content, and speaker notes—generated in minutes from your key points and data. You focus on refining and adding your expertise rather than starting from zero. What took 4+ hours now takes under 1.

**What You'll Have When Done:**
- Complete slide-by-slide content with headers and bullets
- Logical narrative flow through the presentation
- Speaker notes for each slide
- Suggested visualizations and data placement
- A foundation you can polish in your presentation tool

---

## When to Use This Recipe

**Good Fit:**
- Business presentations and strategy decks
- Project updates and status presentations
- Sales presentations and pitches
- Training and enablement materials
- Conference talks and webinars
- Team and department updates

**Not a Good Fit:**
- Highly visual/design-focused presentations (use a designer)
- Presentations requiring extensive proprietary data visualization
- Situations where the presentation itself is the deliverable for review
- Quick 5-slide updates (might be faster to just create directly)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You know your topic and key message
- [ ] You know your audience and what they care about
- [ ] You have any data, points, or content to include
- [ ] You know the presentation length (number of slides or time)
- [ ] You have 15-30 minutes for generation and initial refinement

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Creates logical presentation structure and flow
- Translates ideas into slide-appropriate content
- Generates concise, impactful bullet points
- Writes speaker notes that complement slide content
- Suggests where to use visuals, charts, or data
- Maintains consistent format throughout the deck

**Where Human Judgment Is Essential:**
- Final narrative and messaging decisions
- Data accuracy and appropriateness
- Design and visual choices
- Audience-specific customization
- Proprietary information and context
- Delivery preparation beyond notes

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Key points | Bullet list of main ideas | Core content for slides |
| Data files | `quarterly-metrics.xlsx` | Specific numbers to feature |
| Existing docs | `project-proposal.docx` | Source material to transform |
| Audience info | "Senior leadership, 30 min slot" | Tailors depth and tone |
| Examples | "Similar to our Q2 review deck" | Style reference |

**Sample Input (What You Might Provide):**
```
Need a presentation for:
- Quarterly business review for leadership team
- 20 minutes, expect 10 minutes Q&A
- Audience: CEO, CFO, VP Sales, VP Product

Key points to cover:
- Q3 revenue: $8.2M (105% of target)
- Customer growth: 23% YoY
- Churn improved from 4.2% to 3.1%
- Launched 3 major features
- Opened new enterprise segment
- Challenge: sales cycle lengthening
- Q4 priorities: enterprise focus, reduce time-to-close
- Need: approval for 2 additional sales hires

Tone: Confident but realistic
```

---

## Step-by-Step Implementation

### Step 1: Gather Your Inputs
**Time: 5-10 minutes**

Collect what you know needs to be in the presentation:
- Key points and main message
- Any data or metrics to include
- Decisions or asks you're making
- Audience context and constraints

Dump these into a simple text file or prepare to paste them directly.

**Pro Tip:** Don't worry about organization yet. The messier your dump, the more value Claude adds by structuring it.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

If you have supporting documents:
```bash
cd ~/Documents/qbr-prep
claude
```

---

### Step 3: Run the Presentation Generator Prompt
**Time: 3-5 minutes for Claude to process**

---

**PRIMARY PROMPT: Presentation Generator**

```
Please create a complete presentation for me.

PRESENTATION CONTEXT:
- Topic: [e.g., Q3 Business Review, Project Proposal, Sales Pitch]
- Audience: [e.g., Executive team, Board, Clients, All-hands]
- Duration: [e.g., 20 minutes presentation + 10 min Q&A]
- Slide count target: [e.g., 10-12 slides]
- Tone: [e.g., Confident and professional, Conversational, Formal]
- Goal: [e.g., Inform, get approval, persuade, educate]

KEY CONTENT TO INCLUDE:
"""
[PASTE YOUR KEY POINTS, DATA, AND IDEAS HERE]
"""

PLEASE PROVIDE:

1. PRESENTATION OUTLINE
   - Title slide concept
   - Section breakdown with flow logic
   - Key transition points

2. SLIDE-BY-SLIDE CONTENT
   For each slide, provide:
   - Slide title (clear and action-oriented where appropriate)
   - Main content (bullets, key points—not paragraphs)
   - Suggested visual/chart (if applicable)
   - Speaker notes (2-4 sentences of what to say)

3. FORMAT GUIDELINES
   - Maximum 4-5 bullets per slide
   - Bullets should be concise (one line each)
   - Include specific data points where relevant
   - Suggest "visual slides" where a chart/image beats text

4. CLOSING ELEMENTS
   - Clear call to action or summary slide
   - Recommended Q&A talking points
   - Anticipated tough questions with suggested responses
```

---

### Step 4: Review the Structure
**Time: 5-10 minutes**

Before diving into slides, review the outline:

**Flow check:**
- Does the narrative make sense?
- Is it the right depth for your audience?
- Are the sections in the right order?

**Coverage check:**
- Are all your key points addressed?
- Is anything important missing?
- Is anything included that shouldn't be?

If the structure needs changes, adjust now before refining individual slides.

---

### Step 5: Refine Individual Slides
**Time: 10-15 minutes**

Once structure is right, refine specific slides:

**To strengthen a slide:**
```
Slide 5 on customer growth needs more impact. Can you reframe it to emphasize the YoY improvement and what it means for our trajectory?
```

**To add data:**
```
For the revenue slide, the actual numbers are: Q3 $8.2M, Q2 $7.8M, Q1 $7.5M. Please update with a quarter-over-quarter growth narrative.
```

**To simplify:**
```
Slide 7 is too dense. Split it into two slides or reduce to the 3 most important points.
```

**To adjust tone:**
```
The challenges slide sounds too negative. Reframe as "areas of focus" with a more confident tone.
```

**To add speaker notes:**
```
Expand the speaker notes for slides 3-5. I need more detail on what to say during the data-heavy section.
```

---

### Step 6: Export and Build
**Time: 2 minutes + build time**

Once content is finalized:

```
Save this as "QBR-Q3-2024-Presentation.md"
```

Then create the actual presentation:
```
Please create this as a PPTX file named "QBR-Q3-2024.pptx"
```

Or, for greater control, use the markdown output to build slides in your preferred tool (PowerPoint, Google Slides, Keynote).

---

## Example Output

Below is abbreviated example output for a quarterly business review:

---

> **PRESENTATION OUTLINE**
>
> 1. Title: Q3 2024 Business Review
> 2. Executive Summary (the story in one slide)
> 3. Revenue Performance (the win)
> 4. Customer Growth & Retention (momentum)
> 5. Product Highlights (what we delivered)
> 6. Enterprise Expansion (new opportunity)
> 7. Challenges & Focus Areas (honest assessment)
> 8. Q4 Priorities (where we're headed)
> 9. Resource Request (the ask)
> 10. Summary & Discussion
>
> ---
>
> **SLIDE 2: Executive Summary**
>
> *Title:* Q3 Delivered Strong Results with Clear Path Forward
>
> *Content:*
> - Revenue: **$8.2M** (105% of target, +5% QoQ)
> - Customer base grew **23% YoY** with churn improving to 3.1%
> - Launched 3 major platform features; enterprise segment opened
> - **Challenge:** Sales cycle lengthening—requires focus
> - **Q4 Priority:** Accelerate enterprise with additional sales capacity
>
> *Visual:* Dashboard-style summary metrics
>
> *Speaker Notes:* "Before we dive into details, here's the headline: Q3 was our strongest quarter this year on revenue and customer growth. We hit 105% of target and significantly improved retention. We also opened a major new segment—enterprise. The one area requiring focus is our lengthening sales cycle, and I'll cover our plan to address that, including a specific resource request."
>
> ---
>
> **SLIDE 3: Revenue Performance**
>
> *Title:* Revenue Exceeded Target for Third Consecutive Quarter
>
> *Content:*
> - Q3 Revenue: **$8.2M** (105% of plan)
> - Q1: $7.5M → Q2: $7.8M → Q3: $8.2M
> - **9% growth** from Q1 to Q3
> - Expansion revenue up 34% (existing customer growth)
> - New logo revenue on target
>
> *Visual:* Bar chart showing quarterly revenue with trendline
>
> *Speaker Notes:* "Revenue continues its upward trajectory. The $8.2M represents our best quarter ever and our third consecutive beat. Particularly encouraging is expansion revenue—our existing customers are growing with us, up 34%. This speaks to product-market fit and customer success effectiveness."
>
> ---
>
> **SLIDE 7: Challenges & Focus Areas**
>
> *Title:* Addressing Our Sales Cycle Challenge
>
> *Content:*
> - Average sales cycle: 45 days → 58 days (+29%)
> - Root cause: Enterprise deals have longer procurement
> - Impact: Q4 pipeline healthy but timing risk
> - **Actions underway:**
>   - Streamlined security review process
>   - Added procurement acceleration resources
>   - Enhanced ROI/business case tools
>
> *Visual:* Simple chart showing cycle length trend with inflection point when enterprise started
>
> *Speaker Notes:* "I want to address our main challenge head-on. Our sales cycle has lengthened from 45 to 58 days. This is almost entirely driven by enterprise—exactly the segment we're excited about, but one with longer procurement cycles. We've already implemented several changes and are seeing early improvement. However, to fully address this and not leave revenue on the table, I'm requesting additional sales capacity, which I'll cover next."
>
> ---
>
> **ANTICIPATED Q&A**
>
> *Q: Why is the sales cycle lengthening?*
> A: Direct result of enterprise expansion. Enterprise deals are 3-4x larger but have procurement/security review cycles. We're addressing with process changes and expect improvement in Q4.
>
> *Q: What's the ROI on additional sales hires?*
> A: Current pipeline supports 2x coverage with right capacity. At our average deal size, each hire should generate $1.5M+ annually by month 6, with 8-month payback.
>
> *Q: How confident are we in the Q4 forecast?*
> A: Pipeline coverage is 2.8x, our highest ever. The question is timing, which is why addressing sales cycle is priority one.

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Slides too text-heavy | Default comprehensive output | Specify: "Maximum 4 bullets, maximum 8 words per bullet" |
| Wrong level of detail | Audience not specified clearly | Clarify: "This is for executives who want headlines, not details" |
| Missing key points | They weren't in your input | Add them: "Please add a slide on customer churn improvement showing the trend" |
| Narrative doesn't flow | Structure issue | Ask: "Reorder the slides to tell this story: [describe desired narrative]" |
| Too many slides | Duration not specified | Specify: "Must be 10 slides maximum for a 15-minute presentation" |
| Wrong tone | Tone not calibrated | Provide example: "Use more confident language. Instead of 'we saw some improvement' say 'we achieved strong improvement'" |
| Generic content | Specifics not provided | Add data: "Here are the actual numbers: [provide data]" |

---

## Tips from Experience

1. **Start with your key message.** What's the one thing the audience must remember? Build around that.

2. **Provide real data.** Generic presentations come from generic input. The more specific data you provide, the more specific (and useful) the output.

3. **Specify "visual slides."** Tell Claude when a slide should be mostly visual: "Slide 4 should be a single chart with minimal text."

4. **Generate Q&A preparation.** Always include anticipated tough questions. This prep is often more valuable than the slides themselves.

5. **Create multiple versions.** A 20-slide detailed version and a 5-slide executive summary from the same content takes 2 minutes extra and provides flexibility.

6. **Don't skip the speaker notes.** Even if you know your material, structured notes help with timing and ensure you hit key points.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] Presentation creation time dropped by 50%+
- [ ] You spend more time refining than building from scratch
- [ ] Narrative flow is consistently strong
- [ ] Audience feedback is positive
- [ ] You don't dread creating presentations anymore

**Track over time:**
- Time from "need a presentation" to "done"
- Number of revision cycles needed
- Audience engagement and feedback

---

## Variations

### Sales Pitch Deck
For persuasive client-facing presentations:
```
This is a sales pitch to [prospect type]. Please structure as:
1. Hook: Their problem/pain (1 slide)
2. Stakes: Cost of status quo (1 slide)
3. Solution: Our approach (2-3 slides)
4. Proof: Results/testimonials (1-2 slides)
5. How it works: Process/implementation (1-2 slides)
6. Ask: Clear next step (1 slide)

Tone should be confident but not pushy. Focus on their outcomes, not our features.
```

### Training/Enablement Deck
For educational internal presentations:
```
This is training material for [audience]. Please structure for learning:
1. Overview: What and why
2. Concept breakdown: Core ideas with examples
3. How-to: Step-by-step process
4. Practice: Exercises or scenarios
5. Common mistakes: What to avoid
6. Resources: Where to learn more

Use visuals and examples heavily. Include knowledge check questions.
```

### All-Hands / Company Update
For broad organizational communication:
```
This is for our monthly all-hands (150 employees). Please include:
1. Win celebrations (start positive)
2. Business metrics (transparency)
3. Key initiatives update (what's happening)
4. Challenges we're facing (honesty)
5. What's ahead (forward-looking)
6. Recognition / shout-outs (culture)
7. Q&A preview (anticipated questions)

Tone: Energetic but authentic. Mix serious content with moments of lightness.
```

### Conference Talk
For external speaking engagements:
```
This is a [X-minute] conference talk on [topic]. Audience is [description].

Structure for engagement:
1. Opening hook (story or surprising stat)
2. Problem framing (why this matters)
3. Key insight 1 (with example)
4. Key insight 2 (with example)
5. Key insight 3 (with example)
6. Practical takeaways (what to do differently)
7. Memorable close (circle back to opening)

Minimize bullets. Maximize storytelling and concrete examples.
```

---

## Building Your Repeatable System

After creating several presentations, establish your system:

1. **Save prompt templates** for your common presentation types
2. **Create a "brand voice" guide** with your preferred tone and style
3. **Build a content library** of frequently used slides/sections
4. **Store data sources** you regularly include (metrics, backgrounds)
5. **Maintain a "presentation archive"** for reference

**Sample Setup:**
```
presentations/
├── templates/
│   ├── qbr-prompt.txt
│   ├── sales-pitch-prompt.txt
│   └── all-hands-prompt.txt
├── brand-guide/
│   └── presentation-style.txt
├── data/
│   ├── company-metrics.xlsx
│   └── brand-assets.md
└── archive/
    ├── 2024-Q1-QBR/
    ├── 2024-Q2-QBR/
    └── ...
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**key points → structured narrative → formatted output**—applies broadly:

| Role | Application |
|------|-------------|
| **Executives** | Board presentations, investor decks, strategy reviews |
| **Sales** | Pitch decks, proposals, deal reviews |
| **Product** | Roadmap presentations, feature launches, stakeholder updates |
| **Marketing** | Campaign readouts, brand presentations, event content |
| **HR** | Training materials, policy rollouts, company updates |
| **Finance** | Budget presentations, financial reviews, planning decks |

---

## Next Steps

1. **This week:** Use this for your next presentation
2. **Save your best prompt:** Customize for your common presentation types
3. **Try variations:** Experiment with sales, training, or all-hands formats
4. **Share:** When a deck turns out well, share the recipe with a colleague who struggles with presentations

---

*Recipe #5 of 100 in the Claude Code Knowledge Worker Recipe Collection*
