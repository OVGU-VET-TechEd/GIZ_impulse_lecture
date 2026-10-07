# Task – improve an offline draft (unattended)

`README.md` is a LiaScript keynote drafted offline by a local model (qwen3.8:27b) with the Teaching-Agent.
Your job: **improve this draft into a finished keynote – do not start from scratch.** Keep its structure,
slide order and good passages; change what is needed. Work unattended, ask nothing.

Binding: `inputs/rahmen.md` (audience, tone, time budget, structure, header, format).
Only fact base: `inputs/quelle_keynote.md`. Lint result of the draft: `inputs/lint.txt`.

Fix in particular:
1. **Keynote, not fact sheet:** the draft copies the fact base nearly verbatim. Cut bullets, one idea per slide,
   max ~5 short lines visible per reveal step; move detail into the speaker notes.
2. **Plain English:** replace jargon (e.g. calibrate, troubleshoot, escalate, purpose limitation, value chain without
   explanation) with plain words, or explain once in one line.
3. **Invent nothing:** remove claims not in the fact base (e.g. "already visible in partner countries");
   label own illustrations "Example:" or "Imagine …"; keep every `PRÜFEN` as `<!-- PRÜFEN: … -->`.
4. Title slide must show speaker name, institution and event on the slide, not only in the notes.
5. Speaker notes: every slide, every reveal step has a matching `--{{n}}--` note placed directly after its block;
   no note for a step that does not exist; notes are what the speaker says (2–4 sentences, warm, concrete).
6. A stronger human thread: a few concrete people (job-seeker, technician, teacher, learner) instead of abstract lists.
7. Keep 14–18 slides, both polls (options `- [(n)]`, not indented), three take-aways and a concrete call to action.

Write the result back to `README.md`. Then write `improve_report.md` (max 25 lines): what you changed and why,
what you kept from the draft, and the share of the draft you estimate you kept (%).
