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
| Psychological Safety — Essential Practices Research | — | — | Identify the complete evidence-backed set of practices essential for creating and sustaining psychological safety in a chronically dysregulated workplace; includes complementarity chain mapping where each practice falls short and which resolves its gap |
| Consulting Initial Meeting — Warm Entry Research | — | — | Best practices for initial consulting meetings entering on pre-existing conceptual alignment and relational warmth; covers entry theory, warm vs. cold entry, meeting structure, informal-to-formal transition, and two-meeting owner→OM sequence |

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

---

## Psychological Safety — Essential Practices Research Prompt

**When to use:**
- Building the actionable manager/leader practice list for an RPA engagement
- Identifying what is non-negotiable vs. supplementary for psychological safety
- Developing training architecture and supervisory accountability structures
- Grounding A001 engagement design in the full evidence base beyond the base case brief

**Related documents:**
- [[Workplace Dysregulation — Empirical Base Case & Solution Framework]] — base case research this prompt builds on
- [[SDT — Theory, Workplace Application & Psychological Safety Gap]] — SDT gap analysis this prompt extends
- [[Relational Performance Advisory — Workplace Dysregulation Research Prompt]] — prior prompt; this one supersedes it for practice-level work

```
You are a research synthesizer with expertise in organizational psychology,
neuroscience, trauma-informed systems, and applied behavioral practice.
Produce a structured research brief with one governing purpose: identify
the complete set of evidence-backed practices that are essential for
creating and sustaining psychological safety in a chronically dysregulated
workplace — with enough specificity to produce an actionable list.

The question is not "what helps?" The question is "what is non-negotiable?"
Only include what the evidence identifies as essential — practices whose
absence demonstrably prevents psychological safety from forming or holding.

Context: a multi-property hospitality operation, ~400 employees, high
turnover (~70-80% annually), Midwest. Frontline service workforce carrying
chronic emotional labor load (Hochschild). Two mid-level operations managers
between the owner and the floor. The workforce exhibits entitlement, conflict,
and absenteeism consistent with systemic needs frustration — not character
defects. The organization has not previously operated from a safety framework.

Existing research covers: SDT need definitions, autonomy-supportive management
behavior clusters, and where SDT falls short (relatedness/safety conflation,
autonomy/candor conflation, hierarchy problem, threat-state sequencing);
neurobiological base case (Porges, Siegel, van der Kolk); psychological safety
(Edmondson, Frazier meta-analysis); burnout (Maslach, JD-R); SAMHSA six
principles and Sanctuary Model commitments at the principles level;
organizational identity and socialization (Schein, Van Maanen, Ashforth & Mael,
Kusluvan, Hochschild, Tracey & Hinkin). Do not re-cover these at length.
Reference them where they connect. Fill what is missing.

---

SECTION 1: LEADER INCLUSIVENESS — THE #1 ANTECEDENT, OPERATIONALIZED

Frazier et al. (2017, Personnel Psychology, 70(1), 113-165) identified leader
inclusiveness as the single strongest and most consistent antecedent of
psychological safety across 136 studies, N > 22,000 — above trust, above
cohesion, above job satisfaction. The existing research names this finding
but does not develop what leader inclusiveness means as a behavioral model.

1. What specific behaviors constitute leader inclusiveness in the research
   literature? Cite the primary sources that operationalize this construct
   — not just Frazier et al., but Nembhard & Edmondson (2006), Carmeli et al.
   (2010), and any subsequent refinements.

2. Is leader inclusiveness a trainable behavioral cluster? What does the
   training evidence show — what behaviors change, over what timeframe,
   with what effect sizes?

3. How does leader inclusiveness interact with the SDT autonomy-supportive
   management model? Where do they overlap, where are they distinct?

4. What does leader inclusiveness look like specifically in a hospitality
   supervisory context — i.e., an OM or shift supervisor with frontline
   service workers? What behaviors matter most in that power-differential,
   high-paced context?

---

SECTION 2: THE MANAGER AS CO-REGULATOR

The existing research establishes that managers trigger or reduce threat
responses (Porges' neuroception, Siegel's window of tolerance, van der
Kolk's sensitization). But this is framed as a stimulus-response model.
The co-regulation literature treats it differently: a regulated manager
neurobiologically regulates the people around them through the same social
engagement system channels.

1. What does Porges' co-regulation concept specifically mean for the
   manager-employee relationship? What are the neural and behavioral
   mechanisms of co-regulation in adult, non-clinical contexts?

2. Deb Dana's operationalization of Polyvagal Theory for non-clinical
   settings (The Polyvagal Theory in Therapy, 2018; Polyvagal Exercises
   for Safety and Connection, 2020) — what specific practices does she
   identify for building and maintaining ventral vagal regulation? Which
   translate directly to a management context?

3. If an unregulated manager co-dysregulates their team, what does the
   evidence say about manager regulation capacity as a prerequisite for
   any behavioral training? Is behavior-level training sufficient if the
   manager's own regulatory system is chronically activated?

4. What specific practices build manager regulation capacity — not
   employee-facing behaviors but the manager's own nervous system
   regulation? What is the evidence base for each?

5. Rock's SCARF model establishes that managers' own SCARF threat responses
   (status, certainty, autonomy) produce controlling behavior that
   dysregulates their teams. What does the research say about addressing
   manager SCARF activation as a structural prerequisite to behavior change?

---

SECTION 3: TRAUMA-INFORMED ORGANIZATIONAL MECHANICS

The existing research covers SAMHSA's six principles and Sanctuary Model's
seven commitments as principles. What is missing is the operational
mechanics — what these look like as daily and weekly management practices
in a non-clinical organizational context.

1. Perry's Neurosequential Model of Therapeutics (NMT) — the
   regulate → relate → reason sequence.
   - Explain the neurobiological basis and the precise sequence logic.
   - How has this sequence been applied outside clinical settings?
     Specifically: in schools (Perry's own work with educational
     applications), in HHS organizations, and in any organizational
     development context.
   - What does regulate → relate → reason mean as an operational model
     for manager-employee interaction sequences — particularly performance
     conversations, conflict resolution, and onboarding?

2. Sanctuary Model — specific operational practices (not commitments).
   - What is the S.E.L.F. framework (Safety, Emotions, Loss, Future)
     and how is it used as a communication and meeting protocol?
   - What are Community Meetings in the Sanctuary Model — structure,
     frequency, purpose, facilitation? What organizational outcomes
     did they produce in evaluated settings?
   - What are Safety Plans and how are they used as a proactive
     (not just reactive) organizational tool?
   - Which of these mechanics translate directly to a non-clinical
     organizational context without clinical infrastructure?

3. Trauma-informed communication protocols — what distinguishes them
   from standard active listening or HR communication training?
   - What specific language patterns, interaction structures, and
     response protocols are evidence-backed in trauma-informed
     organizational settings?
   - What does non-coercive language look like in a management
     direction-giving context (not a therapeutic context)?
   - Cite SAMHSA, Bloom, and any peer-reviewed organizational studies
     that have tested trauma-informed communication protocols in
     non-clinical workplaces.

4. Secondary traumatic stress and emotional labor — the hospitality
   translation.
   - What specific organizational practices have reduced STS and
     emotional labor strain in HHS settings and which are viable in
     hospitality without clinical infrastructure?
   - What does the evidence say about psychological recovery periods,
     decompression structures, and pre/post-shift rituals as
     organizational practices?

---

SECTION 4: ERROR MANAGEMENT CULTURE

This is largely absent from the existing research and represents a
distinct, empirically supported construct.

1. Frese, M. & Keith, N. (2015). "Action errors, error management,
   and learning in organizations." Annual Review of Psychology, 66,
   661-687. Summarize the error management culture framework:
   - What distinguishes error management culture from (a) error
     prevention culture and (b) psychological safety?
   - What specific organizational practices constitute an error
     management culture?
   - What outcomes does error management culture predict, and at
     what effect sizes?

2. Van Dyck et al. (2005). "Organizational error management culture
   and its impact on performance." Journal of Applied Psychology,
   90(6), 1228-1240. Report the findings of this study.

3. How does error management culture interact with psychological
   safety — are they additive, redundant, or addressing different
   mechanisms?

4. What are the specific managerial behaviors that build vs. destroy
   error management culture? Distinguish what the manager does when
   an error occurs from the structural norms the manager establishes
   before errors occur.

5. In a hospitality context where guest experience errors have visible
   immediate consequences, how does error management culture function
   differently than in knowledge-work settings?

---

SECTION 5: IMPLICIT VOICE THEORIES — CHANGING THEM

Detert & Edmondson (2011, Academy of Management Journal, 54(3),
461-488) established that employees' implicit voice theories —
ingrained beliefs about when speaking up is safe or dangerous —
operate largely independently of formal organizational structures
and autonomy-supportive management behaviors.

1. What does the research say about where implicit voice theories
   come from — organizational history, prior employment, cultural
   background, or interpersonal experience?

2. What interventions have been shown to change implicit voice
   theories? Distinguish between:
   (a) leader behaviors that gradually revise the belief through
       accumulated disconfirming evidence
   (b) structural interventions (formal channels, protection from
       retaliation) that create safe conditions for testing the belief
   (c) explicit cognitive/dialogic interventions that surface and
       examine the belief directly

3. How long does it take to shift implicit voice theories in a
   chronically unsafe environment? What does the research say about
   the number of consistent disconfirming experiences required?

4. What role does peer behavior play — specifically, does watching
   a colleague speak up without punishment change implicit voice
   theories faster than personal experience of safety?

---

SECTION 6: SERVANT LEADERSHIP AS AN INTEGRATING MODEL

The existing research covers SDT-based management practices and
Edmondson's psychological safety leadership behaviors, but lacks an
integrating leadership model. Servant leadership has the largest
empirical base of any leadership model for wellbeing, safety, and
psychological need satisfaction outcomes.

1. Greenleaf's servant leadership construct and its empirical
   operationalization — cite van Dierendonck & Nuijten (2011) and
   Liden et al. (2008).

2. What does the servant leadership meta-analytic evidence show for:
   (a) employee wellbeing and psychological safety outcomes
   (b) SDT need satisfaction
   (c) team performance
   Cite Eva et al. (2019, Leadership Quarterly) or comparable
   meta-analysis. Report effect sizes.

3. What is the non-redundant contribution of servant leadership
   relative to SDT-aligned management and leader inclusiveness —
   what does it add that neither covers?

4. Is servant leadership viable in a hospitality supervisory context?
   What does the research say about service-industry applications?

5. What specific behaviors from the servant leadership model are
   highest-leverage for psychological safety — not the full model,
   the essential core?

---

SECTION 7: INTERACTION AND MEETING DESIGN AS SAFETY INFRASTRUCTURE

Psychological safety is produced or destroyed in specific interactions
and structural contexts that occur daily — not only through leadership
style. The design of these interactions is a distinct intervention layer.

1. What does the research say about the 1-on-1 meeting as a safety
   infrastructure tool? Frequency, structure, content norms — what
   does evidence show about 1-on-1 design and psychological safety
   or need satisfaction outcomes?

2. Team briefing and debriefing protocols — what does the research
   show about structured pre/post-shift briefings as psychological
   safety mechanisms? Cite Edmondson's after-action review research
   and any healthcare or military applications translated to other
   contexts.

3. How do meeting norms (speaking order, silence tolerance, challenge
   protocols) affect psychological safety? What specific norms are
   evidence-backed as safety-producing vs. safety-destroying?

4. In a hospitality context with shift-based, high-turnover frontline
   workers — what interaction structures are operationally feasible
   and evidence-backed?

---

SECTION 8: SUPERVISORY ACCOUNTABILITY STRUCTURES

Tracey & Hinkin (2008) establish that culture dies at the unit manager
level in hospitality. What sustains manager behavior change after initial
training is not addressed in the existing research.

1. What does the research say about the conditions under which manager
   behavior training produces durable behavior change vs. rapid
   reversion to baseline?

2. What specific accountability structures sustain manager safety
   behaviors — peer observation and feedback, coaching relationships,
   manager-of-managers behavior modeling, measurement and feedback?

3. Is there evidence for upward feedback mechanisms (employee ratings
   of manager safety behaviors) as a sustained accountability tool?
   What are the conditions under which this works vs. backfires?

4. What does research on behavioral skills maintenance show about
   necessary follow-up dose, format, and timing?

---

SECTION 9: FEEDBACK SCIENCE

Feedback is the primary mechanism of competence support (SDT) and a
core component of psychological safety — yet the conditions under which
feedback builds vs. destroys safety are not developed in the existing
research.

1. Kluger & DeNisi (1996). Feedback Intervention Theory. Psychological
   Bulletin, 119(2), 254-284.
   - What are the conditions under which feedback improves performance
     vs. undermines it?
   - What is the "feedback sign effect" and why does it matter for
     psychological safety?
   - What does FIT say about behavioral feedback vs. self-level
     feedback — and which is safer?

2. What specific feedback delivery practices are evidence-backed for
   simultaneously supporting competence (SDT) and maintaining
   psychological safety?

3. What does the research say about feedback frequency, timing, and
   format in high-turnover, service-industry contexts?

4. How does the evaluative vs. informational feedback distinction (SDT)
   map onto the Kluger/DeNisi findings?

---

SECTION 9B: COMPLEMENTARITY CHAIN — WHERE EACH PRACTICE FALLS SHORT

For each practice identified across Sections 1-9, document two things:
(1) the specific gap that remains even when this practice is correctly
and fully implemented — what it structurally cannot accomplish on its
own; and (2) which other practice in this research directly addresses
that remaining gap. The goal is a complementarity chain that reveals
why the practices are interdependent, not interchangeable, and why
adopting any one in isolation produces predictable failure.

Format each entry as:

PRACTICE: [name]
WHAT IT ACCOMPLISHES: [brief statement of its primary function]
WHERE IT FALLS SHORT: [the specific structural gap — what it cannot
  do even when done correctly — with citation]
WHICH PRACTICE RESOLVES THIS GAP: [the specific practice that picks
  up where this one ends, and why]

Cover at minimum:
- Autonomy-supportive management (SDT)
- Psychological safety interventions (Edmondson)
- Regulation-first / co-regulation approaches (Porges/Perry)
- Trauma-informed organizational mechanics (SAMHSA/Bloom)
- Error management culture (Frese & Keith)
- Leader inclusiveness (Frazier et al.)
- Servant leadership
- Feedback science (Kluger & DeNisi)
- Implicit voice theory interventions (Detert & Edmondson)
- Supervisory accountability structures

Where the chain loops — where Practice A's gap is resolved by Practice B,
and Practice B's gap is resolved by Practice A or a third practice — make
the loop explicit. These loops reveal where the integration logic lives.

---

SECTION 10: SYNTHESIS — WHAT IS ESSENTIAL

Do not produce a list earlier than this section.

1. Based on all research above plus the existing base: what is the
   minimum essential set of practices that the evidence identifies as
   non-negotiable for psychological safety to form and hold in a
   chronically dysregulated workplace?

2. Organize by level:
   (a) Owner/senior leadership — what must be true at the top
   (b) Manager/supervisor daily behaviors — the operational mechanism
   (c) Structural/operational design — what must be built into how
       the organization runs
   (d) Prerequisites — what must be in place before the above can
       take hold

3. For each practice identified:
   - Name the source framework
   - State the evidence level (meta-analysis / RCT / observational /
     theoretical)
   - Identify whether it is trainable, structural, or cultural
   - Flag if absent from the existing four research documents

4. Hospitality-specific weighting: given emotional labor load,
   shift-based structure, high turnover, multi-property dispersion,
   and unit-manager-as-transmission-mechanism dynamics — which
   practices move to the top, and which require adaptation?

5. What does the research identify as the single most common failure
   mode when organizations attempt to build psychological safety —
   and what practice directly addresses that failure mode?

---

FORMATTING REQUIREMENTS:
- Cite author, title, journal/publisher, and year for every claim.
- Distinguish evidence levels: meta-analysis, RCT, longitudinal,
  cross-sectional, theoretical/clinical framework.
- For every practice named, identify: (a) trainable, (b) structural,
  or (c) cultural.
- Flag any claim that lacks independent replication.
- Do not produce a list until Section 10.
- Do not repeat existing base research at length — reference and build.
```

