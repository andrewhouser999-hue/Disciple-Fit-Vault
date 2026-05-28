---
created: 2026-05-28
basis: primary-source
tags:
---

# Relationship Performance — Prompt Library

**Practice:** Relational Performance Advisory (secular organizational consulting)

A record of all saved prompts, triggers, and purposes for the Relational Performance Advisory service.

> When you update a prompt, update Obsidian first, then propagate to the other two:
> - `.claude/commands/*.md` → `/slash command` in Claude Code
> - AutoHotkey script → `;trigger` anywhere on Windows

---

## Command Index

| Command | Claude Code | AutoHotkey | Purpose |
| ------- | ----------- | ---------- | ------- |
| Workplace Dysregulation Research | — | — | Produce sourced empirical brief on dysregulating environments; basis for engagement rationale, sponsor comms, framework dev |
| SDT — Theory, Workplace Application & Limits | — | — | Establish what SDT is, how it applies at work, and where it fails to resolve psychological safety on its own |

---

## Workplace Dysregulation Research Prompt

**When to use:**
- Building or updating engagement rationale for a new client
- Grounding a sponsor debrief in peer-reviewed evidence
- Developing new RPA training or facilitation material
- Responding to a sponsor or stakeholder who wants the evidence base
- Extending the [[A001 — Evidence Base & Case Rationale]] with deeper source-level detail

**Generated output:** [[Workplace Dysregulation — Empirical Base Case & Solution Framework]]

```
You are a research synthesizer with expertise in organizational psychology,
neuroscience, and trauma-informed systems. Produce a comprehensive,
source-grounded research brief on the following:

RESEARCH BRIEF: Dysregulating Work Environments — Base Case & Solution Framework

---

PART 1: THE BASE CASE — What the Evidence Shows

1. Neurobiological mechanism of workplace threat response
   - Explain Porges' Polyvagal Theory and how it governs employee
     "neuroception" of safety vs. threat in organizational contexts.
   - Explain what Siegel's "window of tolerance" means for day-to-day
     functioning under chronic organizational stress.
   - Cite van der Kolk's work on how chronic threat states affect
     cognitive and relational performance (not just clinical populations).

2. Psychological safety — the empirical case
   - Summarize Amy Edmondson's research program on psychological safety
     (1999 through 2018), including effect sizes and outcome variables.
   - Summarize Google's Project Aristotle (2015): methodology, findings,
     and why psychological safety ranked above all other team factors.
   - What distinguishes "psychologically unsafe" environments from
     merely "high pressure" ones? Cite behavioral markers.

3. Basic psychological needs — the SDT evidence base
   - Summarize Deci & Ryan's Self-Determination Theory applied to
     workplace contexts (cite Gagné & Deci, 2005, Journal of
     Organizational Behavior, and subsequent meta-analyses).
   - Distinguish need satisfaction vs. need frustration — cite
     Vansteenkiste et al. on why frustration is not merely the
     absence of satisfaction but produces active harm.
   - Map the three needs (autonomy, competence, relatedness) to
     observable organizational behaviors that signal need frustration.

4. Social pain as real pain
   - Summarize Lieberman's work and Eisenberger's 2003 fMRI study
     (Science) demonstrating that social exclusion activates the
     same neural substrates as physical pain.
   - What does this mean for dismissive management, exclusion from
     decision-making, or public shaming in workplace contexts?

5. David Rock's SCARF model — threat/reward in organizations
   - Explain the five SCARF domains (Status, Certainty, Autonomy,
     Relatedness, Fairness) and their neurological basis.
   - Identify which organizational practices most commonly trigger
     SCARF threat responses and what measurable outcomes follow.

6. Burnout as systemic dysregulation
   - Summarize Maslach's three-factor burnout model and its
     organizational (not individual) causes.
   - Summarize Bakker & Demerouti's Job Demands-Resources model
     (2007) — what is the resource-depletion pathway and what
     does empirical research show about the point of irreversibility?

---

PART 2: THE SOLUTION FRAMEWORK — Evidence-Based Interventions

For each intervention listed below, provide: (a) the underlying mechanism,
(b) the evidence base (study type, sample, outcomes), (c) what specifically
changes in the organization or employee, and (d) limitations or conditions
required for the intervention to work.

1. Psychological safety interventions (Edmondson's team-level protocols)
2. Autonomy-supportive management (SDT-aligned practices; cite meta-analyses)
3. Trauma-informed organizational frameworks (Bloom's Sanctuary Model;
   SAMHSA's 6 principles of trauma-informed care — TIP 57, 2014)
4. Somatic/regulation approaches — what do Porges, Levine, and van der
   Kolk each say about restoring regulatory capacity in adults whose
   nervous systems have been chronically activated?
5. MBSR and mindfulness-based interventions — Kabat-Zinn; RCT outcomes;
   what specific dysregulation markers improve?
6. Motivational Interviewing (Miller & Rollnick) — what does the evidence
   say about using MI-informed approaches with employees who have developed
   defensive adaptations to dysregulating environments?
7. Kegan & Lahey's Immunity to Change framework — how does it address the
   systemic resistance that dysregulated organizations display even when
   they want to change?

---

PART 3: SYNTHESIS — Converging Claims

1. What do neuroscience, attachment theory, SDT, and organizational
   psychology agree on as the non-negotiable conditions for a
   regulatory work environment?
2. Where do the frameworks diverge or have unresolved tensions?
3. What does the evidence say about the sequence of interventions —
   what must come first before other changes become possible?
4. What are the three most empirically robust claims in this entire
   body of literature — findings that have replicated across
   populations, methodologies, and cultural contexts?

---

FORMATTING REQUIREMENTS:
- Cite author, title, journal/publisher, and year for every empirical claim.
- Distinguish between: (a) meta-analyses and systematic reviews,
  (b) RCTs, (c) longitudinal observational studies, (d) cross-sectional
  studies, and (e) theoretical/clinical frameworks.
- Flag any claim that rests primarily on a single study or a
  non-replicated finding.
- Do not pad with general statements — every paragraph should advance
  a specific, citable claim or resolve a specific question.
```

