# GST Notice Responder — Claude Plugin

**Built by Rohan Vidhate**
**Project**: GST Notice Responder
**Purpose**: AI-powered GST notice reading, analysis, and reply drafting for Indian tax practitioners

---

## What This Plugin Does

Paste or upload any GST notice — the agent will:
1. **Read** and identify the notice type (ASMT-10, DRC-01 SCN, etc.)
2. **Analyse** the allegations and check for procedural defects
3. **Load** the relevant statutory provisions from the skill library
4. **Draft** a structured reply strategy with legal grounds and case law
5. **Generate** a ready-to-file reply (ASMT-11 or DRC-06)

---

## How to Use

### Step 1 — Paste the notice
Simply paste the text of the GST notice into Claude and say:
> *"Analyse this GST notice and help me draft a reply."*

### Step 2 — Claude reads the notice
The `gst-notice-interpreter` skill activates automatically and:
- Identifies the notice type and section cited
- Extracts GSTIN, tax period, demand amount, reply deadline
- Checks for procedural defects (DIN, jurisdiction, limitation)
- Flags urgency if deadline is close

### Step 3 — Defence strategy
Claude loads the relevant skill files and presents:
- Allegation-wise rebuttal strategy
- Which grounds to contest vs accept
- Legal provisions and case law to cite
- Whether to pay (DRC-03) or contest

### Step 4 — Draft the reply
Claude generates a complete ASMT-11 or DRC-06 reply with:
- Preliminary objections (if any)
- Discrepancy-wise responses
- Legal submissions
- Prayer for closure

---

## Skill Library

```
.claude/skills/
│
├── gst-notice-interpreter/     ← START HERE for any notice
│   └── SKILL.md                   Master orchestrator
│
├── gst-thresholds/             ← Penalty rates, interest rates, deadlines
│   └── SKILL.md
│
├── cgst-act-reference/         ← Statutory provisions
│   ├── section-16.md              ITC eligibility
│   ├── section-17.md              Blocked credits
│   ├── section-50.md              Interest on delayed payment
│   ├── section-61.md              Scrutiny of returns
│   ├── section-62.md              Best judgement assessment — §62(2) auto-withdrawal remedy
│   ├── section-65.md              GST audit by officers — ADT-01 procedure + taxpayer rights
│   ├── section-73.md              Non-fraud demand (up to FY 2023-24)
│   ├── section-74.md              Fraud demand (up to FY 2023-24)
│   ├── section-74a.md             Unified demand (FY 2024-25+)
│   ├── section-75.md              General provisions — hearing rights, penalty cap, speaking order
│   └── section-107.md             Appeal to Appellate Authority — APL-01, pre-deposit, stay
│
├── cgst-rules-reference/       ← Procedural rules
│   ├── rule-99.md                 ASMT-10/11/12 procedure
│   ├── rule-142.md                DRC forms — full demand lifecycle
│   ├── rule-86a.md                ITC blocking — challenge and restoration
│   └── rule-36-4.md               ITC restriction to GSTR-2B — defence strategy
│
├── gst-notice-types/           ← Notice-specific guides
│   ├── adt-01-audit.md            ADT-01 audit notice — document checklist + how to handle
│   ├── asmt-10-scrutiny.md        ASMT-10 scrutiny notice deep dive
│   ├── asmt-13-bja.md             ASMT-13 best judgement assessment — 30-day filing remedy
│   ├── drc-01-scn.md              DRC-01 Show Cause Notice (§73/74/74A)
│   ├── drc-01a-intimation.md      DRC-01A pre-SCN intimation guide
│   ├── drc-07-order.md            DRC-07 adjudication order — read, accept vs appeal
│   ├── gstr-3a-non-filer.md       GSTR-3A notice to non-filers
│   ├── rfd-06-rejection.md        RFD-06 refund rejection order — appeal vs re-filing strategy
│   └── reg-03-reg-17.md           REG-03 (registration query) + REG-17 (cancellation SCN)
│
├── gst-common-defences/        ← Reusable defence playbooks
│   ├── itc-mismatch.md            GSTR-2A/2B mismatch defence
│   ├── gstr1-gstr3b-mismatch.md   Turnover mismatch defence
│   ├── rcm-non-payment.md         RCM non-payment defence + ITC offset strategy
│   ├── gstr9-gstr3b-mismatch.md   Annual return vs GSTR-3B mismatch defence
│   ├── blocked-credit-section-17.md  §17(5) blocked ITC — what is blocked, what is not
│   ├── fake-itc-section74.md      §74 fraud / fake ITC allegation — burden of proof + defences
│   ├── place-of-supply-dispute.md IGST vs CGST/SGST misclassification — §77 wrong-head refund
│   └── valuation-dispute.md       §15 valuation — related party, discounts, free samples
│
├── gst-calculators/            ← Step-by-step calculators
│   ├── interest-calculator.md     §50 interest — formula + worked examples
│   ├── penalty-calculator.md      §73/74/74A penalty at each stage
│   └── limitation-checker.md      Is the SCN time-barred? FY-wise deadline table
│
└── gst-reply-templates/        ← Ready-to-file templates
    ├── asmt-11-reply.md           ASMT-11 reply template (for ASMT-10 scrutiny)
    ├── drc-06-reply.md            DRC-06 reply template (for DRC-01 SCN)
    ├── apl-01-appeal.md           APL-01 appeal template (against DRC-07 order)
    ├── reg-04-reply.md            REG-04 reply template (for REG-03 registration query)
    └── reg-18-reply.md            REG-18 reply template (for REG-17 cancellation SCN)
```

