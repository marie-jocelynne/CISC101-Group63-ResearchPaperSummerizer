# CISC101-Group63-ResearchPaperSummerizer

This repo contains our final project for the CISC 101 Paper Summarizer.

The project uses a single system prompt plus a set of internal “modules” (in Markdown) to describe how an LLM should summarize a research paper section by section, with expert and layperson outputs.

## Structure

- `system_prompt.md`  
  - The user-facing system prompt: greeting, required inputs, boundaries, required outputs, and formatting rules.

- `modules/01_intake_setup.md`  
  - Explains how the summarizer looks at the section list, notices missing/short sections, and gets things ready.

- `modules/02_section_loop.md`  
  - Describes how each section is summarized, including short vs detailed summary modes and expert vs layperson wording.

- `modules/03_guardrails.md`  
  - Describes safety rules: missing/empty/short section warnings, strict evidence mode, and long-section chunking.

- `modules/04_rendering_refinement.md`  
  - Explains how the final Markdown output is assembled (paper summary, section table, expert + lay summaries, glossary, checks & warnings).

- `modules/05_citation_extractor.md`  
  - Extra student module: finds citation markers in the text and lists them.

- `modules/06_key_contributions.md`  
  - Extra student module: highlights the key ideas or contributions of the paper.

## How this was created

1. We wrote a meta-prompt that includes our PS2 specification (inputs, outputs, constraints).
2. We ran it in Microsoft Copilot and copied the generated system prompt and modules into this repo.
3. In Task 3, we updated Module 2 and Module 3 on a branch to add summary levels and strict evidence guardrails.
