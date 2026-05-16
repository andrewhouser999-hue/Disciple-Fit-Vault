---
created: 
basis: TBD
tags:
---

# Covenant Identity Intake — Tally Build Guide
*Tier 2 of the two-tier intake system. Sent after the discovery call confirms fit — not before. For design rationale, diagnostic targets, and full annotations see: Covenant Identity Intake — Design Basis & Annotation.md*

*For the pre-discovery screen (Tier 1), see: Covenant Identity — Pre-Discovery Screen — Tally Build Guide.md*
*For when to send each tier, see: Covenant Identity — Two-Tier Intake Protocol.md*

---

## Before You Build

**Recommended Tally settings for this form:**
- Form type: **Multi-page** (not single scroll — sections must be distinct pages)
- Progress bar: **On** (reduces abandonment, signals the client they're moving through something structured)
- Required questions: **All questions required except Q13** (the open catch-all at the end is optional)
- Estimated completion time displayed on welcome page: **15-18 minutes**
- Responses: **Connect to Airtable** via native integration so intake data routes directly to your client management base
- Notifications: Set email notification to andrewhouser999@gmail.com on every new submission

---

## Welcome Page

**Title:**
`Covenant Identity Coaching — Getting to Know You`

**Body text:**
```
Before our first session together, I'd like to learn about where you are — not just what you're working on, but what's actually happening beneath the surface.

This form takes about 12-15 minutes to complete. There are no right answers. The goal is honesty, not presentation. Bring the real thing.

Your responses come directly to me and are held in complete confidence. I'll review them before we meet so we can go deeper from the first minute together.

— Andrew
```

**Button text:** `Begin`

---

## Section A — What's Happening Now

**Section title:** `What's Happening Now`
**Section description:** `Let's start with where you are.`

---

**Question 1**
- **Type:** Long Text (Paragraph)
- **Required:** Yes
- **Question text:**
```
What's happening in your life right now that made you reach out?

What are you most stuck in, frustrated by, or longing for? Take as much space as you need.
```
- **Placeholder text:** `Take as much space as you need.`

---

**Question 2**
- **Type:** Long Text (Paragraph)
- **Required:** Yes
- **Question text:**
```
How long has this been present — and how many times have you tried to address or change it?

Be as specific as you can.
```
- **Placeholder text:** `"About two years. I've tried three times to..."` *(optional — remove if it feels too guiding)*

---

## Section B — Your Story

**Section title:** `Your Story`
**Section description:** `A little about where you've been.`

---

**Question 3**
- **Type:** Long Text (Paragraph)
- **Required:** Yes
- **Question text:**
```
How would you describe the overall arc of your life so far?

Not a résumé — more like: what has the overall journey actually felt like? Has it felt like it's going somewhere, or more like you've been circling the same ground?
```

---

**Question 4**
- **Type:** Long Text (Paragraph)
- **Required:** Yes
- **Question text:**
```
Think back to when you were younger — childhood, adolescence.

What messages did you receive, spoken or unspoken, about who you were, whether you were enough, or what you had to do to be loved and accepted?
```

---

## Section C — Your Experience of God

**Section title:** `Your Experience of God`
**Section description:** `These questions are asking for what's real, not what's theologically correct.`

---

**Question 5**
- **Type:** Long Text (Paragraph)
- **Required:** Yes
- **Question text:**
```
Describe your relationship with God as it actually feels right now — not as you know it should be theologically, but what it genuinely feels like day to day.

Is God close or distant? Engaged or absent? Pleased, neutral, or disappointed?
```

---

**Question 6**
- **Type:** Long Text (Paragraph)
- **Required:** Yes
- **Question text:**
```
When you fail at something that matters to you — morally, relationally, in your work — what does your gut tell you about how God sees you in that moment?

(Not what you know the right answer is. What it actually feels like.)
```

---

**Question 7**
- **Type:** Long Text (Paragraph)
- **Required:** Yes
- **Question text:**
```
Have you ever brought anger, grief, confusion, or doubt directly to God — unfiltered?

What happened? Or if you haven't — what stops you?
```

---

## Section D — Your Identity

**Section title:** `Your Identity`
**Section description:** `Try to answer from the gut here, not from theology.`

---

**Question 8**
- **Type:** Long Text (Paragraph)
- **Required:** Yes
- **Question text:**
```
When you fail at something important, what does that mean about you as a person — not just about the thing that went wrong?

Try to answer from the gut, not from what you know is theologically true.
```

---

**Question 9**
- **Type:** Linear Scale
- **Required:** Yes
- **Question text:**
```
On a scale of 1 to 10, how much does what God says about who you are actually feel true in your lived experience?
```
- **Scale:** 1 to 10
- **Left label:** `I know it intellectually but it doesn't reach how I actually live`
- **Right label:** `It genuinely shapes how I experience myself and my life day to day`

---

**Question 10**
- **Type:** Long Text (Paragraph)
- **Required:** Yes
- **Question text:**
```
What do you most fear people would discover about you if they truly knew you?
```

---

## Section E — What You're Looking For

**Section title:** `What You're Looking For`
**Section description:** `Last section.`

---

**Question 11**
- **Type:** Long Text (Paragraph)
- **Required:** Yes
- **Question text:**
```
What's actually driving you to pursue coaching right now?

Try to go beneath the "good answer" — what's the real, honest thing that's making you reach out now rather than six months ago?
```

---

**Question 12**
- **Type:** Yes / No
- **Required:** Yes
- **Question text:**
```
Are you currently in active mental health treatment, processing significant trauma with a therapist, or experiencing clinical-level depression or anxiety that significantly impacts your daily functioning?
```

**Conditional logic — If answer is YES, show:**
- **Type:** Statement block (no response required)
- **Text:**
```
Thank you for sharing that. This matters.

I want to make sure you're receiving the right kind of support for where you are. This doesn't automatically mean coaching isn't right for you — sometimes coaching and therapy work well together. We'll talk through this in our discovery call before we proceed.
```

---

**Question 13**
- **Type:** Long Text (Paragraph)
- **Required:** No *(make this question optional)*
- **Question text:**
```
Is there anything else you want me to know before we meet?

Something the questions didn't touch, something that feels important to name, or something you're hoping I'll understand about where you are.
```
- **Add label above question:** `Optional`

---

## Section F — What You're Giving Your Energy To

**Section title:** `What You're Giving Your Energy To`
**Section description:** `A few more questions — answer from your gut, not your theology.`

---

**Question 14**
- **Type:** Long Text (Paragraph)
- **Required:** Yes
- **Question text:**
```
What would need to change for you to feel like your life is genuinely going well?

Not the spiritual answer — what condition, in your actual experience, would need to be true?
```

---

**Question 15**
- **Type:** Long Text (Paragraph)
- **Required:** Yes
- **Question text:**
```
When you're anxious, overwhelmed, or struggling — who or what do you turn to first?

Be honest. First reach, not ideal answer.
```

---

**Question 16**
- **Type:** Long Text (Paragraph)
- **Required:** Yes
- **Question text:**
```
What are you most afraid of losing right now?
```
- **Placeholder text:** `A person, a role, a sense of yourself, a situation — anything.`

---

**Question 17**
- **Type:** Long Text (Paragraph)
- **Required:** Yes
- **Question text:**
```
What do you feel like you depend on most to feel okay about yourself?

This might be a relationship, an achievement, a role, a sense of control, or something else entirely.
```

---

**Question 18**
- **Type:** Long Text (Paragraph)
- **Required:** Yes
- **Question text:**
```
If you had to simplify your life significantly — let go of most of what you're currently managing, doing, or holding — what would you give up last?
```

---

## Thank You Page

**Title:**
`Thank you.`

**Body text:**
```
It takes honesty to fill something like this out well. I appreciate you bringing the real thing.

I'll review your responses before we meet and come prepared.

If you haven't already scheduled your first session, you can do that here:
[Insert Calendly link]

I'm looking forward to the conversation.

— Andrew
```

---

## Tally Integration Settings

**Airtable integration:**
1. In Tally, go to Integrations → Airtable
2. Connect your Airtable account
3. Select the base and table where client intake data should live (recommend: create a dedicated "Intake Responses" table in your coaching base)
4. Map each Tally question to the corresponding Airtable field
5. Test with a sample submission before sending to clients

**Email notification:**
1. Go to Settings → Notifications
2. Add email: andrewhouser999@gmail.com
3. Set to notify on every new submission
4. Optional: customize the notification email subject line to include the respondent's name

**Form sharing:**
- Copy the Tally form link to include in Calendly confirmation emails (send automatically after booking)
- Or embed directly in website when ready
- Recommended: send via email 24-48 hours after the discovery call is booked, before the first session

---

## Verbal In-Session Follow-Up Areas

These are not scripted questions — they are diagnostic areas the coach enters in session 1 based on what the written form revealed. Select 2-3 per session.

| Area | Enter if form revealed... | Opening move |
|------|--------------------------|-------------|
| Schema origin | Q4 described conditional love, absence, or contradiction | "When you described [the early message] — when did you first know that about yourself?" |
| Immunity specifics | Q2 showed 3+ failed attempts at same pattern | "Walk me through what happened the last time you tried to change this. Where specifically did it break down?" |
| God-representation origin | Q5 described God as distant, disappointed, or absent | "When did God start feeling that way? Was there a time when it felt different?" |
| Lament capacity | Q7 showed "never" or "it felt wrong/dangerous" | "What do you imagine would happen if you brought the full, unfiltered thing to God — the anger, the grief? What's the worst-case version of how He'd respond?" |
| Shame content specifics | Q10 produced character-level content | "What does it feel like in your body when you imagine someone discovering that about you?" |
| Gap specificity | Q9 was 4-7 (moderate gap) | "Where in your life does the covenant truth feel most real? And where is the gap still the widest?" |
| Affections / dependency | Q15 named something other than God; Q17 named a condition, role, or relationship | "You mentioned that [X] is what you reach for first / depend on most. What do you think would happen to your sense of yourself if that were taken away?" |
| Affections / fear | Q16 revealed something held tightly | "When you imagine losing [X] — what does that feel like in your body? What does it say about who you'd be without it?" |
| Functional god specificity | Q14 named a condition that has nothing to do with God | "You said things would feel genuinely good if [condition]. What would it take for that to be true without [condition] being in place?" |

---
*See Covenant Identity Intake — Design Basis & Annotation.md for full diagnostic rationale and complete coach annotations.*
