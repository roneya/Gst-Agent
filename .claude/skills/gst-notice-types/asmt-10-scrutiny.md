---
name: gst-notice-type-asmt10
description: Deep-dive guide for ASMT-10 scrutiny notices. Load when the notice form is ASMT-10 to understand what the officer is doing, what the taxpayer must do, and how to respond via ASMT-11.
---

# Notice Type: ASMT-10 (Scrutiny Notice under Section 61)

## What is ASMT-10?
ASMT-10 is a scrutiny notice issued by the GST officer under Section 61 read with Rule 99. It is a **pre-demand** notice — no tax has been demanded yet. The officer has spotted a discrepancy in the return and is asking for an explanation.

## Key Facts
- **Issued under**: Section 61 + Rule 99
- **Reply form**: ASMT-11 (taxpayer) 
- **Closure form**: ASMT-12 (officer, if reply accepted)
- **Reply deadline**: 30 days from service (extendable)
- **Escalation if no reply**: §73/§74/§74A SCN or §65/§66 audit

## Immediate Checklist on Receipt

| Check | Action |
|---|---|
| DIN present on notice? | If missing → notice invalid (CBIC Circular 128/47/2019) |
| Reply deadline? | Calculate 30 days from service date |
| Less than 7 days left? | Flag as URGENT — request extension immediately |
| Is the discrepancy specified clearly? | If vague → raise in preliminary objection |
| Officer jurisdiction correct? | Verify ward/circle matches GSTIN |

## Common Discrepancies in ASMT-10

1. **GSTR-2A/2B vs GSTR-3B** — ITC mismatch → load `itc-mismatch.md`
2. **GSTR-1 vs GSTR-3B** — Turnover mismatch → load `gstr1-gstr3b-mismatch.md`
3. **Non-payment of RCM** — Purchases from unregistered dealers
4. **ITC on blocked items** — Motor vehicles, food, CSR → load `section-17.md`
5. **Late payment interest** — Interest not paid on delayed GSTR-3B → load `section-50.md`
6. **GSTR-9 vs GSTR-3B** — Annual return mismatch

## Reply Strategy

**Goal**: Get ASMT-12 (closure). Avoid escalation to §73/§74 SCN.

1. File ASMT-11 on portal before the 30-day deadline
2. Address every discrepancy by serial number
3. For accepted discrepancies: pay via DRC-03, quote ARN in ASMT-11
4. For disputed discrepancies: give factual + legal explanation + attach documents
5. End with prayer for ASMT-12

## Portal Path
Services → User Services → My Applications → Application Type: Reply to Notice → Select ASMT-10 reference → File ASMT-11
