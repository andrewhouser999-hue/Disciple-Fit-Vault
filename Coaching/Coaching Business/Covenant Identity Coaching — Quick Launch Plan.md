---
created: 2026-07-30
basis: "[[Disciple Fit — Marketing Charter]] — buyer's journey stages, trust rules, segment targeting, and brand voice guardrails, all applied directly rather than re-derived; [[Branding & Core Competency]] (Word Within — CIC Messaging Architecture section) — positioning statement and draft homepage copy adapted back to the Covenant Identity Coaching name per Andrew's 2026-07-30 decision to launch under the existing name rather than the unfinished rename; [[Disciple Fit Coaching — Coaching Agreement]] — pricing and engagement terms; [[Covenant Identity — Two-Tier Intake Protocol]] — intake/payment sequence; [[Covenant Identity — Discovery Call Guide]] — call structure; [[Covenant Identity — Pre-Practice Readiness Action Plan]] and [[Covenant Identity — Methodology & Readiness Review for Clinical Consultation]] — safety-readiness gaps named but not resolved here, per Andrew's explicit instruction to set aside further practitioner education and a slower ramp-up for this specific plan. Updated 2026-08-07: Phase 0's Airtable row corrected per [[project_cic_airtable_notes_system]] — base build completed and fully verified 2026-08-03, removing the spreadsheet-workaround note. Updated 2026-08-24: added two Phase 0 rows — professional email (never provisioned; domain was bought for the credibility this row closes) and the Session Notes AI pipeline (spec'd 2026-08-23 per [[feedback_ai_client_data_deidentification]] and [[project_cic_airtable_notes_system]], not yet built live) — both previously unchecked by this plan. Added a Cost column the same day, correcting The Business Notes.md's Google Workspace figure ($7/yr is stale/wrong — Business Starter is ~$7.20/user/month, ~$86/yr) in the process; that source doc still needs the same fix. The email row's Cloudflare-vs-Google deliverability rationale is from the same day's conversation, not yet captured in any standalone doc."
tags:
  - marketing
  - launch-plan
  - covenant-identity-coaching
---

# Covenant Identity Coaching — Quick Launch Plan

*What this is: a sequenced, fast-path plan to get Covenant Identity Coaching in front of real prospects and into paid discovery calls using only what's already built in the vault — no new site build, no rebrand, no new research commissioned for this plan. Built at Andrew's request for a "quick launch" scenario, which explicitly set aside further practitioner education, a slower ramp-up, and open questions about market demand or product effectiveness as out of scope for this exercise.*

*What this is not: a resolution of the practice's pre-launch safety gaps. [[Covenant Identity — Methodology & Readiness Review for Clinical Consultation]] (built 2026-07-27) confirms zero live client sessions run to date, no confirmed scope-boundary clinical supervisor, no confirmed QPR (suicide-prevention gatekeeper) training completion, and no built referral network of outside therapists. Those are named once here, in the closing section, and not solved — they were set aside for this specific exercise on Andrew's direction, but they don't stop being real risks once an actual person is on the other end of a discovery call.*

---

## Decisions Locked for This Launch (2026-07-30)

