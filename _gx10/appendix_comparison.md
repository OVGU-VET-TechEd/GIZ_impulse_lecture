

<!-- ===== APPENDIX – added afterwards by Claude Code, not part of the agent run that produced this deck ===== -->

# Behind the scenes: one keynote, built three ways

**Same brief, same fact sheet, same open-source Teaching Agent – three ways of running it.**

                --{{0}}--
This keynote practises what it preaches. I built it with an open-source Teaching Agent, in three ways: offline on our own university server, with a commercial cloud AI, and offline first with the cloud AI improving the draft. Here is what that cost and what it gave.


## Three routes

```ascii
               brief + fact sheet + Teaching Agent  (same for all three)
                                  |
        +-------------------------+-------------------------+
        |                         |                         |
   V1 OFFLINE                V2 CLOUD ONLY            V3 OFFLINE + CLOUD
   local open model          Claude Opus 5.5          V1 draft, then Claude
   on the university         builds the whole         improves it (one
   AI server (GX10)          keynote                  editing session)
        |                         |                         |
   46 min, no cloud           4 min, all in            46 min offline
   tokens, data stays         the cloud                + 3 min cloud
   on campus
```

                --{{0}}--
All three started from the same written brief and the same fact sheet. Only the engine changed: a free open model on a desktop-sized server at our university, a commercial cloud model, or both one after the other.


## Token usage and effort (measured)

| | V1 Offline (GX10) | V2 Cloud only (Claude) | V3 Offline + Claude improve |
| --- | --- | --- | --- |
| Model | qwen3.8:27b, local | Claude Opus 5.5 | qwen3.8:27b → Claude Opus 5.5 |
| Runtime | 46 min (23 steps) | 4.2 min (38 turns) | 46 min + 2.9 min (12 turns) |
| Local model tokens (in / out) | 947 k / 35 k | – | 947 k / 35 k |
| Claude fresh input + cache write | 0 | 162 k | 41 k |
| Claude cache reads | 0 | 1.19 M | 0.32 M |
| Claude output (incl. thinking) | 0 | 35.8 k (13.9 k) | 18.5 k (6.9 k) |
| **Claude input-token equivalents¹** | **0** | **≈ 459 k** | **≈ 165 k (–64 %)** |
| Claude list price | 0 € | ≈ 2.25 USD | ≈ 0.76 USD |
| Syntax errors (lint) | 0 | 0 | 0 |
| Slides | 17 | 18 | 18 |

<small>¹ Weighting as in the GX10 wiki: fresh input/cache write × 1, cache read × 0.1, output × 5. Not included and the same for all three: preparing brief and fact sheet (≈ 150 k equivalents, estimated) and the human review before the talk.</small>

                --{{0}}--
The numbers are measured from the logs. The offline run used almost a million tokens of model work, but none of them cost cloud tokens. Improving the offline draft took about a third of the cloud effort of writing the keynote directly with the cloud model.


## Pros and cons

| | Pros | Cons |
| --- | --- | --- |
| **V1 Offline** | no cloud cost · data never leaves the university · clean syntax · follows the brief and the fact sheet faithfully | slow (46 min) · reads like the fact sheet, copied almost word for word · jargon kept · crowded slides · small claims nobody asked for · its own self-check said "all fine" and gave a wrong date |
| **V2 Cloud only** | best keynote straight away · plain words and clear tables · self-review caught jargon · ready in 4 min | highest cloud cost · all material goes to a cloud provider · still needs the speaker's review |
| **V3 Offline + improve** | quality on the level of V2, with a thread of people (Amina, Grace, Joseph, Sara) and a concrete call to action · ≈ 64 % fewer cloud tokens than V2 · offline part can run overnight | two steps, ≈ 50 min in total · only about 55 % of the offline draft survived · the draft still goes to the cloud for improvement |

                --{{0}}--
The pattern is the same one we saw for skilled workers. The local model does the heavy, routine part. A stronger system and finally a human check, shorten and make it human. None of the three versions was ready without that last human look.


## What this means for GIZ projects

- **Local open models are good enough for first drafts** – and keep sensitive data in the country.
- **Quality comes from the improvement step** – by a stronger model *and* by people.
- **Mix and match:** offline for volume and privacy, cloud for polish – it costs about a third.
- **Never trust the AI's own quality report** – check it yourself.

                --{{0}}--
For partner institutions this is encouraging. A small local AI server can do much of the routine work at no running cost, and data stays at home. The polish, and the responsibility, stay with people.
