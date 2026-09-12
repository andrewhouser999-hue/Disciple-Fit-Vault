---
created: 2026-07-30
basis: "[[Disciple Fit — Marketing Charter]] — buyer's journey stages, trust rules, segment targeting, and brand voice guardrails, all applied directly rather than re-derived; [[Branding & Core Competency]] (Word Within — CIC Messaging Architecture section) — positioning statement and draft homepage copy adapted back to the Covenant Identity Coaching name per Andrew's 2026-07-30 decision to launch under the existing name rather than the unfinished rename; [[Disciple Fit Coaching — Coaching Agreement]] — pricing and engagement terms; [[Covenant Identity — Two-Tier Intake Protocol]] — intake/payment sequence; [[Covenant Identity — Discovery Call Guide]] — call structure; [[Covenant Identity — Pre-Practice Readiness Action Plan]] and [[Covenant Identity — Methodology & Readiness Review for Clinical Consultation]] — safety-readiness gaps named but not resolved here, per Andrew's explicit instruction to set aside further practitioner education and a slower ramp-up for this specific plan. Updated 2026-08-07: Phase 0's Airtable row corrected per [[project_cic_airtable_notes_system]] — base build completed and fully verified 2026-08-03, removing the spreadsheet-workaround note. Updated 2026-08-24: added two Phase 0 rows — professional email (never provisioned; domain was bought for the credibility this row closes) and the Session Notes AI pipeline (spec'd 2026-08-23 per [[feedback_ai_client_data_deidentification]] and [[project_cic_airtable_notes_system]], not yet built live) — both previously unchecked by this plan. Added a Cost column the same day, correcting The Business Notes.md's Google Workspace figure ($7/yr is stale/wrong — Business Starter is ~$7.20/user/month, ~$86/yr) in the process; that source doc still needs the same fix. The email row's Cloudflare-vs-Google deliverability rationale is from the same day's conversation, not yet captured in any standalone doc. Updated 2026-09-08: Stripe Payment Link row expanded after live build surfaced two real setup errors — a single combined link double-charges ($1,680 + $560/mo stacked, confirmed in Stripe's own checkout preview) rather than offering either/or, and the 3-Month Plan price has no built-in cycle cap in Andrew's Stripe account, so it will bill indefinitely ('until you cancel') unless manually stopped after the 3rd payment. Updated 2026-09-09: this plan's locked segment (Sunday-Monday Christian, set 2026-07-30) was stale against [[_Segment Index]]'s 2026-09-09 promotion of Wilderness Christian to Target Market — corrected throughout at Andrew's explicit direction. Phase 1 homepage copy replaced with [[Branding & Core Competency]]'s 'Wilderness Christian — Homepage Copy (Doorway Design)' section (including its pending-approval flag on the personal-story paragraph); Phase 2's pastor referral sheet replaced with a Facebook-groups tactic per [[Wilderness Christian]]'s own channel notes, which name pastoral referral as unreliable for this segment; Phase 3's post rewritten from Sunday-Monday's voice into Wilderness Christian's felt-cost doorway language. Updated 2026-09-12: re-synced Phase 1's doorway copy against Branding & Core Competency, which had independently diverged (4 of 8 doors and the 'Not Describing Eight Problems' section revised there 2026-09-10, not yet copied here); fixed a stale 'all four problems' leftover to 'all eight'; and swapped in Andrew's 2026-09-11 rewrite of the personal-story section (`My Story.md`'s 'Institutional Wounds, Compressed Working Draft'), included at his direction pending legal review — not yet cleared for live publish."
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
- **Segment:** Wilderness Christian — current Target Market per the Segment Registry (updated 2026-09-09; this plan originally launched against Sunday-Monday Christian on 2026-07-30, corrected here on 2026-09-09 to match the promotion). Primarily 45–65, sincere and spiritually serious, failed or wounded by the institutional church and still pursuing God privately; does **not** self-identify around the institutional wound — self-identifies as stuck, plateaued, not enough, disconnected, with an unlived calling or "is this it" ache underneath. Marketing must lead with the felt gap, never the diagnostic or theological root (the Charter's Governing Rule), and — per this segment's own profile, unlike Sunday-Monday Christian — must **not** route acquisition through pastoral or church-network referral; see the Phase 2 change below.

---

## Phase 0 — Confirm What's Actually Ready (1-2 days)

Everything below assumes these pieces work. Each is a five-minute check against the live system, not a rebuild — flag anything that fails the check before Phase 1 goes out.

| Asset                                                                                   | Status per vault                                                                                                                                                                  | Check before launch                                                                                                                                                  | Cost                                                                                                                                                                          |
| --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Coaching Agreement                                                                      | Signable, terms finalized 2026-07-28 ($1,680 / 12 sessions, or 3×$560)                                                                                                            | Ready — no action                                                                                                                                                    | $0                                                                                                                                                                            |
| Stripe Payment Link                                                                     | Two separate live links built 2026-09-08: Full Payment ($1,680 one-time) and 3-Month Plan ($560/mo). No automatic billing-cycle cap available in Andrew's Stripe account for the 3-Month Plan — bills indefinitely ("until you cancel") unless manually stopped. | **Standing manual task:** track each 3-Month Plan client's 3rd payment date (via Airtable `Payment Plan Selected` + `Payment Date`) and manually cancel their Stripe subscription once paid in full — nothing stops it automatically. | $0 flat + 2.9% + $0.30/transaction                                                                                                                                           |
| Tier 1 Pre-Discovery Tally form                                                         | Confirmed built and connected to Airtable as of 2026-09-08                                                                                                                        | Ready — no action                                                                                                                                                     | $0 (Tally free tier)                                                                                                                                                          |
| Tier 2 Intake Tally form                                                                | Confirmed built and connected to Airtable as of 2026-09-08                                                                                                                        | Ready — no action                                                                                                                                                     | $0 (Tally free tier)                                                                                                                                                          |
| Calendly booking link                                                                   | Live as of 2026-09-08. Free tier only — Workflows (automated post-booking emails) is paywalled (~$10-12/mo), so Tier 1 delivery is NOT automated via Calendly.                    | **Workaround adopted instead of upgrading:** the Carrd landing page presents the Tally Tier 1 link as a first step, then the Calendly booking button as a second step, framed sequentially — not automated delivery, but zero added cost. A static fallback note was also added directly on the Calendly event's description. | $0 (free tier) — revisit the ~$144/yr Standard upgrade only if prospects skip the sequenced landing-page step often enough to matter |
| Airtable base (5 tables: Clients, Pre-Discovery, Intake, Alliance Pulse, Session Notes) | Built and fully verified against the live base 2026-08-03, including the Referral Flag Automation                                                                                 | Ready — log clients directly in Airtable from first inbound reply, no spreadsheet workaround needed                                                                  | $0 (free tier)                                                                                                                                                                |
| `@covenantidentitycoaching.com` email                                                   | Fully provisioned and authenticated (MX/SPF/DKIM all confirmed) as of 2026-09-05                                                                                                  | Ready — no action                                                                                                                                                     | ~$86/yr (Google Workspace Business Starter, ~$7.20/mo) |
| Session Notes AI pipeline (Tally → Make.com → Claude → Table 5)                         | `Client Code` field built live in Airtable 2026-09-08. Tally form built but its Make.com webhook was never connected. Make.com scenario itself not built — deferred, running manually instead. | **Interim manual workflow adopted 2026-09-08:** coach pastes Client Code + Session Date + Raw Notes into Claude.ai chat by hand, copies the six drafted fields into Airtable, then does the same review pass. Automate later once volume justifies the Anthropic API cost (negligible, but requires a small prepaid balance). | $0 now; Claude API usage (pay-per-token, negligible) only once automated |

*Cost column added 2026-08-24 — figures are current-tier estimates, not locked contracts; re-check before relying on them for a formal budget.*

---

## Phase 1 — Landing Page, No Site Build (Day 1-2)

Point `covenantidentitycoaching.com` at a single page — Carrd, or a one-page Squarespace/Notion page, whichever Andrew can stand up fastest. Do not attempt a full site.

Reuse the homepage copy already drafted for this segment in Branding & Core Competency's "Wilderness Christian — Homepage Copy (Doorway Design)" section — it was built directly from Wilderness Christian's felt-cost leads and the Marketing Charter's Multi-Entry Recognition method, so it doesn't need rewriting, only publishing. **Updated 2026-09-12:** the copy below was re-synced against that source doc, which had diverged — 4 of the 8 doors and the "You're Not Describing Eight Problems" section were revised there on 2026-09-10 and hadn't yet been copied into this plan. The personal-story section ("I'm Not Asking You to Trust a Stranger With This") also now uses Andrew's 2026-09-11 rewrite, included in the build at his direction — **but it is pending legal review and not yet cleared for live publish.** Build and preview the Carrd site with this content, but do not actually publish it live until legal clears that section specifically.

> **HERO**
> *Still Pursuing God. Still Stuck. Still Not Sure Why.*
>
> This is for the Christian who never stopped believing — who's tried harder, prayed more, studied deeper — and is still stuck in the same place. You haven't walked away from God. You've kept showing up, kept believing, kept trying — and something in you still isn't moving. If any of that sounds familiar, you're not the only one, and there's a reason for it that isn't "you're not trying hard enough."
>
> **[ Find Your Starting Point ↓ ]**
>
> ---
>
> **FIND WHAT YOU RECOGNIZE**
>
> Everyone's version of "stuck" looks a little different. Pick whichever one sounds the most like you — there's no wrong door.
>
> **"You don't know who you are outside of what you do."** Take away the role, the title, the usefulness — and you genuinely don't know what's left. You're not sure you have a self underneath all of it.
>
> **"You can list your accomplishments. You can't say who you are underneath them."** Objectively thriving by every measure anyone can see, and privately unable to say who you are apart from the measures — which makes the success feel hollow instead of earned.
>
> **"You're surrounded by people and still feel completely alone."** You show up. You perform fine. But no one actually knows what's happening inside you — and you're not sure you know how to let them, or if it's even safe.
>
> **"You could disappear for a month before anyone actually noticed something was wrong."** Known by name, present for years, and still — if you quietly stopped showing up tomorrow, it would take longer than it should for anyone to notice something was actually wrong.
>
> **"You know what you believe. You just can't seem to live from it."** You've read the books, sat through the sermons, maybe even taught the class. The truth is in your head — clear, memorized, ready. Then Monday comes, or the pressure hits, and you react the same way you always have. It's not that you don't know enough. Something isn't translating.
>
> **"You've prayed this away more times than you can count. It keeps coming back."** The anxiety, the shame, the same tight-chest feeling — you've repented, you've prayed, you've claimed what's true. And your body hasn't gotten the message yet. That's not a sign your faith is thin.
>
> **"You're not walking away from God. You're just... flat."** No crisis, no dramatic doubt — just years at the same place. You do the things. Nothing moves. You've wondered if it's discipline, or sin, or something deeper, and none of those answers has actually explained it.
>
> **"Who you are at church and who you are the rest of the week are starting to feel like two different people."** You're not faking it on Sunday. But Monday runs on a different set of rules — sharper, more anxious, more self-protective — and you didn't consciously choose that split. It just runs.
>
> If you found yourself in more than one door — that's the norm here, not the exception. Keep reading.
>
> ---
>
> **YOU'RE NOT DESCRIBING EIGHT PROBLEMS**
>
> Whichever door you picked, here's what's actually true: underneath all eight is the same shape. An identity built on performance and role — because it was never safe enough to actually be known by anyone. That's not a knowledge problem; you already have real belief, real effort, real years invested. What's missing is what that belief needed in order to reach the rest of you: a self secure enough to receive it, formed in relationship, not performance.
>
> That's not a "try harder" problem. It's worth understanding why.
>
> ---
>
> **I'M NOT ASKING YOU TO TRUST A STRANGER WITH THIS** *(Rewritten by Andrew 2026-09-11 — pending legal review, not yet cleared for live publish; see note above)*
>
> Who gets themselves kicked out of church — and more than one, at that?
>
> My life changed in minutes. Jesus met me, and I surrendered everything — friends, old places, an old way of living — to follow Him. My faith was alive in a way I'd never known. Six months in, someone told me that now that I was a Christian, I should probably go to church. That sounded right, so I went.
>
> It didn't take long before something I couldn't quite name started happening. The same loyalty to Jesus that had changed my life kept running into friction with how the institution wanted to run. Small things at first — a role I was asked to perform in a way that went against my conscience. Then bigger ones: leadership that didn't want to be questioned, even respectfully, even in writing, even when I was the one who'd been asked to lead.
>
> I was marginalized. Then asked to leave. Then it happened again at the next church, and the one after that — four different congregations, four different versions of the same pattern: genuine service, a conscience issue, and then the door.
>
> By the third or fourth time, I stopped being surprised and started being something worse — quietly convinced the problem must be me.
>
> Then something shifted. I separated to focus on my growth in Christ, so that I could become who I was called to be — and possibly return one day to contribute to a body of believers I may live a formative life alongside.
>
> I've carried that for over a decade now. I still believe I need the Body of Christ, and I haven't found my way back yet. What I found instead was a way to actually work through the wound rather than just survive it — which is part of what became Covenant Identity Coaching.
>
> ---
>
> **WHAT WAS ACTUALLY IN THE WAY**
>
> Here's the pattern underneath all eight problems above: your identity — who you actually believe you are, at the level that runs your reactions — got shaped by something other than what God says about you. Maybe it was a community that let you down. Maybe it was years of proving your worth through performance. Maybe both. Either way, the truth you know intellectually and the identity that's actually running your life haven't been the same thing for a long time.
>
> That's not a discipline gap. It's an identity gap. And it's the thing Covenant Identity Coaching is built to close — not by teaching you more truth, but by finding exactly where the old story is still operating, and working there directly.
>
> ---
>
> **WHAT'S ON THE OTHER SIDE OF THIS**
>
> Closing the identity gap isn't the destination — it's what clears the way. On the other side of it is the thing you've probably stopped letting yourself want out loud: the calling you've sensed but haven't pursued, a life that actually adds up to something, the thing you keep almost building before something in you shuts it down.
>
> The healing work isn't instead of that. It's what makes it possible.
>
> ---
>
> **WHAT THIS IS NOT**
>
> - Not a replacement for the church — a companion to a faith that church, on its own, hasn't fully reached.
> - Not therapy or clinical treatment — if what you're carrying needs a therapist or physician, I'll say so and help you find one.
> - Not a technique or a formula — no verse, exercise, or declaration works by itself; this is a diagnostic, relational process, not a script.
> - Not fast, and not sold as fast — this took me years to work through myself; I won't pretend it's quicker for you.
> - Not a pitch dressed up as a conversation — a discovery call is a real conversation about whether this is the right next step, not a sales call with extra steps.
>
> ---
>
> **START WITH A CONVERSATION**
>
> If one or more of those doors sounded like your life, the next step isn't a program — it's a conversation. A discovery call is exactly that: we talk through what you're actually carrying, and whether this is the right fit. No pressure, no pitch.
>
> **[ Book a Discovery Call ]**
>
> ---
>
> *"The word is very near you, in your mouth and in your heart." — Deuteronomy 30:14 (ESV)*

---

## Phase 2 — Outreach Sequence (Day 1 onward, runs parallel to Phase 1)

Per the Buyer's Journey in the Marketing Charter, this audience doesn't respond to being told they have a problem — they respond to being *seen* precisely, on their own terms, before anything is asked of them. Warm channels outperform cold ones for a quick launch regardless of audience, but they're especially load-bearing here because this segment actively distrusts generic Christian marketing.

1. **Personal outreach (Day 1).** Direct message or call to everyone in Andrew's existing network who is a plausible fit or a plausible referral source — not a mass blast, individual messages. Lead with recognition, not a pitch: describe the gap using Wilderness Christian's own felt-cost language (stuck, plateaued, not enough, disconnected — one of the doorway lines from the homepage works well here), then ask if it's familiar rather than announcing the offer immediately.
2. **Facebook outreach (Day 2-3) — replaces the pastor referral sheet.** Wilderness Christian's own segment profile is explicit that pastoral referral is **not** a reliable channel here — this segment typically doesn't have, or deliberately holds at a distance, the church relationships a pastor referral sheet depends on; that tactic fit Sunday-Monday Christian, not this segment. The segment's own channel notes name Facebook as a viable companion channel instead for this 45–65 age band: faith-based groups, marriage/midlife groups, and church-adjacent communities where this audience is actually active. Post the Phase 3 recognition post (below) into 3-5 relevant groups Andrew has access to or can join, shared as a personal post, not an ad. **Word of mouth** — a direct ask to any past clients who resemble this profile for a referral — is the segment's other named channel and can run in parallel; it wasn't previously listed here because it applies regardless of segment.
3. **Public post (Day 3+).** The rewritten founding-cohort post below. Goes out after 1-2 has already produced at least one or two live conversations, so it isn't the first thing prospects see — social proof from Phase 2, even a single "I talked to someone about this," makes the public post land as confirmation rather than a cold pitch.

---

## Phase 3 — The Post (Charter-compliant rewrite)

The original draft used a five-spot scarcity mechanic ("opening five spots," "comment IN") that reads as pressure under the Charter's own trust research for this audience. Rewritten to lead with recognition (Buyer's Journey Stage 2), name the felt gap before any root language, and drop the countdown. **Rewritten a second time on 2026-09-09** — the version below had been written in Sunday-Monday Christian's voice ("you know the truth... in your sleep"); this one uses Wilderness Christian's own felt-cost doorways instead, per the segment correction above:

> Maybe you know exactly what you believe about God — and Monday still comes, and you're running on empty again, same as always.
>
> Maybe you've prayed the same anxiety away more times than you can count, and it keeps coming back, and some part of you has started to wonder what's wrong with your faith.
>
> Maybe you're not walking away from God. You're just flat. Have been for years. You do the things. Nothing moves.
>
> If any of that sounds like you — you're not the only one, and it's not a sign you're not trying hard enough.
>
> I've spent the last year building a coaching process — Covenant Identity Coaching — for exactly that kind of stuck. Not more input, not another study. A process that finds exactly what's actually in the way, and works there directly.
>
> I'm taking on a small number of founding clients right now, at a reduced rate, in exchange for their honest feedback as I refine the process. If any of this sounds familiar — in yourself, or in someone you know — reply here or send me a message and I'll walk you through what it looks like.

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
