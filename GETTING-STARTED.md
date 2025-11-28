# Getting Started with Claude Code

**Your Guide to Installing and Using Claude Code for the Top 100 Recipes**

*Last Updated: November 2025*

---

## What is Claude Code?

Claude Code is Anthropic's official command-line interface (CLI) tool that brings Claude's AI capabilities directly into your terminal. Unlike the web interface at claude.ai, Claude Code is designed for professionals who work with files, code, documents, and data on their local machines.

With Claude Code, you can:
- Analyze and transform documents directly from your file system
- Generate reports, summaries, and communications
- Work with spreadsheets, presentations, and business documents
- Automate repetitive knowledge work tasks
- Process multiple files and create structured outputs

The **Top 100 Claude Code Recipes for Knowledge Workers** are designed to work with Claude Code's ability to read your files, understand context, and produce professional outputs—all from your terminal.

---

## Before You Begin: What You'll Need

### Account Requirements

You need **one** of the following to use Claude Code:

| Option | Best For | How to Get It |
|--------|----------|---------------|
| **Claude Pro/Max** | Individual professionals | Subscribe at claude.ai/pricing |
| **Claude Console** | Developers, pay-as-you-go | Create account at console.anthropic.com |
| **Enterprise** | Organizations | Contact Anthropic sales or use AWS Bedrock/Google Vertex AI |

**Recommendation for Recipe Users:** Claude Max subscription provides the best experience with higher usage limits at a predictable monthly cost. This is ideal if you plan to use multiple recipes regularly.

### System Requirements

| Requirement | Minimum | Recommended |
|-------------|---------|-------------|
| **RAM** | 4 GB | 8 GB+ |
| **Storage** | 500 MB free | 1 GB+ free |
| **Internet** | Required | Stable broadband |
| **Location** | Anthropic-supported country | — |

### Operating System Compatibility

| OS | Versions Supported | Notes |
|----|-------------------|-------|
| **macOS** | 10.15 (Catalina) or higher | Native support |
| **Windows** | Windows 10 or higher | WSL recommended; native PowerShell available |
| **Linux** | Ubuntu 20.04+, Debian 10+ | Native support |

---

## Installation Instructions

Choose your operating system below and follow the steps.

### macOS Installation

macOS users have the smoothest installation experience. Choose one method:

#### Method 1: Homebrew (Recommended)

If you have Homebrew installed (most Mac developers do):

```bash
brew install --cask claude-code
```

#### Method 2: Direct Installation

Open Terminal and run:

```bash
curl -fsSL https://claude.ai/install.sh | bash
```

After installation completes, reload your shell:

```bash
source ~/.zshrc
```

*(If you use bash instead of zsh, run `source ~/.bashrc`)*

#### Verify Installation

```bash
claude --version
claude doctor
```

You should see the version number and a health check confirming everything is working.

---

### Windows Installation

Windows users have several options. We recommend WSL for the best experience.

#### Method 1: WSL (Windows Subsystem for Linux) — Recommended

WSL gives you a Linux environment inside Windows, providing the most reliable Claude Code experience.

