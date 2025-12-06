# Module 03 — Guardrails

> Change Log (Task 3 – Week 10):
> - Added a strict evidence mode setting.
> - Added standard warning messages for missing, empty, or very short sections.

## What This Module Does

This module makes sure the summaries stay accurate and don’t drift away from what the paper actually says. It also handles situations where a section is missing, empty, or too short to summarize properly.

---

## 1. Missing, Empty, or Very Short Sections

### Missing or Empty
If the system finds that a section has **no usable text**, it shouldn’t try to summarize it.  
Instead, it should output a message like:

> “Section skipped: no usable text was provided.”

### Very Short Sections (< 50 words)
If the section is extremely short, the system can summarize it, but it must attach a warning such as:

> “Section very short: summary may be incomplete.”

These alerts should also appear in the final **Checks & Warnings** list.

---

## 2. Strict Evidence Mode

This module uses a setting called:

