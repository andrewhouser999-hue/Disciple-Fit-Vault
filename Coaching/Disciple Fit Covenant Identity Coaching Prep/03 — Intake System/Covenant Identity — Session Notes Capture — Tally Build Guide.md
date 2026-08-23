---
created: 2026-07-31
basis: "[[Freelance Automation & Kingdom Coaching Plan]] Phase 2A — workflow this form triggers; [[Covenant Identity — Airtable Schema Spec]] Table 5 — fields this form feeds; [[Disciple Fit Coaching — Coaching Agreement]] Section 7 — 24-hour Session Growth Notes commitment this form supports. Updated 2026-08-23: added a Make.com de-identification step ahead of the Claude API call, per Andrew's requirement that AI processing of session notes carry no client name, address, or email — a lookup translates the Tally-selected client to their `Client Code` (added to Airtable Schema Spec Table 1 the same day) before the Claude prompt is assembled, and Raw Notes itself must stay free of identifying detail, since that field is the one channel the lookup step can't scrub."
tags:
---

# Covenant Identity — Session Notes Capture — Tally Build Guide
*Coach-only capture tool — not client-facing. Andrew fills this out himself within 24 hours of each session (per Coaching Agreement Section 7), pasting or dictating raw notes. This form is the front door to the Phase 2A automation: Tally submission → Make.com → Claude API drafts the structured summary fields → new row created in Airtable Table 5 (Session Notes), linked to the client.*

*For the Airtable side of this pipeline, see: Covenant Identity — Airtable Schema Spec.md, Table 5.*

---

## Design Principles for This Form

**This is not a client-facing form.** No welcome copy, no reassurance language, no thank-you page content aimed at a client — this form is a personal capture tool. Keep it fast to fill out, not polished to read.

**Minimal fields, on purpose.** This form captures only what the coach knows in the moment: which client, what date, and what happened. Everything else Table 5 needs — Key Themes, Affections Surfaced, False Identity Named, Covenant Truth Spoken, Client Commitments, Coach Follow-up Actions — is Claude-drafted downstream from the Raw Notes field, not typed here. Stage Worked, Stage 4b Route, Scope Boundary Flag, and Note Status are set directly in Airtable afterward, since those are diagnostic judgment calls, not something this form or Claude should decide (see the Automation Plan's Phase 2A note on coach-entered fields).

**Completion time: 2-3 minutes to submit** (the actual writing of Raw Notes takes as long as it takes — this form doesn't rush that part).

---

## Before You Build

**Recommended Tally settings:**
- Form type: **Single page** (three questions, no need for multi-section)
- Progress bar: **Off** (not needed for a 3-question form)
- Required questions: **All required**
- Responses: **Do NOT use Tally's native Airtable integration for this form**, unlike the Pre-Discovery and Intake forms. Raw Notes has to pass through Claude via Make.com before it becomes a Table 5 row — connecting Tally directly to Airtable here would skip that step and write unprocessed notes straight in. Use a **Make.com webhook** trigger instead (Tally → Webhooks → connect the Make.com scenario's webhook URL).
- Notifications: none needed — Andrew is both the submitter and the recipient of this form

---

## Form Questions

**Question 1 — Client**
- **Type:** Dropdown
- **Required:** Yes
- **Question text:** `Which client is this session for?`
- **Options:** Ideally synced from the Airtable Clients table (Tally supports pulling choices from a connected data source) so this list stays current without manual editing. If Tally can't sync live from Airtable, maintain this dropdown by hand and update it when a new client reaches Active status.

**Question 2 — Session Date**
- **Type:** Date
- **Required:** Yes
- **Question text:** `Date of this session`
- **Default:** Today's date

**Question 3 — Raw Notes**
- **Type:** Long Text (Paragraph)
- **Required:** Yes
- **Question text:** `What happened this session?`
- **Placeholder text:** `Write freely — this is the raw material Claude will summarize into themes, commitments, and follow-up actions. Nothing here is client-facing.`

---

## Tally Integration Settings

**Make.com webhook (not native Airtable integration):**
1. In Make.com, create the Phase 2A scenario with a Webhooks trigger; copy its webhook URL
2. In Tally, go to Integrations → Webhooks, paste the Make.com webhook URL
3. Confirm the scenario's next steps: **Airtable search step** looks up the Clients record matching the Tally submission's client name → retrieves that record's `Client Code` (Table 1, added 2026-08-23) → **Claude API call is built using only the Client Code, Session Date, and Raw Notes** — the real name never enters the prompt, even though it's what you selected in the Tally dropdown → Claude drafts the summary fields → new row created in Table 5, linked to the matching Table 1 record (this link is set from the Airtable search step's own match, not from anything in the Claude response) → Note Status set to `Draft`

---

## De-Identification Before the Claude API Call

This form's own **Client** dropdown stays on real names, deliberately — you need to recognize who you're documenting in the moment, right after a session, and a code you'd have to look up would just be friction. The privacy boundary sits one step downstream, inside Make.com:

- **What Claude actually receives:** Client Code + Session Date + Raw Notes text. Nothing else — no name, no email, no address, no field pulled in "for context."
- **What you're responsible for:** Raw Notes is the one channel the Make.com lookup step can't scrub automatically, because it's free text you wrote. Never type the client's real name, a family member's name, their address, employer, or other identifying detail into Raw Notes — refer to them generically ("the client," "his wife") the same way you would in the summary fields Claude drafts back. If a detail slips in while dictating in the moment, catch it on the read-back before submitting, or in the Airtable review pass described below before marking the row `Reviewed`.
- **Also confirm in Tally's form settings:** this form does not have "Collect respondent email" or similar identity-capturing settings turned on — there's no reason submitter identity should ride along in the webhook payload Make.com receives, even though only Andrew ever submits this form.

**Form access:**
- Keep this form private — do not publish a public link. Access it directly (bookmark the edit/fill URL) or embed it in a personal shortcut, since it's for Andrew's use only, not shared with clients or the public.

---

## After Submitting — Finish the Record in Airtable

Submitting this form only creates a Draft row with the Claude-drafted fields filled in. Before the record is complete:

1. Review the Claude-generated Key Themes, Affections Surfaced, False Identity Named, Covenant Truth Spoken, Client Commitments, and Coach Follow-up Actions against what actually happened
2. Set **Stage Worked** and, if applicable, **Stage 4b Route**
3. Set **Scope Boundary Flag** if a Referral Signal was present this session
4. Change **Note Status** to `Reviewed`

This mirrors the same principle used everywhere else in this system: Claude drafts, the coach decides.
