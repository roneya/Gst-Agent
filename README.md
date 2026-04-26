# GST Notice Responder

**An AI-powered GST notice reading, analysis, and reply drafting tool built as a Claude plugin.**

Built by **Rohan Vidhate** for Indian tax practitioners — CA firms, advocates, and in-house tax teams.

---

## What It Does

Paste any GST notice into Claude and get:

- **Notice identification** — type, section, demand amount, reply deadline
- **Procedural defect check** — DIN, jurisdiction, limitation period, GSTR-3A pre-condition
- **Allegation-wise defence strategy** — what to contest, what to accept, case law to cite
- **Ready-to-file reply** — ASMT-11, DRC-06, APL-01, REG-04, REG-18 (complete legal document)
- **Calculator outputs** — interest under §50, penalty under §73/74/74A, limitation deadlines

---

## Notices Covered

| Notice / Form | What It Is |
|---|---|
| **ASMT-10** | Scrutiny notice — return mismatch |
| **ASMT-13** | Best Judgement Assessment — non-filer (§62 auto-withdrawal in 30 days) |
| **ADT-01** | GST audit notice under §65 |
| **DRC-01A** | Pre-SCN intimation — penalty saving window |
| **DRC-01** | Show Cause Notice under §73 / §74 / §74A |
| **DRC-07** | Adjudication order — accept or appeal decision |
| **GSTR-3A** | Non-filer notice |
| **REG-03** | Registration query notice |
| **REG-17** | Registration cancellation SCN |
| **RFD-06** | Refund rejection order |

---

## Defence Playbooks

| Dispute Type | Playbook |
|---|---|
| ITC mismatch (GSTR-2A/2B vs 3B) | Yes |
| GSTR-1 vs GSTR-3B turnover mismatch | Yes |
| GSTR-9 vs GSTR-3B annual return mismatch | Yes |
| RCM non-payment | Yes |
| §17(5) blocked credit disputes | Yes |
| Fake ITC / §74 fraud allegation | Yes |
| Place of supply dispute (IGST vs CGST/SGST) | Yes |
| Valuation dispute (§15, related party, discounts) | Yes |

---

## Skill Library — 42 Files

```
.claude/skills/
│
├── gst-notice-interpreter/        Master orchestrator — reads any notice
├── gst-thresholds/                Rates, late fees, deadlines, penalty tables
│
├── cgst-act-reference/            11 statutory provisions
│   ├── section-16.md              ITC eligibility
│   ├── section-17.md              Blocked credits (§17(5) list)
│   ├── section-50.md              Interest on delayed payment
│   ├── section-61.md              Scrutiny of returns
│   ├── section-62.md              Best judgement assessment + §62(2) remedy
│   ├── section-65.md              GST audit by officers
│   ├── section-73.md              Non-fraud demand (up to FY 2023-24)
│   ├── section-74.md              Fraud / fake ITC demand
│   ├── section-74a.md             Unified demand (FY 2024-25 onwards)
│   ├── section-75.md              General provisions — hearing rights, penalty cap
│   └── section-107.md             Appeal — APL-01, pre-deposit, stay
│
├── cgst-rules-reference/          4 procedural rules
│   ├── rule-36-4.md               ITC restriction to GSTR-2B
│   ├── rule-86a.md                ITC blocking by officer — challenge & restoration
│   ├── rule-99.md                 ASMT-10/11/12 scrutiny procedure
│   └── rule-142.md                DRC forms — full demand lifecycle
│
├── gst-notice-types/              9 notice-specific deep-dive guides
│   ├── adt-01-audit.md
│   ├── asmt-10-scrutiny.md
│   ├── asmt-13-bja.md
│   ├── drc-01-scn.md
│   ├── drc-01a-intimation.md
│   ├── drc-07-order.md
│   ├── gstr-3a-non-filer.md
│   ├── rfd-06-rejection.md
│   └── reg-03-reg-17.md
│
├── gst-common-defences/           8 reusable defence playbooks
│   ├── itc-mismatch.md
│   ├── gstr1-gstr3b-mismatch.md
│   ├── gstr9-gstr3b-mismatch.md
│   ├── rcm-non-payment.md
│   ├── blocked-credit-section-17.md
│   ├── fake-itc-section74.md
│   ├── place-of-supply-dispute.md
│   └── valuation-dispute.md
│
├── gst-calculators/               3 step-by-step calculators
│   ├── interest-calculator.md     §50 interest — 18% / 24% — worked examples
│   ├── penalty-calculator.md      §73 / §74 / §74A penalty at each stage
│   └── limitation-checker.md      Is the SCN time-barred? FY-wise deadline table
│
└── gst-reply-templates/           5 ready-to-file reply templates
    ├── asmt-11-reply.md           For ASMT-10 scrutiny notice
    ├── drc-06-reply.md            For DRC-01 Show Cause Notice
    ├── apl-01-appeal.md           Appeal against DRC-07 order
    ├── reg-04-reply.md            For REG-03 registration query
    └── reg-18-reply.md            For REG-17 cancellation SCN
```

---

## How to Use

### 1. Paste the notice
```
"Here is a GST notice I received. Please analyse it and draft a reply."
```

### 2. Ask for a calculator
```
"Calculate interest on ₹5,00,000 tax paid 45 days late."

"Is this Section 73 SCN issued on 15-Jan-2025 for FY 2020-21 time-barred?"

"What is the penalty if we pay within 30 days of the DRC-01 SCN?"
```

### 3. Ask for a specific reply
```
"Draft a DRC-06 reply. We accept Ground 1 (₹2 lakhs ITC) but 
want to contest Ground 2 (output tax underreported)."

"Draft an APL-01 appeal against this DRC-07 order for ₹18 lakhs."

"Draft a REG-18 reply for this REG-17 cancellation notice."
```

### 4. Ask for defence strategy
```
"Our supplier's GSTIN was cancelled retrospectively. 
Officer is denying our ITC. How do we defend?"

"We charged IGST but officer says it's intra-state. 
Is there revenue loss? What is our remedy?"

"Officer says our related-party transaction value is too low 
and wants to revalue it. What is our defence?"
```

---

## Key Legal Coverage

- **Demand lifecycle:** DRC-01A → DRC-01 → DRC-06 → DRC-07 → APL-01
- **Registration lifecycle:** REG-03 → REG-04 → REG-17 → REG-18 → REG-21
- **Audit lifecycle:** ADT-01 → ADT-02 → DRC-01
- **Non-filer lifecycle:** GSTR-3A → ASMT-13 → §62(2) auto-withdrawal
- **Refund lifecycle:** RFD-01 → RFD-05 / RFD-06 → APL-01
- **ITC disputes:** §16, §17(5), Rule 36(4), Rule 86A — full coverage
- **Fraud defence:** §74 burden of proof, bona fide purchaser protection, due diligence checklist

---

*GST Notice Responder — Built by Rohan Vidhate*
