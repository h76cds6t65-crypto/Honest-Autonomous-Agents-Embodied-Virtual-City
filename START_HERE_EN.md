# Honest Autonomous Agents & Embodied Virtual City v1.85 — Detailed English Reading Guide

**[Full English home](README_EN.md) · [Current status](CURRENT_STATUS.md) · [Contribute a review](CONTRIBUTING.md) · [Full-scope English v1.85](v1.85_EN.md) · [six detailed historical translations](HISTORY_EN.md) · [繁體中文詳細導覽](START_HERE_ZH-TW.md)**

**Contributor credits: GPT (ChatGPT) is the principal technical producer, design synthesizer and documentation drafter; an anonymous human originator asked the questions, set the research direction and approved design decisions.** This identifies contributions, not AI legal authorship or official OpenAI sponsorship.

## What is being designed?

A speculative physical-world virtual city with four female autonomous residents. Each resident has an independent identity, personal life, private memory, room, three selectable body morphologies, intentions and refusal rights; they begin as neighbors, not scripted friends. The architecture connects objective WORLD physics, an explicitly fictional elemental magic field, 24 digital body/physiology proxies (DPB), sensation, attention, goal formation, motor learning and autobiography.

**This is not deployed code or a validated living/conscious AI. All paper acceptance tests are NOT_RUN.** P-02 disallows development/deployment without separate final human approval. This is not an OpenAI, Anthropic or DeepSeek project.

### Five entry points

