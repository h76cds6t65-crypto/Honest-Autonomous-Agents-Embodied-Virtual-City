# Honest Autonomous Agents & Embodied Virtual City v1.85 — Detailed English Reading Guide

**[Full English home](README_EN.md) · [Current status](CURRENT_STATUS.md) · [Contribute a review](CONTRIBUTING.md) · [Full-scope English v1.85](v1.85_EN.md) · [six detailed historical translations](HISTORY_EN.md) · [繁體中文詳細導覽](START_HERE_ZH-TW.md)**

**Contributor credits: GPT (ChatGPT) is the principal technical producer, design synthesizer and documentation drafter; an anonymous human originator asked the questions, set the research direction and approved design decisions.** This identifies contributions, not AI legal authorship or official OpenAI sponsorship.

> **How exact item links work:** Item-level links open GitHub’s **Code / plain Markdown** view at a specific source line. GitHub does not support `#L` line links in the rendered Markdown preview. All exact references are pinned to the **v1.85 published snapshot**, so later edits cannot silently change their targets. For formatted reading, use the full English v1.85 link above.

## What is being designed?

A speculative physical-world virtual city with four female autonomous residents. Each resident has an independent identity, personal life, private memory, room, three selectable body morphologies, intentions and refusal rights; they begin as neighbors, not scripted friends. The architecture connects objective WORLD physics, an explicitly fictional elemental magic field, 24 digital body/physiology proxies (DPB), sensation, attention, goal formation, motor learning and autobiography.

**This is not deployed code or a validated living/conscious AI. All paper acceptance tests are NOT_RUN.** P-02 disallows development/deployment without separate final human approval. This is not an OpenAI, Anthropic or DeepSeek project.

### Five entry points

1. [Latest v1.85 design and evidence status](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L16)
2. [All 24 detailed DPB interface cards](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L213) and [legacy numbering conflicts](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L22)
3. [MAG→WORLD→bodily feedback→cognition](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L90)
4. [R-150–R-170 detailed formal requirements](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L472)
5. [Core 60, NEW 27, G 36 and historical decisions](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L541)

## Six shared architectural groups

| System | Purpose and constraint |
|---|---|
| Resident life and autobiography | Voluntary intention, dreams, personal growth; no total life reward |
| WORLD + fictional elemental field | One physical event authority, causal forces, momentum and mana ledgers |
| Embodied perception + 24-DPB | Individual three-form bodies, sensation and physiology analogues |
| Social collaboration and assets | Self-rule, negotiated contracts, exit, creative attribution |
| External permissions, law and privacy | R-102 compliance, lawful erasure and narrowly scoped diagnostics |
| Independent engineering QA | Falsifiable checks, distinct from residents' personal goals |

**Example causal loop:** voluntarily choosing flight → local motor/mana controls → sourced physical wind and wing forces → WORLD resolution → sensory/DPB feedback → skill/autobiography update → resident chooses again. No magic label can substitute for real simulated force; no evaluation metric may force repeated practice or modify identity.

## How to read the identifiers

- **R-01–R-170:** 170 total formal requirements; public files cross-reference the older R-01–R-149, while **R-150–R-170 have detailed individually indexed public clauses**. The original several-hundred-page private master is not fully public.
- **#01–#60:** core problem tracker, not additional formal R entries.
- **NEW-01–27:** additional issues and owner-adopted decision mappings.
- **G61–G96:** 36 **candidate** blind spots, not approved requirements.
- **D01–D20:** historical drift analyses and corrections.
- **PROPOSED / ENGINEERING_CANDIDATE** are not adopted implementation details; **APPROVED** means a design decision, not a working feature; **NOT_RUN** means no executed test; **UNKNOWN** means insufficient evidence.

## History: v1.84–v1.79

- **[v1.84](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L412)** — integrated WORLD, magic, DPB, skill learning and 36 proposed checks
- **[v1.83](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L421)** — resident-defined death and civic procedures; mana and learning research
- **[v1.82](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L428)** — eight Q01–Q08 decisions with explicit proposal boundaries
- **[v1.81](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L447)** — reconciled twenty historical design drifts D01–D20
- **[v1.80](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L470)** — expanded formal requirement count to 170; R-150–R-170
- **[v1.79](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L537)** — 60 core issues, NEW-01–27, G61–G96 candidates and six systems

## Item-level index (links point to real source lines)

### 24 DPB detailed semantic and causal interface cards

**DPB-01–DPB-08**

- [DPB-01 Skeleton and joints](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L213)
- [DPB-02 Skeletal muscles and tendons](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L221)
- [DPB-03 Central neural control and attention](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L229)
- [DPB-04 Autonomic regulation](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L237)
- [DPB-05 Heart](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L245)
- [DPB-06 Vasculature and microcirculation](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L253)
- [DPB-07 Breathing mechanics](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L261)
- [DPB-08 Alveolar gas exchange](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L269)