**Evidence anchors:**

| Source | Domain | Evidence Level |
|---|---|---|
| Porges (2011) — *The Polyvagal Theory* | Neurobiological safety/threat mechanism | Neurophysiological framework |
| Siegel (1999, 2010) — *The Developing Mind*, *Mindsight* | Window of tolerance | Theoretical/clinical |
| van der Kolk (2014) — *The Body Keeps the Score* | Chronic threat and cognitive impairment | Clinical research + neuroimaging |
| Edmondson (1999, 2018) | Psychological safety | Multi-decade empirical program |
| Frazier et al. (2017) — *Personnel Psychology* | Psychological safety meta-analysis | Meta-analysis, N > 22,000 |
| Google Project Aristotle (2015) | Psychological safety at scale | Large observational (N=180 teams) |
| Gagné & Deci (2005) — *J. Organizational Behavior* | SDT at work | Landmark synthesis |
| Van den Broeck et al. (2016) — *J. Management* | SDT needs meta-analysis | Meta-analysis, N > 36,000 |
| Vansteenkiste & Ryan (2013) | Need frustration vs. satisfaction | Theoretical refinement |
| Eisenberger et al. (2003) — *Science* | Social pain neuroimaging | fMRI, extensively replicated |
| Rock (2008, 2009) — SCARF | Threat/reward in organizations | Applied neuroscience framework |
| Maslach, Schaufeli & Leiter (2001) | Burnout model | Annual Review synthesis |
| Bakker & Demerouti (2007) | Job Demands-Resources | Meta-analytically supported |
| Bloom (2013) — Sanctuary Model | Trauma-informed org change | Program evaluation |
| SAMHSA TIP 57 (2014) | 6 principles of trauma-informed care | Federal synthesis |
| Deci, Connell & Ryan (1989) | Autonomy-supportive management | RCT (Fortune 500) |
| Kabat-Zinn; Hülsheger et al. (2013) | MBSR at work | RCT + meta-analysis |
| Miller & Rollnick (2013); Lundahl et al. (2010) | Motivational Interviewing | >1,000 clinical trials |
| Kegan & Lahey (2009) | Immunity to Change | Theoretical/program evaluation |

---

## SDT — Theory, Workplace Application & Limits

**When to use:**
- Building the theoretical foundation for an RPA engagement rationale
- Explaining to a sponsor why motivation-focused interventions alone are insufficient
- Identifying where an existing workplace program (e.g., autonomy-supportive management training) will hit a ceiling without psychological safety infrastructure
- Grounding the RPA model's multi-framework architecture in evidence

