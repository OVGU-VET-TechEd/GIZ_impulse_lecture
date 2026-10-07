# AI in TVET and Employment Promotion – Applying AI Sensibly

Impulse keynote (12–15 min, virtual) for the GIZ TVET and Labour Market community.
**Hannes Tegelbeckers**, Otto von Guericke University Magdeburg – Engineering pedagogy and technical education.

## ▶ Open the presentation

| Format | Link |
| --- | --- |
| **▶ Run the presentation directly** (interactive web) | **https://ovgu-vet-teched.github.io/GIZ_impulse_lecture/presentation.html** |
| Overview page (all versions, LiaScript examples) | https://ovgu-vet-teched.github.io/GIZ_impulse_lecture/ |
| Behind the scenes: one keynote built three ways | https://ovgu-vet-teched.github.io/GIZ_impulse_lecture/behind-the-scenes.html |
| **LiaScript version** (V3 + interlude “A new way to talk to computers”) | **https://ovgu-vet-teched.github.io/GIZ_impulse_lecture/liascript.html** · [direct LiaScript link](https://liascript.github.io/course/?https://raw.githubusercontent.com/OVGU-VET-TechEd/GIZ_impulse_lecture/main/keynote.md) |
| LiaScript – V3 as generated (offline draft + cloud polish) | [open in LiaScript](https://liascript.github.io/course/?https://raw.githubusercontent.com/OVGU-VET-TechEd/GIZ_impulse_lecture/main/V3_GX10_Claude_improved/README.md) |
| LiaScript – V2 (cloud only) | [open in LiaScript](https://liascript.github.io/course/?https://raw.githubusercontent.com/OVGU-VET-TechEd/GIZ_impulse_lecture/main/V2_Claude/README.md) |
| LiaScript – V1 (offline only, local GX10 server) | [open in LiaScript](https://liascript.github.io/course/?https://raw.githubusercontent.com/OVGU-VET-TechEd/GIZ_impulse_lecture/main/V1_Offline_GX10/README.md) |

Any LiaScript file in this repo opens with `https://liascript.github.io/course/?` followed by the raw GitHub URL of the file.

### Using the web presentation

- `←` `→` / space / presenter clicker: next build or slide · `N`: speaker notes · `F`: full screen
- “All builds” shows every slide fully (default on phones) · ◐ switches light/dark
- Deep link to a slide with `#<number>`, e.g. `…/GIZ_impulse_lecture/presentation.html#9`

## Structure of the talk

1. **Setting the scene** – AI arrives quietly · poll · *apply, don't build*
2. **Interlude: a new way to talk to computers** – click → code → prompt · offline vs online AI · *the AI never touches the computer* (step-through of a real agent run)
3. **Pillar 1 – Data for labour market analysis** – job ad → decision (skill-finder demo) · data sovereignty · the informal sector (ILO dot grid)
4. **Pillar 2 – Training *for* AI-supported systems** – Grace's leak-detection game · three skill levels · task sorter + [IAB Job-Futuromat](https://job-futuromat.iab.de)
5. **Pillar 3 – Training humans *with* AI** – Joseph's AI tutor · OER · co-pilot, not autopilot (spot-the-error)
6. **Conclusion** – where GIZ should invest · three take-aways · call to action · links to play with

All interactive elements run in the browser; no data is sent anywhere and no AI service is called.

## Repository content

| Path | Content |
| --- | --- |
| `index.html` | Overview page (GitHub Pages start page) with links to all presentations |
| `presentation.html`, `assets/` | Interactive web presentation |
| `keynote.md`, `liascript.html` | Final LiaScript keynote (V3 + interlude, quiz on agent permissions) and the Pages link that opens it in LiaScript |
| `behind-the-scenes.html` | Comparison of the three production routes: runtime, tokens, cost, pros and cons |
| `V1_Offline_GX10/README.md` | LiaScript keynote drafted fully offline by the open-source Teaching Agent with a local open model (qwen3.8:27b on a GX10 server) |
| `V2_Claude/README.md`, `V2_Claude/_run/` | Same brief, built with a cloud model (Claude Opus 5.5) – plus journal and agent report |
| `V3_GX10_Claude_improved/README.md`, `…/_run/` | V1 draft improved in one cloud editing session – plus improvement report |
| `_gx10/` | Job configuration, task and full logs of the offline run; `appendix_comparison.md` |

## Licence

Text and slides: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) · Code (`*.html`, `assets/`): MIT – unless stated otherwise.
