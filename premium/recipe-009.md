---
description: Clean up and standardize messy data for analysis
---

Please clean and standardize this data:

$ARGUMENTS

If the content above shows "$ARGUMENTS" (meaning no data was provided), please:
1. Explain that no data was provided when they called the command
2. Inform them they can provide the information in several ways:
   - Type or paste it directly in their next message
   - Reference a file using @filename (e.g., @data.csv, @spreadsheet.xlsx, @rawdata.txt)
   - Reference a URL using the URL directly (if the data is accessible via URL)
   - Re-run the command with inline arguments: /recipe-009 <data to clean>
3. Ask the user to provide the data they want cleaned and standardized
4. Wait for them to share the details
5. Then proceed with the full cleanup

Otherwise, proceed immediately with data cleanup:

CLEANUP REQUIREMENTS:

1. COLUMN STANDARDIZATION
   - Standardize column names (lowercase, underscores, descriptive)

2. DATE FORMATTING
   - Target format: YYYY-MM-DD
   - Handle various input formats
   - Flag any unparseable dates

3. TEXT STANDARDIZATION
   - Names: Title Case
   - Emails: lowercase
   - Trim whitespace

4. MISSING VALUES
   - Flag empty required fields
   - Note patterns in missing data

5. DUPLICATES
   - Identify duplicate rows
   - Flag for review

6. DATA VALIDATION
   - Email format validation
   - Numeric columns check

PLEASE PROVIDE:

1. CLEANED DATA - Full cleaned dataset

2. CHANGE LOG - Summary of all changes made

3. DATA QUALITY REPORT
   - Missing value count per column
   - Duplicate rows found
   - Validation failures
   - Any anomalies noticed