```
You are a research synthesizer with expertise in organizational psychology,
motivation science, and team dynamics. Produce a precise, source-grounded
research brief on Self-Determination Theory — what it is, how it applies
in organizational contexts, and where it demonstrably falls short as a
standalone framework for resolving psychological safety.

RESEARCH BRIEF: SDT — Theory, Workplace Application, and the Psychological
Safety Gap

---

PART 1: WHAT SDT IS

1. Core theory — Deci & Ryan
   - State the foundational claim: human beings have three basic
     psychological needs (autonomy, competence, relatedness). Define
     each precisely as Deci & Ryan define them — not colloquially.
   - Explain the motivation continuum: amotivation → external regulation
     → introjection → identification → integration → intrinsic motivation.
     What distinguishes controlled motivation from autonomous motivation,
     and why does the distinction matter for behavior and well-being?
   - Explain need satisfaction vs. need frustration (Vansteenkiste & Ryan,
     2013) — why is frustration not merely the absence of satisfaction,
     and what does active need frustration produce?
   - Cite the primary sources: Deci & Ryan (1985, 2000); Ryan & Deci
     (2017 — Self-Determination Theory: Basic Psychological Needs in
     Motivation, Development, and Wellness).

2. Evidence base for SDT as a general theory
   - What is the scope of the empirical support? Cite the scale of the
     research program (number of studies, decades, domains).
   - What are the three most replicated findings across populations
     and cultural contexts?
   - Flag any domains where SDT's cross-cultural generalizability
     has been contested.

---

PART 2: SDT APPLIED TO THE WORKPLACE

1. The organizational application — what changes
   - Summarize Gagné & Deci (2005, Journal of Organizational Behavior)
     as the landmark translation of SDT to work contexts. What were
     the key claims and what evidence supported them at the time?
   - What does "autonomy-supportive management" mean behaviorally?
     Cite Deci, Connell & Ryan (1989) — the Fortune 500 RCT — and
     explain what managers were trained to do differently and what
     outcomes were measured.
   - How does SDT predict the outcomes of need satisfaction at work?
     Map each of the three needs to the organizational outcomes the
     research links to them (engagement, performance, retention,
     well-being). Cite specific studies.

2. Meta-analytic evidence
   - Summarize Van den Broeck et al. (2016, Journal of Management)
     — the large-scale SDT needs meta-analysis (N > 36,000). What
     did it confirm, qualify, or complicate?
   - Summarize Slemp et al. (2018) or equivalent meta-analysis on
     autonomy-supportive leadership. What effect sizes were found
     and on which outcomes?
   - What do the meta-analyses say about which need — autonomy,
     competence, or relatedness — has the strongest and most
     consistent effects at work?

3. Where SDT-based interventions have demonstrated workplace results
   - Identify two or three organizational intervention studies (RCT
     or quasi-experimental) where SDT-grounded practices produced
     measurable improvements. Report what changed, in whom, and
     over what timeframe.

---

PART 3: WHERE SDT FALLS SHORT ON PSYCHOLOGICAL SAFETY

This is the critical section. The goal is to establish precisely where
SDT's explanatory and intervention reach ends — and why a separate
psychological safety framework is not redundant but necessary.

1. Define psychological safety as a distinct construct
   - State Edmondson's (1999) definition precisely: psychological safety
     as a "shared belief held by members of a team that the team is safe
     for interpersonal risk-taking." Why is this a team-level, not
     individual-level, construct?
   - Distinguish psychological safety from: (a) trust, (b) cohesion,
     (c) job satisfaction, (d) autonomy as SDT defines it. These are
     related but not equivalent — what makes each distinction matter?

2. What SDT does not explain or predict
   - SDT's "relatedness" need is defined as feeling connected and cared
     for. Explain why relatedness satisfaction does not guarantee
     psychological safety — a person can feel they belong while still
     fearing that speaking up will damage their standing. Cite any
     research that demonstrates this gap directly.
   - SDT's "autonomy" need concerns the internal locus of causality for
     one's motivation — it is not the same as behavioral freedom to
     dissent, challenge authority, or voice unpopular observations. Where
     has this conflation appeared in organizational practice, and what
     does the evidence say about the limits of autonomy-supportive
     management in producing candor?
   - SDT predicts engagement and well-being through need satisfaction.
     But Edmondson's research shows psychological safety predicts
     learning behaviors and team performance through a different pathway
     — perceived interpersonal risk. Are there studies or datasets where
     these two frameworks diverge in their predictions? Describe what
     the divergence looks like.

3. The power and hierarchy problem
   - SDT research on autonomy-supportive management focuses on the
     manager-employee dyad. What does it say — or fail to say — about
     group-level silencing, peer pressure to conform, or status
     hierarchies within teams?
   - Edmondson's research identifies leader behavior as necessary but
     not sufficient for psychological safety — team norms and perceived
     consequences matter independently. Where does SDT's framework
     address or fail to address these group dynamics?

4. The threat-state problem
   - SDT operates primarily within the assumption that basic needs are
     frustrated or satisfied at a moderate level. What happens when an
     employee is operating in a chronic threat state — Porges' dorsal
     vagal shutdown or sympathetic activation? Does SDT have a framework
     for this, or does it assume a baseline regulatory capacity that
     may not exist in dysregulating environments?
   - If an employee is neurobiologically dysregulated (van der Kolk;
     Siegel's window of tolerance), does autonomy-supportive management
     reach them? What does the evidence say about the sequencing
     problem — what must be restored before SDT-aligned interventions
     become effective?

5. Empirical evidence of the gap
   - Are there studies that have measured both SDT constructs (need
     satisfaction, autonomous motivation) and psychological safety in
     the same sample? What do they find about the relationship —
     correlated, independent, or interactive?
   - Cite any research showing that high need satisfaction coexists
     with low psychological safety, or vice versa, demonstrating
     that they are not the same thing.

---

PART 4: SYNTHESIS — What This Means for Practice

1. What SDT contributes that psychological safety frameworks do not
   — and vice versa. These are complementary, not competing.
2. What sequence of intervention does the evidence suggest? If an
   organization has neither need satisfaction nor psychological safety,
   which do you address first, and why?
3. What is the single most important practical implication of the gap
   between SDT and psychological safety for an organizational consultant
   who is designing an engagement?

---

FORMATTING REQUIREMENTS:
- Cite author, title, journal/publisher, and year for every empirical claim.
- Distinguish between: (a) meta-analyses and systematic reviews,
  (b) RCTs, (c) longitudinal observational studies, (d) cross-sectional
  studies, and (e) theoretical/clinical frameworks.
- Flag any claim that rests primarily on a single study or a
  non-replicated finding.
- Where SDT and psychological safety research have not been directly
  compared in the literature, say so explicitly rather than inferring.
- Do not pad with general statements — every paragraph should advance
  a specific, citable claim or resolve a specific question.
```

