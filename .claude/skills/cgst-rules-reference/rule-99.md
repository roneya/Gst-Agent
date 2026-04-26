---
name: cgst-rule-99
description: Reference for Rule 99 of CGST Rules 2017 - Scrutiny of returns. Load this skill when working with ASMT-10 (scrutiny notice), ASMT-11 (taxpayer reply), or ASMT-12 (closure order) forms, or when drafting the procedural framework for a Section 61 scrutiny response.
---

# Rule 99 — Scrutiny of Returns (CGST Rules, 2017)

## Plain-English Summary

Rule 99 is the **procedural backbone** of Section 61. While §61 gives the officer the power to scrutinize returns and ask for explanations, Rule 99 prescribes **how** that process works — the forms to be used, the timelines, and the steps from notice to closure.

Three forms govern the entire §61 lifecycle:

| Form | Who issues | Purpose |
|---|---|---|
| **ASMT-10** | Proper officer | Scrutiny notice — informs taxpayer of discrepancies |
| **ASMT-11** | Registered person (taxpayer) | Reply to scrutiny notice |
| **ASMT-12** | Proper officer | Closure order — if reply is acceptable |

---

## Rule 99(1) — The ASMT-10 Notice

### When issued
When a return is **selected for scrutiny**, the proper officer:
1. Scrutinizes the return under §61 with reference to **information available with him**
2. If discrepancies are found — issues **FORM GST ASMT-10**

