<!--
author: Hannes Tegelbeckers
language: en
-->

# GIZ Keynote – AI in TVET and Employment Promotion

## Dashboard

_Generated from the project sections below. Do not edit manually._

### Current State

__Current step:__ ✅ Session 1 (keynote) built — material, validation, and persona review complete
__Course validation:__ Session-mode PASS with concerns (two open `PRÜFEN` items)
__Sessions complete:__ 1 / 1
__Last updated:__ 2026-02-14

### Next Commands

1. [👁 Preview keynote](agent:teaching/preview?file=materials/01-giz-keynote/README.md) `:preview materials/01-giz-keynote/README.md` — review the slides in the DevServer
2. [🔍 Full course validation](agent:teaching/validate-course) `:validate-course` — course-mode gate before publishing
3. [🛠️ Publish](agent:development/create-project) `:agent development` → `:create-project` — after course-mode PASS

### Agents

🎓 __Teaching__ — refine content or re-run validation · [🔍 Validate course](agent:teaching/validate-course) `:validate-course`
🎨 __Artist__ — no image generation for this keynote · [🎨 Switch to Artist](agent:artist/switch) `:agent artist`
🧑‍🎓 __Learner__ — re-review as Amina · [🧑‍🎓 Review as Amina](agent:learner/review-as-persona?name=Amina&number=1&type=keynote) `:review-as-persona Amina 1 keynote`
🛠️ __Development__ — publishing after course-mode PASS · [🛠️ Create project](agent:development/create-project) `:create-project`

### Quality State

- Session 1 (keynote): session-mode validation **PASS with concerns** — two `PRÜFEN` items open
- Persona review (Amina): **OK** — no blocking concerns
- Publishing gate: not yet open (needs course-mode PASS)

### Session Progress

| # | Title | Status | Next step |
|---|-------|--------|-----------|
| 1 | AI in TVET and Employment Promotion | ✅ done | [🛠️ Publish](agent:development/create-project) `:create-project` (after course-mode PASS) |

### Open Blockers

- Two `PRÜFEN` items to verify before the talk (ILO figures; Teaching-Agent drafting mention) — see `## Notes Backup` · [🔍 Validate course](agent:teaching/validate-course) `:validate-course`

### Quick Links

- Material: `materials/01-giz-keynote/README.md`
- Validation report + persona review: `journal.md` → `## Sessions` → `### 1. AI in TVET and Employment Promotion`

## Course Context

__Course Type:__ single-lesson

__Terminology:__ keynote (session), conference (course), participants (learners)

__Course Profile:__ One LiaScript presentation: a 12–15 minute virtual inspirational keynote for the GIZ TVET and Labour Market community. Fact base: `inputs/quelle_keynote.md`. Binding brief: `inputs/rahmen.md`.

__File Structure:__ multi-file

__Conventions & Standards:__ see `inputs/rahmen.md` (binding).

__LiaScript conventions:__ English; `mode: Presentation`; `classroom: enable`; speaker notes `--{{0}}--` on every slide; no external templates; no images.

__Additional Notes:__ The run produces exactly one keynote. The rest of the conference exists outside this project.

## Outline

__Title:__ AI in TVET and Employment Promotion – Applying AI Sensibly

__Target Audience:__ GIZ staff and partner-country experts in TVET and labour-market projects; online; not AI experts.

__Time Commitment:__ 12–15 minutes, no discussion part.

__Abstract:__ AI is quietly entering work and learning. For development cooperation the question is not building AI models but applying AI sensibly: better labour-market data, training skilled workers for AI-augmented systems, and training humans with AI – with people, local ownership and the informal sector in focus.

__Learning Objectives:__
1. Participants can explain in plain words why GIZ should focus on applying, not building, AI.
2. Participants can name opportunities and risks of AI along the labour-market-information value chain, incl. data sovereignty and the informal sector.
3. Participants can describe how TVET must change to prepare skilled workers for AI-augmented systems.
4. Participants can argue for AI as a co-pilot in teaching, with human judgement at the centre.

## Didactics

__Didactic Concept:__ Inspirational keynote: story-driven, concrete examples, one idea per slide, a clear red thread (apply – people – data), call to action. Details: `inputs/rahmen.md`.

__Professor Persona:__ University researcher in engineering pedagogy and technical education, practical, warm, uses concrete examples from vocational schools and workplaces in partner countries.

__Teaching Style:__ short slides with step-by-step reveal, one or two live polls for the online audience, no graded quiz.

__Course Type:__ single-lesson

__Didactic Framework:__ Constructive Alignment

__Default Session Method:__ gagne

