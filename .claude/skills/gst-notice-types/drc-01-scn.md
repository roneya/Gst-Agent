---
skill: drc-01-scn
description: Deep-dive guide for DRC-01 Show Cause Notice under Section 73 / 74 / 74A — demand notice lifecycle, immediate checklist, reply strategy, and escalation map
type: notice-type
---

# DRC-01 — Show Cause Notice (SCN)

## What Is a DRC-01?

DRC-01 is the **Show Cause Notice (SCN)** issued by the proper officer demanding tax, interest, and penalty under:
- **Section 73** — Non-fraud cases (up to FY 2023-24)
- **Section 74** — Fraud / willful misstatement / suppression cases (up to FY 2023-24)
- **Section 74A** — Unified demand for FY 2024-25 and onwards

This is a **formal tax demand notice** — unlike ASMT-10 (pre-demand scrutiny), a DRC-01 carries a specific monetary demand and penalty.

---

## DRC Form Lifecycle

```
DRC-01A (optional pre-notice intimation)
    ↓
DRC-01 (Show Cause Notice — formal demand)
    ↓
DRC-06 (Taxpayer's reply to SCN)
    ↓
DRC-07 (Order: confirmed / dropped / partial)
    ↓
DRC-08 (Summary of order — demand register entry)
```

---

## Immediate Checklist on Receipt

1. **DIN Check** — Every DRC-01 must carry a Document Identification Number (DIN). If missing or invalid → preliminary objection citing CBIC Circular No. 128/47/2019-GST.
2. **Limitation Period** — Cross-check issue date against the applicable deadline:
   - §73: 3 years from due date of annual return for that FY
   - §74: 5 years from due date of annual return for that FY
   - §74A: 42 months (up to ₹20 lakh) / 60 months (above ₹20 lakh) from due date of annual return
   - Load `section-73.md`, `section-74.md`, or `section-74a.md` for exact calculation
3. **Reply Deadline** — DRC-06 must be filed within **30 days** of service of DRC-01. Check if extension is needed.
4. **Urgency Flag** — If deadline is ≤ 7 days → flag as urgent immediately.
5. **Jurisdiction Check** — Confirm issuing officer is the proper officer for the taxpayer's GSTIN (State GST vs Central GST jurisdiction).
6. **DRC-01A Issued First?** — If DRC-01A (intimation) was never served, check if mandatory for the section applied.
7. **Personal Hearing** — The taxpayer has a right to be heard (§75(4)). Ensure hearing is requested in DRC-06 reply.

---

## Common Grounds of Demand in DRC-01

| Allegation | Cross-reference skill |
|---|---|
| ITC wrongly availed (GSTR-2A/2B mismatch) | `itc-mismatch.md` + `section-16.md` |
| ITC on blocked credit items (§17) | `section-17.md` |
| Output tax underreported (GSTR-1 vs GSTR-3B) | `gstr1-gstr3b-mismatch.md` |
| RCM tax not paid | `section-73.md` / `section-74.md` |
| Interest on delayed payment | `section-50.md` + `gst-thresholds` |
| GSTR-9 vs GSTR-3B difference | `gstr1-gstr3b-mismatch.md` |
| Excess ITC claimed beyond Rule 36(4) limit | `section-16.md` |
| Tax on exempt supply not reversed | `section-17.md` |

---

## Reply Strategy

### Step 1 — Preliminary Objections (if applicable)
Raise before going to merits:
- Missing / invalid DIN → notice void ab initio
- Time-barred under §73 / §74 / §74A → demand not maintainable
- Jurisdiction defect → proper officer not authorised
- DRC-01A not served → mandatory pre-condition not met (check section)
- Demand vague / not quantified allegation-wise → violates natural justice

### Step 2 — Factual Background
State the taxpayer's business, GSTIN, the tax period in question, and a brief summary of the transactions being disputed.

### Step 3 — Allegation-wise Response
Address each ground of demand serially (matching DRC-01 serial numbers):
- **Contesting:** Provide factual explanation + supporting documents + legal provision + case law
- **Accepting:** State acceptance, quote DRC-03 ARN (payment reference), interest calculation

### Step 4 — Legal Submissions
Cite relevant sections, rules, circulars, and case law in support of contested grounds.

### Step 5 — Request for Personal Hearing
Explicitly request a personal hearing under §75(4) before any order is passed.

### Step 6 — Prayer
- Drop the SCN / issue DRC-07 in favour of the taxpayer
- For accepted amounts — acknowledge DRC-03 payment and pray for closure of that head

---

## Payment Options at SCN Stage (Section 73 — Non-Fraud)

| Stage | Penalty |
|---|---|
| Before SCN (DRC-03 voluntary) | Nil penalty |
| Within 30 days of DRC-01 | 10% of tax or ₹10,000 (whichever is higher) |
| After 30 days / adjudication | 10% of tax (minimum) up to 100% of tax |

Load `gst-thresholds` SKILL.md for exact penalty rates under §74 (fraud) and §74A.

---

## GST Portal Filing Path

```
Services → User Services → My Applications
→ Reply to Notice → Select DRC-01 reference number
→ File DRC-06
```

---

## Key Case Law to Check

- **Validity of notice without DIN:** CBIC Circular 128/47/2019; Pradeep Oil Corp (Del HC)
- **Time-bar under §73:** Limitation runs from due date of annual return, not extended due dates
- **Natural justice — personal hearing:** §75(4) is mandatory if requested
- **ITC mismatch — GSTR-2A not conclusive:** Dyna Automation Pvt Ltd; Rajasthan HC decisions

---

*GST Notice Responder — Built by Rohan Vidhate*
