---
name: cgst-section-50
description: Reference for Section 50 of CGST Act 2017 - Interest on delayed payment of tax. Load this skill when the notice demands interest on late tax payment, interest on ITC wrongly availed and utilised, or when computing interest liability alongside a §73/§74 demand.
---

# Section 50 — Interest on Delayed Payment of Tax

## Plain-English Summary

Section 50 mandates interest when:
1. **§50(1)** — Tax is not paid within the prescribed period (late payment of output tax)
2. **§50(3)** — ITC has been wrongly availed **and utilised**

Interest is not a penalty — it is automatic and accrues by operation of law. The taxpayer is required to pay it **on his own** without waiting for a notice.

Two key rates:
- **18% p.a.** — late payment of tax (§50(1))
- **24% p.a.** — ITC wrongly availed and utilised (§50(3))

---

## §50(1) — Interest on Late Tax Payment

### Who pays
Every person **liable to pay tax** who fails to pay within the prescribed period.

### Rate
**Not exceeding 18% p.a.** — Government notifies the actual rate on GST Council recommendation. Currently notified at **18% p.a.**

### From when
Interest runs from the **day succeeding** the due date of payment (§50(2)) — i.e., if tax was due on 20th of the month, interest starts from the 21st.

### The Proviso — Cash Ledger Interest (Critical Amendment)

**Before the proviso (original position)**: Interest was on the **gross tax liability** — even if ITC was available in the credit ledger, interest was charged on the full amount.

**After the proviso (w.e.f. 01.09.2020 — prospective; but see below)**: Interest on **late-filed returns** is levied only on the **net cash component** — i.e., the portion of tax paid by debiting the **electronic cash ledger** — NOT on the portion discharged through ITC.

**Conditions for the proviso to apply**:
1. The tax pertains to **supplies made during a tax period**
2. The return for that period is **filed after the due date** (late GSTR-3B)
3. The late filing happens **before commencement of §73/§74/§74A proceedings**

**If §73/§74/§74A proceedings have commenced**: The proviso does NOT apply — interest is on the **gross tax liability** (full amount, including ITC portion).

### Interest calculation formula (§50(1))
```
Interest = Tax amount × 18% ÷ 365 × number of days of delay
```
Days of delay = from the day after the due date to the date of actual payment (both inclusive of the end date).

### Prescribed due dates for GSTR-3B (reference)
| Taxpayer type | Monthly due date |
|---|---|
| Turnover > ₹5 Cr | 20th of following month |
| Turnover ≤ ₹5 Cr (Staggered) | 22nd or 24th depending on state |
| Quarterly filers (QRMP) | 22nd or 24th of month following quarter |

---

## §50(2) — Starting Point of Interest

Interest is calculated from the **day succeeding the day on which tax was due** — i.e., from the 21st (if due date is 20th).

**Agent alert**: Officers sometimes calculate interest from the wrong date. Always verify the start date in the demand. If the officer has started interest from the due date itself (not the day after), challenge the calculation.

---

## §50(3) — Interest on Wrongly Availed and Utilised ITC

### Rate
**Not exceeding 24% p.a.** — currently notified at **24% p.a.**

### Trigger
ITC has been **wrongly availed AND utilised**.

**Two-stage test** — both must be present:
1. **Wrongly availed** — ITC was taken in the credit ledger when it was not eligible
2. **Utilised** — the wrongly availed ITC was actually used to discharge output tax liability

### Critical distinction: Availed but not utilised

If ITC was wrongly availed (credited to e-credit ledger) but **not yet utilised** (still sitting as balance in the credit ledger) — **§50(3) does NOT apply**. The taxpayer reverses the credit without interest.

**Supreme Court position** — *Union of India v. Bharti Airtel Ltd. (SC, 2021)*:
> Held: Interest under §50(3) is payable only when ITC is **utilised** — mere availment in the credit ledger without utilisation does not attract interest. The government cannot demand interest on credit that has not been drawn upon.

