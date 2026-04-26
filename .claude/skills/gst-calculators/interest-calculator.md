---
skill: interest-calculator
description: Calculate GST interest under Section 50 — simple step-by-step formula for delayed tax payment, ITC reversal interest, and wrong availment interest
type: calculator
---

# GST Interest Calculator — Section 50

## Reference Skill
Load `section-50.md` and `gst-thresholds` SKILL.md for full statutory text.

---

## Interest Rates (Section 50)

| Situation | Rate |
|---|---|
| Delayed payment of output tax | **18% per annum** |
| Wrongly availed and utilised ITC | **24% per annum** |
| ITC reversed (not utilised) | **18% per annum** |

---

## Interest Formula

```
Interest = (Tax Amount × Rate × Number of Days) ÷ 365
```

- **Tax Amount** — the net tax payable in cash (not ITC portion)
- **Rate** — 18% or 24% as applicable
- **Number of Days** — from the day after due date to the date of actual payment (both dates inclusive per practice)

---

## Step-by-Step Calculation

### Step 1 — Identify the tax amount
- For GSTR-3B delayed payment: tax liability paid in cash ledger (not set off from ITC)
- For ITC reversal: the ITC amount reversed (if already utilised → 24%; if reversed before utilisation → 18%)

### Step 2 — Find the due date
| Return | Normal Due Date |
|---|---|
| GSTR-3B (monthly, large taxpayer) | 20th of following month |
| GSTR-3B (quarterly QRMP) | 22nd / 24th of month after quarter end |
| GSTR-1 (monthly) | 11th of following month |

### Step 3 — Count the days
```
Days = Date of Payment − Due Date
```
Example: Due date 20-Apr-2023, paid on 05-Jun-2023
Days = 10 (Apr) + 31 (May) + 5 (Jun) = 46 days

### Step 4 — Apply formula
```
Interest = Tax × 18% × Days ÷ 365
```

---

## Worked Examples

### Example 1 — Late GSTR-3B Payment
- Tax paid in cash: ₹5,00,000
- Due date: 20-Apr-2023
- Payment date: 05-Jun-2023
- Days late: 46

```
Interest = 5,00,000 × 18% × 46 ÷ 365
         = 5,00,000 × 0.18 × 46 ÷ 365
         = 90,000 × 46 ÷ 365
         = 41,40,000 ÷ 365
         = ₹11,342 (approx)
```

### Example 2 — ITC Wrongly Availed and Utilised
- ITC wrongly availed and used: ₹2,00,000
- Due date of return: 20-Jul-2022
- Reversal date: 15-Mar-2023
- Days: 238

```
Interest = 2,00,000 × 24% × 238 ÷ 365
         = 48,000 × 238 ÷ 365
         = ₹31,298 (approx)
```

### Example 3 — ITC Reversed Before Use
- ITC reversed without utilisation: ₹1,50,000
- Days late: 90

```
Interest = 1,50,000 × 18% × 90 ÷ 365
         = 27,000 × 90 ÷ 365
         = ₹6,658 (approx)
```

---

## Important Legal Points

1. **Interest on net cash liability only** — Per Finance Act 2021 amendment to §50(1), interest applies only on the portion paid through cash ledger, not on ITC-set-off portion. This is retrospective from 01-Jul-2017.

2. **No interest on ITC ledger balance** — If the taxpayer had sufficient ITC balance but filed GSTR-3B late, interest applies only on the cash shortfall, not the entire liability.

3. **24% rate is penal** — Applies only when ITC was both wrongly availed AND utilised. If availed but not utilised (still sitting in credit ledger), 18% applies.

4. **SCN interest demand** — When an officer demands interest in DRC-01, verify:
   - Whether the demand is on gross liability or net cash liability
   - Whether 18% or 24% rate is correctly applied
   - Whether days are correctly counted

5. **Rounding** — Round interest to nearest rupee; paise ignored for payment.

---

## How to Use This in a Notice Reply

When an SCN includes an interest demand:
1. Run this calculation with actual figures
2. Compare with officer's computation
3. If officer computed on gross liability → raise objection citing Finance Act 2021 amendment
4. State correct interest figure in DRC-06 reply
5. Pay correct amount via DRC-03 (quote ARN in reply)

---

*GST Notice Responder — Built by Rohan Vidhate*