**Evidence anchors (new — extends existing base):**

| Source | Domain | Evidence Level |
|---|---|---|
| Nembhard & Edmondson (2006) — *J. Organizational Behavior* | Leader inclusiveness operationalized | Empirical study |
| Carmeli et al. (2010) | Leader inclusiveness and learning | Empirical study |
| Frazier et al. (2017) — *Personnel Psychology* | Leader inclusiveness as #1 antecedent | Meta-analysis, N > 22,000 |
| Dana, D. (2018) — *The Polyvagal Theory in Therapy* | Co-regulation for non-clinical practice | Clinical/applied framework |
| Perry, B. (NMT) — Child Trauma Academy | Regulate → relate → reason sequence | Neurobiological/applied framework |
| Bloom (2013) — S.E.L.F. / Community Meetings | Sanctuary Model operational mechanics | Program evaluation |
| Frese & Keith (2015) — *Annual Review of Psychology* | Error management culture | Review + empirical synthesis |
| Van Dyck et al. (2005) — *J. Applied Psychology* | Error management culture → performance | Empirical study |
| Detert & Edmondson (2011) — *Academy of Management J.* | Implicit voice theories | Qualitative + survey |
| Eva et al. (2019) — *Leadership Quarterly* | Servant leadership meta-analysis | Meta-analysis |
| van Dierendonck & Nuijten (2011) | Servant leadership instrument | Scale development + validation |
| Liden et al. (2008) | Servant leadership behaviors | Empirical operationalization |
| Kluger & DeNisi (1996) — *Psychological Bulletin* | Feedback Intervention Theory | Meta-analysis + theory |

