<!--
author: Hannes Tegelbeckers
language: en
-->

# GIZ Keynote – AI in TVET and Employment Promotion

## Dashboard

__Updated:__ 2026-10-06 (autopilot run `:build-session 1 keynote`)

| Area | Status |
| --- | --- |
| Course Context · Outline · Didactics · Agenda | ✅ present |
| Session 1 – AI in TVET and Employment Promotion | ✅ Done (material, session validation PASS with concerns, persona review OK) |
| Course-level validation / publishing gate | ⬜ not run – publishing locked |
| Open `PRÜFEN` items | 2 (ILO figures; Teaching Agent mention) |

__Next steps:__

1. Resolve the two `PRÜFEN` comments in `materials/01-giz-keynote/README.md` (instructor)
2. [Full course check](agent:teaching/validate-course) `:validate-course`
3. [Live chat with Amina](agent:learner/review-as-persona?name=Amina&number=1&type=keynote) `:review-as-persona Amina 1 keynote`

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
| 1 | AI in TVET and Employment Promotion | keynote | ✅ | ✅ | ✅ Done |

### 1. AI in TVET and Employment Promotion

**Type:** keynote · **Method:** gagne · **Date:** GIZ conference 2026 · **Output:** `materials/01-giz-keynote/README.md`

**Summary:** Setting the scene (AI is already here; apply, don't build) → Pillar 1 data for labour-market analysis (value chain, sovereignty, informal sector) → Pillar 2 training for AI-augmented systems (smart water, solar, automation; job-specific AI skills) → Pillar 3 training humans with AI (personalised learning, OER, co-pilot pedagogy) → conclusion and call to action for GIZ.

**Content:** Source: `inputs/quelle_keynote.md` (all sections 0–4). Time budget per part in `inputs/rahmen.md`.

**Activities:** Opening poll "Where did you meet AI this week?" · optional second poll in the conclusion "Where should your project start?" · three take-aways.

#### Validation Report

<section>

__Material:__ `materials/01-giz-keynote/README.md`  
__Mode:__ session · __Date:__ 2026-10-06 · __Iterations:__ 2 (content loop) + 1 re-check after persona fixes  
__Result:__ PASS with concerns

##### Content

- ✅ Learning objectives 1–4 addressed (apply vs. build; value chain, sovereignty, informal sector; skill levels and TVET changes; co-pilot pedagogy).
- ✅ No placeholder or empty slide. All facts come from `inputs/quelle_keynote.md`; own illustrations are labelled "Imagine …" / "Example (illustrative)".
- ✅ References named where claims are made (Cedefop Skills-OVATE, ESCO, EU AI Act 2024, ILO, UNESCO 2019 / 2024).
- ⏭️ `reference-checker`: skipped – skill not installed, no web lookup in this run.
- ✅ Session type `keynote`: five parts in order with `#` dividers and a one-line question each; 2 live polls (max. 2); three take-aways plus call to action; speaker notes on every slide; 18 slides (allowed 14–18).
- ⚠️ `[pedagogical]` Method `gagne`: attention hook ✅ (poll, plumber in Nairobi), prior knowledge activated ✅ (opening poll), practice with feedback only partly – the second poll is an application step, but feedback is limited to the speaker's comments. This fits a keynote; noted, not auto-fixed.
- ✅ Duration (advisory): ~1,500 words of speaker notes ≈ 11.5 min at 130 words/min + 2 polls ≈ 1.5–2 min → about 13–14 min, within 70–150 % of 15 min.
- ⚠️ Two `<!-- PRÜFEN: … -->` items open (ILO figures; whether to mention the Teaching Agent / how this keynote was drafted).

##### Persona & style

- ✅ Tone: plain, short sentences, concrete people (no `### Coauthor` role present – fell back to `__Professor Persona__` / `__Teaching Style__`; consider syncing a Coauthor role).
- ✅ Terminology: keynote / conference / participants.

##### LiaScript syntax

1. Metadata header – ✅ identical to `inputs/rahmen.md`
2. Heading structure – ⚠️ accepted deviation: 6 `#` headings (title + 5 part dividers), as required by `inputs/rahmen.md` (binding); all other slides `##`
3. Code blocks – ✅ one `ascii` block, closed
4. Alerts – ✅ none used
5. Citations – ✅ no citation blockquotes
6. Animations & TTS – ✅ every slide has `--{{0}}--`; every `{{n}}` has a matching `--{{n}}--`; note text not indented
7. Media – ✅ no media (no images by design)
8. Diagrams – ✅ `ascii` tag
9. Formulas – ✅ none
10. Quizzes & surveys – ✅ 2 single-choice surveys, options `- [(n)]` not indented (list form required by rahmen; cheat sheet shows the form without `- `)
11. Includes – ✅ none
12. Variables & macros – ✅ none
13. HTML blocks – ✅ only `<section>`, `<small>`, comments; all `<section>` closed

##### Recommended actions

1. Instructor: resolve both `PRÜFEN` comments before the talk.
2. Check once in the LiaScript preview that `- [(n)]` options render as a survey.
3. Run `:validate-course` (course mode) before publishing.

</section>

#### Persona Reviews

<section>

##### Amina

__Date:__ 2026-10-06  
__Persona:__ Amina – GIZ TVET project advisor in East Africa, economist, curious but sceptical  
__Material:__ `materials/01-giz-keynote/README.md`  
__Result:__ OK (round 2; round 1: Issues found)

###### Overall Impression

"Good – this is not another hype talk. 'Apply, don't build' and 'data with care' are things I can say to the ministry. In round 1, the technical slides lost me with words like calibrate, troubleshoot and escalate. Now they read fine."

###### Dimension Findings

**a) Language level** – Round 1: Issues found ("calibrate, troubleshoot, configure, escalate" on *Working with the system*; "open AI models" sounded like the company OpenAI). Round 2: OK after quick fixes.