__Session Types:__
  1. __Keynote__ (slug: `keynote`) — Inspirational talk in LiaScript presentation mode, 12–15 min, 14–18 slides. Required: five parts of `inputs/rahmen.md` in order with chapter dividers; at least one live poll; three take-aways and a call to action; speaker notes on every slide.

__Difficulty Level:__ Non-experts; no technical prior knowledge assumed.

## Visual Identity

_Not needed (no image generation, no image files)._

## Templates

_No external templates._

## Agenda

| # | Title | Type | Method | Duration | Status |
|---|---|---|---|---|---|
| 1 | AI in TVET and Employment Promotion | keynote | gagne | 15 min | ✅ |

## Sessions

| # | Title | Type | Skeleton | Material | Validation |
|---|---|---|---|---|---|
| 1 | AI in TVET and Employment Promotion | keynote | ✅ | ✅ | ✅ |

### 1. AI in TVET and Employment Promotion

**Type:** keynote · **Method:** gagne · **Date:** GIZ conference 2026 · **Output:** `materials/01-giz-keynote/README.md`

**Summary:** Setting the scene (AI is already here; apply, don't build) → Pillar 1 data for labour-market analysis (value chain, sovereignty, informal sector) → Pillar 2 training for AI-augmented systems (smart water, solar, automation; job-specific AI skills) → Pillar 3 training humans with AI (personalised learning, OER, co-pilot pedagogy) → conclusion and call to action for GIZ.

**Content:** Source: `inputs/quelle_keynote.md` (all sections 0–4). Time budget per part in `inputs/rahmen.md`.

**Activities:** Opening poll "Where did you meet AI this week?" · optional second poll in the conclusion "Where should your project start?" · three take-aways.

#### Validation Report

<section>

__Date:__ 2026-02-14
__Material:__ materials/01-giz-keynote/README.md
__Result:__ PASS with concerns
__Mode:__ session

##### Content
- All four learning objectives addressed (apply-don't-build: "Apply, don't build" slide; LMI value chain + sovereignty + informal sector: Part 2; AI-augmented systems + job-specific skills: Part 3; co-pilot pedagogy with human judgement: Part 4)
- No placeholder-only or vague sections; all facts traceable to `inputs/quelle_keynote.md`
- Both planned polls present (opening + conclusion); three take-aways and closing line on final slide
- Duration: ~15 slides at ~1 slide/min for a 12–15 min keynote — inside 70%–150% of declared 15 min (advisory check, no flag)
- ⚠️ Two `PRÜFEN` items remain open (ILO figures; Teaching-Agent drafting mention) — kept as `<!-- PRÜFEN: … -->` per binding rule

##### Type Consistency
- Session Type: `keynote` — Erforderlich (from `## Didactics` → `__Session Types:__`): five parts of `inputs/rahmen.md` in order with chapter dividers; at least one live poll; three take-aways and a call to action; speaker notes on every slide
- All satisfied: five `#` chapter dividers in order (Setting the scene / data question / TVET-prep question / learning question / invest question), two polls, three take-aways + call to action, `--{{0}}--` notes on every slide

##### Persona & Style
- Tone matches binding brief: plain, non-technical, concrete people/situations (water technician in Nairobi, job-seekers, teachers); risks named without fear-mongering
- Terminology matches `## Course Context` (keynote, participants, no German leftovers)

##### LiaScript Syntax
- Metadata header — ✅ (author, email, version, language, narrator, mode, classroom, title, comment)
- Heading structure — ✅ (one `#` title + five `#` part dividers; all slides `##`; no bare `####`+)
- Code blocks — ✅ (single `ascii` value-chain diagram, properly fenced)
- Alerts / citations / formulas / media / includes / variables — ✅ (not used)
- Animations & TTS — ✅ (numbering resets per slide; every `{{n}}` has a matching `--{{n}}--`)
- Surveys — ✅ (two single-choice vectors, `- [(1)] …` options, not indented)
- HTML blocks — ✅ (none used)

##### Recommended Actions
1. Verify the two `PRÜFEN` items before the talk (ILO figures; decide on Teaching-Agent drafting mention) — see `## Notes Backup`

</section>

#### Persona Reviews

<section>

##### Amina (GIZ TVET project advisor)

__Date:__ 2026-02-14
__Persona:__ Amina — GIZ TVET project advisor in East Africa, curious but sceptical, wants 2–3 usable ideas
__Material:__ materials/01-giz-keynote/README.md
__Result:__ OK

###### Overall Impression
Honestly, this felt like someone talking to *us*, not to a tech audience. I was a bit suspicious at the start ("another donor hype?"), but the "we don't build the engine, we train drivers" line and the data-sovereignty part calmed me down. I can actually take the three take-aways to my ministry meeting next week.

###### Dimension Findings

**a) Verständlichkeit / Sprachniveau**
Short sentences, no unexplained jargon. "Data sovereignty", "OER", "high-risk" are all explained in plain words in the same slide. Verdict: OK

**b) Schwierigkeitsgrad / Überforderung**
One idea per slide, three pillars, clear red thread. The skill model (Use / Understand / Maintain) is the densest part, but it is concrete. Verdict: OK

