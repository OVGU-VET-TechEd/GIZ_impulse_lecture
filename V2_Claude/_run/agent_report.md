# Agent report – `:build-session 1 keynote` (autopilot, 2026-10-06)

**Output:** `materials/01-giz-keynote/README.md` · 18 slides · English · no images

## Steps

| Step | What happened |
| --- | --- |
| Activation | Read `AUTOPILOT.md`, `inputs/rahmen.md` and `inputs/quelle_keynote.md` first, then `journal.md`. Read only these specs: `build-session`, `promote-session`, `validate-course`, `validate-syntax`, `review-as-persona`, `duration-heuristic`, and the relevant parts of `didactic-methods` (gagne) and the cheat sheet. `specs/course-input/fd2` belongs to a different course and was not used. |
| 0 Skeleton | Already present (✅). |
| 1a Promote | Material generated with the 5-part structure from the rahmen. No `### Coauthor` role → used Professor Persona / Teaching Style instead. |
| 1b Images | Skipped (AUTOPILOT: no image generation). |
| 1c–d Content loop | **Iteration 1:** FAIL. The note on the investment-poll slide had 5 sentences (limit is 2–4), and one note assumed the poll result ("Look at the results: most …"). Quick-fixed. **Iteration 2:** PASS. That fix pushed the opening-poll note to 5 sentences, so it was merged back to 4 and rechecked. |
| 2 Persona review | Amina, report-only mode. **Round 1:** 2 blocking issues: jargon in Pillar 2 (calibrate, troubleshoot, configure, escalate) and "open AI models" misread as the company OpenAI. Quick-fixed, then step 1 rechecked (still PASS). **Round 2:** OK, no blocking issue. |
| 3 Images | Skipped (none planned). |
| 4 Finalize | Session marked ✅ Done; Agenda status ✅; Dashboard, Validation Report, Persona Review and Notes Backup written into `journal.md`. |

Iterations: content loop 2 of 2, persona loop 2 of 2. Caps were respected. No escalation to `:coauthor-materials` was needed.

## Validation (session mode): PASS with concerns

- Header identical to the rahmen. 18 slides: title, then 5 `#` dividers each with a one-line question, then `##` content slides. Parts are in order: Scene, Pillar 1, Pillar 2, Pillar 3, Conclusion.
- Every slide has a `--{{0}}--` note. Every `{{n}}` reveal has a matching `--{{n}}--` note. Note text is never indented. Notes are 2–4 sentences each.
- 2 surveys (opening "Where did you meet AI this week?", closing "Where should your project start?"). Options are `- [(n)]` and not indented. There is no graded quiz.
- One `ascii` diagram (the value chain). The only HTML used is `<section>`, `<small>` and comments.
- Duration estimate is about 13–14 minutes: roughly 1,500 words of notes at 130 words per minute, plus the two polls. This is a hand count; the automated check script could not run here (Bash was not approved), so all checks were done with Grep and by reading the file.
- Concerns:
  1. 6 `#` headings instead of 1. This is an accepted deviation because the rahmen requires the part dividers.
  2. The `- [(n)]` list form for surveys differs from the cheat sheet. Check it once in the LiaScript preview.
  3. `[pedagogical]` Gagné "practice with feedback" is only partly met. This is normal for a keynote: the second poll is the application step.

## Persona review: Amina

The final result is **OK**. She liked "Apply, don't build", data sovereignty, the informal sector point and the investment poll. One point is open but not blocking: "What does a small first pilot cost?" The source has nothing on this, so it was left out. It is a good question for the conference discussion.

## Decisions (also in `journal.md` → `## Notes Backup`)

- `#` dividers and the `- [(n)]` survey form follow the rahmen, which overrides the generic syntax rules.
- There is a divider with a question for all five parts, not only the three pillars.
- To stay within 18 slides, the AI definition is revealed on the opening poll slide, and the take-aways slide doubles as the closing slide.
- A second poll is used for the call to action: the five investment areas are the poll options.
- Notes were added for every reveal step. Time cues are HTML comments only, because the narrator reads the notes aloud.
- The Teaching Agent example is on the co-pilot slide. The "this keynote was drafted in three ways" detail stays only in a `PRÜFEN` comment, because the source says the speaker should decide.

## Cuts (source content not used on slides)

- The detailed list of UNESCO framework areas: "AI techniques and applications" and "system design" are not shown. Only "human-centred mindset and ethics" appear, in the notes.
- "This very keynote was drafted with it in three ways …": left in the PRÜFEN comment only.
- The opening examples "voice messages transcribed" and "route planning" appear only as poll options; there is no separate slide for them.
- No new facts were added. Own illustrations are labelled "Imagine …" or "Example (illustrative)": the plumber in Nairobi, the learner on her phone, and the three technical workplaces from the source.

## Open PRÜFEN items (2)

1. **ILO figures** (slide *The blind spot: the informal sector*): about 2 billion informal workers, roughly 6 in 10 worldwide, around 85 % in Africa. Check against the latest ILO data.
2. **Teaching Agent** (slide *Co-pilot, not autopilot*): decide whether to mention the example, and whether to say that this keynote was drafted with it.

## Next steps for the instructor

1. Resolve both PRÜFEN items.
2. Open the file in the LiaScript preview once (survey rendering, presentation mode).
3. Run `:validate-course` (course mode) before publishing, then use `:agent development`.
