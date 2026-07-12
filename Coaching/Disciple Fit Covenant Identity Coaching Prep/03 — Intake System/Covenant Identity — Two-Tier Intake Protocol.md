---
created: 
basis: "TBD (original); updated 2026-07-11 to add a Vision-Led branch to Go/No-Go Criterion 1 — see [[Covenant Identity — Diagnostic Lens Transition Logic]], Entry Fork addendum"
tags:
---

# Covenant Identity — Two-Tier Intake Protocol
*Governs when each intake tier is sent, what each is for, and the go/no-go decision gate between them. This document is the operational bridge between the two intake forms.*

---

## The Two-Tier System at a Glance

| | Tier 1 — Pre-Discovery Screen | Tier 2 — Covenant Identity Intake |
|---|---|---|
| **File** | Covenant Identity — Pre-Discovery Screen — Tally Build Guide.md | Covenant Identity Intake — Tally Build Guide.md |
| **When sent** | Automatically, when discovery call is booked | Manually, after discovery call confirms fit |
| **Trigger** | Calendly confirmation email | Coach sends within 24 hours of discovery call |
| **Completion time** | 5-7 minutes | 12-15 minutes |
| **Question depth** | Surface — presenting problem, season, God-relationship (light), identity gap scale, motivation, clinical screen | Full — schema origin, God-at-failure, lament capacity, failure meaning, shame content, deep motivation |
| **Theological load** | Light — no model vocabulary required | Full — assumes readiness for covenant identity framing |
| **Purpose** | Pre-conversation orientation for coach; low-friction first encounter for client | Diagnostic baseline for the full engagement |
| **Audience** | Any potential client — model fit not yet confirmed | Clients who have confirmed fit and agreed to the engagement |

---

## The Sequence

```
Client books discovery call
        ↓
Tier 1 Pre-Discovery Screen sent automatically (Calendly confirmation email)
        ↓
Client completes Tier 1 (5-7 min)
        ↓
Coach reviews Tier 1 before discovery call
        ↓
Discovery call (30-45 min)
        ↓
Go/No-Go Decision (see criteria below)
        ↓
        ├── NO-GO → Graceful close or referral
        │
        └── GO → Coaching Agreement + Stripe Payment Link sent within 24 hours
                        ↓
                Client signs agreement and completes payment
                (full $1,680, or first $560 installment on a payment plan)
                        ↓
                Tier 2 Covenant Identity Intake sent
                        ↓
                Client completes Tier 2 (12-15 min) — at least 48 hours before Session 1
                        ↓
                Coach reviews Tier 2 → Session 1
```

---

## Payment Gate (GO path only)

**Added 2026-07-08 — alpha clients are paying clients, not free/beta.**

Tier 2 is not sent on a Go decision alone. It is sent only after both of the following are true:

1. **Coaching Agreement signed** — terms per `Disciple Fit Coaching — Coaching Agreement.md` Sections 3–4 (12 sessions, $140/session, $1,680 full engagement fee, full-pay or 3-month installment plan).
2. **Payment received** — full $1,680, or the first $560 installment if the client chose the payment plan. Check the Clients record's `Payment Status` field in Airtable (Paid or Payment Plan Active) before manually sending Tier 2.

This mirrors the logic already in Coaching Agreement Section 4: the $145 intake component is non-refundable once the intake form is submitted, which only makes sense if payment precedes submission. Sending Tier 2 before payment clears inverts that logic and creates a collections problem instead of a payment gate.

**If payment doesn't clear within a reasonable window after the agreement is sent** (e.g., 3-5 days with no response), follow up once. If it still doesn't clear, the engagement does not proceed — do not send Tier 2 on the assumption payment is forthcoming.

---

## Go/No-Go Decision Gate

**Send Tier 2 only when ALL five criteria are met after the discovery call.**

This is not a gut call. Work through each criterion before deciding.

---

**Criterion 1 — Change Readiness**
Client demonstrated at minimum *Contemplation* stage readiness: they are aware of the gap between who they are declared to be in Christ and how they actually live, and they are willing to look at it honestly.

*Pre-contemplation signal* (not ready for Tier 2): Client attributes the problem entirely to external factors; cannot name any internal pattern; shows no curiosity about why the same issues keep recurring.

*Contemplation or higher* (ready): Client names an internal dimension to the problem, even tentatively. Shows emotional weight around the question of who they actually are vs. who they want to be.