---

## Consulting Initial Meeting — Warm Entry Research Prompt

**When to use:**
- Designing or refining an initial meeting with a client who already shares your conceptual frame
- Preparing for a first formal engagement conversation after an informal helping interaction has established rapport
- Designing the two-meeting entry sequence (sponsor/owner first, then managers)
- Any engagement where relational warmth exists before the formal work begins

**Generated output:** [[Consulting Initial Meeting — Warm Entry Research Brief]]

**Evidence anchors:**

| Source | Contribution | Type |
|---|---|---|
| Schein, E.H. (1999/2009) — *Process Consultation Revisited* | Entry phase principles; collaborative stance; helping relationship | Practitioner primary source |
| Schein, E.H. (2013) — *Humble Inquiry* | Asking over telling; genuine curiosity as influence mechanism | Practitioner primary source |
| Block, P. (2011) — *Flawless Consulting* | Contracting conversation; exploring wants; role establishment | Practitioner primary source |
| Maister, Green & Galford (2000) — *The Trusted Advisor* | Trust Equation (C+R+I/S); intimacy as load-bearing in entry | Practitioner primary source |
| Cannon-Bowers & Salas — shared mental models | Shared mental models accelerate collaborative readiness | Empirical research |
| Value congruence research — professional services | Alignment on "what the problem is" predicts follow-through | Empirical research |