**Step 1: Install WSL** (if you haven't already)

Open PowerShell as Administrator and run:

```powershell
wsl --install
```

Restart your computer when prompted.

**Step 2: Open your WSL terminal**

After restart, open "Ubuntu" from your Start menu (or whichever Linux distribution you installed).

**Step 3: Install Claude Code**

In your WSL terminal:

```bash
curl -fsSL https://claude.ai/install.sh | bash
source ~/.bashrc
```

**Step 4: Verify**

```bash
claude --version
claude doctor
```

#### Method 2: Native Windows with PowerShell

If you prefer not to use WSL:

**Step 1: Install Git for Windows**

Download and install from [git-scm.com](https://git-scm.com/download/win) if you don't have it.

**Step 2: Run the installer**

Open PowerShell and run:

```powershell
irm https://claude.ai/install.ps1 | iex
```

**Step 3: Verify**

Open a new terminal window and run:

```bash
claude --version
claude doctor
```

#### Method 3: NPM Installation

If you have Node.js 18+ installed:

```bash
npm install -g @anthropic-ai/claude-code
```

**Important:** Do NOT use `sudo` with npm installations—this can cause permission issues.

---

### Linux Installation

#### Standard Installation (Recommended)

Open your terminal and run:

```bash
curl -fsSL https://claude.ai/install.sh | bash
source ~/.bashrc
```

*(Use `source ~/.zshrc` if you use Zsh)*

#### If "command not found" appears

Add Claude Code to your PATH:

```bash
echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

#### Verify Installation

```bash
claude --version
claude doctor
```

---

## First-Time Setup and Authentication

After installation, you need to authenticate Claude Code with your account.

### Step 1: Navigate to a Project Folder

Claude Code works best when launched from a directory containing files you want to work with. For the recipes, this might be:

- A folder with documents you want to analyze
- Your company's shared drive
- A project folder with reports and data

```bash
cd ~/Documents/my-project
```

Or for the recipes collection:

```bash
cd path/to/exec-ai-recipes
```

### Step 2: Launch Claude Code

```bash
claude
```

### Step 3: Complete Authentication

On first launch, Claude Code will guide you through authentication:

1. A browser window will open (or you'll see a URL to visit)
2. Log in with your Claude account
3. Authorize Claude Code to access your account
4. Return to your terminal—you're now connected

Your credentials are stored securely on your local machine. You won't need to authenticate again unless you log out or your session expires.

### Step 4: Verify Everything Works

Run the health check:

```bash
claude doctor
```

This confirms:
- Installation is correct
- Authentication is working
- You're ready to use Claude Code

---

## Basic Usage

### Starting an Interactive Session

The most common way to use Claude Code is in interactive mode:

```bash
claude
```

You'll see a prompt where you can type requests:

```
> summarize the document in reports/quarterly-review.pdf
> analyze this spreadsheet and identify the top 5 trends
> help me write an email responding to the customer complaint in inbox/
```

### One-Time Commands

For quick tasks, you can run Claude Code with a direct command:

```bash
claude "summarize all the PDF files in this folder"
claude "what is this project about?"
claude "list all the TODO items in these documents"
```

### Useful Commands Inside Claude Code

| Command | What It Does |
|---------|--------------|
| `/clear` | Clear the conversation history |
| `/help` | Show available commands |
| `exit` or `Ctrl+C` | Exit Claude Code |

### Working with Files

Claude Code can read files in your current directory and subdirectories:

```
> read the file reports/sales-data.xlsx and summarize the key metrics
> compare document-v1.docx with document-v2.docx
> analyze all the .csv files in the data folder
```

---

## Preparing to Use the Recipes

The Top 100 Recipes are designed to work with real business inputs. Here's how to prepare:

### Organizing Your Input Files

For best results, create a working folder structure:

```
my-work/
├── inputs/           # Put source materials here
│   ├── emails/
│   ├── reports/
│   ├── data/
│   └── documents/
├── outputs/          # Claude's generated content goes here
└── templates/        # Any templates you use regularly
```

### Typical Recipe Workflow

1. **Gather your inputs** — Collect the documents, data, or information the recipe calls for
2. **Navigate to your folder** — `cd path/to/your/working/folder`
3. **Launch Claude Code** — `claude`
4. **Follow the recipe steps** — Paste or adapt the prompts from the recipe
5. **Review and refine** — Ask Claude to adjust the output as needed
6. **Save the output** — Copy to your destination or ask Claude to write to a file

### Example: Using Recipe 001 (Meeting Notes to Action Items)

```bash
# Navigate to your work folder
cd ~/Documents/work

# Launch Claude Code
claude

# Follow the recipe
> I just finished a project kickoff meeting. Here are my raw notes:
>
> Attendees: Sarah (PM), Mike (Engineering), Lisa (Design), John (Sales)
>
> - discussed timeline, Mike says 6 weeks for MVP
> - Lisa needs brand guidelines from marketing by Friday
> - John will send customer requirements doc
> - need to schedule weekly syncs - Sarah to set up
> - budget approved but need to track hours
> - Mike concerned about API dependencies
> - next meeting Monday 10am
>
> Please extract all action items with owners and deadlines, then create
> a formatted meeting summary I can share with the team.
```

---

## Tips for Success

### Working with Large Documents

Claude Code handles large files well, but for very large documents:

- Break them into sections if possible
- Ask Claude to analyze specific parts first
- Use the "summarize first, then analyze" approach

### Getting Better Results

1. **Be specific** — "Analyze sales trends" is good; "Analyze Q3 sales trends focusing on regional differences and seasonal patterns" is better
2. **Provide context** — Tell Claude about your role, audience, and goals
3. **Iterate** — Ask for revisions: "Make it more concise" or "Add more detail about X"
4. **Use examples** — "Format it like the example in template.docx"

### Managing Your Session

- Long conversations use more context—start fresh for new topics with `/clear`
- Save important outputs immediately
- Keep your working folder organized

---

## Troubleshooting Common Issues

### "Command not found: claude"

**macOS/Linux:** Your PATH may not include Claude Code's location.

```bash
echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

**Windows:** Try opening a new terminal window, or verify the installation completed successfully.

### Authentication Problems

If authentication fails or expires:

```bash
claude /login
```

This will restart the authentication flow.

### Slow Responses

- Check your internet connection
- Very large files may take longer to process
- Try breaking large requests into smaller parts

### Permission Errors

- Make sure you have read access to the files you're asking Claude to analyze
- On macOS, you may need to grant Terminal access to your Documents folder in System Preferences > Privacy & Security

### Getting Help

Run the health check for diagnostic information:

```bash
claude doctor
```

For more help:
- Claude Code documentation: docs.anthropic.com
- Community support: github.com/anthropics/claude-code/issues

---

## Quick Reference Card

### Installation Commands

| OS | Command |
|----|---------|
| macOS (Homebrew) | `brew install --cask claude-code` |
| macOS/Linux | `curl -fsSL https://claude.ai/install.sh \| bash` |
| Windows (PowerShell) | `irm https://claude.ai/install.ps1 \| iex` |
| Any (with Node.js) | `npm install -g @anthropic-ai/claude-code` |

### Essential Commands

| Action | Command |
|--------|---------|
| Start Claude Code | `claude` |
| One-time query | `claude "your question here"` |
| Check installation | `claude doctor` |
| Check version | `claude --version` |
| Re-authenticate | `claude /login` |
| Exit | `exit` or `Ctrl+C` |

### Your First Session Checklist

- [ ] Account created (Claude Pro/Max or Console)
- [ ] Claude Code installed
- [ ] Installation verified with `claude doctor`
- [ ] First authentication completed
- [ ] Test query successful
- [ ] Ready to use the recipes!

---

## Next Steps

You're now ready to use Claude Code with the Top 100 Recipes. Start with recipes that match your immediate needs:

**New to Claude Code?** Try these beginner-friendly recipes first:
- [Recipe 001: Meeting Notes to Action Items](recipes/Recipe-001-Meeting-Notes-to-Action-Items.md)
- [Recipe 002: Weekly Status Report Generation](recipes/Recipe-002-Weekly-Status-Report-Generation.md)
- [Recipe 003: Email Drafting and Response](recipes/Recipe-003-Email-Drafting-and-Response.md)
- [Recipe 004: Document Summarization](recipes/Recipe-004-Document-Summarization.md)

**Looking for quick wins?** These recipes deliver fast results:
- [Recipe 005: Rapid Presentation Development](recipes/Recipe-005-Rapid-Presentation-Development.md)
- [Recipe 007: Research Synthesis](recipes/Recipe-007-Research-Synthesis.md)
- [Recipe 010: Quick Reference Guide Creation](recipes/Recipe-010-Quick-Reference-Guide-Creation.md)

**Ready for advanced use?** Explore these powerful recipes:
- [Recipe 021: Competitive Intelligence Synthesis](recipes/Recipe-021-Competitive-Intelligence-Synthesis.md)
- [Recipe 025: Financial Analysis and Trend Interpretation](recipes/Recipe-025-Financial-Analysis-Trend-Interpretation.md)
- [Recipe 051: Dashboard Narrative Generation](recipes/Recipe-051-Dashboard-Narrative-Generation.md)

Browse the full collection in the [README.md](README.md) or the `recipes/` folder, organized by tier and numbered for easy reference.

---

*Happy automating! The recipes are designed to save you hours of work—pick one that matches a task you're facing today and experience the productivity gains firsthand.*
