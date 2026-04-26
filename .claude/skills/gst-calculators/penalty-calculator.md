---
skill: penalty-calculator
description: Calculate GST penalty under Section 73 (non-fraud), Section 74 (fraud), and Section 74A (FY 2024-25+) at each stage of the demand lifecycle
type: calculator
---

# GST Penalty Calculator — §73 / §74 / §74A

## Reference Skills
Load `section-73.md`, `section-74.md`, `section-74a.md`, and `gst-thresholds` SKILL.md.

---

## Which Section Applies?

| Situation | Section |
|---|---|
| Non-fraud, no suppression — FY up to 2023-24 | **Section 73** |
| Fraud / willful misstatement / suppression — FY up to 2023-24 | **Section 74** |
| Any reason — FY 2024-25 onwards | **Section 74A** |

---

## SECTION 73 — Non-Fraud Penalty Table

| Stage | Penalty |
|---|---|
| Voluntary payment before DRC-01A / DRC-01 (DRC-03) | **NIL** |
| Payment within 30 days of DRC-01A or DRC-01 SCN | **10% of tax** (min ₹10,000) |
| After adjudication — DRC-07 order passed | **10% of tax** (min ₹10,000) |

> **Section 73 max penalty is always 10% of tax — never 100%**

### Section 73 Penalty Calculation

```
Penalty = MAX(10% of tax demand, ₹10,000)
```

**Example:**
- Tax demand: ₹8,00,000
- Stage: DRC-01 SCN received, paying within 30 days
- Penalty = MAX(10% × 8,00,000, 10,000) = MAX(80,000, 10,000) = **₹80,000**

**Example (small demand):**
- Tax demand: ₹50,000
- Penalty = MAX(10% × 50,000, 10,000) = MAX(5,000, 10,000) = **₹10,000** (minimum applies)

---

## SECTION 74 — Fraud / Suppression Penalty Table

| Stage | Penalty |
|---|---|
| Voluntary payment before DRC-01A / DRC-01 (DRC-03) | **15% of tax** |
| Payment within 30 days of DRC-01A | **25% of tax** |
| Payment within 30 days of DRC-01 SCN | **25% of tax** |
| Payment within 30 days of DRC-07 order | **50% of tax** |
| After 30 days of DRC-07 / no payment | **100% of tax** |

> **Section 74 — pay early, save massively**

### Section 74 Penalty Calculation

```
Penalty = Tax demand × applicable % (based on stage)
```

**Example — Paying within 30 days of DRC-01 SCN:**
- Tax demand: ₹10,00,000
- Penalty = 25% × 10,00,000 = **₹2,50,000**
- Total outflow = ₹10,00,000 + interest + ₹2,50,000

**Example — Not paying, after DRC-07:**
- Tax demand: ₹10,00,000
- Penalty = 100% × 10,00,000 = **₹10,00,000**
- Total outflow = ₹10,00,000 + interest + ₹10,00,000 = **₹20,00,000+**

---

## SECTION 74A — FY 2024-25 Onwards Penalty Table

| Stage | Penalty |
|---|---|
| Voluntary payment before notice (DRC-03) | **NIL** |
| Payment within 60 days of DRC-01 SCN | **15% of tax** |
| Payment after 60 days but before DRC-07 order | **25% of tax** |
| Payment within 30 days of DRC-07 order | **25% of tax** |
| No payment / after 30 days of DRC-07 | **50% of tax** |

> Note: §74A has a **60-day window** (vs 30 days under §73/74) for reduced penalty.

---

## Side-by-Side Comparison — Same ₹10,00,000 Demand

| Stage | §73 (Non-Fraud) | §74 (Fraud) | §74A (FY25+) |
|---|---|---|---|
| Before notice (voluntary) | **NIL** | 15% = ₹1.5L | **NIL** |
| Within 30/60 days of SCN | 10% = ₹1L | 25% = ₹2.5L | 15% = ₹1.5L |
| After DRC-07 (within 30d) | 10% = ₹1L | 50% = ₹5L | 25% = ₹2.5L |
| No payment | 10% = ₹1L | 100% = ₹10L | 50% = ₹5L |

---

## Total Outflow Calculator

```
Total to Pay = Tax + Interest + Penalty
```

### Full Example — §73, DRC-01 SCN Stage

- Tax demand: ₹5,00,000
- Days late (for interest): 180 days
- Interest = 5,00,000 × 18% × 180 ÷ 365 = **₹44,384**
- Penalty (within 30 days of SCN) = 10% × 5,00,000 = **₹50,000**
- **Total = ₹5,94,384**

---

## Key Legal Points

1. **Penalty under §73 is capped at 10%** — Officers cannot demand 100% penalty for non-fraud cases. Raise objection if SCN demands more.

2. **Fraud must be proved** — §74 applies only when the officer can establish fraud, willful misstatement, or suppression with positive evidence. Mere return mismatch is not fraud.

3. **Nil penalty window is valuable** — Voluntary DRC-03 payment before any notice = zero penalty under §73 and §74A.

4. **Multiple periods** — Calculate penalty separately for each financial year's demand.

5. **Minimum penalty** — Under §73, minimum ₹10,000 per proceeding regardless of tax amount.

---

## How to Use in a Notice Reply

1. Calculate the correct penalty for the current stage
2. Compare with penalty demanded in the SCN
3. If officer demands §74 penalty but no fraud evidence → object in DRC-06, state §73 applies
4. If accepting and paying → quote correct penalty in DRC-03 and reference in reply

---

*GST Notice Responder — Built by Rohan Vidhate*
