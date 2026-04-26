---
skill: drc-07-order
description: Guide for DRC-07 adjudication order — how to read it, what it means, accept vs appeal decision, pre-deposit calculation, and next steps
type: notice-type
---

# DRC-07 — Order-in-Original (Adjudication Order)

## What Is a DRC-07?

DRC-07 is the **adjudication order** passed by the proper officer after considering the taxpayer's DRC-06 reply and personal hearing. It is the final order at the first level of GST proceedings.

- Governed by: **Section 73 / 74 / 74A** of CGST Act, 2017
- Section 75 applies: order must be a speaking order with reasons
- Can confirm, modify, or drop the demand from the DRC-01 SCN

---

## DRC-07 in the Demand Lifecycle

```
DRC-01 SCN → DRC-06 Reply → Personal Hearing → DRC-07 Order
                                                      ↓
                                          DRC-08 (demand summary — enters demand register)
```

---

## How to Read a DRC-07 Order

### Key Items to Extract

| Item | Where to find it | What to check |
|---|---|---|
| Order number | Header | Note for appeal reference |
| Date of order | Header | 3-month appeal clock starts here |
| Tax confirmed | Demand table | Compare with SCN amount |
| Interest confirmed | Demand table | Verify §50 computation |
| Penalty confirmed | Demand table | Correct section? Correct rate? |
| Grounds dropped | Body of order | What the officer accepted |
| Grounds confirmed | Body of order | What still stands |
| Reasons given | Body of order | Is it a speaking order? |
| Personal hearing | Body of order | Was it granted / held? |

---

## Types of DRC-07 Orders

### 1. Full Confirmation
All grounds confirmed, full demand upheld. → Appeal or pay.

### 2. Partial Confirmation
Some grounds dropped, some confirmed. → Appeal against confirmed portion only, or pay.

### 3. Full Dropping
SCN dropped entirely. → No further action needed. Keep copy for records.

### 4. Enhanced Order *(Rare / Illegal)*
Officer tries to confirm more than the SCN amount. → Challenge immediately — §107(11) bars enhancement beyond SCN.

---

## Immediate Checklist on Receipt of DRC-07

1. **Note the date of communication** — 3-month appeal clock starts (§107(1))
2. **Calculate appeal deadline** — Date of order + 3 months
3. **Flag if < 30 days** — urgent, pre-deposit and APL-01 must be filed
4. **Check if it is a speaking order** — Reasons must be recorded (§75(5))
5. **Check personal hearing** — Was it granted? If requested and denied → strong appeal ground
6. **Compare demand with SCN** — Has the officer gone beyond the SCN? (§107(11) bar)
7. **Calculate pre-deposit** — 10% of confirmed tax (§107(6))
8. **Decide: accept or appeal?**

---

## Accept vs Appeal Decision Matrix

| Situation | Recommendation |
|---|---|
| Demand is factually correct, legal position weak | **Pay** — avoid interest accumulation during appeal |
| Demand confirmed on wrong legal ground | **Appeal** — strong case |
| Non-speaking order (no reasons) | **Appeal** — procedural ground alone is strong |
| Personal hearing denied despite request | **Appeal** — §75(3) violation |
| Officer went beyond SCN amount | **Appeal immediately** — §107(11) bar |
| Demand is time-barred but confirmed | **Appeal** — jurisdictional bar |
| Amount is small (< ₹1L) and legal position moderate | **Consider paying** — cost of appeal may exceed demand |
| Amount is large (> ₹5L) and legal position strong | **Appeal** — saving justifies pre-deposit |

---

## Pre-Deposit Calculation for Appeal

```
Pre-deposit = 10% of tax confirmed in DRC-07

(Exclude amounts already paid via DRC-03 before the order)
```

**Example:**
- DRC-07 confirms: Tax ₹12,00,000 + Interest ₹1,80,000 + Penalty ₹1,20,000
- Already paid via DRC-03: ₹2,00,000 (tax)
- Disputed tax = ₹12,00,000 − ₹2,00,000 = ₹10,00,000
- Pre-deposit = 10% × ₹10,00,000 = **₹1,00,000**
- Balance stayed during appeal = ₹10,00,000 (tax) + ₹1,80,000 (interest) + ₹1,20,000 (penalty) − ₹1,00,000 (pre-deposit) = **₹11,00,000 stayed**

---

## After Decision to Appeal

Load `apl-01-appeal.md` → full APL-01 template ready to file.

**Steps:**
1. Calculate pre-deposit (above)
2. Pay pre-deposit via DRC-03 / cash ledger
3. Draft APL-01 using `apl-01-appeal.md` template
4. File on GST portal within 3 months of DRC-07 date
5. Demand automatically stayed on filing (§107(7))

---

## After Decision to Pay (Not Appeal)

1. Pay confirmed tax + interest + penalty via **DRC-03** (if not already paid)
   - Portal: Payments → Create Challan → DRC-03
2. Intimate the officer with DRC-03 ARN
3. Officer issues **DRC-08** (demand register entry / paid challan summary)
4. Keep DRC-07 + DRC-08 + DRC-03 ARN for records

---

## DRC-08 — What It Means

DRC-08 is the **summary of the DRC-07 order** that enters the demand register. It is not a fresh demand — it is just the accounting entry. No reply is needed to DRC-08.

---

## Key Deadlines Summary

| Action | Deadline |
|---|---|
| File APL-01 appeal | 3 months from DRC-07 date |
| Condonable delay | Up to 1 additional month (§107(4)) |
| Pay demand (if not appealing) | As per DRC-07 / DRC-08 |

---

*GST Notice Responder — Built by Rohan Vidhate*