However, §50(3) was amended prospectively — check whether the period in dispute is pre or post the amendment. For pre-amendment periods, the original text (which was interpreted by courts as requiring utilisation) applies.

### Interest calculation formula (§50(3))
```
Interest = ITC wrongly utilised × 24% ÷ 365 × number of days
```
Days = from the date of utilisation to the date of reversal/payment.

---

## Rate Summary Table

| Situation | Rate | Section |
|---|---|---|
| Late payment of output tax | **18% p.a.** | §50(1) |
| Late-filed return — cash component only (proviso) | **18% p.a.** (on cash portion only) | §50(1) proviso |
| ITC wrongly availed AND utilised | **24% p.a.** | §50(3) |
| ITC wrongly availed but NOT utilised | **NIL** | §50(3) not triggered |

---

## When Interest Is Mandatory vs Waivable

### Mandatory — cannot be waived
- Interest under §50 is a statutory obligation — it accrues automatically by operation of law
- Courts have consistently held that the department **cannot waive interest** even by administrative order or circular
- No discretion with the adjudicating officer to reduce or remit interest

### Can interest be contested?

Yes — on the following grounds:

| Ground | Argument |
|---|---|
| Wrong base amount | Officer computed interest on gross tax; proviso applies — only cash component is the base |
| Wrong period | Interest starts the day **after** due date, not on the due date itself |
| Wrong rate | Officer applied 24% instead of 18% for output tax delay |
| Utilisation not proved | For §50(3): department must prove ITC was actually utilised, not merely availed |
| Pre-§73/§74 proceeding commencement | If return was filed before any SCN issued — proviso applies (cash ledger basis) |
| Disputed principal tax | If the underlying tax demand itself is contested, interest cannot be sustained independently |

---

## The Proviso — Deep Dive

### What changed
| Pre-proviso | Post-proviso (w.e.f. 01.09.2020) |
|---|---|
| Interest on **gross tax liability** | Interest on **net cash payment** only |
| ITC balance in credit ledger irrelevant | ITC discharged amount excluded from interest base |
| Higher interest burden | Lower interest burden for compliant taxpayers with ITC |

### Example
- Tax liability for August: ₹10,00,000
- ITC available and used: ₹8,00,000
- Cash paid: ₹2,00,000
- Return filed 10 days late

**Pre-proviso**: Interest = ₹10,00,000 × 18% ÷ 365 × 10 = ₹4,932
**Post-proviso**: Interest = ₹2,00,000 × 18% ÷ 365 × 10 = ₹986

### When the proviso does NOT apply
1. §73/§74/§74A proceedings have **already commenced** for the period — the proviso is expressly excluded
2. The return is filed **after** the SCN is served — same exclusion
3. The interest demand is not on a late-filed return but on a **tax not paid at all** (no return filed) — proviso covers late-filed returns, not non-filers

### "Commencement of proceedings" — what counts?
Proceedings commence when:
- A notice under §73(1) / §74(1) is **served** on the taxpayer, OR
- An ASMT-10 notice under §61 is served (this is a precursor to §73/§74 — check if this counts as "commencement"; conservative position: §73/§74 proceedings commence on SCN, not ASMT-10)

**Agent alert**: If the client filed the return late but before any SCN was issued, the proviso applies and interest is only on the cash component. Verify the timeline of return filing vs SCN issuance.

---

## Interest in the Context of §73/§74 Demands

Interest under §50 is mandatory alongside every §73/§74 demand:
- §73(1): "…pay the amount specified in the notice along with interest payable thereon under section 50"
- §74(1): same language

### Key points for demand replies

1. **Always check the interest computation** attached to the SCN. Officers frequently:
   - Apply interest from the wrong date
   - Use gross tax as the base when the proviso applies
   - Apply 24% rate for output tax delays (should be 18%)
   - Compute interest on the entire ITC reversed, including the portion not utilised

2. **Include an alternative prayer**: Even if the tax demand is upheld, pray for recomputation of interest on the correct base and correct rate.

