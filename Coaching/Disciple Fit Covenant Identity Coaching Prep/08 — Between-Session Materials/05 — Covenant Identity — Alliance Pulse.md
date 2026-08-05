---
created: 2026-07-10
basis: "[[Covenant Identity — Formation Self-Assessment]] — administration cadence and 1-5 scale convention matched for instrument consistency, and named as the outcome side this instrument is read against; [[Covenant Identity — Airtable Schema Spec]] — Table 4 added to log responses; [[Covenant Identity — Post-Session Client Debrief Card]] — adjacent per-session touchpoint, distinguished in Section I; Bordin (1979) three-factor pantheoretical alliance model (Bond/Task/Goal) — theoretical structure only, not the copyrighted WAI/WAI-SR instrument, which is not used here due to clinical wording and licensing restrictions"
tags: [between-session, client-facing, alliance, pilot-instrument, phase-1, phase-2, phase-3, phase-4]
---

# Covenant Identity — Alliance Pulse

*Practitioner reference with embedded client-facing instrument. Three-item alliance check, completed independently after every session, all phases including Phase 1. Built as a pre-launch pilot instrument — see Pilot Status before treating this as a permanent fixture.*

---

## Section I — Practitioner Reference

### Pilot Status (read first)

This is not yet a permanent part of the CIC system documents — it is not in the System Document Master List, Document Reading Order, or Coaching Agreement. It is being tested with the alpha cohort to answer two questions before it's adopted permanently:

1. Do alpha clients actually complete a 3-item form after every session, or does response rate drop off partway through the engagement?
2. Does the alliance trajectory it produces show any relationship to the outcome trajectory already captured by the Formation Self-Assessment?

Add it to sessions going forward only — do not send a retroactive request for sessions an alpha client has already completed. If, after the first alpha client finishes a full 12-session engagement, response rate held up and the trend data was actually useful for a go/no-go read, promote it: add to the Engagement Onboarding Document, System Document Master List, and Document Reading Order Block 7.

### Why This Instrument, Not the WAI

The Working Alliance Inventory (Horvath & Greenberg) and its short form, the WAI-SR, are the standard psychometric instruments for alliance research, but two things rule out using them directly: they are copyrighted, and they are worded for clinical relationships ("counselor," "therapy") — using clinical-register language in a coaching engagement misstates CIC's non-clinical scope. What's retained here is Bordin's underlying three-factor account of alliance (Bond, Task, Goal) — that's the theory, not the instrument, and theory isn't copyrightable.

The trade-off, stated plainly: this instrument carries no published reliability or validity numbers of its own. It is a face-valid pulse check, not a validated psychometric tool. Treat its output as a directional trend signal for this pilot, not a clinical-grade score — and don't describe it to anyone outside this file as "the WAI" or "based on the WAI represented instrument," since it isn't.

### Deployment

**Every session, all phases, starting Session 1.** Unlike the Post-Session Client Debrief Card (which begins once Phase 2 opens), alliance tracking starts immediately — a weak alliance in Phase 1 is the highest-value signal to catch, because early rupture is exactly when a client is most likely to quietly disengage before any other feedback channel would surface it.

**Timing:** same day as the session, completed independently and not in front of the coach — self-report on the coaching relationship is more honest when the client isn't answering to the person being rated. Once Phase 2 begins, send the Tally link alongside (not merged into) the Post-Session Debrief Card, as a separate short form. In Phase 1, before the Debrief Card is in use, send the Alliance Pulse link on its own.

**How to frame it for the client:** "This isn't feedback on me as a person — it's three quick questions about whether our sessions are working the way they need to for you. Answer honestly; it helps me adjust before something that isn't working becomes a pattern."

### Tracking

A fourth table has been added to the existing intake Airtable base — see the updated [[Covenant Identity — Airtable Schema Spec]] for the field-level spec (Table 4 — Alliance Pulse Responses). One row per client per session, linked to the Clients table, with numeric Bond/Task/Goal fields and an auto-summed total. Sort by session number within a client's records to read the trend; there's no need to build a chart until the first alpha client has enough sessions logged to make one worth the effort — a sorted table view showing the numbers climb, flatten, or drop is enough to read for now.

**Tally build note:** three number-scale questions (1-5) matching the client-facing instrument below, plus one optional open-text field. Reuse the existing Tally→Airtable native integration already configured for the intake forms (see the Airtable Schema Spec's Automation Notes) — no new Make.com scenario needed. Match to the Clients table by email, same pattern as Tables 2 and 3. Session Number is filled in by the coach when sending the link, not client-reported, so it stays reliable even if a client submits late or out of order.

**What to do with a drop:** A single-session dip of one point isn't a signal — normal variation, especially after a heavy session. A drop that holds across two consecutive sessions, or one concentrated in a single factor (Goal falling while Bond and Task hold, for instance), is worth raising directly in the next session: "I noticed [factor] felt off recently — what's going on there for you?" Don't wait for the client to raise it; alliance ruptures that go unnamed are the ones that end in a client quietly not rebooking.

**Reading it against the Formation Self-Assessment:** Once a client has Alliance Pulse data across several sessions and at least two Formation Self-Assessment administrations (phase transitions), lay the two on the same session timeline. The question worth watching across the alpha cohort: does a client's Formation Self-Assessment movement — or lack of it — track with what the Alliance Pulse was already showing? If low alliance consistently precedes flat outcome scores, that's a leading indicator worth building a response protocol around later. If the two move independently, alliance may matter less to CIC's specific outcomes than general alliance research suggests for other modalities — that's also a real finding, not a failed pilot.

---

## Section II — Client-Facing Instrument

*Three quick questions about today's session. Takes under a minute. Same day, please — right after the session while it's fresh.*

**The scale:**

> **1** — Not at all
> **2** — A little
> **3** — Somewhat
> **4** — Mostly
> **5** — Completely

---

**1.** I felt understood and safe with my coach in today's session.
`1 — 2 — 3 — 4 — 5`

---

**2.** What we did in today's session felt like a useful way to spend our time toward what I'm working on.
`1 — 2 — 3 — 4 — 5`

---

**3.** My coach and I are working toward the same goal right now, and I could name what that goal is if asked.
`1 — 2 — 3 — 4 — 5`

---

*Optional — one sentence, only if something's on your mind:*

