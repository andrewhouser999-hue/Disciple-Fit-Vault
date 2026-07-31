---
created: 2026-07-31
basis: "design judgment — no binding external standard governs non-clinical coaching record retention (ICF confirms no ICF standard exists); policy below is built by analogy from adjacent-field evidence, cited in the Sources section. Cross-references [[Disciple Fit Coaching — Coaching Agreement]] Sections 7-8 and [[Covenant Identity — Crisis & Referral Protocol]]."
tags:
  - coaching-business
  - legal
  - data-policy
---

# Client Records Retention Policy
**Disciple Fit Coaching / Covenant Identity Coaching — Internal Policy**
*Governs how long client records are kept and when/how they may be deleted. Internal document — not client-facing. See the Coaching Agreement, Section 7, for what clients are told about record-keeping.*

---

## 1. Why This Policy Exists

Coaching Agreement Section 7 commits to maintaining growth documentation (Intake Addendum, Session Growth Notes, Mid-Engagement Snapshot, Growth Report), and the Airtable Schema Spec now stores structured session data in the Clients and Session Notes tables. Neither document specifies how long that data should be kept or when it should be deleted. Records get kept forever by default or deleted ad hoc without one — both are worse than a written, consistently-applied schedule: keeping everything forever creates unnecessary exposure if a base is ever compromised, and deleting inconsistently looks like evidence destruction if a dispute ever arises. This policy sets the schedule.

## 2. Scope

Applies to all client records generated through a Disciple Fit / Covenant Identity Coaching engagement, wherever stored:
- Airtable: Clients table, Session Notes table (Table 5), Pre-Discovery Responses, Intake Responses, Alliance Pulse Responses
- Growth documents referenced in Coaching Agreement Section 7 (Intake Addendum, Session Growth Notes, Mid-Engagement Snapshot, Growth Report), wherever they are drafted or stored (Google Docs, Airtable attachments, etc.)
- Any raw session notes, whether stored in Airtable's Raw Notes field or elsewhere

## 3. No Binding External Standard

There is no ICF requirement on record retention length — ICF's own ethics guidance directs coaches to their local/national law instead of an ICF standard, and no law currently requires this of Andrew as a non-clinical coach operating in Nebraska. This means the schedule below is a **design judgment**, not a legal or professional-body requirement. It is built by taking the closest analogous fields — clinical psychology record-keeping guidance, state statutory patterns for licensed health professionals, malpractice statute-of-limitations practice, and professional liability insurance industry norms — and adopting their point of convergence as a reasonable, defensible baseline. See Section 7 for the specific sources.

## 4. Retention Schedule

**Default — all client records:** retain 7 years after the client's last date of service (last completed session, or last contact if the engagement ended before session 1).

**Exception — Referral Flag or Scope Boundary Flag cases:** any client record where the Airtable `Referral Flag` (Clients table) or `Scope Boundary Flag` (Session Notes table) was ever checked is retained indefinitely, or at minimum is individually reviewed by Andrew before any deletion — never auto-deleted on the standard 7-year clock. This is the category of case most likely to resurface as a dispute or liability question years after the fact, per the sourced guidance in Section 7.

**Minors:** not currently applicable — Disciple Fit / CIC does not currently coach clients under 18. If that changes, add: retain until the client reaches age 18, plus the standard 7-year period from Section 4, whichever is later. Update this policy at that time rather than assuming the adult schedule applies.

## 5. Storage & Archival

Two-tier storage, split by engagement status, using tools already in the stack — no new software introduced:

**Tier 1 — Active (Status = Discovery through Active):** stays in the live operational Airtable base exactly as designed in the Airtable Schema Spec. This is the day-to-day working set.

**Tier 2 — Archive (Status = Completed, through the remainder of the 7-year retention window):** on each annual review (Section 8), export any client whose Status has moved to `Completed` out of the live base — a CSV export of their Airtable rows (native Airtable export, no added tool) plus their growth documents (already stored in Google Docs per the automation plan) — into a dedicated, access-restricted Google Drive folder, then remove the record from the live/operational base.

**Why split it:** a live base accumulating years of closed clients is unnecessary exposure — every closed record stays reachable by anything with base access, and it clutters the views used daily. Archiving out shrinks the blast radius of the system in active use.

**Why Google Drive specifically:** it's already part of the approved stack (growth documents are delivered through it today per the Freelance Automation & Kingdom Coaching Plan), consistent with that plan's own rule not to add tools before using the ones already in place. The archive folder must be restricted to Andrew's account only — no link-sharing, no team access — with 2FA enabled on the Google account holding it.

**Hard rule — this data does not touch the Obsidian vault.** The vault syncs to GitHub for backup, which is appropriate for coaching frameworks and prep material but not for client records in a Git-backed repository. This is the same reasoning that already put session notes in Airtable instead of Obsidian at the schema-design stage — the same exposure, recurring at the archive layer, and closed off the same way.

## 6. Disposal Process

- Deletion happens on the same scheduled annual review (Section 8), not ad hoc, and not triggered by a single record simply reaching 7 years while other related material stays.
- Before deleting a Clients record (from either tier), confirm no linked Session Notes record has Referral Flag / Scope Boundary Flag checked (Section 4 exception).
- Deletion is logged (date, client identifier only — not content) so there is a record that disposal followed this policy rather than occurring arbitrarily.
- Growth documents that belong to the client (Growth Report, Mid-Engagement Snapshot, per Coaching Agreement Section 7) may be deleted from Andrew's storage on the same schedule; the client's own copy is theirs to keep or discard.

## 7. Sources — Evidence Base for the 7-Year Default

These are analogous, not binding — no source here directly governs a non-clinical coach. Cited so the 7-year figure is traceable rather than asserted:

- ICF Code of Ethics / Insights and Considerations for Ethics — confirms no ICF-specific retention standard exists; coaches directed to local/national law instead
- APA Record Keeping Guidelines — psychologists (closest analogous licensed field) advised to retain full records 7 years after last date of service, or 3 years after a minor reaches majority, whichever is later
- State statutory patterns for licensed health professionals (e.g., CA, NC, TN, CT require 7 years) — not binding on coaching, but shows where legal baselines cluster when law does apply to an adjacent field
- General attorney/malpractice-exposure guidance — 7-10 years commonly recommended as a safe baseline for adult client files, keyed to state statutes of limitations for negligence claims
- Professional liability insurance industry norms — 5-7 years standard retention recommendation, up to 10, reflecting what carriers underwrite against

## 8. Review

Review this policy annually alongside the Coaching Agreement's own annual review (Section 12, "review annually"). Revisit sooner if Andrew adds a professional liability policy, pursues a coaching certification with its own retention standard (see the open trauma-certification decision), or begins coaching minors.

## 9. Open Items

- **Decided 2026-07-31:** the Coaching Agreement will not be updated to disclose the specific retention period. Current Section 7/8 language ("records are kept confidentially") stands as sufficient client-facing disclosure.
- Not yet built, left alone for now (2026-07-31): the actual scheduled-review process (e.g., an annual calendar reminder) to make Sections 5-6 happen rather than stay theoretical
