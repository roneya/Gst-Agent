---
name: cgst-section-61
description: Reference for Section 61 of CGST Act 2017 - Scrutiny of Returns. Load this skill when the notice is issued under Section 61, when the form is ASMT-10, or when the officer is scrutinizing returns and pointing out discrepancies.
---

# Section 61 — Scrutiny of Returns

## Plain-English summary

Section 61 lets a GST officer examine a registered person's filed returns, flag any discrepancies, and ask for an explanation. It is the **gateway provision** for GST scrutiny — the officer cannot jump straight to a tax demand without first issuing a Section 61 notice (typically in Form **ASMT-10**) and giving the taxpayer a chance to explain.

This is a **pre-adjudication** stage. No tax demand has been raised yet. The taxpayer's reply (in Form **ASMT-11**) decides whether the matter ends here or escalates.

## When this section applies

A notice cites Section 61 when:
- The proper officer has scrutinized GSTR-1, GSTR-3B, GSTR-9, GSTR-2A/2B, or related particulars
- A discrepancy has been noticed (mismatch in turnover, ITC, tax payable, etc.)
- The officer is asking the taxpayer to explain the discrepancy
- The notice form is **ASMT-10** (issued under Rule 99 of CGST Rules)

If the notice cites Section 73 or 74 directly without a prior Section 61 step, that is a different (later-stage) proceeding — see `section-73.md` / `section-74.md` instead.

## Sub-section breakdown

### Section 61(1) — The scrutiny power
The proper officer **may** scrutinize the return and related particulars to verify correctness, and inform the registered person of any discrepancies in the manner prescribed (Rule 99 → Form ASMT-10), seeking the taxpayer's explanation.

**Key words for the agent**:
- "May scrutinize" — discretionary power, not mandatory
- "Related particulars" — extends beyond the return itself to GSTR-2A/2B, e-way bills, books, etc.
- "Inform him of the discrepancies" — the notice must specify each discrepancy clearly
- "Seek his explanation" — the taxpayer has the right to be heard

### Section 61(2) — When the explanation is accepted
If the taxpayer's explanation is found acceptable, the registered person **shall be informed accordingly** and **no further action** shall be taken. This closure is communicated through Form **ASMT-12**.

**Strategic implication**: A well-drafted ASMT-11 reply that the officer accepts results in ASMT-12 (closure). This is the goal of every reply.

### Section 61(3) — Escalation paths if explanation is unsatisfactory
If **either** of the following happens within **30 days of being informed** (or such further period as the officer may permit):

(a) The taxpayer does not furnish a satisfactory explanation, **OR**
(b) The taxpayer accepts the discrepancy but fails to take corrective measures in the return for the month of acceptance,

then the proper officer **may** initiate any of the following:
- Audit under **Section 65** (departmental audit)
- Special audit under **Section 66** (audit by chartered/cost accountant)
- Inspection / search / seizure under **Section 67**
- Determination of tax under **Section 73** (non-fraud cases)
- Determination of tax under **Section 74** (fraud / wilful misstatement / suppression)
- Determination of tax under **Section 74A** (inserted via Finance Act 2024 — applies to FY 2024-25 onwards; consolidates §73/§74 timelines)

## Time limits

| Event | Time limit |
|---|---|
| Reply to ASMT-10 (under §61) | **30 days** from receipt of notice |
| Extension of reply period | At officer's discretion ("such further period as may be permitted") |
| Officer's window to initiate §73/§74 after non-reply | Governed by §73/§74 limitation, not §61 itself |

## Critical interpretive points

### 1. Section 61 is procedural, not substantive
No tax can be demanded under Section 61. It is purely a notice-and-reply mechanism. Demands flow from Section 73 / 74 / 74A.

### 2. The 30-day clock matters
Missing the 30-day deadline does NOT automatically result in a demand — but it removes the taxpayer's opportunity to explain at this stage and almost guarantees escalation to §73/§74.

### 3. "Accept and rectify" is a legitimate path
Section 61(3)(b) acknowledges that the taxpayer can accept the discrepancy and rectify it in a subsequent return. If done within 30 days, escalation is avoided. The reply should clearly state acceptance and reference the corrective return (GSTR-3B for the month of acceptance, with DRC-03 if tax was short-paid).

### 4. Audit / inspection are alternative escalation routes
Many practitioners forget that §61(3) allows the officer to choose §65, §66, or §67 in addition to §73/§74. A weak reply may trigger a full departmental audit instead of just a tax demand.