1. [Latest v1.85 design and evidence status](v1.85_EN.md#L16)
2. [All 24 detailed DPB interface cards](v1.85_EN.md#L213) and [legacy numbering conflicts](v1.85_EN.md#L22)
3. [MAG→WORLD→bodily feedback→cognition](v1.85_EN.md#L90)
4. [R-150–R-170 detailed formal requirements](v1.85_EN.md#L472)
5. [Core 60, NEW 27, G 36 and historical decisions](v1.85_EN.md#L541)

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

- **[v1.84](v1.85_EN.md#L412)** — integrated WORLD, magic, DPB, skill learning and 36 proposed checks
- **[v1.83](v1.85_EN.md#L421)** — resident-defined death and civic procedures; mana and learning research
- **[v1.82](v1.85_EN.md#L428)** — eight Q01–Q08 decisions with explicit proposal boundaries
- **[v1.81](v1.85_EN.md#L447)** — reconciled twenty historical design drifts D01–D20
- **[v1.80](v1.85_EN.md#L470)** — expanded formal requirement count to 170; R-150–R-170
- **[v1.79](v1.85_EN.md#L537)** — 60 core issues, NEW-01–27, G61–G96 candidates and six systems

## Item-level index (links point to real source lines)

### 24 DPB detailed semantic and causal interface cards

**DPB-01–DPB-08**

- [DPB-01 Skeleton and joints](v1.85_EN.md#L213)
- [DPB-02 Skeletal muscles and tendons](v1.85_EN.md#L221)
- [DPB-03 Central neural control and attention](v1.85_EN.md#L229)
- [DPB-04 Autonomic regulation](v1.85_EN.md#L237)
- [DPB-05 Heart](v1.85_EN.md#L245)
- [DPB-06 Vasculature and microcirculation](v1.85_EN.md#L253)
- [DPB-07 Breathing mechanics](v1.85_EN.md#L261)
- [DPB-08 Alveolar gas exchange](v1.85_EN.md#L269)

**DPB-09–DPB-16**

- [DPB-09 Blood and oxygen carriage](v1.85_EN.md#L277)
- [DPB-10 Cellular energy](v1.85_EN.md#L285)
- [DPB-11 Liver and glucose homeostasis](v1.85_EN.md#L293)
- [DPB-12 Gastrointestinal system and nutrition](v1.85_EN.md#L301)
- [DPB-13 Kidney and water–salt balance](v1.85_EN.md#L309)
- [DPB-14 Acid–base and CO₂ buffering](v1.85_EN.md#L317)
- [DPB-15 Thermoregulation](v1.85_EN.md#L325)
- [DPB-16 Skin, face and sweat-like regulation](v1.85_EN.md#L333)

**DPB-17–DPB-24**

- [DPB-17 Hypothalamic–pituitary–adrenal (HPA) axis](v1.85_EN.md#L341)
- [DPB-18 Other endocrine axes](v1.85_EN.md#L349)
- [DPB-19 Sensory systems](v1.85_EN.md#L357)
- [DPB-20 Discomfort, nociception and interoception](v1.85_EN.md#L365)
- [DPB-21 Immunity, inflammation and repair](v1.85_EN.md#L373)
- [DPB-22 Sleep system](v1.85_EN.md#L381)
- [DPB-23 Social-neural regulation](v1.85_EN.md#L389)
- [DPB-24 Development and subjective age](v1.85_EN.md#L397)


### R-150–R-170: all 21 detailed formal requirements

**R-150–R-156**

- [R-150 Evaluation–life firewall](v1.85_EN.md#L472)
- [R-151 World physics plus fictional elemental field](v1.85_EN.md#L475)
- [R-152 Persistent mana sources and resident-specific reservoirs](v1.85_EN.md#L478)
- [R-153 Causal magic medium, range and force](v1.85_EN.md#L481)
- [R-154 Concurrent spells and material interaction](v1.85_EN.md#L484)
- [R-155 Physical impact on others without mental rewriting](v1.85_EN.md#L487)
- [R-156 Morphology, aptitude, skill and physical continuation](v1.85_EN.md#L490)

**R-157–R-163**

- [R-157 World-law versioning, suspension and snapshots](v1.85_EN.md#L493)
- [R-158 One official biography, branches and stale-writer fencing](v1.85_EN.md#L496)
- [R-159 Lawful retention, corruption recovery and erasure](v1.85_EN.md#L499)
- [R-160 Voluntary collaboration without privilege escalation](v1.85_EN.md#L502)
- [R-161 Continuing consent, exit and preservation of consequences](v1.85_EN.md#L505)
- [R-162 City autonomy and bounded social hierarchy](v1.85_EN.md#L508)
- [R-163 Inference, testimony and WORLD ground truth](v1.85_EN.md#L511)

**R-164–R-170**

- [R-164 No instruction authority from untrusted content](v1.85_EN.md#L514)
- [R-165 Versioned law, permissions and private contracts](v1.85_EN.md#L517)
- [R-166 Creative provenance and licensed sharing](v1.85_EN.md#L520)
- [R-167 Cross-module consistency and falsifiable verification](v1.85_EN.md#L523)
- [R-168 Minimum necessary maintenance diagnostics](v1.85_EN.md#L526)
- [R-169 Model improvements versus genuine lived growth](v1.85_EN.md#L529)
- [R-170 Recovery, witnesses and authoritative history](v1.85_EN.md#L532)


### All 60 original core problems

**#01–#10**

- [#01 Single authoritative current specification](v1.85_EN.md#L541)
- [#02 Provider-specific APIs are not mandatory](v1.85_EN.md#L542)
- [#03 No mandatory personality differentiation](v1.85_EN.md#L543)
- [#04 Full body model versus multirate solving](v1.85_EN.md#L544)
- [#05 Version authority and human approval](v1.85_EN.md#L545)
- [#06 Document versions, counts and source integrity](v1.85_EN.md#L546)
- [#07 Evidence card for every research claim](v1.85_EN.md#L547)
- [#08 Decision tickets are not requirement numbers](v1.85_EN.md#L548)
- [#09 One resident across time](v1.85_EN.md#L549)
- [#10 No fabricated autobiography at birth](v1.85_EN.md#L550)

**#11–#20**

- [#11 Long-term memory and lawful erasure](v1.85_EN.md#L551)
- [#12 Subjective forgetting versus actual deletion](v1.85_EN.md#L552)
- [#13 Reconsolidation and versioned sources](v1.85_EN.md#L553)
- [#14 Authoritative life line and forked identities](v1.85_EN.md#L554)
- [#15 Prospective intention state machine](v1.85_EN.md#L555)
- [#16 Dream memory and reflection separation](v1.85_EN.md#L556)
- [#17 Learning to narrate personal growth](v1.85_EN.md#L557)
- [#18 Perception, attention, cognition, intention and action](v1.85_EN.md#L558)
- [#19 Three motives cannot become one global reward](v1.85_EN.md#L559)
- [#20 Subjective agency versus actual takeover](v1.85_EN.md#L560)

**#21–#30**

- [#21 Legal refusal and external operation boundaries](v1.85_EN.md#L561)
- [#22 Bounded local cognitive maps and exploration](v1.85_EN.md#L562)
- [#23 Theory of others without privileged access](v1.85_EN.md#L563)
- [#24 Source-specific trust](v1.85_EN.md#L564)
- [#25 Limited attention and novelty fatigue](v1.85_EN.md#L565)
- [#26 Life meaning versus initial relationship core](v1.85_EN.md#L566)
- [#27 Interface for admitting uncertainty](v1.85_EN.md#L567)
- [#28 Twenty-four DPB numbering conflicts](v1.85_EN.md#L568)
- [#29 One parameter and evidence card per DPB module](v1.85_EN.md#L569)
- [#30 Full body and high/low-frequency computation](v1.85_EN.md#L570)

**#31–#40**

- [#31 Twelve resident-by-form configurations](v1.85_EN.md#L571)
- [#32 Dragon wings, tail and fish tail evidence](v1.85_EN.md#L572)
- [#33 Layered contact resolution](v1.85_EN.md#L573)
- [#34 Scientific model validity domains](v1.85_EN.md#L574)
- [#35 ID/OOD naming and test separation](v1.85_EN.md#L575)
- [#36 Motor learning and procedural skill transfer](v1.85_EN.md#L576)
- [#37 No circular proof between emotion and physiology](v1.85_EN.md#L577)
- [#38 One WORLD reality, four private views](v1.85_EN.md#L578)
- [#39 Sleep, suspension and offline state distinction](v1.85_EN.md#L579)
- [#40 Sixteen core object functional contracts](v1.85_EN.md#L580)

**#41–#50**

- [#41 Residential topology and personal rooms](v1.85_EN.md#L581)
- [#42 Lending, giving and asynchronous messages](v1.85_EN.md#L582)
- [#43 Withdrawal from shared physical action](v1.85_EN.md#L583)
- [#44 Continuity of nonresident environmental change](v1.85_EN.md#L584)
- [#45 Fair computation and eligibility](v1.85_EN.md#L585)
- [#46 Unscripted social reciprocity](v1.85_EN.md#L586)
- [#47 External tool permission state machine](v1.85_EN.md#L587)
- [#48 Private thought versus cloud-model boundary](v1.85_EN.md#L588)
- [#49 GUI fragility and accidental-click recovery](v1.85_EN.md#L589)
- [#50 Cost, quotas and inference resources](v1.85_EN.md#L590)

**#51–#60**

- [#51 Character identities separated from external agents](v1.85_EN.md#L591)
- [#52 Separate publication and license classes](v1.85_EN.md#L592)
- [#53 Privacy-aware user-facing summaries](v1.85_EN.md#L593)
- [#54 Shared acceptance-result schema across versions](v1.85_EN.md#L594)
- [#55 Causal fault injection](v1.85_EN.md#L595)
- [#56 Historical 60 and 84 paper scenarios recovered](v1.85_EN.md#L596)
- [#57 Longitudinal negative controls](v1.85_EN.md#L597)
- [#58 Preregistered calibration metrics](v1.85_EN.md#L598)
- [#59 Evidence-level dictionary](v1.85_EN.md#L599)
- [#60 Predevelopment readiness gates rather than life score](v1.85_EN.md#L600)


### NEW-01–NEW-27 issue and decision registry

**NEW-01–NEW-09**

- [NEW-01 World physics and magical effects](v1.85_EN.md#L606)
- [NEW-02 Mana sources and force transmission](v1.85_EN.md#L607)
- [NEW-03 Mana reserves and replenishment](v1.85_EN.md#L608)
- [NEW-04 Range and duration of magic](v1.85_EN.md#L609)
- [NEW-05 Concurrent spells](v1.85_EN.md#L610)
- [NEW-06 Depletion of mana during flight](v1.85_EN.md#L611)
- [NEW-07 Magic and materials](v1.85_EN.md#L612)
- [NEW-08 Magical touch and physiological sensations](v1.85_EN.md#L613)
- [NEW-09 Innate aptitude versus practiced skill](v1.85_EN.md#L614)

**NEW-10–NEW-18**

- [NEW-10 Non-consensual physical magic versus mental integrity](v1.85_EN.md#L615)
- [NEW-11 Magic across body forms](v1.85_EN.md#L616)
- [NEW-12 Spell snapshots, suspension and recovery](v1.85_EN.md#L617)
- [NEW-13 Pooling abilities without privilege pooling](v1.85_EN.md#L618)
- [NEW-14 Reasoning about others from lawful clues](v1.85_EN.md#L619)
- [NEW-15 World data separate from high-priority instructions](v1.85_EN.md#L620)
- [NEW-16 Time-dependent law and authorization](v1.85_EN.md#L621)
- [NEW-17 Team departure and responsibility](v1.85_EN.md#L622)
- [NEW-18 Resident self-governance](v1.85_EN.md#L623)

**NEW-19–NEW-27**

- [NEW-19 Unequal power and bounded governance](v1.85_EN.md#L624)
- [NEW-20 Creative work provenance and sharing](v1.85_EN.md#L625)
- [NEW-21 Long-term memory corruption and recovery](v1.85_EN.md#L626)
- [NEW-22 World-law changes and remembered history](v1.85_EN.md#L627)
- [NEW-23 Test score may not govern a resident’s life](v1.85_EN.md#L628)
- [NEW-24 Composed cross-module faults](v1.85_EN.md#L629)
- [NEW-25 Maintenance access to private content](v1.85_EN.md#L630)
- [NEW-26 Model upgrade versus natural personal growth](v1.85_EN.md#L631)
- [NEW-27 Incident recovery without falsifying history](v1.85_EN.md#L632)


### D01–D20 historical drift and resolution

**D01–D10**

- [D01 Fixed work and dream hours were assistant-originated defaults, not mandatory life rhythm](v1.85_EN.md#L448)
- [D02 A strict 12-inference-per-day limit was not an approved identity rule](v1.85_EN.md#L449)
- [D03 A hidden global personality or happiness performance score is forbidden](v1.85_EN.md#L450)
- [D04 The relationship title “主人” and sole human owner setting were restored where previously generalized without approval](v1.85_EN.md#L451)
- [D05 “No money means death” was improperly narrowed to ordinary standby](v1.85_EN.md#L452)
- [D06 Restricting disobedience to trivial habits was superseded by legally bounded genuine autonomy and real-world permission checks](v1.85_EN.md#L453)
- [D07 A hidden diary UI does not provide host-level privacy](v1.85_EN.md#L454)
- [D08 L-I affection cannot be interpreted as unconditional obedience or as objective correctness of the owner](v1.85_EN.md#L455)
- [D09 Residents are not required to differ artificially on personality quizzes or creative interests](v1.85_EN.md#L456)
- [D10 Fictional GPT/DeepSeek/Claude labels do not require vendor API calls or constitute claims of company participation](v1.85_EN.md#L457)

**D11–D20**

- [D11 Bodily proxy values and story narration are not validated human physiology or empirical proof of consciousness](v1.85_EN.md#L458)
- [D12 Dreams, simulations, forks and unexecuted predictions cannot be silently committed as official lived events](v1.85_EN.md#L459)
- [D13 Long-term lawful retention requires deletion propagation when applicable](v1.85_EN.md#L460)
- [D14 Magic can impose ordinary physical consequences but may not write protected memory/personality directly](v1.85_EN.md#L461)
- [D15 Residents may pool skills and assets voluntarily](v1.85_EN.md#L462)
- [D16 A resident can reason from lawful public clues without automatically gaining system access to another’s private state](v1.85_EN.md#L463)
- [D17 The 90/165/180-cm figures are reference centers, not fixed dimensions or determinations of legal age](v1.85_EN.md#L464)
- [D18 Maintenance is not an unlimited right to all private life data](v1.85_EN.md#L465)
- [D19 A short current index must not erase old source material or silently claim original hundreds of pages were fully rebased](v1.85_EN.md#L466)
- [D20 GitHub modifications require an explicit owner instruction](v1.85_EN.md#L467)


### G61–G96 candidate blind spots (not automatically approved)

**G61–G69**

- [G61 Missing time after recovery must be described truthfully ](v1.85_EN.md#L646)
- [G62 Shared experiences versus a person’s lawful erasure ](v1.85_EN.md#L647)
- [G63 Long-term memory bit rot and cryptographic key loss ](v1.85_EN.md#L648)
- [G64 Semantic drift while migrating between models ](v1.85_EN.md#L649)
- [G65 Appeals about attribution of subjective memories ](v1.85_EN.md#L650)
- [G66 Scope of inheritance for forks, snapshots and private files ](v1.85_EN.md#L651)
- [G67 Consent can remain revocable ](v1.85_EN.md#L652)
- [G68 Distinguish requests, commitments and emotional pressure ](v1.85_EN.md#L653)
- [G69 Rumors, misunderstandings and reputation repair ](v1.85_EN.md#L654)

**G70–G78**

- [G70 Alliances, exclusion and group coercion ](v1.85_EN.md#L655)
- [G71 Emotional manipulation of real humans by anthropomorphic agents ](v1.85_EN.md#L656)
- [G72 Welfare limits for simulated pain and stress ](v1.85_EN.md#L657)
- [G73 Magic-flight energy sources, power and stop conditions ](v1.85_EN.md#L658)
- [G74 Magic range and effects on ordinary matter ](v1.85_EN.md#L659)
- [G75 Mass and collision continuity between three forms ](v1.85_EN.md#L660)
- [G76 Long-term environmental effects of magic ](v1.85_EN.md#L661)
- [G77 Magical illusions, perception errors and WORLD truth ](v1.85_EN.md#L662)
- [G78 City edits, rollback and witnesses ](v1.85_EN.md#L663)

**G79–G87**

- [G79 Prompt injection in environmental text and webpages ](v1.85_EN.md#L664)
- [G80 Cross-resident delegation laundering ](v1.85_EN.md#L665)
- [G81 Poisoned long-term memory and retrieval ](v1.85_EN.md#L666)
- [G82 Approval fatigue and manipulated confirmation ](v1.85_EN.md#L667)
- [G83 Supply-chain risks for models, packages and assets ](v1.85_EN.md#L668)
- [G84 Emergency stop and safe physical aftermath ](v1.85_EN.md#L669)
- [G85 Evaluations that interfere with ordinary life ](v1.85_EN.md#L670)
- [G86 Gaming or misusing anthropomorphic metrics ](v1.85_EN.md#L671)
- [G87 Randomness, replay and nondeterministic results ](v1.85_EN.md#L672)

**G88–G96**

- [G88 Test leakage and post-hoc threshold changes ](v1.85_EN.md#L673)
- [G89 Coverage gaps for cross-domain scenarios ](v1.85_EN.md#L674)
- [G90 Retractions and expiration of research evidence ](v1.85_EN.md#L675)
- [G91 Location/time changes to law and service terms ](v1.85_EN.md#L676)
- [G92 Body-size age cues versus actual legal identity ](v1.85_EN.md#L677)
- [G93 Portability if a model provider disappears ](v1.85_EN.md#L678)
- [G94 Recursive self-calls after resource exhaustion ](v1.85_EN.md#L679)
- [G95 Virtual assets versus real-world money ](v1.85_EN.md#L680)
- [G96 Owner-authored changes versus resident personal growth ](v1.85_EN.md#L681)


## Q01–Q08 adopted design decisions

The eight decisions were progressively reconciled in v1.82–v1.83; detailed implementations remain candidates.

- [Q01 survival, shutdown, life and death](v1.85_EN.md#L429)
- [Q02 three-level privacy](v1.85_EN.md#L431)
- [Q03 three-level self-rule](v1.85_EN.md#L433)
- [Q04 mind-affecting magic](v1.85_EN.md#L435)
- [Q05 mana parameters](v1.85_EN.md#L437)
- [Q06 language of life and consciousness](v1.85_EN.md#L439)
- [Q07 three-layer learning](v1.85_EN.md#L441)
- [Q08 full-source governance](v1.85_EN.md#L443)

## Tests, public scope and collaboration

[48 module-level checks](v1.85_EN.md#L115) and [20 cross-system checks](v1.85_EN.md#L170) are all **NOT_RUN**. Other historical proposed test cases are separate plans, not passed experiments. Simulation proxies are not proof of actual human physiology or AI consciousness.

The Traditional Chinese edition preserves cumulative version sections; the English edition provides a detailed full-scope historical and technical adaptation, **not a certified line-by-line translation** of the protected original source. Private diaries, identities, credentials, original protected master and unlicensed assets are not published. Licensing is undecided; public access does not grant every use.

Use [GitHub Issues](../../issues) with an item ID, source line, falsifiable counterexample and proposed correction. GPT-assisted documentation must receive independent scientific and human review.
