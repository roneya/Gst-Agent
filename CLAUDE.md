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
│   ├── asmt-10-scrutiny.md        ASMT-10 scrutiny notice deep dive
│   ├── drc-01-scn.md              DRC-01 Show Cause Notice (§73/74/74A)
│   ├── drc-01a-intimation.md      DRC-01A pre-SCN intimation guide
│   ├── drc-07-order.md            DRC-07 adjudication order — read, accept vs appeal
│   ├── gstr-3a-non-filer.md       GSTR-3A notice to non-filers
│   └── reg-03-reg-17.md           REG-03 (registration query) + REG-17 (cancellation SCN)
│
├── gst-common-defences/        ← Reusable defence playbooks
│   ├── itc-mismatch.md            GSTR-2A/2B mismatch defence
│   └── gstr1-gstr3b-mismatch.md   Turnover mismatch defence
│
├── gst-calculators/            ← Step-by-step calculators
│   ├── interest-calculator.md     §50 interest — formula + worked examples
│   ├── penalty-calculator.md      §73/74/74A penalty at each stage
│   └── limitation-checker.md      Is the SCN time-barred? FY-wise deadline table
│
└── gst-reply-templates/        ← Ready-to-file templates
    ├── asmt-11-reply.md           ASMT-11 reply template (for ASMT-10 scrutiny)
    ├── drc-06-reply.md            DRC-06 reply template (for DRC-01 SCN)
    └── apl-01-appeal.md           APL-01 appeal template (against DRC-07 order)
```

---

## Notice Type → Which Skills Load

| Notice received | Skills loaded |
|---|---|
| ASMT-10 (§61 scrutiny) | interpreter + section-61 + rule-99 + asmt-10-scrutiny |
| DRC-01A (pre-SCN intimation) | interpreter + drc-01a-intimation + section-73/74/74a + thresholds |
| DRC-01 SCN (§73) | interpreter + section-73 + rule-142 + drc-01-scn + drc-06-reply |
| DRC-01 SCN (§74) | interpreter + section-74 + rule-142 + drc-01-scn + drc-06-reply |
| DRC-01 SCN (§74A) | interpreter + section-74a + rule-142 + drc-01-scn + drc-06-reply |
| GSTR-3A (non-filing notice) | interpreter + gstr-3a-non-filer + thresholds |
| REG-03 (registration query) | interpreter + reg-03-reg-17 |
| REG-17 (cancellation SCN) | interpreter + reg-03-reg-17 |
| ITC mismatch allegation | section-16 + section-17 + itc-mismatch |
| Turnover mismatch | section-73/74 + gstr1-gstr3b-mismatch |
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
```

---

*GST Notice Responder — Built by Rohan Vidhate*
