---
created: 2026-07-06
basis: "[[Covenant Identity — Two-Tier Intake Protocol]], [[Covenant Identity — Pre-Discovery Screen — Tally Build Guide]], [[Covenant Identity Intake — Tally Build Guide]] — field-level schema derived from these three documents' question sets and pipeline logic; no prior schema existed. Table 4 added 2026-07-10 per [[Covenant Identity — Alliance Pulse]]. Table 5 (Session Notes) added 2026-07-31 — mirrors the CIC diagnostic sequence (affections → false identity → covenant truth → stage work) and the Crisis & Referral Protocol's scope-boundary check; reconciled against the existing schema rather than built as a separate base. Name fields split into First/Last (with a Full Name formula as primary) across all four person-holding tables (1-4) on 2026-07-31, since no real client data existed yet to disrupt."
tags:
---

# Covenant Identity — Airtable Schema Spec
*Field-level base structure for the two-tier intake system, now extended to cover ongoing session documentation. Both Tally Build Guides say "connect to Airtable" but neither specifies fields — this document is that missing layer. Build one Airtable base with the five tables below.*

**Who it's for:** Andrew, building the alpha-phase Airtable base by hand.
**What it is not:** An automation spec. See the Automation Notes at the end for what needs Make.com vs. what Airtable/Tally handle natively.

---

## Table 1 — Clients (master pipeline)
**Airtable tab name (not yet created):** "Clients" — the "(master pipeline)" label is this doc's own descriptor, not part of the tab name to type in Airtable.

One row per prospective or active client. This is the table you actually look at day to day; the two response tables feed it but are not where you track pipeline state.

