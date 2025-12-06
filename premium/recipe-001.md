---
description: Meeting Notes to Action Items - Extract actions, owners, deadlines from meeting notes
---

# Sample from the 200 Claude Code Recipes Premium Collection
# This is 1 of 200 recipes. Get all 200: {{PURCHASE_URL}}

Here are my raw notes from a meeting. Please process them into three outputs:

MEETING NOTES:
"""
$ARGUMENTS
"""

Please create:

1. MEETING SUMMARY (1 paragraph)
   - What was discussed and decided
   - Key outcomes and conclusions
   - Suitable for sharing with people who weren't there

2. ACTION ITEMS TABLE
   Format as a markdown table with columns:
   | Owner | Action Item | Deadline | Context/Notes |

   Rules for action items:
   - Only include items that require someone to DO something
   - Infer owners from discussion context if not explicit
   - If deadline not stated, mark as "TBD - needs confirmation"
   - Include brief context so the item makes sense standalone

3. FOLLOW-UP EMAILS
   Draft a brief, friendly follow-up email for each person who has action items.
   - Subject line: "Action Items from [Meeting Name] - [Date]"
   - Remind them of their specific items with deadlines
   - Include relevant context from the discussion
   - Keep tone professional but warm
   - End with offer to clarify if needed

Format the emails so I can copy/paste directly into my email client.