---

## Notice Type → Which Skills Load

| Notice received | Skills loaded |
|---|---|
| ASMT-10 (§61 scrutiny) | interpreter + section-61 + rule-99 + asmt-10-scrutiny |
| ASMT-13 (best judgement assessment) | interpreter + asmt-13-bja + section-62 + thresholds |
| ADT-01 (audit notice §65) | interpreter + adt-01-audit + section-65 |
| DRC-01A (pre-SCN intimation) | interpreter + drc-01a-intimation + section-73/74/74a + thresholds |
| DRC-01 SCN (§73) | interpreter + section-73 + rule-142 + drc-01-scn + drc-06-reply |
| DRC-01 SCN (§74) | interpreter + section-74 + rule-142 + drc-01-scn + drc-06-reply + fake-itc-section74 |
| DRC-01 SCN (§74A) | interpreter + section-74a + rule-142 + drc-01-scn + drc-06-reply |
| GSTR-3A (non-filing notice) | interpreter + gstr-3a-non-filer + thresholds |
| REG-03 (registration query) | interpreter + reg-03-reg-17 + reg-04-reply |
| REG-17 (cancellation SCN) | interpreter + reg-03-reg-17 + reg-18-reply |
| RFD-06 (refund rejection) | interpreter + rfd-06-rejection + section-107 |
| ITC mismatch allegation | section-16 + section-17 + itc-mismatch |
| Fake ITC / fraud allegation | section-74 + fake-itc-section74 + rule-86a |
| Turnover mismatch | section-73/74 + gstr1-gstr3b-mismatch |
| Place of supply dispute | interpreter + place-of-supply-dispute + thresholds |
| Valuation dispute | interpreter + valuation-dispute + thresholds |
| Interest demand | section-50 + thresholds |
| DRC-07 order received | interpreter + drc-07-order + section-107 + apl-01-appeal |
| Any notice | thresholds (always loaded for deadlines) |

---

## Sample Prompts

```
"Here is a GST notice I received. Please analyse it and tell me 
what I need to do."

"Draft an ASMT-11 reply for this ASMT-10 notice. The GSTR-2A 
mismatch allegation is for FY 2022-23."

"My client got a Section 73 SCN for ₹12 lakhs ITC reversal. 
The SCN was issued on 15-Jan-2025 for FY 2020-21. Is it 
time-barred?"

"Draft a DRC-06 reply for this DRC-01 SCN. We accept Ground 1 
(₹2 lakhs ITC) but want to contest Ground 2 (output tax 
underreported)."

"My client received a DRC-01A intimation for ₹8 lakhs. Should 
we pay now or wait for the SCN? What is the penalty saving?"

"Client got a GSTR-3A notice for not filing GSTR-3B for 
April to August 2024. What is the late fee and what should 
we do?"

"Our client's GST registration got a REG-17 cancellation notice 
for not filing returns. How do we save the GSTIN?"

"Calculate interest on ₹5,00,000 tax paid 45 days late."

"What penalty will apply if we pay within 30 days of this 
Section 73 SCN?"

"I received an ASMT-13 order dated 20-Apr-2026. Can I still 
withdraw it by filing my GSTR-3B?"

"Our client got an ADT-01 audit notice for FY 2022-23. What 
documents do we need to prepare and what are our rights?"

"GST officer has sent an SCN alleging fake ITC from a supplier 
whose GSTIN was cancelled. How do we defend?"

"My refund application was rejected via RFD-06 because ITC is 
not reflecting in GSTR-2B. What are my options?"

"We charged IGST on a supply but the officer says it was 
intra-state. Is there revenue loss? How do we rectify?"

"Officer is demanding GST on the full MRP but we gave a 20% 
trade discount on invoice. Is the discount deductible?"
```

---

*GST Notice Responder — Built by Rohan Vidhate*
