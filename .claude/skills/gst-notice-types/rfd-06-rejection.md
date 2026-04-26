---
skill: rfd-06-rejection
description: Guide for RFD-06 refund rejection order — types of refund rejection, how to contest, appeal path, and re-filing strategy
type: notice-type
---

# RFD-06 — Refund Rejection Order

## What Is RFD-06?

RFD-06 is the **order rejecting a GST refund application** in full or in part. It is issued by the proper officer after processing the taxpayer's RFD-01 (refund application).

---

## Refund Lifecycle

```
RFD-01 (Refund Application)
        ↓
RFD-02 (Acknowledgement — if in order)
        OR
RFD-03 (Deficiency Memo — if documents insufficient)
        ↓
RFD-04 (Provisional refund — 90% within 7 days for exports)
        ↓
RFD-05 (Payment order — amount sanctioned)
        OR
RFD-06 (Rejection order — full or partial rejection)
        ↓
Appeal under §107 → APL-01
```

---

## Common Grounds for RFD-06 Rejection

| Ground | What the officer is saying |
|---|---|
| ITC not reflected in GSTR-2B | ITC claimed in refund not matching GSTR-2B |
| Supplier has not paid tax | Tax paid to supplier but supplier not deposited to govt |
| LUT/Bond expired or invalid | Export without IGST payment — LUT not valid for the period |
| Goods/services not exported | No proof of actual export (shipping bill, BRC, FIRC) |
| GSTR-1 not filed | Refund blocked as returns not filed |
| Inverted duty — tax rate calculation wrong | Officer disputes the net ITC eligible for refund |
| Time limit exceeded | Refund application filed after 2 years from relevant date |
| Documents incomplete | Shipping bills, invoices, declaration not proper |
| Place of supply incorrect | IGST charged but place of supply is within state |

---

## Immediate Checklist on Receiving RFD-06

1. **Note date of RFD-06** — Appeal must be filed within 3 months (§107)
2. **Read grounds of rejection carefully** — Each ground must be addressed separately
3. **Check if partial rejection** — Accepted portion may already be processed in RFD-05
4. **Assess strength of grounds** — Which can be cured by documentation? Which require legal contest?
5. **Check if re-filing is possible** — For some deficiencies, fresh RFD-01 may be faster than appeal

---

## Defence Strategy

### Ground: ITC Not in GSTR-2B
**Defence:** Produce supplier's GSTR-1 filing confirmation + GSTR-2B of subsequent month showing the invoice. Argue that §16(2) conditions are met and GSTR-2B restriction cannot permanently deny valid ITC refund.

### Ground: Supplier Not Paid Tax
**Defence:** Provide supplier's GSTR-3B extract showing tax paid + bank transfer proof of payment to supplier. If supplier has since been cancelled → argue taxpayer acted in good faith.

### Ground: LUT Expired / Invalid
**Defence:** Produce valid LUT for the period. If LUT was renewed but not updated on portal → produce renewal acknowledgement. If genuine LUT expiry → pay IGST on exports + claim refund under the alternative route.

### Ground: Export Not Proved
**Defence:** Provide shipping bill (for goods) / FIRC / BRC (for services) / bank remittance advice. Coordinate with customs / bank to obtain missing documents.

### Ground: Time Limit Exceeded
**Defence:** Verify the "relevant date" carefully:
- Exports: Date of export (shipping bill date)
- Inverted duty: End of financial year in which ITC accumulated
- If disputed → argue correct relevant date + file within 2 years thereof

---

## Appeal Path (If Contesting RFD-06)

1. File APL-01 (appeal) within **3 months** of RFD-06 date
2. Pre-deposit: Not applicable for refund appeals (refund was never paid)
3. Demand stay: Not applicable — this is a refund, not a demand
4. Load `apl-01-appeal.md` for the appeal template

---

## Re-Filing Route (Alternative to Appeal)

For certain rejection grounds, re-filing RFD-01 with corrected documents is faster than appeal:
- If rejected for incomplete documents → gather documents → re-file RFD-01
- If rejected for GSTR-1 not filed → file GSTR-1 → re-file RFD-01
- **Time limit:** New RFD-01 must be within 2 years of relevant date

---

## Key Provisions

| Provision | Subject |
|---|---|
| Section 54 | Refund of tax |
| Section 55 | Refund in special cases |
| Rule 89 | Application for refund (RFD-01) |
| Rule 92 | Order for refund (RFD-05 / RFD-06) |
| Circular 125/44/2019-GST | Refund procedure clarification |

---

*GST Notice Responder — Built by Rohan Vidhate*
