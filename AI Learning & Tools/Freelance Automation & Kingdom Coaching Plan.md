# Freelance Automation & Kingdom Coaching Plan

---

## Now the Path Makes Sense — Mostly

Given that goal, the core direction is correct. Here's the honest breakdown of what actually matters.

---

### What's Solid

**Make.com is the right starting point over n8n.** — *Strong inference*

For a non-technical person going after freelance clients, Make.com wins early on:
- Faster to get your first workflow working
- Better documentation for beginners
- Most small business clients won't host their own server (n8n requires that for free use)
- More tutorials, more templates, more Stack Overflow equivalent answers

Learn n8n later when a client specifically needs it or you hit Make.com's pricing ceiling.

**The freelance market for this is real.** — *Fact*

Small businesses are drowning in manual repetitive tasks. Lead follow-up, invoice generation, social posting, CRM updates, client onboarding sequences. They don't have engineers. They don't want to learn software. They will pay someone $500-$2,000 to set it up once and leave it running. This is a legitimate income path.

---

### What Will Actually Determine If You Succeed

**You don't need 35 tools. You need 8.** — *Strong inference*

Master these and you can handle 80% of real freelance automation jobs:

| Category | Tool |
|---|---|
| Workflow platform | Make.com (primary), n8n (secondary) |
| LLM | Claude or OpenAI API — pick one, learn it deeply |
| CRM/data | Airtable or Google Sheets |
| Email | Gmail API or SMTP |
| Forms/triggers | Typeform or Tally |
| Docs | Google Docs API |
| Payments | Stripe webhooks |
| Comms | Slack or Telegram |

Everything else is a variation on these patterns.

**The real skill gap isn't tools — it's scoping client work.** — *Opinion/estimate, but strongly held*

Most people who learn automation fail at freelancing not because they can't build workflows, but because they can't:
- Identify which of a client's problems is actually worth automating
- Scope a project so it doesn't creep into 3x the original work
- Explain what they built so the client trusts it and refers others

The course will teach you none of this. You have to deliberately practice it.

---

### The Honest Ceiling

**Pure no-code automation freelancing has a real income ceiling.** — *Strong inference*