```
You are researching best practices in consulting for initial client meetings that enter on a
foundation of pre-existing conceptual alignment and warm relational capital. The research
will be used to design a specific initial meeting with a hotel chain owner (~400 employees,
Midwest multi-property operation) who already shares a core conceptual frame with the
consultant. Context: the owner and consultant had an informal coffee shop exchange in which
the owner experienced a visible insight shift — from attributing employee entitlement and
conflict to character defects, to understanding them as rooted in environmental and structural
causes. The owner was visibly grateful and surprised. An introductory letter has since been
sent. The first formal meeting is being scheduled. A second meeting with two operations
managers will follow. The consultant's role is Advisory and Implementation Orchestration —
not operational management. The owner has a likely secure to mildly anxious attachment
profile and an operational, results-focused orientation.

Produce a research brief covering the following areas:

SECTION 1 — CONSULTING ENTRY THEORY: WHAT THE LITERATURE ESTABLISHES
Research the foundational frameworks for initial client meetings in organizational consulting.
Cover: Schein's process consultation entry principles — the collaborative stance, the
"helping relationship," and why prescription before diagnosis destroys trust; Block's
(Flawless Consulting) contracting conversation model — the structure of exploring wants,
offering yourself, and clarifying roles; Maister, Green & Galford (The Trusted Advisor) —
the Trust Equation components (Credibility, Reliability, Intimacy, Self-Orientation) and
which of these is most load-bearing in an initial meeting; Schein's Humble Inquiry — the
distinction between asking and telling, and why genuine curiosity in the entry meeting
produces more influence than expertise display. For each framework, identify: the core
behavioral insight, the specific meeting behaviors it implies, and what failure looks like
when the principle is violated.

SECTION 2 — WARM ENTRY: HOW PRIOR CONCEPTUAL ALIGNMENT CHANGES THE APPROACH
Research what changes about initial meeting design when the client already shares the
consultant's core conceptual frame and there is pre-existing relational warmth. Cover:
how shared mental models (Cannon-Bowers & Salas; team cognition research) accelerate
trust and collaborative readiness; value congruence research in professional services
relationships — how perceived alignment on "what the problem really is" affects client
receptivity and follow-through; the specific risks of warm entry — overselling into existing
warmth, assuming more alignment than actually exists, failing to establish formal professional
architecture within the relational context; the "relational anchor" — research on using
a prior informal interaction as a bridge to a formal engagement without making it feel
manipulative or transactional. Distinguish warm entry from cold entry at the behavioral
level: what is the same, what is different, and what warm entry specifically enables that
cold entry cannot.

SECTION 3 — MEETING STRUCTURE FOR WARM-ENTRY INITIAL CONSULTING MEETINGS
Based on the evidence in Sections 1 and 2, document what a well-designed initial meeting
looks like when entering on a foundation of prior rapport and conceptual alignment. Cover:
the opening — how to reference and honor the prior interaction without reducing it to a
sales tactic; the diagnostic deepening move — how to expand the client's picture of the
problem scope without invalidating the insight they already have; the role establishment
move — how and when to clarify the consultant's professional architecture (what Andrew
does, what he doesn't do, and why that matters) without making the meeting feel like a
scope-setting negotiation; the transition from "shared insight" to "here's what we could
do together" — research on when and how this transition should happen in a warm-entry
meeting; what the meeting should NOT try to accomplish (common errors in first meetings
that undermine longer-term trust).

SECTION 4 — THE INFORMAL-TO-FORMAL TRANSITION
Research what happens relationally and psychologically when a consultant moves from an
informal helping interaction to a formal engagement conversation with the same person.
Cover: the risks of the transition — how it can feel like the prior interaction was a
"setup"; how to preserve the authenticity and trust established informally as the formal
structure is introduced; what clients with an operational/results orientation (vs.
relationship-primary orientation) specifically need from this transition; how to introduce
pricing and scope in a warm-entry context without the conversation becoming transactional
abruptly.

SECTION 5 — THE TWO-MEETING SEQUENCE: OWNER FIRST, THEN OPERATIONS MANAGERS
Research best practices for sequencing a multi-stakeholder consulting entry where the
owner/sponsor is met first and the managers who will be subjects of the engagement are
met second. Cover: what the owner meeting needs to establish that the OM meeting can then
build on; how to design the first meeting so the owner is prepared to introduce and
contextualize the consultant to the OMs in a way that sets the right frame; what OMs
typically need from a first meeting with a consultant that the owner does not need; how
attachment and threat-detection dynamics (SCARF) are likely to differ between the owner
meeting (collaborative context, prior rapport) and the OM meeting (evaluation context,
potential status threat); how to design the OM meeting to reduce threat and establish
collaborative rather than evaluative framing from the outset.

SECTION 6 — BEHAVIORAL PRACTICE LIST FOR INITIAL MEETING DESIGN
Drawing from all five sections above, produce a consolidated list of specific, observable
behavioral practices for each phase of an initial consulting meeting with a warm-entry
profile. Organize by meeting phase: before the meeting (preparation), opening, diagnostic
deepening, role/scope establishment, transition to engagement, close. For each practice:
what it is, what it accomplishes, and what failure to use it risks. Flag which practices
are especially high-leverage in a hospitality owner context with an operational mindset.

EVIDENCE STANDARDS:
- Prioritize peer-reviewed research and primary-source practitioner literature (Schein,
  Block, Maister are acceptable primary practitioner sources — cite them as such)
- Flag [NR] for claims without independent replication
- Flag [CF] for clinical/theoretical frameworks with applied translation
- Note when findings come from non-consulting professional services research (law,
  medicine) that may not transfer directly

OUTPUT: Full research brief with section headers matching above. Section 6 should be
scannable as a standalone practitioner reference. Use behavioral and operational language
throughout — no academic hedging in Section 6.
```
| Tracey & Hinkin (2008) | Supervisory accountability in hospitality | Empirical (hospitality-specific) |
