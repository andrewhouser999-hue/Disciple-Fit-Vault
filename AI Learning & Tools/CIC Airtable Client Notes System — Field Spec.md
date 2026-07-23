---
created: 2026-07-23
basis: "[[Freelance Automation & Kingdom Coaching Plan]] — Phase 1/2A revision; [[Covenant Identity — Diagnostic Lens Transition Logic]] — diagnostic sequence field mapping; [[Covenant Identity — Stage 4b Implicit Level Practitioner Reference]] — Route A/B fork; [[Covenant Identity — Crisis & Referral Protocol]] — scope boundary field"
tags:
---

# CIC Airtable Client Notes System — Field Spec

## Purpose

Defines the Airtable table structure for storing CIC/Disciple Fit client records and session notes. This replaces the earlier Phase 2A design in the Freelance Automation & Kingdom Coaching Plan, which routed session notes to Obsidian with no link back to the client's CRM record — a gap that would have made "show me everything for Client X" unresolvable as client count grew. Airtable's linked-table model (one Clients record, many linked Session Notes records) solves this directly.

**Status as of 2026-07-23:** This is a field-level spec only. The Airtable base has not yet been built. No Tally form fields have been defined yet for raw session-note capture. Build this once Phase 1 of the automation plan is underway.

## Design principle

Fields mirror CIC's own diagnostic sequence — affections discovered → false identity named → covenant truth spoken → stage worked — rather than importing clinical SOAP-note language. This keeps the record-keeping system consistent with CIC's non-clinical scope: it documents what happened in coaching terms, not clinical assessment terms.

Fields that require diagnostic judgment (Stage Worked, Stage 4b Route) are coach-entered, not Claude-generated. Claude drafts the descriptive summary fields (Key Themes, Affections Surfaced, etc.) from raw notes, but stage/route classification stays a human call — the same principle already in place for client-facing emails, which are always drafted for review, never auto-sent.

## Table 1 — Clients

| Field | Type | Notes |
|---|---|---|
| Client Name | Primary field | |
| Status | Single select | Prospect / Active / Paused / Completed |
| Intake Date | Date | Populated from Tally intake form |
| Discovery Call Date | Date | |
| Current Stage | Single select | Discovery / Stage 1 / Stage 2-3 / Stage 4a / Stage 4b / Completed |
| Confirmed Goal | Long text | Client's own language, captured per Discovery Call Guide Movement 4 |
| Confirmed Task | Long text | Alliance task agreement, same source |
| Referral Flag | Checkbox | Set to true if any linked Session Notes record has Scope Boundary Flag checked |
| Session Notes | Linked record | Links to Table 2, one client to many sessions |
| Next Session Date | Date | |

## Table 2 — Session Notes

| Field | Type | Notes |
|---|---|---|
| Client | Linked record | Links to Table 1 — every session note must be attached to a client record |
| Session Date | Date | |
| Session # | Autonumber or formula | Sequential count of sessions for the linked client |
| Raw Notes | Long text | Pasted from Tally form or dictated/emailed, unedited |
| Key Themes | Long text | Claude-generated summary from raw notes |
| Affections Surfaced | Long text | What the client is prioritizing, trusting, or relying on this session — Claude-drafted from raw notes |
| False Identity Named | Long text | Optional — only populated if a false identity was explicitly surfaced this session |
| Covenant Truth Spoken | Long text | Optional — only populated if covenant truth was spoken against the named false identity this session |
| Stage Worked | Single select | Same options as Clients.Current Stage — **coach-entered, not Claude-inferred** |
| Stage 4b Route | Single select | Route A – Relational / Route B – Body/Felt-Sense / N/A — only populated when Stage Worked = Stage 4b; **coach-entered, not Claude-inferred**. Note: Route B is not yet field-tested in a live session as of this writing, so early entries using it also function as test data for whether the fork holds up in practice, not just documentation. |
| Client Commitments | Long text | Claude-drafted from raw notes |
| Coach Follow-up Actions | Long text | Claude-drafted from raw notes |
| Scope Boundary Flag | Checkbox | Set if a Referral Signal was present this session, per the Crisis & Referral Protocol |
| Note Status | Single select | Draft / Reviewed — Draft until Andrew has checked the Claude-generated fields and entered Stage Worked / Stage 4b Route |

## Proposed automation flow (Make.com)

```
Raw session notes submitted (Tally form or forwarded email)
  → Make.com triggers
  → Claude API drafts: Key Themes, Affections Surfaced, False Identity Named,
    Covenant Truth Spoken, Client Commitments, Coach Follow-up Actions
  → New row created in Session Notes table, linked to the matching Clients record,
    Note Status set to "Draft"
  → Andrew reviews in Airtable, sets Stage Worked and Stage 4b Route (if applicable)
    and Scope Boundary Flag, changes Note Status to "Reviewed"
  → If Scope Boundary Flag is checked, Clients.Referral Flag updates to true
    (rollup or automation trigger)
```

## Open items

- Airtable base not yet created
- Tally form fields for raw note capture not yet defined
- Rollup/automation logic for Clients.Referral Flag not yet built in Make.com
- Once the base exists, confirm this doc against the actual field names/types used, since Airtable build decisions sometimes diverge from spec
