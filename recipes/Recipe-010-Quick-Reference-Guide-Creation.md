# Quick Reference Guide Creation

**Recipe #10: From Complex Processes to Concise Guides**

---

| Setup Time | Time Saved | Difficulty | Best For |
|------------|------------|------------|----------|
| 10 minutes (first time) / 5 minutes (repeat) | 1-2 hours per guide | Beginner | Power users, trainers, support staff, anyone documenting expertise |

---

## The Problem

Complex processes, tools, and systems live in your head or scattered documentation. When others need help, you explain the same thing repeatedly. When you need a refresher after months away from a task, you struggle to remember the steps. Comprehensive documentation exists but nobody reads 50-page manuals for a quick answer.

**Pain Points:**
- Repeating explanations to colleagues constantly
- Forgetting steps for infrequent but important tasks
- Existing documentation too long or outdated
- No quick reference for common tasks
- Tribal knowledge that disappears when people leave
- Training new team members takes excessive time

---

## The Outcome

Concise, scannable quick reference guides that capture the essential steps, shortcuts, and tips for any process or tool. The kind of 1-2 page guide that lives on your desk (or desktop) and answers 90% of questions instantly.

**What You'll Have When Done:**
- Step-by-step procedures in scannable format
- Keyboard shortcuts and quick commands
- Common troubleshooting solutions
- Decision trees for "if X then Y" situations
- Tips and tricks from experience
- Reference that fits on 1-2 pages

---

## When to Use This Recipe

**Good Fit:**
- Documenting processes you explain repeatedly
- Creating training aids for new team members
- Building personal reference cards for complex tools
- Capturing tribal knowledge before someone leaves
- Converting lengthy docs into quick references
- Standard operating procedure summaries

**Not a Good Fit:**
- Comprehensive system documentation (this is a supplement, not replacement)
- Processes still being developed or frequently changing
- Situations requiring extensive context or judgment (guide format too limited)

---

## Before You Start: Quick Checklist

- [ ] Claude Code is installed and working
- [ ] You know the process or tool you're documenting
- [ ] You have notes, existing docs, or the knowledge in your head
- [ ] You know who will use this guide and their skill level
- [ ] You have 15-30 minutes for creation and refinement

---

## How Claude Code Helps

**What Claude Code Does Well:**
- Structures information in scannable formats
- Converts lengthy explanations into concise steps
- Creates consistent formatting across guides
- Generates decision trees and flow logic
- Organizes tips and troubleshooting logically
- Produces multiple format options (text, markdown, cheat sheet)

**Where Human Judgment Is Essential:**
- Verifying accuracy of steps and commands
- Adding tips that only come from experience
- Knowing which steps are critical vs. optional
- Including edge cases specific to your environment
- Testing the guide actually works

---

## Input Examples

**Ideal Source Materials:**

| Input Type | Example | What Claude Uses It For |
|------------|---------|------------------------|
| Process description | Verbal explanation of how you do something | Core content |
| Existing documentation | Long-form SOPs or manuals | Source material to condense |
| Screenshots or notes | Your personal notes on a process | Captures details |
| Tool interface | Description of menus/options | Accurate references |
| Common questions | "People always ask me..." | FAQ/troubleshooting |

**Sample Input (What You Might Provide):**
```
Need a quick reference guide for: Deploying code to production

What I usually explain to people:
- First you need to make sure all your tests pass locally
- Then create a pull request and get at least one approval
- Merge to main branch
- The CI/CD pipeline runs automatically - watch for green
- If it's a major release, you need to notify in #releases Slack channel
- Deployments are disabled during code freeze (Dec 15-Jan 5)
- If something goes wrong, there's a rollback script at /scripts/rollback.sh
- After deploy, always check the health dashboard
- Common issues: Docker build fails (usually means dependency mismatch), pipeline timeout (rerun usually fixes it)
```

---

## Step-by-Step Implementation

### Step 1: Gather Your Knowledge
**Time: 5-10 minutes**

Document what you know about the process:
- Write out the steps as you explain them
- Note any shortcuts or tips you always share
- List common problems and solutions
- Include any "gotchas" or warnings

Don't worry about organization—just dump your knowledge.

---

### Step 2: Launch Claude Code
**Time: 30 seconds**

```bash
claude
```

---

### Step 3: Run the Quick Reference Prompt
**Time: 2-3 minutes for Claude to process**

---

**PRIMARY PROMPT: Quick Reference Guide Generator**

```
Please create a quick reference guide based on my process knowledge.

TOPIC: [e.g., Deploying Code to Production]

MY KNOWLEDGE DUMP:
"""
[PASTE YOUR NOTES, STEPS, TIPS, AND EXPLANATIONS HERE]
"""

CONTEXT:
- Audience: [e.g., Junior developers, new team members, all staff]
- Skill level: [Beginner / Intermediate / Advanced]
- Format preference: [Quick reference card / Step-by-step / Cheat sheet]

PLEASE CREATE A QUICK REFERENCE GUIDE WITH:

1. TITLE AND PURPOSE
   - Clear title
   - One-line description of what this guide covers
   - When to use this guide

2. PREREQUISITES / BEFORE YOU START
   - What you need before starting
   - Access or permissions required
   - Any setup or preparation

3. QUICK STEPS (The Core Process)
   - Numbered steps, concise
   - Each step on one line if possible
   - Critical steps marked or highlighted
   - Optional steps clearly noted

4. KEY COMMANDS / SHORTCUTS
   - Table format for quick scanning
   - Commands, keyboard shortcuts, menu paths
   - What each does

5. COMMON ISSUES & SOLUTIONS
   - Table: Problem → Solution
   - Keep solutions brief
   - When to escalate

6. TIPS & BEST PRACTICES
   - Numbered list of pro tips
   - Things that save time or prevent problems
   - "Wish I knew this when I started"

7. DECISION TREE (if applicable)
   - If X, then Y format
   - For processes with branching logic

8. KEY CONTACTS / RESOURCES
   - Who to ask for help
   - Link to detailed documentation
   - Related guides

FORMAT REQUIREMENTS:
- Must fit on [1 page / 2 pages] when printed
- Use tables, bullets, and headers for scannability
- Bold critical warnings or steps
- Include command examples where relevant
```

---

### Step 4: Review for Accuracy
**Time: 5-10 minutes**

This step is critical—verify the guide actually works:

**Test the steps:**
- Walk through mentally (or actually) to verify sequence
- Check that no steps are missing
- Verify commands and syntax

**Check accuracy:**
- Are technical details correct?
- Are warnings in the right places?
- Did any of your tips get lost?

**Assess usability:**
- Would someone new actually be able to follow this?
- Is anything assumed that shouldn't be?

---

### Step 5: Refine and Enhance
**Time: 5-10 minutes**

**To add missing steps:**
```
Add a step between 3 and 4: you need to run "npm run build" to create the production bundle before the CI/CD pipeline works correctly.
```

**To add warnings:**
```
Add a prominent warning before step 5: "NEVER deploy during market hours (9am-4pm ET) without VP approval"
```

**To improve troubleshooting:**
```
Add these common issues:
- "Permission denied" error → need to re-authenticate with `aws sso login`
- Deployment stuck at "waiting" → check VPN connection
```

**To simplify:**
```
Steps 7-9 can be combined. Also, remove the section on legacy deployment—we don't use that anymore.
```

**To add a visual:**
```
Create a simple flowchart for the decision tree section using text/ASCII.
```

---

### Step 6: Export and Distribute
**Time: 2 minutes**

Save the guide:
```
Save this as "Production-Deployment-Quick-Reference.md"
```

For multiple formats:
```
Also create a minimal "cheat sheet" version that's just the commands and shortcuts, nothing else. Save as "Deployment-Cheat-Sheet.md"
```

---

## Example Output

Below is an abbreviated quick reference guide example:

---

> # Production Deployment Quick Reference
>
> **One-liner:** How to deploy code changes to production safely
> **When to use:** Any time you need to release code to production
>
> ---
>
> ## Prerequisites
> - [ ] Tests passing locally (`npm test`)
> - [ ] PR approved by at least one reviewer
> - [ ] Not during code freeze (Dec 15 - Jan 5)
> - [ ] Not during market hours without VP approval
>
> ---
>
> ## Quick Steps
>
> | Step | Action | Notes |
> |------|--------|-------|
> | 1 | Run `npm test` locally | All tests must pass |
> | 2 | Create Pull Request | Target: `main` branch |
> | 3 | Get approval | Minimum 1 reviewer |
> | 4 | Run `npm run build` | Creates production bundle |
> | 5 | Merge to main | CI/CD triggers automatically |
> | 6 | Watch pipeline | Green = success |
> | 7 | Post to #releases | Major releases only |
> | 8 | Check health dashboard | `dashboard.internal/health` |
>
> ---
>
> ## Key Commands
>
> | Command | What it does |
> |---------|--------------|
> | `npm test` | Run all tests |
> | `npm run build` | Create production bundle |
> | `./scripts/rollback.sh` | **Emergency rollback** |
> | `kubectl get pods` | Check deployment status |
>
> ---
>
> ## Common Issues
>
> | Problem | Solution |
> |---------|----------|
> | Docker build fails | Check dependencies match package-lock.json |
> | Pipeline timeout | Re-run pipeline (usually transient) |
> | "Permission denied" | Run `aws sso login` to re-authenticate |
> | Health check fails | Check logs: `kubectl logs -f deployment/app` |
>
> ---
>
> ## Tips
>
> 1. **Always check #releases for ongoing deployments** before starting yours
> 2. Deploy early in your day—gives time to fix issues
> 3. For risky changes, deploy to staging first (`npm run deploy:staging`)
> 4. Keep rollback script location bookmarked: `/scripts/rollback.sh`
>
> ---
>
> ## When to Escalate
>
> - Health dashboard red for >5 minutes → Page on-call
> - Customer-facing issue → #incidents + page on-call
> - Unsure about rollback → Ask before acting
>
> **On-call:** #oncall-platform | **Docs:** wiki/deployment

