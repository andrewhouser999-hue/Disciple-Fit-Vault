---
created: 2026-07-06
basis: "[[Covenant Identity — Two-Tier Intake Protocol]], [[Covenant Identity — Pre-Discovery Screen — Tally Build Guide]], [[Covenant Identity Intake — Tally Build Guide]] — field-level schema derived from these three documents' question sets and pipeline logic; no prior schema existed"
tags:
---

# Covenant Identity — Airtable Schema Spec
*Field-level base structure for the two-tier intake system. Both Tally Build Guides say "connect to Airtable" but neither specifies fields — this document is that missing layer. Build one Airtable base with the three tables below.*

**Who it's for:** Andrew, building the alpha-phase Airtable base by hand.
**What it is not:** An automation spec. See the Automation Notes at the end for what needs Make.com vs. what Airtable/Tally handle natively.

---

## Table 1 — Clients (master pipeline)

One row per prospective or active client. This is the table you actually look at day to day; the two response tables feed it but are not where you track pipeline state.

| Field | Type | Notes |
|---|---|---|
| Client Name | Single line text (primary field) | |
| Email | Email | Match key for linking response tables |
| Phone | Phone number | |
| Status | Single select | Options: `Discovery Booked` → `Pre-Discovery Complete` → `Discovery Call Done` → `Go – Agreement Sent` → `Go – Tier 2 Sent` → `Active` → `Completing` → `Closed` → `No-Go / Referred` |
| Discovery Call Date | Date | |
| Go/No-Go Decision | Single select | `Go` / `No-Go` / `Pending` |
| Go/No-Go Notes | Long text | Rationale against the 5 criteria in the Two-Tier Protocol |
| Payment Status | Single select | `Not Invoiced` / `Invoiced` / `Paid` / `Payment Plan Active` / `Refunded`. Check this is `Paid` or `Payment Plan Active` before manually sending Tier 2 — see the Payment Gate in the Two-Tier Intake Protocol. |
| Payment Plan Selected | Single select | `Full ($1,680)` / `3-Month Plan ($560/mo)` |
| Amount Paid | Currency | |
| Payment Date | Date | Date of most recent payment (full payment or latest installment) |
| Emergency Contact Name | Single line text | Mirrors Q19 once Tier 2 is submitted |
| Emergency Contact Phone | Phone number | Mirrors Q20 |
| Emergency Contact Relationship | Single line text | Mirrors Q21 |
| Current City/State | Single line text | Mirrors Q22 — required before Session 1 for every client, remote or local |
| Pre-Discovery Response | Link to record → Pre-Discovery Responses | |
| Intake Response | Link to record → Intake Responses | |
| Alpha Cohort | Checkbox | Marks the first cohort of clients for tracking purposes (e.g., early feedback, first-cohort testimonials) — alpha clients pay the same rates as later cohorts as of 2026-07-08 |
| Coach Notes | Long text | Free-form, not part of any client-facing document |

---

## Table 2 — Pre-Discovery Responses (Tier 1)

One row per Tally submission of the Pre-Discovery Screen. Field order matches the Tally Build Guide 1:1 so mapping during Tally→Airtable setup is mechanical.

| Field | Type | Source |
|---|---|---|
| Respondent Name | Single line text (primary field) | |
| Submission Date | Date | Auto-populated by Tally |
| Q1 – Presenting Issue | Long text | Q1 |
| Q2 – Duration & Prior Attempts | Long text | Q2 |
| Q3 – Season Description | Long text | Q3 |
| Q4 – God-Relationship Now | Long text | Q4 |
| Q5 – Identity Gap Scale (1-10) | Number | Q5 |
| Q6 – Motivation | Long text | Q6 |
| Q7 – Clinical Screen | Single select (Yes/No) | Q7 |
| Q8 – Anything Else | Long text | Q8, optional |
| Client | Link to record → Clients | Match by email |

---

## Table 3 — Intake Responses (Tier 2)

One row per Tally submission of the full Covenant Identity Intake. Includes the new Section G fields (Q19-22) added to the Tally Build Guide.

| Field | Type | Source |
|---|---|---|
| Respondent Name | Single line text (primary field) | |
| Submission Date | Date | Auto-populated by Tally |
| Q1 – Reach-Out Trigger | Long text | Q1 |
| Q2 – Duration & Attempts | Long text | Q2 |
| Q3 – Life Arc | Long text | Q3 |
| Q4 – Childhood Messages | Long text | Q4 |
| Q5 – God-Relationship Actual | Long text | Q5 |
| Q6 – God's View at Failure | Long text | Q6 |
| Q7 – Lament History | Long text | Q7 |
| Q8 – Failure Meaning | Long text | Q8 |
| Q9 – Identity Gap Scale (1-10) | Number | Q9 |
| Q10 – Fear of Discovery | Long text | Q10 |
| Q11 – Real Motivation | Long text | Q11 |
| Q12 – Clinical Screen | Single select (Yes/No) | Q12 |
| Q13 – Anything Else | Long text | Q13, optional |
| Q14 – Life Going Well Condition | Long text | Q14 |
| Q15 – First Reach Under Stress | Long text | Q15 |
| Q16 – Fear of Losing | Long text | Q16 |
| Q17 – Dependency Source | Long text | Q17 |
| Q18 – Last Thing to Give Up | Long text | Q18 |
| Emergency Contact Name | Single line text | Q19 |
| Emergency Contact Phone | Phone number | Q20 |
| Emergency Contact Relationship | Single line text | Q21 |
| Current City/State | Single line text | Q22 |
| Client | Link to record → Clients | Match by email |

---

## Automation Notes — What Actually Needs Make.com (Answer: Almost Nothing, Yet)

Both existing Tally guides already specify native integrations that cover alpha-phase needs without Make.com:

- **Tier 1 delivery:** Calendly sends the Pre-Discovery Screen link automatically in the booking confirmation email — no Make.com scenario needed, this is a Calendly setting.
- **Response capture:** Tally's native Airtable integration writes each submission directly into its response table — no Make.com scenario needed.
- **Tier 2 delivery:** Sent manually by the coach after payment clears — this is an intentional human gate (both the go/no-go call and the payment check), not an automation target.
- **Payment:** Stripe Payment Link, sent manually alongside the Coaching Agreement. No Stripe webhook/automation needed at alpha volume — check the Payment Link's status in Stripe's dashboard directly and update the Clients `Payment Status` field by hand before sending Tier 2.

**The one real gap:** neither native integration automatically links a new response row to the right Clients record or advances Status. Two ways to close it, in order of effort:

1. **Airtable's own native Automations** (not Make.com) — trigger "record created" in a response table → find or create a Clients record matching on email → update Status. This is built into Airtable's free tier and is the right tool for alpha; it's a same-base operation, not a cross-app one.
2. **Make.com** — only becomes necessary once you need to reach outside Airtable itself (e.g., a Stripe webhook auto-updating Payment Status, or a Gmail welcome sequence off a Status change). Not needed yet at alpha volume — manual Stripe dashboard checks and manual welcome emails are fine at this scale.

Don't build a Make.com scenario for intake linking or payment tracking at alpha. It's solving a problem Airtable's native automation (and a five-second manual check) already solves for free.