| Field                          | Type                                     | Notes                                                                                                                                                                                                                                                                   |
| ------------------------------ | ---------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Full Name                      | Formula (primary field)                  | `{Last Name} & ", " & {First Name}` — leftmost/primary so every link reference elsewhere in the base (Tables 2-5's Client field, search, dropdowns) shows a readable full name rather than just a last name. Changed from a single "Client Name" text field 2026-07-31. |
| First Name                     | Single line text                         | Added 2026-07-31, split out of the former "Client Name" field                                                                                                                                                                                                           |
| Last Name                      | Single line text                         | Added 2026-07-31, split out of the former "Client Name" field — sortable, useful once caseload grows                                                                                                                                                                    |
| Email                          | Email                                    | Match key for linking response tables — unaffected by the name split, matching logic (including the Referral Flag automation) keys off Email, not name                                                                                                                  |
| Phone                          | Phone number                             |                                                                                                                                                                                                                                                                         |
| Status                         | Single select                            | Options: `Discovery Booked` → `Pre-Discovery Complete` → `Discovery Call Done` → `Go – Agreement Sent` → `Go – Tier 2 Sent` → `Active` → `Completing` → `Closed` → `No-Go / Referred`                                                                                   |
| Discovery Call Date            | Date                                     |                                                                                                                                                                                                                                                                         |
| Current Stage                  | Single select                            | `Discovery` / `Stage 1` / `Stage 2-3` / `Stage 4a` / `Stage 4b` / `Completed` — CIC diagnostic/coaching stage, tracked separately from `Status` above (which is pipeline/business state, not coaching-model stage). Added 2026-07-31 for Table 5.                       |
| Go/No-Go Decision              | Single select                            | `Go` / `No-Go` / `Pending`                                                                                                                                                                                                                                              |
| Go/No-Go Notes                 | Long text                                | Rationale against the 5 criteria in the Two-Tier Protocol                                                                                                                                                                                                               |
| Referral Flag                  | Checkbox                                 | Mid-engagement scope-boundary signal per the Crisis & Referral Protocol — distinct from `Go/No-Go Decision`, which is a pre-engagement gate. Set to true if any linked Table 5 record has its Scope Boundary Flag checked. Added 2026-07-31.                            |
| Payment Status                 | Single select                            | `Not Invoiced` / `Invoiced` / `Paid` / `Payment Plan Active` / `Refunded`. Check this is `Paid` or `Payment Plan Active` before manually sending Tier 2 — see the Payment Gate in the Two-Tier Intake Protocol.                                                         |
| Payment Plan Selected          | Single select                            | `Full ($1,680)` / `3-Month Plan ($560/mo)`                                                                                                                                                                                                                              |
| Amount Paid                    | Currency                                 |                                                                                                                                                                                                                                                                         |
| Payment Date                   | Date                                     | Date of most recent payment (full payment or latest installment)                                                                                                                                                                                                        |
| Emergency Contact Name         | Single line text                         | Mirrors Q19 once Tier 2 is submitted                                                                                                                                                                                                                                    |
| Emergency Contact Phone        | Phone number                             | Mirrors Q20                                                                                                                                                                                                                                                             |
| Emergency Contact Relationship | Single line text                         | Mirrors Q21                                                                                                                                                                                                                                                             |
| Current City/State             | Single line text                         | Mirrors Q22 — required before Session 1 for every client, remote or local                                                                                                                                                                                               |
| Pre-Discovery Response         | Link to record → Pre-Discovery Responses |                                                                                                                                                                                                                                                                         |
| Intake Response                | Link to record → Intake Responses        |                                                                                                                                                                                                                                                                         |
| Confirmed Goal                 | Long text                                | Client's own language, captured per Discovery Call Guide Movement 4. Added 2026-07-31.                                                                                                                                                                                  |
| Confirmed Task                 | Long text                                | Alliance task agreement, same source. Added 2026-07-31.                                                                                                                                                                                                                 |
| Next Session Date              | Date                                     | Added 2026-07-31.                                                                                                                                                                                                                                                       |
| Session Notes                  | Link to record → Session Notes (Table 5) | Added 2026-07-31.                                                                                                                                                                                                                                                       |
| Alpha Cohort                   | Checkbox                                 | Marks the first cohort of clients for tracking purposes (e.g., early feedback, first-cohort testimonials) — alpha clients pay the same rates as later cohorts as of 2026-07-08                                                                                          |
| Coach Notes                    | Long text                                | Free-form, not part of any client-facing document                                                                                                                                                                                                                       |

---

## Table 2 — Pre Discovery Repsonses (Tier 1)
**Airtable tab name:** "Pre Discovery Repsonses" — matches exactly, including the typo (not "Repsonses" → "Responses," not hyphenated, no "(Tier 1)" suffix in the actual tab). The "(Tier 1)" here is this doc's own clarifying label, not part of the literal Airtable name.

One row per Tally submission of the Pre-Discovery Screen. Field order matches the Tally Build Guide 1:1 so mapping during Tally→Airtable setup is mechanical.

| Field | Type | Source |
|---|---|---|
| Respondent Full Name | Formula (primary field) | `{Respondent First Name} & ", " & {Respondent Last Name}` — matches Table 1's pattern. Changed from a single "Respondent Name" field 2026-07-31. |
| Respondent First Name | Single line text | Tally's native split-name field type — requires rebuilding this form's Name question in Tally and remapping the Airtable integration |
| Respondent Last Name | Single line text | Same as above |
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
**Airtable tab name:** "Intake Responses (Tier 2)" — matches exactly, no change needed.

One row per Tally submission of the full Covenant Identity Intake. Includes the new Section G fields (Q19-22) added to the Tally Build Guide.

| Field | Type | Source |
|---|---|---|
| Respondent Full Name | Formula (primary field) | `{Respondent First Name} & ", " & {Respondent Last Name}` — matches Table 1's pattern. Changed from a single "Respondent Name" field 2026-07-31. |
| Respondent First Name | Single line text | Tally's native split-name field type — requires rebuilding this form's Name question in Tally and remapping the Airtable integration |
| Respondent Last Name | Single line text | Same as above |
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

## Table 4 — Alliance Pulse Responses
**Airtable tab name (not yet created):** "Alliance Pulse Responses" — matches the heading exactly, no separate label needed.

One row per Tally submission of the Alliance Pulse, sent after every session starting with the alpha cohort. See [[Covenant Identity — Alliance Pulse]] for pilot status, deployment timing, and rationale — this table exists to support that pilot and is not yet a permanent fixture of the base.

| Field | Type | Source |
|---|---|---|
| Respondent Full Name | Formula (primary field) | `{Respondent First Name} & ", " & {Respondent Last Name}` — matches Table 1's pattern. Changed from a single "Respondent Name" field 2026-07-31. |
| Respondent First Name | Single line text | Tally's native split-name field type — requires rebuilding this form's Name question in Tally and remapping the Airtable integration |
| Respondent Last Name | Single line text | Same as above |
| Submission Date | Date | Auto-populated by Tally |
| Session Number | Number | Coach fills in when sending the link — not client-reported, so it stays reliable if a submission comes in late or out of order |
| Bond Score | Number (1-5) | Item 1 |
| Task Score | Number (1-5) | Item 2 |
| Goal Score | Number (1-5) | Item 3 |
| Alliance Total | Formula (sum of Bond + Task + Goal) | Auto-calculated |
| Optional Note | Long text | Optional field, often blank |
| Client | Link to record → Clients | Match by email |

---

## Table 5 — Session Notes
**Airtable tab name (not yet created):** "Session Notes" — matches the heading exactly, no separate label needed.

One row per coaching session, linked to the client it belongs to. Unlike Tables 2-4, this table isn't fed by a Tally form via native integration — it's populated from raw session notes (pasted or dictated, via the Session Notes Capture Tally form → Make.com → Claude) plus fields the coach sets after reviewing. Table 1 now has the matching `Session Notes` link field pointing back here (added 2026-07-31).

| Field                   | Type                     | Notes                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| ----------------------- | ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Client                  | Link to record → Clients | Every session note attaches to a client                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Session Date            | Date                     | Sort/group views by this field for chronological order                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| Raw Notes               | Long text                | Pasted from Tally/dictation, unedited. **Access-control note (corrected 2026-07-31):** holds verbatim client disclosure. Airtable has no native field-level permission on *any* plan — access is base-level only (a collaborator either has a role on the whole base or doesn't); the only native workaround for hiding specific fields from specific people is a separate synced base that omits them. This is not a live risk for a solo account with no collaborators — the base password is the full access boundary and is sufficient as-is. It becomes relevant only if a collaborator is ever added (a VA, bookkeeper, or supervisor) who should see some fields but not this one. Two things that matter regardless of collaborators: never generate a public/shared view link for any view containing this field (shared links bypass login entirely), and treat any Make.com/API token connected to this base as a credential equal to the account password. |
| Key Themes              | Long text                | Claude-drafted from Raw Notes                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Affections Surfaced     | Long text                | Claude-drafted — what the client is prioritizing, trusting, or relying on this session                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| False Identity Named    | Long text                | Optional — only if surfaced this session                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Covenant Truth Spoken   | Long text                | Optional — only if spoken this session                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| Stage Worked            | Single select            | `Discovery` / `Stage 1` / `Stage 2-3` / `Stage 4a` / `Stage 4b` / `Completed` — coach-entered, not Claude-inferred                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| Stage 4b Route          | Single select            | `Route A – Relational` / `Route B – Body/Felt-Sense` / `N/A` — only populated when Stage Worked = Stage 4b; coach-entered. Route B is not yet field-tested in a live session, so early entries using it are also test data for whether the fork holds up in practice                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| Client Commitments      | Long text                | Claude-drafted from Raw Notes                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Coach Follow-up Actions | Long text                | Claude-drafted from Raw Notes                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Scope Boundary Flag     | Checkbox                 | Referral Signal present this session, per the Crisis & Referral Protocol                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Note Status             | Single select            | `Draft` / `Reviewed` — Draft until the coach has checked the Claude-generated fields and entered Stage Worked / Stage 4b Route                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Created                 | Created time             | Native Airtable field, auto-populated — basic audit trail independent of note content                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| Last Modified           | Last modified time       | Native Airtable field, auto-populated                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |

**Not built here:** a per-client session sequence number. Airtable's native Autonumber increments across the whole table, not per linked client, so it can't produce "session 1, 2, 3" per client — use the Session Date sort instead rather than building automation around a field that can't do what its name implies.

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

---

## Referral Flag Automation — Step-by-Step (Airtable Automations, not Make.com)

Purpose: when a Session Notes row's `Scope Boundary Flag` gets checked, the matching Clients row's `Referral Flag` should also flip to checked, so a scope-boundary signal is visible from the Clients table without having to open every linked session. This stays entirely inside Airtable, so it's built in the **Automations** tab of your base, not Make.com.

**Build steps:**

1. In your Airtable base, click **Automations** in the left sidebar → **Create automation**.
2. Name it something findable, e.g. "Scope Boundary → Referral Flag."
3. **Add trigger:**
   - Trigger type: **When a record matches conditions**
   - Table: **Session Notes**
   - Condition: `Scope Boundary Flag` **is** checked
4. **Add action:**
   - Action type: **Update record**
   - Table: **Clients**
   - Record to update: click into the "Record" field and insert the dynamic token for the **Client** field from your trigger step (Airtable shows a blue "+" or lightning-bolt icon to insert values from the triggering record — pick the linked Client record from there, not a typed value)
   - Field to update: `Referral Flag`
   - Set value: **checked**
5. Turn the automation **on** (top right toggle).
6. Test it: check `Scope Boundary Flag` on any existing Session Notes row and confirm the linked Clients row's `Referral Flag` flips to checked.

**Note:** this only sets the flag — it never unchecks it automatically. If a flag needs to be cleared (e.g., after individually reviewing a flagged case per the Retention Policy's disposal process), that's a manual, deliberate action in Airtable, not something to automate — the same reasoning as not auto-deleting flagged records.
