---
skill: limitation-checker
description: Check whether a GST Show Cause Notice is time-barred under Section 73, 74, or 74A — step-by-step limitation period calculator with worked examples
type: calculator
---

# GST Limitation Period Checker — §73 / §74 / §74A

## Reference Skills
Load `section-73.md`, `section-74.md`, `section-74a.md`.

---

## Why This Matters

A DRC-01 SCN issued after the limitation period expires is **void and not maintainable in law**. This is one of the strongest preliminary objections available — if the notice is time-barred, the entire demand falls regardless of merits.

---

## Which Section Applies?

| FY of Demand | Applicable Section |
|---|---|
| FY 2017-18 to FY 2023-24 | §73 (non-fraud) or §74 (fraud) |
| FY 2024-25 onwards | §74A (unified — no fraud/non-fraud distinction) |

---

## SECTION 73 — Non-Fraud Limitation

### Rule
SCN must be issued **within 3 years** from the due date of filing the annual return (GSTR-9) for the relevant financial year.

### Due Dates of GSTR-9

| Financial Year | GSTR-9 Due Date | 3-Year Limit (§73 SCN deadline) |
|---|---|---|
| FY 2017-18 | 05-Feb-2020 (extended) | 04-Feb-2023 |
| FY 2018-19 | 31-Dec-2020 (extended) | 30-Dec-2023 |
| FY 2019-20 | 31-Dec-2021 (extended) | 30-Dec-2024 |
| FY 2020-21 | 28-Feb-2022 (extended) | 27-Feb-2025 |
| FY 2021-22 | 31-Dec-2022 | 30-Dec-2025 |
| FY 2022-23 | 31-Dec-2023 | 30-Dec-2026 |
| FY 2023-24 | 31-Dec-2024 | 30-Dec-2027 |

> **Important:** Limitation runs from the **original / extended due date of GSTR-9**, not from the actual filing date by the taxpayer.

### §73 Limitation Check — Step by Step

```
Step 1: Identify FY of demand from the SCN
Step 2: Find GSTR-9 due date for that FY (from table above)
Step 3: Add 3 years → this is the §73 SCN deadline
Step 4: Compare with actual SCN date
Step 5: If SCN date > deadline → TIME-BARRED ✅
```

**Example:**
- SCN for FY 2020-21, issued on 01-Mar-2025
- GSTR-9 due date for FY 2020-21: 28-Feb-2022
- §73 deadline: 28-Feb-2025
- SCN date (01-Mar-2025) > deadline (28-Feb-2025)
- **RESULT: TIME-BARRED under §73**

---

## SECTION 74 — Fraud / Suppression Limitation

### Rule
SCN must be issued **within 5 years** from the due date of filing the annual return (GSTR-9).

### §74 SCN Deadlines

| Financial Year | GSTR-9 Due Date | 5-Year Limit (§74 SCN deadline) |
|---|---|---|
| FY 2017-18 | 05-Feb-2020 | 04-Feb-2025 |
| FY 2018-19 | 31-Dec-2020 | 30-Dec-2025 |
| FY 2019-20 | 31-Dec-2021 | 30-Dec-2026 |
| FY 2020-21 | 28-Feb-2022 | 27-Feb-2027 |
| FY 2021-22 | 31-Dec-2022 | 30-Dec-2027 |
| FY 2022-23 | 31-Dec-2023 | 30-Dec-2028 |
| FY 2023-24 | 31-Dec-2024 | 30-Dec-2029 |

### §74 Limitation Check — Step by Step

```
Step 1: Identify FY of demand
Step 2: Find GSTR-9 due date for that FY
Step 3: Add 5 years → §74 SCN deadline
Step 4: Compare with SCN date
Step 5: If SCN date > deadline → TIME-BARRED ✅
```

**Example:**
- SCN for FY 2017-18 (fraud alleged), issued on 10-Mar-2025
- GSTR-9 due date: 05-Feb-2020
- §74 deadline: 04-Feb-2025
- SCN date (10-Mar-2025) > deadline (04-Feb-2025)
- **RESULT: TIME-BARRED under §74 also**

---

## SECTION 74A — FY 2024-25 Onwards

### Rule
Two-tier limitation based on demand amount:

| Demand Amount | Limitation Period |
|---|---|
| Up to ₹20 lakhs | **42 months** from GSTR-9 due date |
| Above ₹20 lakhs | **60 months** from GSTR-9 due date |

| Financial Year | GSTR-9 Due Date | 42-Month Limit | 60-Month Limit |
|---|---|---|---|
| FY 2024-25 | 31-Dec-2025 | 30-Jun-2029 | 31-Dec-2030 |

---

## Quick Reference — Is My SCN Time-Barred?

**Enter:** FY of demand + SCN date + Section alleged

| FY | §73 Deadline | §74 Deadline | Status if SCN after §73 deadline |
|---|---|---|---|
| 2017-18 | 04-Feb-2023 | 04-Feb-2025 | §73 barred; §74 barred after Feb-2025 |
| 2018-19 | 30-Dec-2023 | 30-Dec-2025 | §73 barred; §74 open till Dec-2025 |
| 2019-20 | 30-Dec-2024 | 30-Dec-2026 | §73 barred after Dec-2024; §74 open |
| 2020-21 | 27-Feb-2025 | 27-Feb-2027 | §73 borderline; §74 open |
| 2021-22 | 30-Dec-2025 | 30-Dec-2027 | Both open |
| 2022-23 | 30-Dec-2026 | 30-Dec-2028 | Both open |
| 2023-24 | 30-Dec-2027 | 30-Dec-2029 | Both open |

---

## Important Legal Points

1. **Limitation is a jurisdictional bar** — A time-barred SCN cannot be validated by any subsequent order. It is void, not merely voidable.

2. **Extended due dates count** — Use the government-notified extended due date for GSTR-9, not the original statutory date, as the starting point.

3. **Officer cannot invoke §74 to extend time if no fraud** — If the officer invokes §74 (5-year limit) without evidence of fraud, that invocation itself is challengeable.

4. **Multiple FYs in one SCN** — Check limitation separately for each FY covered in the SCN. Some FYs may be barred while others are within time.

5. **Covid extensions** — Some GSTR-9 due dates were extended due to Covid notifications. Always verify the actual government-notified due date for the specific FY.

---

## How to Raise Time-Bar Objection in DRC-06

> "The SCN dated [date] relates to FY [XX]. The annual return (GSTR-9) for FY [XX] was due on [date]. The limitation period under Section [73/74] of the CGST Act expires on [calculated date]. The impugned SCN has been issued on [SCN date], which is beyond the prescribed limitation period. The SCN is, therefore, barred by limitation and not maintainable in law. The proceedings are liable to be dropped on this ground alone, without going into the merits of the demand."

Cite supporting case law:
- *Assistant Commissioner of State Tax v. Commercial Steel Ltd.* (SC, 2021) — limitation is mandatory
- Relevant High Court decisions on GST limitation (check jurisdiction)

---

*GST Notice Responder — Built by Rohan Vidhate*