### What ASMT-10 must contain
- Inform the taxpayer of the **discrepancy** found
- Seek the taxpayer's **explanation**
- **Time limit** for reply: **not exceeding 30 days** from date of service (extendable at officer's discretion)
- **Quantification** of tax, interest, and other amounts — "where possible"

### Key interpretive points

**"Where possible" quantification**: The rule says the officer should quantify the demand "where possible." If the ASMT-10 does not quantify the demand, the taxpayer is not prejudiced — but it does mean the taxpayer may not know the exact amount to contest. In the reply (ASMT-11), always ask the officer to provide quantification if absent.

**"Information available with him"**: The officer can use any information in the department's possession — GSTR-1, GSTR-3B, GSTR-2A/2B, e-way bills, e-invoices, third-party data, annual return (GSTR-9/9C), audit reports. The notice is not limited to the return itself.

**30-day reply period**: This is the maximum default. The officer has discretion to grant more time. Always request an extension if 30 days is insufficient given the volume of discrepancies.

---

## Rule 99(2) — The ASMT-11 Reply

### Filed by: Registered person (taxpayer)
### Form: FORM GST ASMT-11

The taxpayer can either:

**(a) Accept the discrepancy and pay**
- Pay the tax + interest + any other amount arising from the discrepancy
- Inform the officer of such payment in ASMT-11
- Include DRC-03 ARN as proof of payment

**(b) Furnish an explanation**
- Explain why the discrepancy is not correct
- Provide supporting documents
- Submit legal / factual grounds for each discrepancy

**(c) Both — partial acceptance + partial dispute**
- Accept some discrepancies (with DRC-03 payment)
- Dispute the remaining discrepancies with explanation

### How to file ASMT-11
Portal path: **Services → User Services → My Applications → Application Type: Reply to Notice** → Select the ASMT-10 reference number → File ASMT-11

### What a good ASMT-11 reply contains
1. **Reference details**: ASMT-10 notice number, date, GSTIN, tax period
2. **Preliminary objections** (if any): jurisdictional issues, vague notice, etc.
3. **Ground-wise response**: address each discrepancy by serial number as raised in ASMT-10
4. **For accepted discrepancies**: DRC-03 ARN, date, amount paid
5. **For disputed discrepancies**: factual explanation + legal submissions + supporting documents
6. **Prayer**: Request for acceptance of reply and closure via ASMT-12
7. **Annexures**: Invoices, GSTR reconciliation, bank statements, e-way bills, etc.

---

## Rule 99(3) — The ASMT-12 Closure

### Issued by: Proper officer
### Form: FORM GST ASMT-12
### When: If the explanation in ASMT-11 is found **acceptable**

The officer informs the taxpayer that the explanation is accepted and **no further action** is taken.

**ASMT-12 = the goal of every §61 reply.** Once ASMT-12 is issued, the matter is closed at the scrutiny stage — no §73/§74 demand follows for those specific discrepancies.

---

## The ASMT-10 → ASMT-11 → ASMT-12 Workflow

```
Officer selects return for scrutiny
          ↓
Officer finds discrepancy
          ↓
Issues ASMT-10 (notice to taxpayer)
          ↓
Taxpayer files ASMT-11 within 30 days (reply)
          ↓
        ┌──────────────────────┬──────────────────────┐
        ↓                      ↓                      ↓
Reply acceptable         Reply not satisfactory   No reply filed
        ↓                      ↓                      ↓
Officer issues           Officer may initiate:   Officer may initiate:
ASMT-12 (closure)       - §65 audit             - §65/§66/§67
                         - §66 special audit     - §73/§74/§74A demand
                         - §67 inspection
                         - §73/§74/§74A demand
```

---

## Timelines Summary

| Event | Timeline |
|---|---|
| Reply to ASMT-10 | **30 days** from service of ASMT-10 (extendable) |
| Extension of reply period | At officer's discretion — request in writing before expiry |
| ASMT-12 issuance (if reply accepted) | No statutory deadline — officer must issue promptly |
| Officer escalation after non-reply | No specific deadline — but §73/§74/§74A limitation applies to the eventual demand |

---

## Procedural Defects in ASMT-10 — What to Check

The ASMT-10 notice is invalid if:

| # | Defect | Consequence |
|---|---|---|
| 1 | Not in FORM GST ASMT-10 | Not a valid scrutiny notice under Rule 99 |
| 2 | Does not specify the discrepancy | Violates Rule 99(1) — taxpayer cannot reply meaningfully |
| 3 | Issued by officer without jurisdiction | Void ab initio |
| 4 | Not served on the registered email/GST portal | Improper service |
| 5 | Reply period given is less than 30 days with no justification | Violates the minimum period under Rule 99(1) |
| 6 | No DIN (Document Identification Number) on the notice | Invalid per CBIC Circular 128/47/2019 — notices without DIN are treated as never issued |

**Agent action**: Check the ASMT-10 for all of the above before drafting the ASMT-11 reply on merits. Raise valid defects as **Preliminary Objections** in the reply.

---

## DIN Requirement — Critical Check

**CBIC Circular No. 128/47/2019-GST** mandates that all communications from GST officers (including ASMT-10) must carry a **Document Identification Number (DIN)** generated from the system.

A notice **without a DIN** (or with a manually written DIN) shall be treated as if it was **never issued** — the taxpayer can ignore it or raise this objection in the reply.

**How to verify DIN**: The DIN is a 20-digit number printed on the notice. It can be verified at: `https://verfiy.cbic.gov.in` (CBIC DIN verification portal).

---

## Extension of Time — How to Request

If 30 days is insufficient to compile the reply:

1. File a **written application** to the proper officer before the 30-day deadline
2. State specific reasons (volume of records, complexity of reconciliation, etc.)
3. Request the extension period needed
4. The officer has discretion — no statutory obligation to grant, but denial of reasonable time can be challenged as violation of natural justice

**Agent tip**: Always file for extension before the deadline — not after. An extension request filed after the 30-day period expires has no legal basis.

---

## What Happens if ASMT-11 Is Not Filed

Rule 99 does not specify a consequence for non-filing of ASMT-11. However, under §61(3) of the CGST Act, if no satisfactory explanation is furnished within 30 days, the officer may:
- Initiate audit (§65 / §66)
- Order inspection/search (§67)
- Proceed to determine tax under §73 / §74 / §74A

**Agent alert**: Always file ASMT-11 — even a brief one — before the deadline. A non-reply is treated as an admission of the discrepancy by the officer in practice.

---

## ASMT-11 Template Structure

```
To,
The Proper Officer,
[GST Office Name and Address]

Subject: Reply to ASMT-10 Notice No. [___] dated [___] for Tax Period [___]
         Under Section 61 read with Rule 99 of CGST Rules, 2017

Reference: GSTIN: [___] | Notice Ref: [ASMT-10 number]

Respected Sir/Madam,

We, M/s [Company Name] (GSTIN: [___]), hereby submit our reply to the
above-captioned notice received on [date].

I. PRELIMINARY OBJECTIONS
[List any procedural defects — DIN missing, jurisdiction, vague notice, etc.]

II. FACTUAL BACKGROUND
[Brief 2-3 line description of the business and the relevant transactions]

III. DISCREPANCY-WISE RESPONSE

Discrepancy No. 1: [Quote the discrepancy from ASMT-10]
Our Response: [Factual + legal explanation]
Supporting Documents: [List annexures]

Discrepancy No. 2: [...]
[If accepted: "We accept this discrepancy and have paid ₹[___] vide
DRC-03 ARN [___] dated [___] along with interest of ₹[___]."]

IV. LEGAL SUBMISSIONS
[Cite relevant sections, rules, CBIC circulars, and case law]

V. PRAYER
In view of the above, we respectfully pray that:
(a) The explanation furnished herein be accepted;
(b) Form GST ASMT-12 be issued closing the proceedings;
(c) No further action be initiated for the discrepancies explained above.

Yours faithfully,
[Authorized Signatory]
[Name, Designation]
[Date]

Annexures:
1. [List all supporting documents]
```

---

## Related Provisions

- **Section 61** — Statutory power behind Rule 99 → `cgst-act-reference/section-61.md`
- **Section 73** — Escalation path (non-fraud demand) → `cgst-act-reference/section-73.md`
- **Section 74** — Escalation path (fraud demand, up to FY 2023-24) → `cgst-act-reference/section-74.md`
- **Section 74A** — Escalation path (FY 2024-25 onwards) → `cgst-act-reference/section-74a.md`
- **CBIC Circular 128/47/2019** — DIN requirement for all officer communications

## What This Skill Does NOT Cover

- Scrutiny selection criteria (risk-based, AI-driven — not prescribed in Rule 99)
- Portal filing mechanics beyond the form names
- Adjudication procedure after escalation to §73/§74 (see Rule 142)

---

**Source**: CGST Rules, 2017 — Rule 99, as notified under the Central Goods and Services Tax Act, 2017.