*Vision-Led signal* (also ready — added 2026-07-11): Client names no presenting problem but demonstrates a specific, felt desire to grow deeper — not vague self-improvement language, but something with actual weight behind it. Willingness to be diagnosed is present. This is not a Pre-Contemplation signal; it is a different entry point into the same readiness requirement. Cross-check against the Lateral Reroute Signal in [[Covenant Identity — Diagnostic Lens Transition Logic]] before confirming — compulsive, KPI-tracked "growth" is a different, Wound-Led picture wearing this one's clothes.

---

**Criterion 2 — Clinical Clearance**
One of the following is true:
- Client answered NO on Q7 (no active mental health treatment, no clinical-level depression/anxiety)
- Client answered YES, AND: (a) they are stable in their current therapeutic work, (b) the therapy and coaching agendas are distinct, and (c) the therapist is aware of and open to coaching

*Not cleared* (do not send Tier 2 yet): Client is in active trauma destabilization, in crisis, or the therapy and coaching agendas overlap significantly. Pause and address referral coordination first.

---

**Criterion 3 — Model Understanding**
Client understood and accepted that this coaching works at the identity level — not just behavior modification or goal achievement. They know the engagement will ask them to look at the gap between declared covenant identity and lived experience.

*Not met*: Client is looking for accountability, productivity, or goal-setting help and showed no interest in the identity-level framing when it was introduced. This is a wrong-fit signal, not a timing issue.

---

**Criterion 4 — Engagement Commitment**
Client confirmed willingness to commit to the full engagement structure (session count, between-session work, the pace of formation rather than quick fixes). They are not looking for one or two sessions.

*Not met*: Client wants to "try a few sessions and see." Do not proceed to Tier 2 — this framing is incompatible with the model. Address the commitment question directly before advancing.

---

**Criterion 5 — Faith Framework Alignment**
The coaching is explicitly Christian and Scripture-grounded. The client is a Christian, is comfortable with that framing, and did not express significant resistance to the theological architecture of the engagement.

*Not met*: Client is not a Christian, holds a significantly different theological framework, or expressed that the faith dimension would be a barrier. This is a referral to a more appropriate model, not a coaching issue to overcome.

---

## If Any Criterion Is Not Met

Do not send Tier 2. Choose one of the following:

**Option A — Graceful no-fit close:**
"Based on our conversation, I want to be honest with you: I don't think this particular model is what you need right now. What I'm hearing is [specific reason]. What I'd suggest instead is [referral / alternative resource]."

**Option B — Pause and address the block:**
If the criterion is a timing issue (not currently stable, needs to resolve an immediate crisis, just entered therapy), hold the engagement open with a specific check-in date: "Let's reconnect in [timeframe] once [specific condition] is resolved."

**Option C — Educate and re-assess:**
If the client didn't understand the identity-level framing, take one more conversation to explain it before deciding. But only once — repeated explanations are a wrong-fit signal.

---

## What Each Tier Does NOT Do

**Tier 1 does not:**
- Replace the discovery call conversation
- Give the coach enough to run Session 1
- Probe schema origin, lament capacity, shame content, or deep God-representation
- Function as a diagnostic baseline (that's Tier 2)

**Tier 2 does not:**
- Replace the discovery call (which happens before it)
- Replace Session 1 verbal intake (Part B of the Intake Addendum)
- Provide clinical assessment — it is a coach-facing diagnostic orientation tool
- Give the client their diagnosis — coach-internal observations never become client-facing labels

---

## Important: What Happens to Tier 1 Responses

Tier 1 responses route to Airtable ("Pre-Discovery Responses" table) and are held separately from the Tier 2 intake data. They serve the discovery call preparation only.

After Tier 2 is completed and the Intake Addendum is begun, Tier 1 responses serve as supplementary context — specifically, note any significant differences between what the client described in Tier 1 and what they described in Tier 2. Discrepancies between the pre-discovery screen and the full intake are diagnostically meaningful: they may indicate the client was more guarded before the relationship was established, or that the discovery call conversation shifted their self-understanding.

---

*Related documents:*
- *Tier 1 form: Covenant Identity — Pre-Discovery Screen — Tally Build Guide.md*
- *Tier 2 form: Covenant Identity Intake — Tally Build Guide.md*
- *Full design rationale: Covenant Identity Intake — Design Basis & Annotation.md*
- *Coach annotation key: Covenant Identity Intake — Coach Annotation Reference.md*