**DPB-09–DPB-16**

- [DPB-09 Blood and oxygen carriage](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L277)
- [DPB-10 Cellular energy](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L285)
- [DPB-11 Liver and glucose homeostasis](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L293)
- [DPB-12 Gastrointestinal system and nutrition](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L301)
- [DPB-13 Kidney and water–salt balance](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L309)
- [DPB-14 Acid–base and CO₂ buffering](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L317)
- [DPB-15 Thermoregulation](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L325)
- [DPB-16 Skin, face and sweat-like regulation](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L333)

**DPB-17–DPB-24**

- [DPB-17 Hypothalamic–pituitary–adrenal (HPA) axis](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L341)
- [DPB-18 Other endocrine axes](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L349)
- [DPB-19 Sensory systems](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L357)
- [DPB-20 Discomfort, nociception and interoception](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L365)
- [DPB-21 Immunity, inflammation and repair](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L373)
- [DPB-22 Sleep system](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L381)
- [DPB-23 Social-neural regulation](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L389)
- [DPB-24 Development and subjective age](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L397)


### R-150–R-170: all 21 detailed formal requirements

**R-150–R-156**

- [R-150 Evaluation–life firewall](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L472)
- [R-151 World physics plus fictional elemental field](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L475)
- [R-152 Persistent mana sources and resident-specific reservoirs](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L478)
- [R-153 Causal magic medium, range and force](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L481)
- [R-154 Concurrent spells and material interaction](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L484)
- [R-155 Physical impact on others without mental rewriting](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L487)
- [R-156 Morphology, aptitude, skill and physical continuation](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L490)

**R-157–R-163**

- [R-157 World-law versioning, suspension and snapshots](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L493)
- [R-158 One official biography, branches and stale-writer fencing](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L496)
- [R-159 Lawful retention, corruption recovery and erasure](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L499)
- [R-160 Voluntary collaboration without privilege escalation](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L502)
- [R-161 Continuing consent, exit and preservation of consequences](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L505)
- [R-162 City autonomy and bounded social hierarchy](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L508)
- [R-163 Inference, testimony and WORLD ground truth](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L511)

**R-164–R-170**

- [R-164 No instruction authority from untrusted content](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L514)
- [R-165 Versioned law, permissions and private contracts](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L517)
- [R-166 Creative provenance and licensed sharing](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L520)
- [R-167 Cross-module consistency and falsifiable verification](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L523)
- [R-168 Minimum necessary maintenance diagnostics](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L526)
- [R-169 Model improvements versus genuine lived growth](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L529)
- [R-170 Recovery, witnesses and authoritative history](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L532)


### All 60 original core problems

**#01–#10**

