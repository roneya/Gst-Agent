---
name: gst-thresholds
description: Quick-reference for all GST numerical thresholds — penalty rates, interest rates, limitation periods, payment windows, and monetary limits. Load when computing interest, checking if limitation has expired, or verifying penalty amounts.
---

# GST Thresholds & Limits — Quick Reference

**Built by Rohan Vidhate**

---

## Penalty Rates

| Situation | Penalty | Section |
|---|---|---|
| §73 — pre-SCN payment | **NIL** | §73(5) |
| §73 — pay within 30 days of SCN | **NIL** | §73(8) |
| §73 — order passed | **10% of tax or ₹10,000 (higher)** | §73(9) |
| §73 — self-assessed tax not paid in 30 days | **Mandatory 10%** | §73(11) |
| §74 — pre-SCN payment | **15% of tax** | §74(5) |
| §74 — pay within 30 days of SCN | **25% of tax** | §74(8) |
| §74 — pay within 30 days of order | **50% of tax** | §74(11) |
| §74 — order passed, no payment | **100% of tax** | §74(9) |
| §74A non-fraud — pre-SCN payment | **NIL** | §74A(8)(i) |
| §74A non-fraud — pay within 60 days of SCN | **NIL** | §74A(8)(ii) |
| §74A non-fraud — order passed | **10% of tax or ₹10,000 (higher)** | §74A(5)(i) |
| §74A fraud — pre-SCN payment | **15% of tax** | §74A(9)(i) |
| §74A fraud — pay within 60 days of SCN | **25% of tax** | §74A(9)(ii) |
| §74A fraud — pay within 60 days of order | **50% of tax** | §74A(9)(iii) |
| §74A fraud — order passed, no payment | **100% of tax** | §74A(5)(ii) |

---

## Interest Rates

| Situation | Rate | Section |
|---|---|---|
| Late payment of output tax | **18% p.a.** | §50(1) |
| Late-filed GSTR-3B — cash component only (post-01.09.2020, before SCN) | **18% p.a. on cash portion** | §50(1) proviso |
| ITC wrongly availed **and utilised** | **24% p.a.** | §50(3) |
| ITC wrongly availed but **not utilised** | **NIL** | §50(3) — Bharti Airtel SC |
| ITC reversal under 180-day rule | **18% p.a.** | §50 + §16(2) proviso |

### Daily interest (per ₹1 lakh)
- 18% p.a. → **₹49.32 per day**
- 24% p.a. → **₹65.75 per day**

---

## Limitation Periods

| Provision | Limitation | Runs from |
|---|---|---|
| §73 — SCN | No separate limit (same as order) | — |
| §73 — Order | **3 years** | Due date of GSTR-9 for relevant FY |
| §73 — SCN gap from order | Min **3 months** before order deadline | §73(2) |
| §74 — SCN | No separate limit (same as order) | — |
| §74 — Order | **5 years** | Due date of GSTR-9 for relevant FY |
| §74 — SCN gap from order | Min **6 months** before order deadline | §74(2) |
| §74A — SCN | **42 months** | Due date of GSTR-9 for relevant FY |
| §74A — Order | **12 months** from SCN date | SCN issuance date |
| §74A — Order extension | Max **+6 months** (Commissioner approval) | Before 12-month expiry |
| §16(4) — ITC claim deadline | **30th November** of next FY | Or GSTR-9 filing, whichever earlier |
| §16(2) — 180-day payment rule | **180 days** from invoice date | Invoice date |

---

## §73/§74 Order Deadlines by FY

| FY | GSTR-9 Due Date | §73 Order Deadline (3Y) | §74 Order Deadline (5Y) |
|---|---|---|---|
| 2017-18 | 31-Dec-2019 | 31-Dec-2022 ❌ Expired | 31-Dec-2024 ❌ Expired |
| 2018-19 | 31-Aug-2020 | 31-Aug-2023 ❌ Expired | 31-Aug-2025 |
| 2019-20 | 28-Feb-2021 | 28-Feb-2024 ❌ Expired | 28-Feb-2026 |
| 2020-21 | 28-Feb-2022 | 28-Feb-2025 | 28-Feb-2027 |
| 2021-22 | 31-Dec-2022 | 31-Dec-2025 | 31-Dec-2027 |
| 2022-23 | 31-Dec-2023 | 31-Dec-2026 | 31-Dec-2028 |
| 2023-24 | 31-Dec-2024 | 31-Dec-2027 | 31-Dec-2029 |

## §74A SCN Deadlines by FY

| FY | GSTR-9 Due Date | §74A SCN Deadline (42M) | Max Order Deadline |
|---|---|---|---|
| 2024-25 | 31-Dec-2025 | 30-Jun-2029 | 31-Dec-2029 (+6M ext.) |
| 2025-26 | 31-Dec-2026 | 30-Jun-2030 | 31-Dec-2030 |

---

## Payment Windows — How Long to Pay

| Stage | §73 window | §74 window | §74A window |
|---|---|---|---|
| Pre-SCN (no penalty) | Any time before SCN | — | Any time before SCN |
| Pre-SCN (15% penalty) | — | Any time before SCN | Any time before SCN (fraud) |
| Post-SCN no/reduced penalty | **30 days** | **30 days** | **60 days** |
| Post-order reduced penalty | N/A | **30 days** (50%) | **60 days** (50%, fraud only) |

---

## Monetary Thresholds

| Threshold | Amount | Provision |
|---|---|---|
| Minimum demand for §74A notice | **₹1,000** per FY | §74A(1) proviso |
| Minimum §73 penalty at order | **₹10,000** or 10% (higher) | §73(9) |
| Minimum §74A non-fraud penalty | **₹10,000** or 10% (higher) | §74A(5)(i) |
| Banking/NBFC 50% ITC option cap | **50% of eligible ITC** | §17(4) |

---

## ITC Time Limits

| FY | Last date to claim ITC (§16(4)) |
|---|---|
| 2021-22 | 30-Nov-2022 or GSTR-9 date |
| 2022-23 | 30-Nov-2023 or GSTR-9 date |
| 2023-24 | 30-Nov-2024 or GSTR-9 date |
| 2024-25 | 30-Nov-2025 or GSTR-9 date |

---

## Reply Deadlines

| Notice type | Default reply period |
|---|---|
| ASMT-10 (§61 scrutiny) | **30 days** (extendable) |
| DRC-01 SCN (§73/§74) | As specified in SCN (typically 15-30 days) |
| DRC-01 SCN (§74A) | As specified in SCN |
| DRC-01A (pre-SCN intimation) | As specified (no statutory minimum) |