3. **If paying under §73(8) (30-day no-penalty payment)**: Pay tax + interest computed correctly. If there is a dispute on the interest amount, pay the admitted interest and note the dispute on the balance.

---

## Interest on ITC Reversal Under 180-Day Rule (§16(2) Second Proviso)

When ITC is reversed under the 180-day payment rule (§16(2)), interest under §50 applies at **18% p.a.**

**From when**: From the date ITC was availed (credited to e-credit ledger and utilised) — not from the date the 180-day period expires.

**CBIC position**: Circular confirms interest runs from date of availment/utilisation. However, some argue it should run from the date the 180-day period expires — this remains contested for pre-reversal periods.

---

## Procedural Defects Checklist — Interest Demands

| # | Defect | Argument |
|---|---|---|
| 1 | Interest computed on gross tax; proviso applies | Recompute on cash component only |
| 2 | Interest start date is the due date itself | Interest starts the day **after** due date per §50(2) |
| 3 | 24% applied on output tax delay | Correct rate is 18%; 24% only for ITC wrongly availed + utilised |
| 4 | §50(3) applied where ITC was availed but not utilised | No interest — Bharti Airtel SC ruling |
| 5 | Proceedings commenced after return was filed late | Proviso applies; cash basis |
| 6 | Interest demanded independently after tax demand dropped | If principal tax is not sustainable, interest cannot survive independently |

---

## Key Case Law

### On proviso — cash ledger basis
**Bharat Oman Refineries Ltd. v. Union of India (Madhya Pradesh HC, 2020)**
> Held (pre-amendment): Interest should be levied only on the net cash liability, not on the gross tax liability. The amendment inserting the proviso was clarificatory in nature and should be applied retrospectively.

**Note**: The SC has not conclusively settled retrospective applicability. For pre-01.09.2020 periods, argue the proviso is clarificatory (not a new rule) and cite the consistent HC trend.

### On §50(3) — utilisation required
**Union of India v. Bharti Airtel Ltd. (SC, 2021)**
> Held: Interest under §50(3) is chargeable only when ITC has been **wrongly utilised** — i.e., actually drawn upon to discharge output tax liability. Mere availment of ITC in the credit ledger without utilisation does not attract §50(3) interest. This is the binding SC position.

### On interest — no waiver power
**Pratibha Processors v. Union of India (Bombay HC)**
> Held: Interest under the GST / Central Excise laws accrues automatically by operation of statute. The department has no power to waive or remit interest. A circular purporting to waive interest has no legal force.

### On interest surviving after tax demand dropped
**Consistent judicial position**
> Interest is consequential to the tax demand. If the principal tax demand is set aside, the interest demand falls with it — it cannot be sustained independently.

---

## Quick Interest Calculator Reference

### 18% p.a. — daily rate
₹1,00,000 × 18% ÷ 365 = **₹49.32 per day**

### 24% p.a. — daily rate
₹1,00,000 × 24% ÷ 365 = **₹65.75 per day**

### Formula
```
Interest = Principal × Rate% ÷ 365 × Days of delay
```

---

## Related Provisions

- **Section 73** — Interest mandatory alongside §73 demand → `cgst-act-reference/section-73.md`
- **Section 74** — Interest mandatory alongside §74 demand → `cgst-act-reference/section-74.md`
- **Section 16(2)** — 180-day rule reversal attracts §50 interest → `cgst-act-reference/section-16.md`
- **Rule 88B** — CGST Rules — manner of calculating interest under §50 (inserted w.e.f. 01.09.2020 to operationalise the proviso)

## What This Skill Does NOT Cover

- Late fee for non-filing of returns (§47) — separate from interest
- Penalty provisions (§73(9), §74(9)) — see those sections
- Interest on erroneous refunds (§50 does not cover this — §56 covers refund interest)

---

**Source**: CGST Act, 2017 (Act No. 12 of 2017), as amended by Finance Act 2019 (insertion of proviso to §50(1), §50(3) amendment), Finance Act 2021 (prospective application of proviso confirmed), Finance Act 2024 (reference to §74A added in proviso).