One-time setup projects ($500-$2k) are the bread and butter, but they don't recur unless you add a maintenance/retainer model. The people who break past $5-8k/month reliably either:
- Specialize in one vertical (e.g., automations only for real estate agents, or only for e-commerce)
- Add light coding (Python scripts, API integrations that no-code can't handle)
- Package it as a productized service rather than custom project work

If your goal is to supplement income or add leverage to a current role, none of this is a problem. If you're trying to replace a full-time income, plan for this ceiling from the start.

---

### Revised Learning Path for Your Actual Goal

**Phase 1 — Get one workflow live (weeks 1-3)**
Make.com + Airtable + one real use case you actually need. Don't learn in the abstract. Build something for yourself first.

**Phase 2 — Add AI integration (weeks 4-6)**
Connect Claude or OpenAI API into a Make.com workflow. Email classification, auto-drafting replies, summarizing documents. These are the jobs clients actually ask for.

**Phase 3 — Learn to find and close a client (weeks 7-8)**
Not a tool skill — a business skill. Pick one niche. Build a before/after demo for a problem that niche has. Show it, don't pitch it.

**Phase 4 — Add JSON/webhooks literacy**
Not full coding. Just enough to understand what's happening when two systems talk to each other. This unblocks 80% of "why isn't this working" moments.

---

### Verdict on the Careerist Course: Fixable as a Starting Point

It will get you oriented. It will not get you clients. Use it to learn the tools, but treat it as scaffolding you'll outgrow in 60 days, not a complete education. The course's value is in forcing you to actually touch the tools — its liability is creating the illusion that tool knowledge equals a freelance business.

**The gap the course won't fill:** niche selection, client scoping, and packaging your service. That work is yours to do, and it's more important than any individual tool you learn.

---

---

## This Changes Everything (In a Good Way)

You're not just learning automation — you're building the operational backbone of your own coaching practice while developing a sellable skill. That's double return on the same investment. And you already have two pieces of the stack: Claude for intelligence, Obsidian for knowledge. Build around what you have.

---

### Your Stack (Revised for Kingdom Coaching)

| Layer | Tool | Why |
|---|---|---|
| Workflow engine | Make.com | Start here. Fastest path to live automations |
| AI brain | Claude API | You already use it. Stay in one ecosystem |
| Knowledge base | Obsidian | Your notes become inputs to automations |
| Client CRM | Airtable | Spreadsheet-like but automation-ready |
| Forms/intake | Tally.so | Free, clean, connects to Make.com easily |
| Email | Gmail | Good enough to start |
| Scheduling | Calendly | Triggers workflows on booking |
| Docs/deliverables | Google Docs | Claude writes into them via API |
| Payments | Stripe | Triggers onboarding workflows |

Do not add tools beyond this list until you've built something real with each one.

---

### Phase 1 — Build Your Own Coaching Intake System (Weeks 1-3)

**What you're learning:** Make.com fundamentals, Airtable, webhooks, form triggers

**The workflow to build:**

```
Tally intake form submitted
  → Make.com receives webhook
  → New row created in Airtable (client CRM)
  → Welcome email sent via Gmail
  → Calendly scheduling link included in email
```

**Why this one first:** You need it. Every coaching client goes through intake. Right now you probably do this manually. Automating your own business is the fastest way to learn because the feedback is real.

**Skills this develops:**
- Understanding triggers vs. actions (the core mental model of all automation)
- Webhooks (how systems talk to each other in real time)
- Airtable data structure (fields, records, views)
- Make.com scenario builder

**Obsidian connection:** Install the Local REST API plugin in Obsidian. This lets Make.com read and write your notes. You won't use it yet — but install it now.

**Deliverable:** A live intake form that automatically creates a client record and sends a welcome email without you touching anything.

---

### Phase 2 — Add Claude Into Your Workflow (Weeks 4-6)

**What you're learning:** Claude API (HTTP module in Make.com), prompt engineering for repeatable tasks, Obsidian automation

**Three workflows to build:**

**2A — Session notes → structured summary → Obsidian**
```
You paste raw session notes into a Tally form (or email yourself)
  → Make.com triggers
  → Claude API: "Turn these coaching notes into:
     1) Key themes 2) Client commitments 3) My follow-up actions"
  → Formatted note written to Obsidian via REST API
  → Follow-up email drafted to client via Gmail drafts
```

**2B — Inquiry email → Claude draft response**
```
New email tagged "coaching inquiry" in Gmail
  → Make.com trigger
  → Claude API: draft a warm, on-brand response based on your voice
  → Saved as Gmail draft (you review and send — never auto-send client replies)
```

**2C — Content repurposing (your highest-leverage workflow)**
```
You write one reflection, journal entry, or teaching note in Obsidian
  → Make.com reads the note (via REST API)
  → Claude API: reformat as LinkedIn post + email newsletter intro + 3 social captions
  → Google Doc created with all four versions
```

**Why 2C matters most:** Content is how Kingdom Coaching grows. This workflow means one piece of writing becomes four distribution-ready pieces with one trigger. You stop being the bottleneck.

**Skills this develops:**
- Claude API via Make.com's HTTP module (no code required)
- System prompts and prompt structure for consistent output
- Obsidian ↔ Make.com data flow
- Building workflows where *you* are the quality gate, not the labor

---

### Phase 3 — Build a Client Journey System (Weeks 7-9)

**What you're learning:** Multi-step sequences, conditional logic, Stripe triggers, delivering value through automation

**The full onboarding workflow:**
```
Stripe payment received (new coaching client)
  → Make.com trigger
  → Airtable: client record updated to "Active"
  → Google Doc created from template: personalized coaching agreement
  → Welcome sequence email #1 sent immediately
  → Email #2 scheduled: Day 3 (what to expect)
  → Email #3 scheduled: Day 7 (pre-session prep questions)
  → Calendly link for first session in email #1
```

**The offboarding/testimonial workflow:**
```
Airtable: client status changed to "Completing"
  → Email sent: reflection questions + testimonial request
  → 7 days later: follow-up if no testimonial submitted
  → Testimonial submitted → saved to Airtable + Obsidian "Social Proof" note
```

**Skills this develops:**
- Conditional routing (if/else logic in workflows)
- Scheduled/delayed actions
- Template-based document generation
- Building sequences that run without you — for weeks

**The marketability turn:** At this point you can demonstrate a complete client system: intake → payment → onboarding → session support → offboarding → testimonial. That's what other coaches will pay you to build for them.

---

### Phase 4 — Understand What's Actually Happening (Weeks 10-12)

**What you're learning:** JSON, HTTP requests, reading API docs, light troubleshooting

This phase is not about new tools. It's about not being helpless when something breaks.

**What to learn specifically:**
- JSON structure — key/value pairs, arrays, nested objects. Make.com's data inspector shows you raw JSON. Learn to read it.
- What a GET vs. POST request is. You use both constantly without knowing it.
- How to read an API doc enough to find the endpoint you need
- Make.com error logs — what common errors mean and how to fix them

**Practical exercise:** Pick any API from a tool you already use (Airtable, Calendly, or Claude). Use Make.com's HTTP module to make a raw API call to it — without a pre-built connector. Just you, the API docs, and the HTTP module. Do this once. It will demystify everything.

**You don't need to code.** You need to understand the shape of data well enough to not be blocked by it.

---

### The Kingdom Coaching Marketability Play

By Phase 3 you can legitimately say:

> *"I build automated client systems for coaches — intake, onboarding, content, and follow-up — using Make.com and Claude."*

That's a specific, credible, demonstrable offer. Other coaches will pay $800-$2,000 for a system like what you built for yourself. Your proof of concept is your own practice.

**The niche pitch:** Don't market yourself as a generic automation freelancer. Market to coaches, specifically faith-based or Christian coaches, because you understand the culture, the language, and the actual work. Niche authority always outcompetes broad skill in freelance.

---

### What to Do Before Phase 1

1. Create a Make.com free account
2. Create an Airtable free account
3. Create a Tally.so free account
4. Install Obsidian's Local REST API plugin
5. Get Claude API access (console.anthropic.com) — you'll need an API key, separate from Claude.ai

None of this costs money to start. Make.com free tier handles everything in Phase 1 and most of Phase 2.

---

### Verdict: Solid — with one watch item

The path is coherent. You have real use cases, a real business to test on, and existing tools to build from. The watch item: **don't let learning become a substitute for shipping.** The trap is taking courses, watching tutorials, and building demo workflows forever without ever showing it to a potential client or using it in your real coaching practice. Phase 1's workflow should be live and handling real intake within 3 weeks. If it isn't, that's the signal to course-correct.