**c) Relevanz / Motivation**
Very high. The informal-sector slide is exactly my daily reality — my apprenticeship partners are invisible in job portals. "People before platforms" is a sentence I can use with the ministry. Verdict: OK

**d) Zugänglichkeit**
Plain English, no assumed AI background. The poll options are simple. Verdict: OK

**e) Formatpräferenz**
Short bullets plus one simple diagram; two quick polls keep an online audience awake. No long text walls. Verdict: Good fit

**f) Vorwissen / fehlende Grundlagen**
- "AI model" / "foundation models" ⚠️ assumed, but explained in one line on the "Apply, don't build" slide
- "ESCO classification" ⚠️ assumed, but named as an example only — acceptable
- "TVET", "LMI", "OER" ✅ likely known (explained inline for OER)
- "EU AI Act" ⚠️ assumed, but framed as "a useful reference point", not required knowledge

###### Priority Issues
1. (None blocking.) Minor: the ILO figures carry a `PRÜFEN` mark — as a sceptic I would want them verified before I repeat them to partners; the speaker note already says so.

###### What Worked Well
The "if it is not in the data, it is not in the decision" line, the concrete Nairobi leak-alarm example, and the honest risk list (confident wrong answers, copying, access) — that honesty is what makes me believe the rest.

</section>

## Agents

### Learner Personas

#### Persona: Amina (GIZ TVET project advisor)

Amina, 38, works in a GIZ TVET project in East Africa, background in economics, coordinates with the ministry and vocational colleges. Uses a chatbot occasionally for emails, is curious but sceptical, worries about data protection and that AI is "another donor hype". Wants two or three ideas she can bring to her partners next week. _Derived from the audience description, not a real person._

## Validation

### Latest Validation Summary

Date: 2026-02-14
Mode: session (session 1)
Result: PASS with concerns
Issues found: 2 (both open `PRÜFEN` items, kept as comments per binding rule)
Sessions checked: 1

Note: This is a session-mode result. The publishing gate requires a course-mode PASS (`:validate-course` with no arguments).

## Notes Backup

_Decisions of the autopilot run are logged here._

**2026-02-14 — `:build-session 1 keynote` (autopilot)**

1. **Question:** Should the second poll ("Where should your project start?") be included?
   **Decision:** Yes, included on the closing slide.
   **Reason:** The journal's session `**Activities:**` line plans it as an optional second poll; the brief allows up to two polls. It gives the online audience a concrete next step.

2. **Question:** How to keep the 14–18 slide budget while keeping all five parts with `#` dividers?
   **Decision:** 17 slides — 1 title + 5 `#` part dividers + 11 `##` content slides. Merged "What do we mean by AI?" into the "AI arrives quietly" slide (as a step-2 reveal), merged "Job-specific AI skills" into "What changes for skilled workers" (step 3), and merged the "Teachers first" message into the "AI as co-pilot" slide (step 3).
   **Reason:** The binding brief requires 14–18 slides including title and closing slide, and one-line question dividers with `#` for each part. Merging via step reveals keeps all content from `quelle_keynote.md` without adding slides.

3. **Question:** Should the "Teaching Agent" example (speaker's own tool) be mentioned?
   **Decision:** Kept as a single labelled "Example:" bullet, with the `<!-- PRÜFEN: decide whether to mention that this keynote was drafted with it in three ways -->` comment preserved.
   **Reason:** It is in the fact base and the brief requires keeping `PRÜFEN` marks; the "three ways" detail is the open decision, so it stays as a comment rather than spoken content.

4. **Question:** Which persona to use for the review?
   **Decision:** Amina (the only persona defined in `journal.md` → `## Agents` → `### Learner Personas`).
   **Reason:** Autopilot instruction 5 names Amina explicitly.

5. **Question:** Image generation (Step 3 of `:build-session`)?
   **Decision:** Skipped.
   **Reason:** Autopilot instruction 3 forbids image generation and image files; the journal's `## Visual Identity` says "Not needed".

6. **Question:** Should the closing slide be a separate `##` or folded into the last content slide?
   **Decision:** Folded into the "Three take-aways" slide as a final step (poll → quote → thanks).
   **Reason:** Keeps the total at 15 slides; the closing line and thanks are the natural end of the take-aways slide. The brief's "closing slide" requirement is satisfied by this final content block.