## Exact statutory text (for citation in the reply)

> **Section 61. Scrutiny of returns.—**
>
> (1) The proper officer may scrutinize the return and related particulars furnished by the registered person to verify the correctness of the return and inform him of the discrepancies noticed, if any, in such manner as may be prescribed and seek his explanation thereto.
>
> (2) In case the explanation is found acceptable, the registered person shall be informed accordingly and no further action shall be taken in this regard.
>
> (3) In case no satisfactory explanation is furnished within a period of thirty days of being informed by the proper officer or such further period as may be permitted by him or where the registered person, after accepting the discrepancies, fails to take the corrective measure in his return for the month in which the discrepancy is accepted, the proper officer may initiate appropriate action including those under section 65 or section 66 or section 67, or proceed to determine the tax and other dues under section 73 or section 74 [or section 74A].

## Related provisions

- **Rule 99, CGST Rules** — Procedure for scrutiny; prescribes Forms ASMT-10, ASMT-11, ASMT-12. See `cgst-rules-reference/rule-99.md`.
- **Section 65** — Audit by tax authorities
- **Section 66** — Special audit
- **Section 67** — Power of inspection, search and seizure
- **Section 73** — Determination of tax (non-fraud)
- **Section 74** — Determination of tax (fraud)
- **Section 74A** — Determination of tax for FY 2024-25 onwards

## Common officer allegations under Section 61

When you see a Section 61 / ASMT-10 notice, the discrepancy almost always falls into one of these buckets:

1. **GSTR-3B vs GSTR-2A/2B mismatch** (excess ITC claimed) → see `gst-common-defences/itc-mismatch.md`
2. **GSTR-1 vs GSTR-3B turnover mismatch** → see `gst-common-defences/gstr1-gstr3b-mismatch.md`
3. **Non-payment of tax under reverse charge mechanism (RCM)**
4. **Ineligible ITC claimed under Section 17(5)** → see `cgst-act-reference/section-17.md`
5. **Mismatch with e-way bills / e-invoices**
6. **Late fee / interest non-payment under Section 50**
7. **Non-filing of GSTR-9 / GSTR-9C reconciliation**

## Defence approach for Section 61 notices

The standard reply structure (in ASMT-11) is:

1. Acknowledge receipt of the ASMT-10 notice with reference number and date
2. Identify each discrepancy raised by the officer (numbered list)
3. For each discrepancy:
   - State whether the discrepancy is **disputed** or **accepted**
   - If disputed: provide the legal/factual defence with supporting documents
   - If accepted: state the corrective action taken (which return, which DRC-03 challan, etc.)
4. Cite relevant statutory provisions, circulars, and case law
5. Pray for closure under Section 61(2) and issuance of Form ASMT-12

For the actual reply structure and template, see `gst-reply-templates/asmt-11-reply.md`.

## Is Section 61 mandatory before a Section 73/74 demand?

This is a live judicial question. The agent must flag it when an officer skips §61 and directly issues a show-cause notice under §73/§74.

### High Court rulings holding §61 is a mandatory precondition
- **Bharti Airtel Ltd. v. Union of India** — Delhi HC held that the proper officer must follow the statutory sequence: scrutiny under §61 → opportunity to explain → only then proceed to §73/§74. Jumping directly to §73 without a prior §61 notice vitiates the demand.
- **Vimal Petro Products v. State of Gujarat** — Gujarat HC reiterated that §61 scrutiny is not an empty formality; skipping it denies the taxpayer the opportunity to explain at the earliest stage, violating principles of natural justice.

### Contra view (minority)
Some High Courts have held that §61 is directory, not mandatory, and that a §73 SCN issued without prior §61 notice is not automatically void if the taxpayer was given full opportunity at the §73 stage itself.

### Agent action
If the notice is a §73/§74 SCN with **no prior ASMT-10**: raise the procedural objection as a **preliminary ground** in the reply — do not let it be the only ground. Argue on merits in the alternative.

---

## Procedural defects checklist — when to challenge the notice itself

Before drafting the reply on merits, check the ASMT-10 for these defects. Each is a ground to object at the outset (while still replying on merits as a backup):

