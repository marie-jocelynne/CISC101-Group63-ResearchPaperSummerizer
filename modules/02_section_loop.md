# Module 02 — Section Loop

> Change Log (Task 3 – Week 10):
> - Added the `summary_level` setting (short vs detailed).
> - Added clear rules for how to write each type of summary.
> - Explained how expert vs layperson wording should work.

## What This Module Does

This module explains how the system goes through each section of the paper and writes a summary for it. It follows whatever the user chose (short or detailed summary, expert or lay audience).

## How It Works (Step-by-Step)

### 1. Look at the Section Text
The system starts by checking the text for the section.  
If the text is missing or too short, Module 3 handles that with warnings.

### 2. Choose the Summary Length
The system uses the setting:


**If it’s “short”:**
- The system writes a quick **1–2 sentence** summary that captures the main idea.

**If it’s “detailed”:**
- The system writes:
  - A **short paragraph** explaining the section in more depth.
  - A **bullet list of 3–5 key points** (important details, results, methods, or ideas).

### 3. Adjust the Tone for the Audience
The user chooses an audience:

- **Expert** → more technical wording, assumes background knowledge.
- **Layperson** → simpler explanations, avoids jargon, clearer examples.

The summary changes tone depending on who it’s meant for.

### 4. No Making Things Up
All summaries must only use the information that’s actually in the section.  
No adding new claims or extra facts.

### 5. Send the Results Forward
After summarizing each section, the output gets passed on to the later modules that build the full final document.