**b) Difficulty** – OK. One idea per slide. The table on *Whose data is it?* is the densest slide but works with the reveal steps.

**c) Relevance** – OK. Data sovereignty, data protection and the informal sector are exactly her worries; the investment poll gives her ideas for next week.

**d) Accessibility** – OK. Phone- and SMS-based solutions are named; speaker notes are in plain English for a mixed audience.

**e) Format** – Good fit. Two polls, short reveals, no long text blocks.

**f) Prior knowledge**
- "model" ✅ explained in the notes · "data sovereignty" ✅ explained · "OER" ✅ explained · "high-risk" (EU AI Act) ✅ understandable · "inverter" ✅ explained in the notes · "Skills-OVATE / ESCO" ⚠️ names only – fine as examples, not needed to follow the talk.

###### Priority Issues

1. ~~Technical jargon in Pillar 2~~ – fixed with plain words (round 1, blocking).
2. ~~"open AI models" could be misread~~ – now "open AI models (free to download)" (round 1, blocking).
3. Non-blocking: "What does a small first pilot cost?" – not covered by the source; a topic for the conference discussion.

###### What Worked Well

The engine / drivers / roads picture, the plumber in Nairobi, "If it is not in the data, it is not in the decision", and three take-aways she can repeat.

</section>

## Agents

### Learner Personas

#### Persona: Amina (GIZ TVET project advisor)

Amina, 38, works in a GIZ TVET project in East Africa, background in economics, coordinates with the ministry and vocational colleges. Uses a chatbot occasionally for emails, is curious but sceptical, worries about data protection and that AI is "another donor hype". Wants two or three ideas she can bring to her partners next week. _Derived from the audience description, not a real person._

## Validation

_No course-mode validation yet (session-mode report for session 1 is stored under `## Sessions`). Publishing stays locked until `:validate-course` returns `Mode: course` + `Result: PASS`._

## Notes Backup

_Decisions of the autopilot run are logged here._

### Autopilot decisions – 2026-10-06 (`:build-session 1 keynote`)

| Question | Decision | Reason |
| --- | --- | --- |
| `validate-syntax` wants exactly one `#`, rahmen wants `#` dividers | 6 `#` headings (title + 5 parts) | `inputs/rahmen.md` is binding; recorded as an accepted deviation |
| Survey form `[(1)]` (cheat sheet) vs. `- [(1)]` (rahmen) | `- [(1)]`, not indented | Rahmen is binding; check rendering in preview |
| No `### Coauthor` role in `## Agents` | Fallback to Professor Persona / Teaching Style | per `promote-session` step 4 |
| How to fit 5 parts into ≤ 18 slides | 18 slides; definition of AI revealed on the opening poll slide; take-aways slide is also the closing slide | Keep one idea per slide while staying within the limit |
| Divider for Introduction and Conclusion too? | Yes, all five parts get a `#` divider with a one-line question | Self-check asks for five parts with dividers |
| Second poll? | Yes – "Where should your project start?" with the five investment areas as options | Turns the call to action into a short application step (Gagné practice); max. two polls respected |
| PRÜFEN "Teaching Agent / how this keynote was drafted" | Teaching Agent example kept on the co-pilot slide; "drafted in three ways" left out of the slide, kept in the `PRÜFEN` comment | Source says "decide whether to mention" – the speaker decides |
| Speaker notes for reveal steps | Added `--{{n}}--` for every `{{n}}` in addition to `--{{0}}--` | `validate-syntax` check 6; notes stay 2–4 sentences each |
| Time cues | `<!-- time: … -->` comments on divider slides, not in notes | Notes are read by the narrator |
| Step 1b / Step 3 images | Skipped | AUTOPILOT: no image generation, no image files |
| Escalation to `:coauthor-materials` | Not needed | All fixes were isolated quick-fixes |