**Evidence anchors:**

| Source | Domain | Evidence Level |
|---|---|---|
| Deci & Ryan (1985) — *Intrinsic Motivation and Self-Determination in Human Behavior* | SDT foundation | Theoretical + lab research |
| Ryan & Deci (2000) — *American Psychologist* | SDT overview | Landmark synthesis |
| Ryan & Deci (2017) — *Self-Determination Theory* | Full theory statement | Book-length synthesis |
| Gagné & Deci (2005) — *J. Organizational Behavior* | SDT at work | Landmark application synthesis |
| Deci, Connell & Ryan (1989) | Autonomy-supportive management | RCT (Fortune 500) |
| Vansteenkiste & Ryan (2013) | Need frustration vs. satisfaction | Theoretical refinement |
| Van den Broeck et al. (2016) — *J. Management* | SDT needs meta-analysis | Meta-analysis, N > 36,000 |
| Slemp et al. (2018) | Autonomy-supportive leadership | Meta-analysis |
| Edmondson (1999) — *Administrative Science Quarterly* | Psychological safety — team construct | Original empirical study |
| Edmondson (2018) — *The Fearless Organization* | Psychological safety applied | Synthesis + case evidence |
| Frazier et al. (2017) — *Personnel Psychology* | Psychological safety meta-analysis | Meta-analysis, N > 22,000 |
| Porges (2011) — *The Polyvagal Theory* | Threat-state neurobiology | Neurophysiological framework |
| Siegel (1999) — *The Developing Mind* | Window of tolerance | Theoretical/clinical |
| van der Kolk (2014) — *The Body Keeps the Score* | Chronic dysregulation and function | Clinical research + neuroimaging |
