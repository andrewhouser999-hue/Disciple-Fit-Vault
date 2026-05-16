---
created: 
basis: TBD
tags:
---

# Covenant Identity — Pre-Discovery Screen — Tally Build Guide
*Tier 1 of the two-tier intake system. Sent automatically when a discovery call is booked (via Calendly confirmation). Completed before the discovery call — not after. Gives the coach orientation before the conversation; gives the client a low-friction first encounter with the coaching frame.*

*For the full diagnostic intake (Tier 2), see: Covenant Identity Intake — Tally Build Guide.md*
*For when to send each tier, see: Covenant Identity — Two-Tier Intake Protocol.md*

---

## Design Principles for This Form

**This is not a diagnostic tool.** It is an orientation tool. It gives the coach enough to arrive at the discovery call with context, and it gives the client a first experience of a coaching relationship that takes them seriously. It does not probe schema origin, shame content, lament capacity, or deep God-representation — those are reserved for the Tier 2 intake, which comes after fit is confirmed.

**Keep the theological load light.** This form goes to clients who may not yet understand the Covenant Identity model. Language is plain, accessible, and does not assume theological vocabulary or readiness for identity-level work.

**Clinical screening is mandatory.** Even at this early stage, the coach must know whether clinical-level material is active. This is the first gate, not the last.

**Completion time: 5-7 minutes.** Friction must be low. This form is sent in the Calendly confirmation email — it competes with everything else a person does in the moment of booking. Eight questions maximum.

---

## Before You Build

**Recommended Tally settings:**
- Form type: **Multi-page** (4 short sections)
- Progress bar: **On**
- Required questions: **All required except Q8** (the open field is optional)
- Estimated completion time displayed on welcome page: **5-7 minutes**
- Responses: **Connect to Airtable** — same base as Tier 2 intake; create a separate "Pre-Discovery Responses" table
- Notifications: Set email notification to andrewhouser999@gmail.com on every new submission

---

## Welcome Page

**Title:**
`Before We Talk`

**Body text:**
```
Before our discovery call, I'd like to know a little about where you are.

This takes 5-7 minutes. There are no right answers. Just bring what's actually true.

Your responses come directly to me and are held in complete confidence.

— Andrew
```

**Button text:** `Begin`

---

## Section A — What's Going On

**Section title:** `What's Going On`
**Section description:** `Start with the real thing.`

---

**Question 1**
- **Type:** Long Text (Paragraph)
- **Required:** Yes
- **Question text:**
```
What's happening in your life right now that made you reach out?

What are you most stuck in, frustrated by, or hoping to change?
```

---

**Question 2**
- **Type:** Long Text (Paragraph)
- **Required:** Yes
- **Question text:**
```
How long has this been present — and have you tried to address it before?

If you've tried, what happened?
```

---

## Section B — A Little Context

**Section title:** `A Little Context`
**Section description:** `Just a few orienting questions.`

---

**Question 3**
- **Type:** Long Text (Paragraph)
- **Required:** Yes
- **Question text:**
```
How would you describe this season of your life?

Are you in a place of movement and momentum — or more like you're stuck, circling the same ground, or waiting for something to shift?
```
- **Placeholder text:** `A few sentences is enough.`

---

**Question 4**
- **Type:** Long Text (Paragraph)
- **Required:** Yes
- **Question text:**
```
How would you describe your relationship with God right now?

Not the theological answer — just what it actually feels like day to day.
```
- **Placeholder text:** `A sentence or two is fine.`

---

## Section C — What You're Looking For

**Section title:** `What You're Looking For`
**Section description:** `Two quick questions.`

---

**Question 5**
- **Type:** Linear Scale
- **Required:** Yes
- **Question text:**
```
On a scale of 1 to 10, how much does who you believe you are in Christ actually shape how you live day to day?
```
- **Scale:** 1 to 10
- **Left label:** `I know it intellectually but it doesn't reach my daily life`
- **Right label:** `It genuinely shapes how I experience myself every day`

---

