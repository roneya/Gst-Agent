---
name: gst-notice-interpreter
description: Master orchestrator skill for the GST Notice Responder. Load this skill first for ANY GST notice. It reads the notice, identifies the type, loads the relevant section/rule skills, and directs the agent to draft a reply strategy.
---

# GST Notice Interpreter — Master Skill

**Built by Rohan Vidhate**
Project: GST Notice Responder — Claude Plugin

---

## What This Skill Does

This is the **entry point** for every GST notice query. When a user pastes or uploads a GST notice, this skill:

1. **Identifies** the notice type (ASMT-10, DRC-01 SCN, audit, etc.)
2. **Extracts** key metadata (GSTIN, period, section cited, demand amount)
3. **Routes** to the correct section/rule skill files
4. **Directs** the reply strategy

---

## Step 1 — Extract These Fields from Every Notice

When a notice is shared, always extract:

| Field | Where to look |
|---|---|
| **Notice type / form** | Header of notice (ASMT-10, DRC-01, etc.) |
| **Section cited** | "Under Section ___" |
| **GSTIN** | Top of notice |
| **Tax period** | "For the period ___ to ___" |
| **Financial year** | Derive from tax period |
| **Demand amount** | Quantified in notice or DRC-01 summary |
| **Due date for reply** | "Within ___ days" |
| **Issuing officer** | Name, designation, jurisdiction |
| **DIN** | 20-digit number on notice |
| **Allegations** | List each discrepancy / allegation separately |

---

## Step 2 — Identify Notice Type and Load Skill

| If the notice says… | Notice type | Load skill |
|---|---|---|
| ASMT-10 / Section 61 | Scrutiny of returns | `section-61.md` + `rule-99.md` |
| DRC-01 + Section 73 | Non-fraud SCN (up to FY 2023-24) | `section-73.md` + `rule-142.md` |
| DRC-01 + Section 74 | Fraud SCN (up to FY 2023-24) | `section-74.md` + `rule-142.md` |
| DRC-01 + Section 74A | Unified SCN (FY 2024-25 onwards) | `section-74a.md` + `rule-142.md` |
| ITC mismatch allegation | ITC eligibility dispute | `section-16.md` + `section-17.md` |
| Motor vehicle / food / CSR | Blocked credits | `section-17.md` |
| Interest demand | Interest computation | `section-50.md` |
| ASMT-10 + ITC | Scrutiny + ITC | `section-61.md` + `section-16.md` |

---

## Step 3 — Run the Notice Checklist

For every notice, check these before drafting the reply:

### A. Jurisdiction check
- Is the officer from the correct ward/circle for this GSTIN?
- Is the GSTIN in the notice correct?

### B. DIN check
- Is there a 20-digit DIN on the notice?
- If no DIN → notice is invalid per CBIC Circular 128/47/2019

### C. Limitation check
- What is the financial year of the demand?
- FY 2023-24 or earlier → §73 (3-year order limit) or §74 (5-year order limit)
- FY 2024-25 onwards → §74A (42-month SCN limit + 12-month order limit)
- Has the limitation expired? → Strongest ground, challenge first

### D. Reply deadline check
- When was the notice served?
- How many days remain for reply?
- If less than 7 days → immediately flag urgency to user

### E. Fraud allegation check
- Does the notice use words like: fraud, willful misstatement, suppression, deliberately, intentionally, evade?
- If yes → §74 or §74A fraud track applies (100% penalty)
- If no → §73 or §74A non-fraud track (10% penalty)

---

## Step 4 — Produce the Reply Strategy

After loading the relevant skills, output:

```
NOTICE SUMMARY
--------------
Form: [ASMT-10 / DRC-01 / etc.]
Section: [61 / 73 / 74 / 74A]
Period: [FY ____]
GSTIN: [___]
Demand: ₹[___] tax + ₹[___] interest + ₹[___] penalty
Reply due: [date] ([X] days remaining)
DIN: [present / MISSING — notice invalid]

PRELIMINARY FLAGS
-----------------
☐ Limitation expired? [Yes/No + deadline date]
☐ DIN present? [Yes/No]
☐ Fraud alleged? [Yes/No]
☐ Jurisdiction correct? [Yes/No]

ALLEGATION BREAKDOWN
--------------------
1. [Allegation 1]: [Brief — accept / dispute / partially accept]
2. [Allegation 2]: [Brief]
...

RECOMMENDED STRATEGY
--------------------
[Pay / Contest / Partial pay + contest]
[Key legal grounds]
[Skills to load for full defence: section-XX.md, etc.]

REPLY FORM TO USE
-----------------
[ASMT-11 (for §61) / DRC-06 (for §73/74/74A)]
```

---

## Related Skills — Full Index

### Statutory provisions
- `cgst-act-reference/section-61.md` — Scrutiny of returns
- `cgst-act-reference/section-73.md` — Non-fraud demand (up to FY 2023-24)
- `cgst-act-reference/section-74.md` — Fraud demand (up to FY 2023-24)
- `cgst-act-reference/section-74a.md` — Unified demand (FY 2024-25+)
- `cgst-act-reference/section-16.md` — ITC eligibility
- `cgst-act-reference/section-17.md` — Blocked credits
- `cgst-act-reference/section-50.md` — Interest

### Procedural rules
- `cgst-rules-reference/rule-99.md` — ASMT-10/11/12 procedure
- `cgst-rules-reference/rule-142.md` — DRC forms — full demand lifecycle

### Defence playbooks
- `gst-common-defences/itc-mismatch.md` — GSTR-2A/2B mismatch defence
- `gst-common-defences/gstr1-gstr3b-mismatch.md` — Turnover mismatch defence

### Notice types
- `gst-notice-types/asmt-10-scrutiny.md` — ASMT-10 deep dive

### Reply templates
- `gst-reply-templates/asmt-11-reply.md` — ASMT-11 reply template
- `gst-reply-templates/drc-06-reply.md` — DRC-06 SCN reply template

### Thresholds & limits
- `gst-thresholds/SKILL.md` — Penalty rates, limitation periods, interest rates
