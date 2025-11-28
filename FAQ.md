# Frequently Asked Questions

**Common Questions About Claude Code and the Top 100 Recipes**

---

## Before You Start

### How much does Claude Code cost?

Claude Code itself is free to install. However, you need a Claude subscription to use it:

| Option | Cost | Best For |
|--------|------|----------|
| **Claude Pro** | $20/month | Casual users, lighter usage |
| **Claude Max** | $100/month | Heavy users, professionals using recipes daily |
| **Claude Console** | Pay-per-use | Developers, variable usage patterns |
| **Enterprise** | Custom pricing | Organizations needing team features |

For regular recipe use, **Claude Max** provides the best value with higher usage limits.

### Is my data private? Can my employer see what I'm working on?

When using Claude Code:

- **Your files stay on your computer** — Claude Code reads files locally and sends only the content you explicitly share to Claude
- **Conversations are not used for training** — Anthropic does not use Claude Pro/Max/Enterprise conversations to train models
- **Enterprise plans** offer additional controls including data residency and audit logs

Check your organization's AI usage policies before using Claude Code for sensitive work. When in doubt, consult your IT or legal team.

### What's the difference between Claude Code and claude.ai?

| Feature | claude.ai | Claude Code |
|---------|-----------|-------------|
| Interface | Web browser | Terminal/command line |
| File access | Upload files manually | Read files directly from your computer |
| Best for | Conversations, quick questions | Working with local documents and data |
| Output | Copy/paste from browser | Can write files directly |

The recipes in this collection are designed for Claude Code because they involve working with files on your computer.

### Do I need to know how to code?

**No.** Claude Code runs in a terminal, which might look technical, but you're just typing text. If you can:
- Open an application
- Type a sentence
- Copy and paste

You can use Claude Code and these recipes. The GETTING-STARTED.md guide walks you through everything step by step.

---

## Using the Recipes

### How long does each recipe take?

Each recipe shows two time estimates:

1. **Setup Time** — How long the first use takes (learning the workflow)
2. **Time Saved** — How much time you save compared to doing it manually

Most recipes take 10-30 minutes the first time. After that, repeat uses are much faster because you know the workflow.

### Should I read the recipes in order?

**No.** Jump to whatever recipe matches a task you're facing today. The recipes are organized by function, not by difficulty progression.

Suggested starting points:
- **Everyone:** Start with Tier 1 (Recipes 001-010) — these are universal tasks
- **By role:** See the "Quick Start by Role" section in README.md
- **By need:** Scan the table of contents for a task you're doing this week

### Can I modify the prompts?

**Absolutely.** The prompts in each recipe are templates. You should:
- Replace `[BRACKETED]` placeholders with your specific information
- Adjust the tone, length, and format to match your needs
- Add context about your role, audience, and goals

Better prompts = better results. Don't be afraid to experiment.

### What if the output isn't what I expected?

This is normal. AI outputs are drafts, not finished products. Try:

1. **Be more specific** — Add details about what you want
2. **Provide examples** — Show Claude what "good" looks like
3. **Iterate** — Ask for revisions: "Make it more concise" or "Add more detail about X"
4. **Check your inputs** — Garbage in = garbage out. Better source material helps.

Each recipe has a "Troubleshooting" section for common issues.

### How do I save Claude's output to a file?

Several options:

1. **Copy and paste** — Select the output and paste into your destination
2. **Ask Claude to write it** — `"Save this to a file called output.md"`
3. **Redirect output** — `claude "your prompt" > output.txt` (for one-time commands)

---

## Technical Questions

### Can Claude Code read Excel files?

**Yes.** Claude Code can read:
- Excel files (.xlsx, .xls)
- CSV files (.csv)
- Word documents (.docx)
- PDFs (.pdf)
- Text files (.txt, .md)
- Most common document formats

### Can Claude Code access the internet?

**Limited.** Claude Code primarily works with files on your computer. For web research, you would:
1. Download/copy content to a local file
2. Have Claude Code analyze that file

Some enterprise configurations may have web access capabilities.

### What if I get "command not found: claude"?

This usually means Claude Code isn't in your PATH. Try:

**Mac/Linux:**
```bash
echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

**Windows:** Open a new terminal window, or reinstall following GETTING-STARTED.md.

### How do I update Claude Code?

Run the same installation command you used originally:

**Mac (Homebrew):**
```bash
brew upgrade claude-code
```

**Mac/Linux (curl):**
```bash
curl -fsSL https://claude.ai/install.sh | bash
```

**npm:**
```bash
npm update -g @anthropic-ai/claude-code
```

### Is there a usage limit?

Yes, depending on your subscription:

| Plan | Limits |
|------|--------|
| Claude Pro | Standard limits, may slow during heavy usage |
| Claude Max | 5x Pro limits |
| Console | Pay-per-use, no preset limits |
| Enterprise | Custom limits based on contract |

If you hit limits, you'll receive a message. Limits typically reset hourly or daily.

---

## About the Recipes

### Who created these recipes?

This collection was created to help knowledge workers get practical value from Claude Code. The recipes are based on real professional tasks across multiple industries and functions.

### How do I suggest a new recipe or report a problem?

Open an issue in the project repository with:
- The recipe number (if applicable)
- What you expected vs. what happened
- Any error messages or unexpected output

### Can I share these recipes with my team?

**Yes.** See LICENSE.md for full terms. In short:
- Share within your organization
- Use commercially in your work
- Modify and adapt for your needs
- Don't resell as a standalone product

### Will there be more recipes?

This collection covers 100 of the most common knowledge worker tasks. Future updates may add:
- New recipes for emerging use cases
- Improvements to existing recipes based on feedback
- Adaptations for new Claude Code features

---

## Best Practices

### How do I get the best results from Claude Code?

1. **Be specific** — Vague prompts get vague results
2. **Provide context** — Your role, audience, goals, constraints
3. **Include examples** — Show what "good" looks like
4. **Iterate** — Treat first outputs as drafts to refine
5. **Review everything** — AI output needs human judgment before use

### What should I NOT use Claude Code for?

Use caution or avoid:
- **Legal documents** that require attorney review
- **Medical advice** that requires professional expertise
- **Financial decisions** without professional validation
- **Confidential data** if your organization restricts AI use
- **Final outputs** without human review

Claude Code is a productivity tool, not a replacement for professional judgment.

### How do I build good habits with Claude Code?

1. **Start with one recipe** — Master it before trying others
2. **Create a workflow** — Same folder structure, same file naming
3. **Save your best prompts** — Keep a file of prompts that work well for you
4. **Review before sending** — Always check AI output before sharing
5. **Track your time savings** — Notice where you're getting the most value

---

## Getting More Help

### Where can I learn more about Claude Code?

- **Official docs:** docs.anthropic.com
- **Community:** github.com/anthropics/claude-code/issues
- **This collection:** Start with GETTING-STARTED.md

### I have a question not answered here

1. Check the GLOSSARY.md for term definitions
2. Check the specific recipe's Troubleshooting section
3. Ask Claude Code directly: `"How do I [your question]?"`
4. Open an issue in the project repository

---

*FAQ last updated: November 2025*