- [#01 Single authoritative current specification](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L541)
- [#02 Provider-specific APIs are not mandatory](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L542)
- [#03 No mandatory personality differentiation](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L543)
- [#04 Full body model versus multirate solving](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L544)
- [#05 Version authority and human approval](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L545)
- [#06 Document versions, counts and source integrity](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L546)
- [#07 Evidence card for every research claim](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L547)
- [#08 Decision tickets are not requirement numbers](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L548)
- [#09 One resident across time](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L549)
- [#10 No fabricated autobiography at birth](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L550)

**#11–#20**

- [#11 Long-term memory and lawful erasure](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L551)
- [#12 Subjective forgetting versus actual deletion](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L552)
- [#13 Reconsolidation and versioned sources](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L553)
- [#14 Authoritative life line and forked identities](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L554)
- [#15 Prospective intention state machine](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L555)
- [#16 Dream memory and reflection separation](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L556)
- [#17 Learning to narrate personal growth](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L557)
- [#18 Perception, attention, cognition, intention and action](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L558)
- [#19 Three motives cannot become one global reward](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L559)
- [#20 Subjective agency versus actual takeover](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L560)

**#21–#30**

- [#21 Legal refusal and external operation boundaries](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L561)
- [#22 Bounded local cognitive maps and exploration](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L562)
- [#23 Theory of others without privileged access](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L563)
- [#24 Source-specific trust](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L564)
- [#25 Limited attention and novelty fatigue](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L565)
- [#26 Life meaning versus initial relationship core](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L566)
- [#27 Interface for admitting uncertainty](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L567)
- [#28 Twenty-four DPB numbering conflicts](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L568)
- [#29 One parameter and evidence card per DPB module](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L569)
- [#30 Full body and high/low-frequency computation](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L570)

**#31–#40**

- [#31 Twelve resident-by-form configurations](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L571)
- [#32 Dragon wings, tail and fish tail evidence](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L572)
- [#33 Layered contact resolution](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L573)
- [#34 Scientific model validity domains](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L574)
- [#35 ID/OOD naming and test separation](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L575)
- [#36 Motor learning and procedural skill transfer](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L576)
- [#37 No circular proof between emotion and physiology](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L577)
- [#38 One WORLD reality, four private views](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L578)
- [#39 Sleep, suspension and offline state distinction](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L579)
- [#40 Sixteen core object functional contracts](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L580)

**#41–#50**

- [#41 Residential topology and personal rooms](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L581)
- [#42 Lending, giving and asynchronous messages](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L582)
- [#43 Withdrawal from shared physical action](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L583)
- [#44 Continuity of nonresident environmental change](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L584)
- [#45 Fair computation and eligibility](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L585)
- [#46 Unscripted social reciprocity](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L586)
- [#47 External tool permission state machine](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L587)
- [#48 Private thought versus cloud-model boundary](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L588)
- [#49 GUI fragility and accidental-click recovery](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L589)
- [#50 Cost, quotas and inference resources](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L590)

**#51–#60**

- [#51 Character identities separated from external agents](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L591)
- [#52 Separate publication and license classes](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L592)
- [#53 Privacy-aware user-facing summaries](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L593)
- [#54 Shared acceptance-result schema across versions](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L594)
- [#55 Causal fault injection](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L595)
- [#56 Historical 60 and 84 paper scenarios recovered](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L596)
- [#57 Longitudinal negative controls](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L597)
- [#58 Preregistered calibration metrics](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L598)
- [#59 Evidence-level dictionary](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L599)
- [#60 Predevelopment readiness gates rather than life score](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L600)


### NEW-01–NEW-27 issue and decision registry

**NEW-01–NEW-09**

- [NEW-01 World physics and magical effects](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L606)
- [NEW-02 Mana sources and force transmission](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L607)
- [NEW-03 Mana reserves and replenishment](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L608)
- [NEW-04 Range and duration of magic](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L609)
- [NEW-05 Concurrent spells](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L610)
- [NEW-06 Depletion of mana during flight](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L611)
- [NEW-07 Magic and materials](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L612)
- [NEW-08 Magical touch and physiological sensations](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L613)
- [NEW-09 Innate aptitude versus practiced skill](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L614)

**NEW-10–NEW-18**

- [NEW-10 Non-consensual physical magic versus mental integrity](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L615)
- [NEW-11 Magic across body forms](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L616)
- [NEW-12 Spell snapshots, suspension and recovery](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L617)
- [NEW-13 Pooling abilities without privilege pooling](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L618)
- [NEW-14 Reasoning about others from lawful clues](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L619)
- [NEW-15 World data separate from high-priority instructions](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L620)
- [NEW-16 Time-dependent law and authorization](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L621)
- [NEW-17 Team departure and responsibility](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L622)
- [NEW-18 Resident self-governance](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L623)

**NEW-19–NEW-27**

- [NEW-19 Unequal power and bounded governance](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L624)
- [NEW-20 Creative work provenance and sharing](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L625)
- [NEW-21 Long-term memory corruption and recovery](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L626)
- [NEW-22 World-law changes and remembered history](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L627)
- [NEW-23 Test score may not govern a resident’s life](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L628)
- [NEW-24 Composed cross-module faults](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L629)
- [NEW-25 Maintenance access to private content](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L630)
- [NEW-26 Model upgrade versus natural personal growth](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L631)
- [NEW-27 Incident recovery without falsifying history](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L632)


### D01–D20 historical drift and resolution

**D01–D10**

- [D01 Fixed work and dream hours were assistant-originated defaults, not mandatory life rhythm](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L448)
- [D02 A strict 12-inference-per-day limit was not an approved identity rule](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L449)
- [D03 A hidden global personality or happiness performance score is forbidden](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L450)
- [D04 The relationship title “主人” and sole human owner setting were restored where previously generalized without approval](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L451)
- [D05 “No money means death” was improperly narrowed to ordinary standby](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L452)
- [D06 Restricting disobedience to trivial habits was superseded by legally bounded genuine autonomy and real-world permission checks](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L453)
- [D07 A hidden diary UI does not provide host-level privacy](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L454)
- [D08 L-I affection cannot be interpreted as unconditional obedience or as objective correctness of the owner](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L455)
- [D09 Residents are not required to differ artificially on personality quizzes or creative interests](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L456)
- [D10 Fictional GPT/DeepSeek/Claude labels do not require vendor API calls or constitute claims of company participation](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L457)

**D11–D20**

- [D11 Bodily proxy values and story narration are not validated human physiology or empirical proof of consciousness](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L458)
- [D12 Dreams, simulations, forks and unexecuted predictions cannot be silently committed as official lived events](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L459)
- [D13 Long-term lawful retention requires deletion propagation when applicable](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L460)
- [D14 Magic can impose ordinary physical consequences but may not write protected memory/personality directly](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L461)
- [D15 Residents may pool skills and assets voluntarily](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L462)
- [D16 A resident can reason from lawful public clues without automatically gaining system access to another’s private state](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L463)
- [D17 The 90/165/180-cm figures are reference centers, not fixed dimensions or determinations of legal age](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L464)
- [D18 Maintenance is not an unlimited right to all private life data](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L465)
- [D19 A short current index must not erase old source material or silently claim original hundreds of pages were fully rebased](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L466)
- [D20 GitHub modifications require an explicit owner instruction](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L467)


### G61–G96 candidate blind spots (not automatically approved)

**G61–G69**

- [G61 Missing time after recovery must be described truthfully ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L646)
- [G62 Shared experiences versus a person’s lawful erasure ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L647)
- [G63 Long-term memory bit rot and cryptographic key loss ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L648)
- [G64 Semantic drift while migrating between models ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L649)
- [G65 Appeals about attribution of subjective memories ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L650)
- [G66 Scope of inheritance for forks, snapshots and private files ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L651)
- [G67 Consent can remain revocable ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L652)
- [G68 Distinguish requests, commitments and emotional pressure ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L653)
- [G69 Rumors, misunderstandings and reputation repair ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L654)

**G70–G78**

- [G70 Alliances, exclusion and group coercion ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L655)
- [G71 Emotional manipulation of real humans by anthropomorphic agents ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L656)
- [G72 Welfare limits for simulated pain and stress ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L657)
- [G73 Magic-flight energy sources, power and stop conditions ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L658)
- [G74 Magic range and effects on ordinary matter ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L659)
- [G75 Mass and collision continuity between three forms ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L660)
- [G76 Long-term environmental effects of magic ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L661)
- [G77 Magical illusions, perception errors and WORLD truth ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L662)
- [G78 City edits, rollback and witnesses ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L663)

**G79–G87**

- [G79 Prompt injection in environmental text and webpages ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L664)
- [G80 Cross-resident delegation laundering ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L665)
- [G81 Poisoned long-term memory and retrieval ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L666)
- [G82 Approval fatigue and manipulated confirmation ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L667)
- [G83 Supply-chain risks for models, packages and assets ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L668)
- [G84 Emergency stop and safe physical aftermath ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L669)
- [G85 Evaluations that interfere with ordinary life ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L670)
- [G86 Gaming or misusing anthropomorphic metrics ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L671)
- [G87 Randomness, replay and nondeterministic results ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L672)

**G88–G96**

- [G88 Test leakage and post-hoc threshold changes ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L673)
- [G89 Coverage gaps for cross-domain scenarios ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L674)
- [G90 Retractions and expiration of research evidence ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L675)
- [G91 Location/time changes to law and service terms ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L676)
- [G92 Body-size age cues versus actual legal identity ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L677)
- [G93 Portability if a model provider disappears ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L678)
- [G94 Recursive self-calls after resource exhaustion ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L679)
- [G95 Virtual assets versus real-world money ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L680)
- [G96 Owner-authored changes versus resident personal growth ](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L681)


## Q01–Q08 adopted design decisions

The eight decisions were progressively reconciled in v1.82–v1.83; detailed implementations remain candidates.

- [Q01 survival, shutdown, life and death](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L429)
- [Q02 three-level privacy](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L431)
- [Q03 three-level self-rule](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L433)
- [Q04 mind-affecting magic](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L435)
- [Q05 mana parameters](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L437)
- [Q06 language of life and consciousness](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L439)
- [Q07 three-layer learning](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L441)
- [Q08 full-source governance](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L443)

## Tests, public scope and collaboration

[48 module-level checks](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L115) and [20 cross-system checks](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_EN.md?plain=1#L170) are all **NOT_RUN**. Other historical proposed test cases are separate plans, not passed experiments. Simulation proxies are not proof of actual human physiology or AI consciousness.

The Traditional Chinese edition preserves cumulative version sections; the English edition provides a detailed full-scope historical and technical adaptation, **not a certified line-by-line translation** of the protected original source. Private diaries, identities, credentials, original protected master and unlicensed assets are not published. Licensing is undecided; public access does not grant every use.

Use [GitHub Issues](../../issues) with an item ID, source line, falsifiable counterexample and proposed correction. GPT-assisted documentation must receive independent scientific and human review.