- **Name:** Covenant Identity Coaching — not the "Word Within" rename explored in the Marketing Charter. That rename is still an open, unfinished exploration (leading candidate, not a decision); adopting it now would require a new domain and DNS work a quick launch can't absorb. The domain already owned, `covenantidentitycoaching.com`, matches the current name.
- **Tone:** Calm, unhurried, no urgency or scarcity mechanics — per the Marketing Charter's own trust research, which names pressure as a universal trust-killer for this specific audience. This overrides the scarcity framing ("five spots," "comment IN") in the first draft of the founding-cohort post; the rewritten version is in Phase 3 below.
- **Segment:** Sunday-Monday Christian — current Target Market per the Segment Registry. High-functioning, theologically literate, does not self-identify as broken, searches for growth/formation content rather than "help" content. Marketing must lead with the felt gap, never the diagnostic or theological root (the Charter's Governing Rule).

---

## Phase 0 — Confirm What's Actually Ready (1-2 days)

Everything below assumes these pieces work. Each is a five-minute check against the live system, not a rebuild — flag anything that fails the check before Phase 1 goes out.

| Asset                                                                                   | Status per vault                                                                                                                                                                  | Check before launch                                                                                                                                                  | Cost                                                                                                                                                                          |
| --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Coaching Agreement                                                                      | Signable, terms finalized 2026-07-28 ($1,680 / 12 sessions, or 3×$560)                                                                                                            | Ready — no action                                                                                                                                                    | $0                                                                                                                                                                            |
| Stripe Payment Link                                                                     | Referenced as built in the Two-Tier Intake Protocol                                                                                                                               | Confirm the link is live and the amount matches                                                                                                                      | $0 flat + 2.9% + $0.30/transaction                                                                                                                                           |
| Tier 1 Pre-Discovery Tally form                                                         | Build guide exists                                                                                                                                                                | Confirm it's actually built and fires from the Calendly confirmation email — if not, skip it for now and ask the Tier 1 questions live on the discovery call instead | $0 (Tally free tier)                                                                                                                                                          |
| Tier 2 Intake Tally form                                                                | Build guide exists                                                                                                                                                                | Same check — if not built, fall back to the Intake Addendum as a live Session 1 form                                                                                 | $0 (Tally free tier)                                                                                                                                                          |
| Calendly booking link                                                                   | Assumed live (Discovery Call Guide references it throughout)                                                                                                                      | Confirm the link works and triggers the right confirmation email                                                                                                     | $0 (free tier likely sufficient at alpha volume) — up to ~$144/yr if a paid tier is later needed                                                                             |
| Airtable base (5 tables: Clients, Pre-Discovery, Intake, Alliance Pulse, Session Notes) | Built and fully verified against the live base 2026-08-03, including the Referral Flag Automation                                                                                 | Ready — log clients directly in Airtable from first inbound reply, no spreadsheet workaround needed                                                                  | $0 (free tier)                                                                                                                                                                |
| `@covenantidentitycoaching.com` email                                                   | Not provisioned — Coaching Agreement and any outreach reply currently default to a personal Gmail                                                                                 | Set up Google Workspace before Phase 1 launches; see standalone setup guide                                                                                          | ~$86/yr (Google Workspace Business Starter, ~$7.20/mo) — recommended over the $0 Cloudflare Email Routing alternative given the DKIM/DMARC deliverability risk to pastor-referral outreach, discussed in-session 2026-08-24 |
| Session Notes AI pipeline (Tally → Make.com → Claude → Table 5)                         | De-identification spec added 2026-08-23 (Client Code field + Make.com lookup step, per [[feedback_ai_client_data_deidentification]]) — not yet built in the live base or Make.com | Build before Session 1, not after — Phase 4 has nowhere for notes to land otherwise                                                                                  | $0 (Make.com free tier likely sufficient at alpha volume) + Claude API usage, pay-per-token, negligible at low session volume                                               |

*Cost column added 2026-08-24 — figures are current-tier estimates, not locked contracts; re-check before relying on them for a formal budget.*

---

## Phase 1 — Landing Page, No Site Build (Day 1-2)

Point `covenantidentitycoaching.com` at a single page — Carrd, or a one-page Squarespace/Notion page, whichever Andrew can stand up fastest. Do not attempt a full site.

Reuse the homepage copy already drafted under the "Word Within" messaging work in Branding & Core Competency — it was written to the Marketing Charter's own voice rules (calm, precise, no exclamation points, diagnosis-before-declaration), so the substance doesn't need to be rewritten, only re-named:

> **HERO**
> *You know the truth. It hasn't reached where you live yet.*
>
> Covenant Identity Coaching is coaching for Christians who believe the right things about who they are in Christ and still feel ruled by the old ones — built to close that gap with precision, not repetition.
>
> **[ Book a Discovery Call ]**
>
> ---
>
> **THE GAP YOU ALREADY FEEL**
>
> You've read the verses. You've heard the sermons. You could recite who God says you are in Christ. And still — under pressure, in conflict, alone with your thoughts — you find yourself governed by an old story instead: not enough, not safe, not wanted, not able.
>
> That gap between what you know and what you feel isn't a failure of faith or effort. It's a sign the truth hasn't yet reached the place that actually runs your life.
>
> ---
>
> **DIAGNOSIS BEFORE DECLARATION**
>
> Truth spoken generically doesn't move what's stuck. This starts by locating exactly where the gap lives in you — which specific belief, tied to which specific pattern — before any truth is spoken into it.
>
> What follows isn't a program everyone runs through the same way. It's coaching built around your particular pattern: naming it precisely, meeting it with the specific covenant truth that answers it, and returning to that truth until it becomes what actually governs you — not just what you know.
>
> ---
>
> **COVENANT TRUTH, NOT SELF-HELP**
>
> The truth at the center of this work isn't a mood you're talked into or a mantra you repeat until it feels real. It's what Scripture actually says about who you are in Christ — spoken with precision, into the place it's needed, and returned to until it takes hold.
>
> This is coaching, not therapy, and not a substitute for your church community or your pastor's teaching — it's the one-on-one, diagnostic layer of formation neither is built to deliver.
>
> ---
>
> **WHAT I'M NOT PROMISING**
>
> - Not a quick fix — formation takes the time formation takes.
> - Not a replacement for your church or your pastor — a companion to both.
> - Not clinical treatment — if what you're carrying needs a therapist or physician, I'll tell you and help you find one.
> - Not a technique that works by effort alone — the Spirit does what only the Spirit can do. This creates the conditions.
>
> ---
>
> **START WITH A CONVERSATION**
>
> A discovery call is a conversation, not a pitch — we'll talk through what you're carrying and whether this is the right next step.
>
> **[ Book a Discovery Call ]**
>
> ---
>
> *"The word is very near you, in your mouth and in your heart." — Deuteronomy 30:14 (ESV)*

---

## Phase 2 — Outreach Sequence (Day 1 onward, runs parallel to Phase 1)

Per the Buyer's Journey in the Marketing Charter, this audience doesn't respond to being told they have a problem — they respond to being *seen* precisely, on their own terms, before anything is asked of them. Warm channels outperform cold ones for a quick launch regardless of audience, but they're especially load-bearing here because this segment actively distrusts generic Christian marketing.

1. **Personal outreach (Day 1).** Direct message or call to everyone in Andrew's existing network who is a plausible fit or a plausible referral source — not a mass blast, individual messages. Lead with recognition, not a pitch: describe the gap in a sentence or two the way the homepage does, then ask if it's familiar rather than announcing the offer immediately.
2. **Pastor referral sheet (Day 2-3).** One page, written to the "peer/referring pastor" translation already drafted in Branding & Core Competency: this is framed as a companion to the pulpit, not competition with it — the one-on-one diagnostic layer a sermon structurally can't deliver. Send to 5-10 pastors or ministry leaders Andrew already has some relationship with, not a cold list.
3. **Public post (Day 3+).** The rewritten founding-cohort post below. Goes out after 1-2 has already produced at least one or two live conversations, so it isn't the first thing prospects see — social proof from Phase 2, even a single "I talked to someone about this," makes the public post land as confirmation rather than a cold pitch.

---

## Phase 3 — The Post (Charter-compliant rewrite)

The original draft used a five-spot scarcity mechanic ("opening five spots," "comment IN") that reads as pressure under the Charter's own trust research for this audience. Rewritten to lead with recognition (Buyer's Journey Stage 2), name the felt gap before any root language, and drop the countdown:

> You know the truth about who you are in Christ. You could say it in your sleep.
>
> And still — under pressure, in an argument, alone with your thoughts at the end of a long day — you find yourself running on an older story instead: not enough, not safe, not able to keep up.
>
> That gap between what you know and what actually governs you in the moment isn't a lack of effort or a lack of faith. It's just what happens when truth hasn't yet reached the place that runs your life.
>
> I've spent the last year building a coaching process — Covenant Identity Coaching — for exactly that gap. Not more input, not another study. A diagnostic process that finds exactly where the old story is still operating, and meets it with the specific truth that actually answers it. Coaching, not therapy.
>
> I'm taking on a small number of founding clients right now, at a reduced rate, in exchange for their honest feedback as I refine the process. If that gap is something you recognize — in yourself, or in someone you know — reply here or send me a message and I'll walk you through what it looks like.

No spot count, no deadline, no exclamation points — consistent with the Charter's "calm, precise, unhurried" voice rule and its "pressure/urgency" trust-killer.

---

## Phase 4 — Discovery Call Through Close (ongoing from first inbound reply)

No new tools needed — run the existing pipeline exactly as documented:

1. Prospect books via Calendly → Tier 1 Pre-Discovery Screen fires automatically (or is asked live, per the Phase 0 check).
2. Discovery call runs per the Discovery Call Guide's five movements — including Movement 4's alliance-formation steps (individualize the task, reflect the client's own goal language back, get explicit confirmation).
3. Go/No-Go decision against the Two-Tier Intake Protocol's five criteria.
4. On Go: Coaching Agreement + Stripe Payment Link sent within 24 hours. Tier 2 Intake is sent only after the Payment Gate clears (signed agreement + payment received) — do not send it on a Go decision alone.
5. Session 1 begins once Tier 2 is complete, at least 48 hours out.

---

## Phase 5 — The Founding Rate (Andrew's decision, not a copywriting one)

Because scarcity/urgency framing is off the table, the founding rate should be offered as a quiet fact stated privately on the discovery call, not broadcast as a countdown in the post itself:

> "Since you'd be one of the first people through this process, I'd like to offer it to you at [X] instead of the standard $1,680, in exchange for your honest feedback as I refine it."

The actual discount amount is a margin decision Andrew needs to set — this plan intentionally doesn't guess at a number. A reasonable range to consider: enough of a discount to remove price as a hesitation for an otherwise-qualified prospect, not so steep that it undercuts the $1,680 anchor for the clients who come after the founding cohort.

---

## What This Plan Deliberately Does Not Solve

Per the Methodology & Readiness Review (2026-07-27): no live client sessions have been run to date, no scope-boundary clinical supervisor is confirmed, QPR training completion is unconfirmed, and no outside referral network is built. This plan gets prospects to a signed agreement and a paid Session 1 as fast as the existing assets allow — it does not close those readiness gaps, which was Andrew's explicit instruction for this exercise, but they remain the load-bearing risk the moment a real client is in the room.