| # | Defect | Ground |
|---|---|---|
| 1 | Notice does not specify the discrepancy clearly | Violates §61(1) — "inform him of the discrepancies"; notice is vague and non-speaking |
| 2 | Notice issued by officer without jurisdiction (wrong ward/circle) | Lack of jurisdiction — void ab initio |
| 3 | Notice not served on the registered email/portal | Non-service / improper service under Rule 99 |
| 4 | Notice is unsigned or bears digital signature of wrong officer | Not a valid notice in law |
| 5 | Notice issued after limitation period for underlying demand has expired | Even if §61 has no own limitation, officer cannot use it as a backdoor after §73/§74 limitation has run out |
| 6 | Same discrepancy already adjudicated in a prior proceeding | Res judicata / issue estoppel |
| 7 | Notice covers a period already under audit (§65) | Double jeopardy — parallel proceedings on same issue not permissible |

**How to use in the reply**: Open the reply with a section titled "Preliminary Objections" listing applicable defects. Then say "Without prejudice to the above objections, the Noticee submits the following explanation on merits…"

---

## DRC-03 — Voluntary payment when accepting a discrepancy

When the taxpayer decides to **accept** the discrepancy (full or partial) under §61(3)(b), the correct process is:

### Step-by-step
1. **File DRC-03** (voluntary payment form) on the GST portal → `Services → Payments → Voluntary Tax Payment (DRC-03)`
2. Select the relevant financial year and tax head (IGST / CGST / SGST / Cess)
3. Select cause as **"Scrutiny"** from the dropdown (maps to §61)
4. Pay the differential tax + applicable interest under **Section 50** (18% p.a. from due date to payment date)
5. **Note the ARN** of the DRC-03 — quote it in the ASMT-11 reply
6. File ASMT-11 referencing the DRC-03 ARN and stating the corrective return (GSTR-3B for the month of acceptance)

### What to mention in the ASMT-11
> "Without prejudice to our submissions on the other discrepancies, the Noticee accepts the discrepancy at Sr. No. [X] amounting to ₹[___] and has discharged the tax liability along with applicable interest vide DRC-03 bearing ARN [___] dated [___]. The corrective disclosure has also been made in the GSTR-3B for the month of [Month, Year]."

### Interest calculation formula
Interest = (Tax amount × 18%) ÷ 365 × number of days of delay

### Key point
Paying via DRC-03 and mentioning it in ASMT-11 is the **strongest way** to close a discrepancy under §61(2). Officers almost always issue ASMT-12 (closure) once DRC-03 is on record.

---

## Key case law for citation in replies

### 1. On right to be heard / opportunity to explain
**Graziano Transmissioni India Pvt. Ltd. v. Additional Commissioner, CGST**
> Held: An ASMT-10 notice that bundles multiple discrepancies without specifying the basis of each calculation does not give the taxpayer a meaningful opportunity to explain. Such a notice is liable to be set aside for violation of natural justice.

### 2. On acceptance of explanation / closure
**Safari Retreats Pvt. Ltd. v. Chief Commissioner of CGST**
> Held: Where the taxpayer furnishes documentary evidence explaining the discrepancy and the officer proceeds to §73 without recording reasons for rejecting the explanation, the §73 SCN is not sustainable. The officer must apply his mind and issue ASMT-12 or record reasons for escalation.

### 3. On limitation — §61 cannot revive time-barred demands
**Suo motu observations in M/s Ratnamani Metals & Tubes Ltd. v. Union of India (Gujarat HC)**
> Held: Section 61 scrutiny cannot be used as a tool to reopen periods for which the limitation under §73/§74 has already expired. The scrutiny power is not independent of the demand limitation.

### 4. On ITC mismatch — difference in GSTR-2A is not automatic disallowance
**ITC mismatch cases (consistent line of High Court rulings — Calcutta, Delhi, Madras HCs)**
> Held: A mismatch between GSTR-2A and GSTR-3B, by itself, is not sufficient to deny ITC. The registered person can demonstrate actual receipt of goods/services and payment of tax by the supplier through independent evidence. See `gst-common-defences/itc-mismatch.md` for the full defence playbook.

---

## What this skill does NOT cover

- Demand stage replies (§73/§74) — see those section files
- Procedural rules (manner of service, format of notice) — see `cgst-rules-reference/rule-99.md`
- Specific defence playbooks — see files in `gst-common-defences/`

---

**Source**: CGST Act, 2017 (Act No. 12 of 2017), as amended up to Finance Act 2024 (insertion of "or section 74A").
