---
skill: asmt-13-bja
description: Guide for ASMT-13 Best Judgement Assessment order under Section 62 — what it means, the 30-day filing remedy, how to withdraw it, and post-30-day options
type: notice-type
---

# ASMT-13 — Best Judgement Assessment (Section 62)

## What Is ASMT-13?

ASMT-13 is the **Best Judgement Assessment order** passed by the proper officer under Section 62 of the CGST Act when a registered person:
1. Fails to file returns despite a GSTR-3A notice (§46)
2. Still does not file within 15 days of the GSTR-3A notice

The officer then **estimates the tax liability** based on available data and raises a demand — usually much higher than the actual liability.

Load `section-62.md` for full statutory provisions.

---

## How ASMT-13 Arises

```
GSTR-3B not filed
        ↓
GSTR-3A notice (§46) — 15-day window
        ↓
Still not filed
        ↓
ASMT-13 — Best Judgement Assessment
(Officer estimates tax based on e-way bills, TDS credits, GSTR-1 of buyers, etc.)
        ↓
Tax demand confirmed in ASMT-13 (usually inflated)
```

---

## THE CRITICAL REMEDY — File Within 30 Days

> **Section 62(2):** If the taxpayer files a valid return within **30 days** of the ASMT-13 order → the order is **automatically deemed withdrawn**.

This is the most powerful remedy in GST law for non-filers — no appeal, no hearing needed. Just file the return.

**The 30-day clock starts from the date of service of ASMT-13.**

---

## Immediate Checklist on Receiving ASMT-13

1. **COUNT THE DAYS** — 30-day window to file actual return. This is your only automatic remedy.
2. **If < 10 days remaining** → File the return TODAY. Everything else can wait.
3. **If < 5 days remaining** → Emergency — file immediately even if figures need revision later
4. **Identify all pending periods** — ASMT-13 may cover multiple months/quarters
5. **Compute actual tax liability** — Will almost always be far less than the ASMT-13 demand
6. **Compute interest + late fee** — Both are payable along with the return
7. **Arrange funds** — Tax + interest + late fee must be paid before return can be submitted

---

## Step-by-Step Filing to Withdraw ASMT-13

### Step 1 — Compute what to pay

```
Tax payable = Output tax − Eligible ITC
Interest = Tax paid in cash × 18% × days late ÷ 365
Late fee = As per §47 (load gst-thresholds SKILL.md for rates)
```

### Step 2 — Pay on portal
```
Services → Payments → Create Challan
→ Pay tax (CGST + SGST / IGST) + interest + late fee
→ Confirm payment
```

### Step 3 — File GSTR-1 (if not filed)
```
Services → Returns → GSTR-1
→ Add all outward supply invoices for the period
→ File
```

### Step 4 — File GSTR-3B
```
Services → Returns → GSTR-3B
→ Enter outward tax, ITC, and net tax
→ Offset from cash ledger (tax paid above)
→ File
```

### Step 5 — Inform the officer
Send a written communication:

> "This is to inform that pursuant to the ASMT-13 order dated [date], the taxpayer has filed the following returns for the relevant periods:
>
> | Period | Return | ARN | Date | Tax Paid | Late Fee |
> |---|---|---|---|---|---|
> | [Month] | GSTR-3B | [ARN] | [Date] | ₹[Amount] | ₹[Amount] |
>
> In terms of Section 62(2) of the CGST Act, 2017, the ASMT-13 order dated [date] stands automatically withdrawn. The ARNs of filed returns and payment challans are enclosed for your records."

---

## If 30 Days Have Passed — What Now?

| Option | What to do |
|---|---|
| **Appeal (§107)** | File APL-01 with 10% pre-deposit; challenge the BJ Assessment quantum and procedure |
| **File return + negotiate** | File the actual return + pay actual liability + request officer to accept and close (discretionary) |
| **Writ petition (HC)** | If ASMT-13 is arbitrary / GSTR-3A was never issued / demand is grossly inflated |

---

## Grounds to Challenge ASMT-13 in Appeal

1. **GSTR-3A not served** — Mandatory pre-condition; if GSTR-3A was never issued, ASMT-13 is without jurisdiction
2. **Demand is arbitrary** — Officer used no rational data; figures have no basis
3. **Double taxation** — ASMT-13 covers a period already assessed
4. **Wrong GSTIN / period** — Factual error in the order
5. **Return was actually filed** — Officer may not have noticed the filing

---

## ASMT-13 vs ASMT-10 — Quick Reference

| | ASMT-10 | ASMT-13 |
|---|---|---|
| Section | §61 | §62 |
| Trigger | Return mismatch | Non-filing |
| Type | Pre-demand notice | Demand order |
| Reply | ASMT-11 | File actual return (§62(2)) |
| Withdrawal | ASMT-12 | Automatic on filing within 30 days |
| Post-30d remedy | N/A | Appeal / writ |

---

## Key Point — Late Fee Cannot Be Waived by Filing

Even after ASMT-13 is withdrawn by filing the return:
- **Tax** → Actual liability (not ASMT-13 inflated amount)
- **Interest** → Runs from original due date to actual payment date
- **Late fee** → Mandatory under §47, no automatic waiver
- **Penalty** → No separate penalty if ASMT-13 is withdrawn; ASMT-13 itself is not a penalty order

---

*GST Notice Responder — Built by Rohan Vidhate*