---

## Troubleshooting Common Issues

| Problem | Likely Cause | Solution |
|---------|--------------|----------|
| Guide is too long | Included too much detail | Specify: "This must fit on one page. Cut to essentials only." |
| Steps out of order | Knowledge dump was disorganized | Ask: "Verify the step sequence is correct and nothing is out of order" |
| Missing critical warnings | Didn't mention them in input | Add explicitly: "Add a warning box before step X about Y" |
| Too basic for audience | Skill level not specified | Clarify: "This is for intermediate users who know Git but not our deployment system" |
| Jargon unexplained | Assumed audience knowledge | Ask: "Add a glossary section for terms like CI/CD, staging, rollback" |
| Commands won't work | Environment-specific issues | Test commands; add notes about environment setup |

---

## Tips from Experience

1. **Test the guide yourself.** Follow your own guide step-by-step. You'll find missing steps immediately.

2. **Include the "why" for critical steps.** For important warnings, explain why: "Don't deploy during market hours (can cause trade delays)" is better than just "Don't deploy during market hours."

3. **Version and date your guides.** Processes change. A dated guide lets users know if it might be outdated.

4. **Put the cheat sheet where it's needed.** Print and post near the context. Digital guides should be findable in <10 seconds.

5. **Capture tribal knowledge before it leaves.** When an expert is departing, make quick reference creation a priority.

6. **Start with your most-repeated explanations.** If you've explained it 3+ times, it needs a guide.

---

## Measuring Success

**You've succeeded with this recipe when:**
- [ ] "How do I...?" questions decrease noticeably
- [ ] New team members can self-serve for common tasks
- [ ] You reference your own guides instead of remembering
- [ ] Others are creating guides using your template
- [ ] Time spent on repeated explanations drops significantly

**Track over time:**
- Number of guides created
- Decrease in repeat questions
- New hire onboarding time

---

## Variations

### Keyboard Shortcut Cheat Sheet
For tool-specific shortcuts:
```
Create a keyboard shortcut cheat sheet for [Tool Name].

Include:
- Navigation shortcuts
- Editing shortcuts
- View/display shortcuts
- Advanced/power user shortcuts

Format as a single-page reference card with:
- Two columns (command | shortcut)
- Grouped by category
- Most-used shortcuts highlighted
```

### Decision Tree Guide
For process with branching logic:
```
Create a decision tree guide for [Process Name].

The key decision points are:
- [Decision 1]: if X do A, if Y do B
- [Decision 2]: depends on [factor]
- [etc.]

Format as a visual flowchart using text/ASCII, with clear paths and outcomes.
```

### Troubleshooting Guide
For support or diagnostic processes:
```
Create a troubleshooting guide for [System/Process].

Common symptoms and causes:
[List what you know about problems and solutions]

Format as:
1. Symptom-based index (What are you seeing?)
2. Diagnostic steps for each symptom
3. Solution steps
4. When to escalate

Focus on the 10 most common issues that cover 80% of cases.
```

### Onboarding Quick Start
For new team member orientation:
```
Create a "First Day/Week Quick Start" guide for new [Role] on our team.

They need to:
- [List setup tasks]
- [List key tools to learn]
- [List people to meet]
- [List initial tasks]

Format as a checklist they can complete in order, with links to detailed resources for each item.
```

---

## Building Your Repeatable System

After creating several guides, establish your system:

1. **Create a guide template** with your standard sections
2. **Build a guide index** so people can find what exists
3. **Establish an update process** (who updates guides when processes change?)
4. **Set up a feedback mechanism** (how do users report issues or suggestions?)
5. **Schedule periodic reviews** (quarterly check for outdated guides)

**Sample Setup:**
```
quick-reference/
├── templates/
│   ├── quick-reference-template.md
│   └── cheat-sheet-template.md
├── guides/
│   ├── deployment/
│   │   ├── production-deploy.md
│   │   └── staging-deploy.md
│   ├── tools/
│   │   ├── jira-shortcuts.md
│   │   └── git-commands.md
│   └── processes/
│       ├── code-review.md
│       └── incident-response.md
└── INDEX.md                       # List of all guides
```

---

## How This Pattern Applies Elsewhere

This recipe's core pattern—**expert knowledge → structured extraction → concise reference**—applies broadly:

| Role | Application |
|------|-------------|
| **IT/Support** | System admin guides, troubleshooting trees |
| **Engineering** | Development workflows, tool guides |
| **Operations** | Process SOPs, checklist creation |
| **Sales** | CRM guides, process quick references |
| **HR** | Policy summaries, system how-tos |
| **Everyone** | Personal productivity tool guides |

---

## Next Steps

1. **This week:** Identify the process you explain most often
2. **Create your first guide:** Use the full prompt
3. **Test it:** Have someone new follow the guide
4. **Iterate:** Refine based on their feedback
5. **Share:** Make the guide findable and tell your team

---

*Recipe #10 of 100 in the Claude Code Knowledge Worker Recipe Collection*