**Question 6**
- **Type:** Long Text (Paragraph)
- **Required:** Yes
- **Question text:**
```
What's actually driving you to pursue coaching right now?

Not the presentable version — what's the real thing making you reach out now rather than waiting?
```

---

## Section D — A Few Quick Checks

**Section title:** `Almost Done`
**Section description:** `One important question, then an optional one.`

---

**Question 7**
- **Type:** Yes / No
- **Required:** Yes
- **Question text:**
```
Are you currently working with a therapist or mental health provider, or experiencing clinical-level depression or anxiety that significantly affects your daily functioning?
```

**Conditional logic — If answer is YES, show:**
- **Type:** Statement block (no response required)
- **Text:**
```
Thank you for sharing that.

This doesn't automatically mean coaching isn't right for you — coaching and therapy can work well together in the right conditions. We'll talk through this in our discovery call before anything moves forward.
```

---

**Question 8**
- **Type:** Long Text (Paragraph)
- **Required:** No
- **Add label above question:** `Optional`
- **Question text:**
```
Is there anything else you'd like me to know before we talk?
```

---

## Thank You Page

**Title:**
`See you soon.`

**Body text:**
```
Thank you for taking a few minutes with this.

I'll review your responses before our call so we can make the most of our time together.

If you have any questions before we meet, you can reach me at [contact email].

— Andrew
```

---

## Tally Integration Settings

**Airtable integration:**
1. In Tally, go to Integrations → Airtable
2. Connect your Airtable account
3. Select the same coaching base as your Tier 2 intake — create a separate **"Pre-Discovery Responses"** table (do not merge with the full intake table)
4. Map each question to the corresponding Airtable field
5. Include a field for discovery call date (populated manually after the call) so responses are linked to the engagement timeline

**Email notification:**
1. Go to Settings → Notifications
2. Add email: andrewhouser999@gmail.com
3. Set to notify on every new submission
4. Customize subject line to include respondent's name: e.g., `Pre-Discovery Screen — [Name]`

**Form sharing:**
- Embed the form link in the Calendly confirmation email so it fires automatically when a discovery call is booked
- Set a 24-hour reminder in Calendly that re-sends the link if the form hasn't been completed
- Do NOT send this form after the discovery call — it is a pre-call tool only

---

## Coach Review — Before the Discovery Call

Read the completed form within 24 hours of receiving it. Note:

| What to read for | Where it shows |
|---|---|
| Ratio of external vs. internal attribution in presenting problem | Q1 |
| Duration + verb used to describe attempts ("tried" vs. "prayed about" vs. "worked on") | Q2 |
| Season description — movement vs. circling — agency language present or absent | Q3 |
| God-relationship tone — flat/formulaic vs. textured and honest; close vs. distant | Q4 |
| Identity gap score — low (1-3), moderate (4-6), higher (7-9), aspirational (10) | Q5 |
| Motivation quality — intrinsic/identified vs. introjected/external; precipitating event | Q6 |
| Clinical flag — if YES on Q7, prepare the discernment conversation | Q7 |
| What they chose to bring when given total freedom | Q8 |

**This review is preparation, not diagnosis.** You are orienting your listening for the discovery call — not forming clinical conclusions. Hold your initial read loosely; the discovery call conversation may shift it entirely.

**Affections Layer — Read Across All Responses:**
After completing the table above, read the form once more through the affections diagnostic lens. Ask: *What is this person depending on — and where is God absent from it?*

- Q1 and Q3: What are they emotionally orbiting? What are they not mentioning?
- Q4: Is God present in the functional texture of their day, or described abstractly and at a distance?
- Q6: What's driving the urgency — what are they afraid of losing or needing to fix?
- Q8: What did they bring when given total freedom? What does that choice reveal about priority?

Note your initial affections read before the call. Carry it as a listening frame — do not lead with it in conversation.

---

*Tier 2 intake (Covenant Identity Intake — Tally Build Guide.md) is sent only after the discovery call confirms fit. See the Two-Tier Intake Protocol for the go/no-go decision criteria.*
