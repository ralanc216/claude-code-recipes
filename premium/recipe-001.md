---
description: Convert meeting notes into action items with owners and deadlines
---

Here are my raw notes from a meeting. Please process them into three outputs:

MEETING NOTES:
"""
$ARGUMENTS
"""

If the MEETING NOTES above shows "$ARGUMENTS" (meaning no data was provided), please:
1. Explain that no data was provided when they called the command
2. Inform them they can provide the information in several ways:
   - Type or paste it directly in their next message
   - Reference a file using @filename (e.g., @data.txt, @document.xlsx, @report.pdf)
   - Reference a URL using the URL directly (if the information is on a webpage)
   - Re-run the command with inline arguments: /recipe-001 <details>
3. Ask the user to provide the necessary information
4. Wait for them to share the details
5. Then proceed with the full analysis

Otherwise, proceed immediately with creating:

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
