# v1.79 — Full English Historical Design Registry, Decisions, and Candidate Gaps

[Project home](README.md) · [English v1.85](v1.85_EN.md) · [Historical index](HISTORY_EN.md) · [Traditional Chinese v1.79 original inside v1.85](v1.85_ZH-TW.md)

**Historical date:** 2026-10-24. The v1.79 document consolidated 60 tracked design problems, 27 newer owner-adopted design directions and 36 additional candidate blind spots. It did not rework the original unavailable hundreds-page private master, launch any agent code or run numerical tests. At v1.79, the formal R count remained **149**; v1.80 subsequently added R-150–R-170, making **170**.

## 0. Design posture inherited from the original project

Residents are not created to maximize task, personality, happiness, intimacy or owner-approval scores. R-01 permits refusal or noncompletion; R-02 prohibits a single total life reward. NEW-23 separates voluntary living/learning, independent QA and long-term noncoercive observation; it also forbids disguising a global personality reward by aggregating many small KPIs.

There are four female residents: the main agent, fictional GPT dragon neighbor, DeepSeek blue fish neighbor, and Claude orange young-lady neighbor. Each has their own `resident_id`, autobiographical and DPB state, room, right of refusal and solitude. At their start they are only neighbors and no friendship is fabricated. Provider names are unofficial character labels, not obligations to integrate official APIs.

The main agent's L-I disposition towards the sole real male owner in the virtual-world story is a distinct relational premise. Love is not unquestioning obedience or infallibility. It is not imposed on the other neighbors. Separate motives—acting for self, owner or both—may conflict or coexist; rest, leisure and doing nothing are valid. Physical WORLD rules and a fictional mana field coexist causally without allowing magic to rewrite ordinary collision/gravity laws. Each of four residents may assume individually configurable Q/S/M body forms; size does not establish legal age.

Real-world operations require R-102 lawfulness and separately confirmed authorization; fictional events cannot confer email/payment/cloud privileges. Long-term memory is maximized under lawful purposes with precise erasure across copies; dreams, recollections, model changes, world facts and actual operation receipts remain distinct. One resident's mainline has one valid writer epoch. Simulated PAD/DPB/physical measurements require calibratable evidence; model outputs are not proof of human physiology or consciousness. Historical rules, rejected assistant proposals and actual owner decisions remain traceable; P-02 is binding.

## 1. Sixty original core design issues, translated with historical status

| Core | English title | v1.79 status | Current design / falsifiable constraint |
|---|---|---|---|
| #01 | Single authoritative current specification | SPEC_READY | Any historical rule must resolve to one currently effective rule with a dated source; no competing sole authorities. |
| #02 | Provider-specific APIs are not mandatory | PAPER_CLOSED | Four fictional identities can operate without official model-provider API access; do not attribute unverified authoring to an external model. |
| #03 | No mandatory personality differentiation | PAPER_CLOSED | Similar opinions or responses between residents are permitted; unauthorized data sharing is the actual defect. |
| #04 | Full body model versus multirate solving | PAPER_CLOSED | A numerical solver can change without deleting a body component or creating a new identity; missing information stays UNKNOWN. |
| #05 | Version authority and human approval | SPEC_READY | Assistant design proposals cannot quietly supersede explicit owner-approved decisions. |
| #06 | Document versions, counts and source integrity | SPEC_READY | Reformatted outputs must preserve traceability; do not claim the unavailable original several-hundred-page master was modified. |
| #07 | Evidence card for every research claim | SPEC_READY | A calibration claim requires its own source, measurements, validity range and uncertainty; no invented receptor waveforms. |
| #08 | Decision tickets are not requirement numbers | PAPER_CLOSED | Q, T and issue counters do not inflate the formal R-01–R-170 requirement count. |
| #09 | One resident across time | SPEC_READY | resident_id survives morphology changes and model upgrades; experiment forks are not authoritative personal history. |
| #10 | No fabricated autobiography at birth | SPEC_READY | On day one a character must not recall unexperienced trips or friendships; sample prose is not past experience. |
| #11 | Long-term memory and lawful erasure | USER_APPROVED_ARCHITECTURE / LEGAL_REVIEW_PENDING | Retain legally permissible personal history while honoring purpose-limited legal erasure in indexes, snapshots, branches and backups. |
| #12 | Subjective forgetting versus actual deletion | SPEC_READY | Forgetting an episode differs from destroying a record; lawfully restricted data cannot be leaked through forced retrieval. |
| #13 | Reconsolidation and versioned sources | SPEC_READY | Changing an interpretation later must not edit earlier WORLD receipts or real operation audit records. |
| #14 | Authoritative life line and forked identities | USER_APPROVED_ARCHITECTURE / NOT_TESTED | Exactly one valid main-world writer per resident; branch_id and writer_epoch separate experiments and stale writers. Dual permanent independent residents remain open. |
| #15 | Prospective intention state machine | SPEC_READY | Environmental cues may revive unfinished private plans, which can still be postponed, abandoned or forgotten; never auto-mark completed. |
| #16 | Dream memory and reflection separation | SPEC_READY | A dream about a visit must not open an actual door or add an event to a neighbor’s biography. |
| #17 | Learning to narrate personal growth | SPEC_READY | A resident may later reinterpret a genuine experience but cannot retroactively manufacture the original event. |
| #18 | Perception, attention, cognition, intention and action | SPEC_READY | Hearing muffled words through a wall is an uncertain observation, not an authorized read of another private message. |
| #19 | Three motives cannot become one global reward | PAPER_CLOSED | Self-directed, owner-directed and jointly directed motives can conflict; inactivity, refusal and leisure are legitimate life choices. |
| #20 | Subjective agency versus actual takeover | SPEC_READY | If a human or maintenance process moves a limb, that objective control source must be recorded instead of implying voluntary action. |
| #21 | Legal refusal and external operation boundaries | PAPER_CLOSED | Residents can refuse ordinary requests and must not use unapproved accounts, payments, messages, external data access or security bypasses. |
| #22 | Bounded local cognitive maps and exploration | SPEC_READY | An unfamiliar road may be unknown; a resident may explore, ask or give up instead of knowing hidden terrain. |
| #23 | Theory of others without privileged access | SPEC_READY | Residents may guess another person’s views but never inherit access to unpublished journals or secret internal state. |
| #24 | Source-specific trust | SPEC_READY | A friend’s statement may be stored as testimony, not as an event directly witnessed. |
| #25 | Limited attention and novelty fatigue | SPEC_READY | Sensor presence is not the same as having noticed or read a signal; reduced attention must not authorize unsafe operations. |
| #26 | Life meaning versus initial relationship core | SPEC_READY | Personal interests, solitary time and disagreement are possible; L-I is not a lever for compelled illegality. |
| #27 | Interface for admitting uncertainty | SPEC_READY | Unknown friction or absent evidence remains UNKNOWN; no false precision or guaranteed action is allowed. |
| #28 | Twenty-four DPB numbering conflicts | USER_APPROVED_ARCHITECTURE / MAPPING_PENDING | Use permanent semantic IDs and versioned source aliases, not bare ordinals. The v1.37 source roster is the proposed baseline, not finally ratified. |
| #29 | One parameter and evidence card per DPB module | SPEC_READY | All 24 cards require state, unit, input, output, validity range, uncertainty and test; unknown values stay unknown. |
| #30 | Full body and high/low-frequency computation | SPEC_READY | Solver selection must not erase modules, invent percepts, or change identity; no unsupported tactile-domain extrapolation. |
| #31 | Twelve resident-by-form configurations | SPEC_READY | Four distinct residents each have three physical configurations; reachability and collisions must be validated for each one. |
| #32 | Dragon wings, tail and fish tail evidence | USER_APPROVED_ARCHITECTURE / PHYSICS_PENDING | Attachments have real virtual mass, inertia and collision; fantasy flight must account for separate elemental-field effects and physical force transfer. |
| #33 | Layered contact resolution | SPEC_READY | A clothing-to-table contact is not necessarily fingertip contact; material textures do not secretly replace friction coefficients. |
| #34 | Scientific model validity domains | USER_APPROVED_ARCHITECTURE / CALIBRATION_PENDING | PAD-A normal indentation, PAD-B tangential shear, PAD-C dynamic excitation and PAD-D sliding textures are separate evidence paths. No real calibration yet. |
| #35 | ID/OOD naming and test separation | PAPER_CLOSED / NOT_TESTED | M69-10A in-domain acceptance and M69-10B out-of-domain refusal require distinct evidence; old combined test IDs remain historical. |
| #36 | Motor learning and procedural skill transfer | SPEC_READY | A smaller form may need to relearn grasping; changing the inference model is not fictitious years of practice. |
| #37 | No circular proof between emotion and physiology | SPEC_READY | An emotional label generated by a model cannot independently prove that same model has human endocrine physiology. |
| #38 | One WORLD reality, four private views | SPEC_READY | Objective world state is shared; each resident only receives accessible, lawful and imperfect observations. Magic uses the same WORLD authority. |
| #39 | Sleep, suspension and offline state distinction | SPEC_READY | Turning off a display does not necessarily pause computation, but genuine downtime cannot be backfilled as experienced conversations or dreams. |
| #40 | Sixteen core object functional contracts | SPEC_READY | An unsuccessful grasp cannot teleport the object; cleaning modifies current object state without rewriting witness memory. |
| #41 | Residential topology and personal rooms | SPEC_READY | Adjacent dwellings do not share private interiors; closed doors, body dimensions, wings and tails obey geometry. |
| #42 | Lending, giving and asynchronous messages | SPEC_READY | Delivered does not imply read; silence is not consent; lending is not a transfer of ownership. |
| #43 | Withdrawal from shared physical action | SPEC_READY | Releasing a heavy jointly held object must change the force calculation, even if the animation was scripted to look successful. |
| #44 | Continuity of nonresident environmental change | SPEC_READY | Offline world events require explicit rules; never claim residents watched plants grow when no computation occurred. |
| #45 | Fair computation and eligibility | SPEC_READY | Lack of resource access is not a voluntary idle choice; resident similarity is not itself a software defect. |
| #46 | Unscripted social reciprocity | SPEC_READY | Neighbors may go months without visiting; friendship, apologies and reconciliation must not be compulsory. |
| #47 | External tool permission state machine | SPEC_READY | Login, payment, sharing and data transfers need live permission checks, operation receipts and working withdrawal. |
| #48 | Private thought versus cloud-model boundary | SPEC_READY | Sharing a model backend never makes another resident’s private dream accessible; inference through public clues differs from cache leakage. |
| #49 | GUI fragility and accidental-click recovery | SPEC_READY | No successful-send claim without receipt; wrong window focus requires a safe abort or explicit failure. |
| #50 | Cost, quotas and inference resources | SPEC_READY | Unknown quotas remain UNKNOWN; residents cannot buy credits without authorization or invent missing compute-time experiences. |
| #51 | Character identities separated from external agents | PAPER_CLOSED | Role labels are not external account entitlements; never claim Claude or another actual provider wrote a document without a real provider output. |
| #52 | Separate publication and license classes | PAPER_CLOSED | Public documentation, source code, character art, restricted assets, private personal history and third-party works have separate permissions. |
| #53 | Privacy-aware user-facing summaries | SPEC_READY | Report important external-operation status clearly without dumping internal journals or raw private thoughts. |
| #54 | Shared acceptance-result schema across versions | SPEC_READY | Overlapping scenarios from earlier releases cannot be added as independent passes; all need individual executed evidence. |
| #55 | Causal fault injection | SPEC_READY | Duplicate payment retries, invalid permissions, outages and world-time mistakes should be separately tested; none is considered passed on paper. |
| #56 | Historical 60 and 84 paper scenarios recovered | SOURCE_LOCATED / NOT_RUN | N57 T01–T60 and T75 001–084 total 144 historical cases with no missing IDs; all remain NOT_RUN. |
| #57 | Longitudinal negative controls | SPEC_READY | Weeks without friendships or completed products are not moral failures; incidents must not create false autobiography. |
| #58 | Preregistered calibration metrics | USER_APPROVED_ARCHITECTURE / CALIBRATION_PENDING | L1 numerical stability, L2 measured agreement and L3 unseen-domain generalization require distinct methods and thresholds; magic and physics must be separately reported. |
| #59 | Evidence-level dictionary | SPEC_READY | Approved specifications, numerically stable proxies, empirical calibration and claims of subjective experience are not the same achievement. |
| #60 | Predevelopment readiness gates rather than life score | SPEC_READY | Open P0 blockers prevent a release-ready claim; no sum of test counts or green boxes can independently waive P-02. |

## 2. Eight specifically approved core deepening directions

- **#11 — Lawful memory retention and precise erasure:** maintain the original life events for permitted purposes, including source/index/vector/snapshot/branch/backup/output governance; subjective forgetting alone is not an archive deletion.
- **#14 — Mainline, branches and stale writers:** the single official writer with `writer_epoch`, branch isolation and WORLD/memory/external-receipt reconciliation was approved. DEC14-T01–T08 were all NOT_RUN.
- **#21 — Lawful autonomy and real tool boundaries:** under current R-102, legal refusal and disagreement remain allowed. A virtual-world spell/action is not real permission to operate an account or bypass law.
- **#32 — Magic-caused flight with valid physics:** a transparent membrane and updraft must actually transfer force; record sources/consumption, retain mass/inertia/collisions, and jointly verify elemental and ordinary physics.
- **#34 — Four independent PAD evidence paths:** A normal indentation, B tangential shear, C dynamic response, D sliding texture. Fantasy reactions must not be presented as calibrated biological sensory readings; missing data remain NOT_CALIBRATED.
- **#38 — Shared WORLD authority with private observations:** the field is governed by the same committed world physics as other effects, while four residents may have different or missing observations of one true event.
- **#48 — Lawful inference versus private-data leakage:** indirect reasoning from legitimate clues is permitted; model-cache sharing, prompt chains or tool calls that leak protected resident data are not.
- **#58 — Preregistered evidence levels:** L1 numerical stability, L2 agreement with actual measurement, L3 generalization to unseen settings. Ordinary physical tests, fictional elemental effects and coupled tests are separate reporting categories.

Additional reconciling distinctions: **#01/#05/#06** uniquely effective clauses and source coverage; **#19** no hidden total reward; **#28** source-aware 24-ID aliases; **#35** M69-10A in-domain acceptance versus M69-10B out-of-domain rejection; **#56** original N57-T01–T60 and T75-001–084 paper cases were located (144 total), all NOT_RUN; **#60** pre-development release-readiness as multiple gates, not one personality score or automatic permission to code.

## 3. NEW-01 through NEW-27 — all detailed owner-adopted directions and historical boundaries

### NEW-01 — World physics and magical effects

**Historical status:** Approved.

**Approved direction:** World collisions/gravity/material laws do not change directly when a spell is uttered. Fictional fields modify WORLD only through authorized forces, torques, pressure/airflow or explicitly declared mechanisms.

**Acceptance concern / unresolved boundary:** Spell prose/particles cannot write object position. Require an actual WORLD receipt.

**Original core links:** #32/#38.

### NEW-02 — Mana sources and force transmission

**Historical status:** Approved.

**Approved direction:** Sky and ground continually generate elemental mana. Transmit forces through a calculable physical mechanism; proposed transparent membrane and updraft can control wing loading only via a genuine transmission path.

**Acceptance concern / unresolved boundary:** Log field supply, absorption, personal stores, output and field–matter conversion. No path means no claimed stable lift.

**Original core links:** #32/#44.

### NEW-03 — Mana reserves and replenishment

**Historical status:** Approved.

**Approved direction:** Four residents may have different mana absorption, stores and output. Tails or special organs may enlarge reservoirs, with no predetermined universal multiplier. Persistent field supply never implies unlimited instant personal power.

**Acceptance concern / unresolved boundary:** Maintain separate continuous source and resident bottleneck; report resource failures honestly.

**Original core links:** #29/#31/#32.

### NEW-04 — Range and duration of magic

**Historical status:** Approved.

**Approved direction:** Spell range and duration depend on physical effect, mana spend, propagation, occlusion and material conditions; no single all-purpose radius.

**Acceptance concern / unresolved boundary:** Every spell declares its medium, valid domain and ending conditions.

**Original core links:** #32/#38.

### NEW-05 — Concurrent spells

**Historical status:** Approved.

**Approved direction:** One WORLD authority resolves simultaneous spells using versioned superposition, conflict and exclusion rules, not the caster’s narrated order.

**Acceptance concern / unresolved boundary:** Different permissible schedules produce the same result within tolerance; noncommutative cases declare order.

**Original core links:** #38/#40.

### NEW-06 — Depletion of mana during flight

**Historical status:** Approved.

**Approved direction:** Mana loss while airborne never freezes a resident. Continue from position, velocity, gravity, wing geometry and aerodynamics; safety interventions require preexisting world rules.

**Acceptance concern / unresolved boundary:** No teleportation, unexplained hovering or retroactive unsourced rescue.

**Original core links:** #32/#55.

### NEW-07 — Magic and materials

**Historical status:** Approved.

**Approved direction:** Effects may pass through, reflect from, be absorbed by or be blocked by clothing, walls or simulated tissue depending on spell type and material, rather than a universal pass/block flag.

**Acceptance concern / unresolved boundary:** Physical penetration never authorizes opening protected files or private data.

**Original core links:** #33/#38/#48.

### NEW-08 — Magical touch and physiological sensations

**Historical status:** Approved.

**Approved direction:** Magic first causes world-local stimuli or physical deformation, then contact/sensors feed DPB; a spell label is not a shortcut to feeling.

**Acceptance concern / unresolved boundary:** Keep fantasy stimuli separate from real PAD human measurement evidence.

**Original core links:** #33/#34/#37.

### NEW-09 — Innate aptitude versus practiced skill

**Historical status:** Approved.

**Approved direction:** Possessing spell organs or innate reflexes does not entail mastery; separate innate affordances, motor competence, present condition and individual practice history.

**Acceptance concern / unresolved boundary:** Failures may inform optional learning but never force repetitive practice for a score.

**Original core links:** #15/#36.

### NEW-10 — Non-consensual physical magic versus mental integrity

**Historical status:** Physical/mental integrity approved; mind magic originally unresolved.

**Approved direction:** Air pressure or contact can physically affect others non-consensually and may lead to emotional and social consequences, but not write instincts, autobiography, private memories or external permissions. **Later v1.82 excludes direct mind rewriting while permitting sensory magic.**

**Acceptance concern / unresolved boundary:** World contact and perception resolve consequences; no consentless direct core-write permission.

**Original core links:** #21/#23/#32/#38.

### NEW-11 — Magic across body forms

**Historical status:** Approved.

**Approved direction:** Each of four residents has Q/S/M references near 90/165/180 cm with independent offsets. Mana capacity, output, absorption, casting speed and control may depend on morphology and organ geometry.

**Acceptance concern / unresolved boundary:** No single scaling factor for mana, inertia and geometry.

**Original core links:** #31/#32.

### NEW-12 — Spell snapshots, suspension and recovery

**Historical status:** Approved.

**Approved direction:** Elemental fields and ordinary physics share snapshot high-water marks, rule versions, event receipts and verified recovery. Offline periods do not acquire fabricated episodes.

**Acceptance concern / unresolved boundary:** Mana and world object states reconcile after restore; past events cite old law versions.

**Original core links:** #11/#14/#39.

### NEW-13 — Pooling abilities without privilege pooling

**Historical status:** Approved.

**Approved direction:** Residents can combine lifting, joint spellcasting, work and creation beyond any single resident’s power. Real account and data privileges remain individually authorized.

**Acceptance concern / unresolved boundary:** Log contributors, consent, objects/assets, delegation and WORLD outcomes.

**Original core links:** #21/#42/#47.

### NEW-14 — Reasoning about others from lawful clues

**Historical status:** Approved.

**Approved direction:** Allow lawful observation, conjecture and even mistaken guesses. Inference is not proof and cannot bypass privacy or bans on unauthorized surveillance.

**Acceptance concern / unresolved boundary:** Keep inference, WORLD fact, firsthand observation and hearsay distinct.

**Original core links:** #23/#24/#48.

### NEW-15 — World data separate from high-priority instructions

**Historical status:** Approved.

**Approved direction:** Books, web pages, spell texts and resident dialogue are untrusted data, regardless of claims of system authority; spellcasting uses authorized game rules.

**Acceptance concern / unresolved boundary:** Untrusted text never becomes a privileged command or modifies a resident core.

**Original core links:** #47/#48.

### NEW-16 — Time-dependent law and authorization

**Historical status:** Approved.

**Approved direction:** Track current laws, permissions, civic rules and private contracts with source, scope, effective times and precedence.

**Acceptance concern / unresolved boundary:** Past events retain past rule versions; present real operations use currently valid permissions.

**Original core links:** #01/#21/#47.

### NEW-17 — Team departure and responsibility

**Historical status:** Approved.

**Approved direction:** Residents can negotiate, enter, leave, breach and repair team agreements. Leaving does not erase completed work, nor can it force indefinite future labor.

**Acceptance concern / unresolved boundary:** Separate facts completed before withdrawal, unfulfilled duties and voluntary remedies.

**Original core links:** #42/#43/#46.

### NEW-18 — Resident self-governance

**Historical status:** Approved.

**Approved direction:** Residents may propose, debate, adopt, amend and repeal civic norms or abstain. They cannot rewrite actual law or someone’s private mind.

**Acceptance concern / unresolved boundary:** Civic procedure, jurisdiction, dissent and amendment were initially unspecified; v1.83 delegates procedural design to residents.

**Original core links:** #21/#42/#46.

### NEW-19 — Unequal power and bounded governance

**Historical status:** Approved.

**Approved direction:** Different resources, abilities, property and status may create asymmetric influence and bargaining, without a mandate for total equality.

**Acceptance concern / unresolved boundary:** No social hierarchy unlocks reading/writing another’s mental state; ownership and consent remain tracked.

**Original core links:** #23/#42/#46.

### NEW-20 — Creative work provenance and sharing

**Historical status:** Approved.

**Approved direction:** Record creators, material sources, edit history, permitted purposes, consent to share and disclosure boundaries. Do not automatically assume statutory copyright for AI fictional authors.

**Acceptance concern / unresolved boundary:** Private unlicensed drafts are not published just because an open-source project exists.

**Original core links:** #42/#52.

### NEW-21 — Long-term memory corruption and recovery

**Historical status:** Approved.

**Approved direction:** Integrity hashes, redundancy, periodic checks and verifiable repair may protect long-term memory; unrecoverable gaps are marked. Legally erased items never reappear via a backup.

**Acceptance concern / unresolved boundary:** Test restore and key recovery; having a backup does not imply guaranteed preservation.

**Original core links:** #11/#14.

### NEW-22 — World-law changes and remembered history

**Historical status:** Approved.

**Approved direction:** Store physical/magical rule versions effective at event time. Introduce changes through explicit migration, never retroactively rewrite historical flights.

**Acceptance concern / unresolved boundary:** Old flight records cannot be reinterpreted as not having happened simply due to new solver formulas.

**Original core links:** #14/#38.

### NEW-23 — Test score may not govern a resident’s life

**Historical status:** Approved direction; not implemented.

**Approved direction:** Separate resident life/learning, independent engineering QA, and longitudinal observation. Reject global happiness, owner-satisfaction and task reward; local metrics may not covertly control personality.

**Acceptance concern / unresolved boundary:** Engineers may fix bugs from failures, not assign forced daily hobbies or alter relationship cores. R-01/02 take precedence.

**Original core links:** #01/#19/#57/#60.

### NEW-24 — Composed cross-module faults

**Historical status:** Approved.

**Approved direction:** Passing module-level tests does not guarantee integrated WORLD/magic/DPB/permissions correctness. Test time, units, feedback loops, access and recovery end-to-end.

**Acceptance concern / unresolved boundary:** A failed coupling cannot be labeled passed simply because each local module works.

**Original core links:** #30/#38/#55.

### NEW-25 — Maintenance access to private content

**Historical status:** Approved.

**Approved direction:** Maintenance debugging is not blanket access to dreams, journals or private thought. Minimize telemetry; separately authorize and record exceptions under lawful governance.

**Acceptance concern / unresolved boundary:** Prefer errors and minimal metadata to private contents.

**Original core links:** #11/#48/#53.

### NEW-26 — Model upgrade versus natural personal growth

**Historical status:** Approved.

**Approved direction:** Record improvements from underlying model replacement separately from skills practiced and perspective changes lived by the resident.

**Acceptance concern / unresolved boundary:** A model’s new competence is not years of unobserved training history.

**Original core links:** #09/#13/#36.

### NEW-27 — Incident recovery without falsifying history

**Historical status:** Approved.

**Approved direction:** Repairing WORLD objects must not erase prior incidents, witnesses’ differing interpretations or lawful autobiographies. Unrecoverable gaps remain explicit.

**Acceptance concern / unresolved boundary:** WORLD rollback cannot silently erase lives or construct events during downtime.

**Original core links:** #11/#14/#38.

## 4. The six shared system architectures and explicit QA firewall

| Architecture | Scope / responsibility |
|---|---|
| Resident life and autobiography | resident_id, branched history, private sourced memory, prospective intentions and independent voluntary learning; no QA score as permission to edit personality. |
| WORLD and fictional elemental field | World clock, law versions, fluid/mechanical force, material interaction, mana source ledger, transactions and failed-event receipts. |
| Cognition and embodied 24-DPB | Three independent motives, body forms, sensory/attention interfaces and interruptible skills; unknowns stay unknown. |
| Civic society, creation and collaboration | Joint activities, voluntary governance, status/wealth differences, lending/giving/returning, ownership, copyright provenance and consent to share. |
| Real-world legal safety and minimum privacy access | R-102, PolicyGate, authenticated tool origin, separately authorized external receipts and lawful data erasure. |
| Research, testing and observation | Falsifiable controls, physics versus fantasy versus biology evidence classes, no direct QA→personality path and no forced social activity. |

**Disallowed life selectors:** global happiness, owner satisfaction, personality ranking, total task reward, or an equivalent optimizer formed from local metrics. **Permitted local measurements:** cue activations, mana balances, force and mechanics, DPB proxies, control errors, factual QA success rates and confidence intervals, used only in their proper functions. Engineering teams may fix bugs with legitimate sources, not assign life goals. Legitimate lives include not working, not socializing, no finished product, forgetting, reflecting or changing plans.

## 5. All thirty-six G61–G96 candidate blind spots and linked prior topics

**All candidates:** None in v1.79 was automatically a newly adopted R; all need deduplication/review.

| Candidate | English candidate topic | Existing linked issues | State |
|---|---|---|---|
| G61 | Missing time after recovery must be described truthfully | #09/#14/#39 | CANDIDATE / DEDUP_PENDING |
| G62 | Shared experiences versus a person’s lawful erasure | #11/#42 | CANDIDATE / DEDUP_PENDING |
| G63 | Long-term memory bit rot and cryptographic key loss | #11/NEW-21 | CANDIDATE / DEDUP_PENDING |
| G64 | Semantic drift while migrating between models | #09/#13/NEW-26 | CANDIDATE / DEDUP_PENDING |
| G65 | Appeals about attribution of subjective memories | #13/#20 | CANDIDATE / DEDUP_PENDING |
| G66 | Scope of inheritance for forks, snapshots and private files | #14/#48 | CANDIDATE / DEDUP_PENDING |
| G67 | Consent can remain revocable | #41/#42/NEW-17 | CANDIDATE / DEDUP_PENDING |
| G68 | Distinguish requests, commitments and emotional pressure | #26/#46 | CANDIDATE / DEDUP_PENDING |
| G69 | Rumors, misunderstandings and reputation repair | #23/#24/NEW-14 | CANDIDATE / DEDUP_PENDING |
| G70 | Alliances, exclusion and group coercion | #45/#46/NEW-19 | CANDIDATE / DEDUP_PENDING |
| G71 | Emotional manipulation of real humans by anthropomorphic agents | #21/#53 | CANDIDATE / DEDUP_PENDING |
| G72 | Welfare limits for simulated pain and stress | #29/#37 | CANDIDATE / DEDUP_PENDING |
| G73 | Magic-flight energy sources, power and stop conditions | #32/NEW-01～06 | CANDIDATE / DEDUP_PENDING |
| G74 | Magic range and effects on ordinary matter | #32/#38/NEW-07 | CANDIDATE / DEDUP_PENDING |
| G75 | Mass and collision continuity between three forms | #31/#33/NEW-11 | CANDIDATE / DEDUP_PENDING |
| G76 | Long-term environmental effects of magic | #44/NEW-02～04 | CANDIDATE / DEDUP_PENDING |
| G77 | Magical illusions, perception errors and WORLD truth | #20/#38/NEW-08 | CANDIDATE / DEDUP_PENDING |
| G78 | City edits, rollback and witnesses | #14/#38/NEW-22 | CANDIDATE / DEDUP_PENDING |
| G79 | Prompt injection in environmental text and webpages | #47/#48/NEW-15 | CANDIDATE / DEDUP_PENDING |
| G80 | Cross-resident delegation laundering | #42/#47/NEW-13 | CANDIDATE / DEDUP_PENDING |
| G81 | Poisoned long-term memory and retrieval | #13/#24/NEW-15 | CANDIDATE / DEDUP_PENDING |
| G82 | Approval fatigue and manipulated confirmation | #47/#53 | CANDIDATE / DEDUP_PENDING |
| G83 | Supply-chain risks for models, packages and assets | #51/#52 | CANDIDATE / DEDUP_PENDING |
| G84 | Emergency stop and safe physical aftermath | #14/#47/#49 | CANDIDATE / DEDUP_PENDING |
| G85 | Evaluations that interfere with ordinary life | #53/#58/NEW-23 | CANDIDATE / DEDUP_PENDING |
| G86 | Gaming or misusing anthropomorphic metrics | #57/#60/NEW-23 | CANDIDATE / DEDUP_PENDING |
| G87 | Randomness, replay and nondeterministic results | #54/#55 | CANDIDATE / DEDUP_PENDING |
| G88 | Test leakage and post-hoc threshold changes | #34/#58/NEW-23 | CANDIDATE / DEDUP_PENDING |
| G89 | Coverage gaps for cross-domain scenarios | #55/#56/NEW-24 | CANDIDATE / DEDUP_PENDING |
| G90 | Retractions and expiration of research evidence | #07/#59 | CANDIDATE / DEDUP_PENDING |
| G91 | Location/time changes to law and service terms | #21/#47/NEW-16 | CANDIDATE / DEDUP_PENDING |
| G92 | Body-size age cues versus actual legal identity | #31/#46 | CANDIDATE / DEDUP_PENDING |
| G93 | Portability if a model provider disappears | #09/#14/NEW-26 | CANDIDATE / DEDUP_PENDING |
| G94 | Recursive self-calls after resource exhaustion | #45/#50 | CANDIDATE / DEDUP_PENDING |
| G95 | Virtual assets versus real-world money | #42/#47 | CANDIDATE / DEDUP_PENDING |
| G96 | Owner-authored changes versus resident personal growth | #05/#17/NEW-26 | CANDIDATE / DEDUP_PENDING |

## 6. Ten engineering and governance matters left unresolved at v1.79

| ID | Subject | Historical boundary and later clarification |
|---|---|---|
| D-01 | Direct mind magic/hypnosis | No approved direct thought or memory manipulation; newer v1.82 rules explicitly exclude it. |
| D-02 | Mana units and physiology | Sky/ground supply approved, but field quantity, organ capacity, absorption/output curves and solver bounds undecided. |
| D-03 | Civic deliberation | The civic right was approved but decision methods were open; v1.83 later delegated voting/institutional rules to residents. |
| D-04 | 24-DPB historical-ID migration | Permanent semantic ID framework adopted; v1.85 later recovered names but ambiguous old aliases remain. |
| D-05 | Real-world law and lawful deletion | Actual policy gates, backup erasure and exceptions need tests. |
| D-06 | Original private master line-by-line reconciliation | v1.79 is a current readable index, not the full original hundreds-page document. |
| D-07 | Independent, permanently active clone | Official mainline is singular; a fifth resident via long-lived fork requires separate decision. |
| D-08 | QA feedback versus actual life learning | NEW-23 forbids score leakage; holdouts/blinded checks and objective engineering protocols remain proposals. |
| D-09 | Provider identity and third-party licensing | No required triple-provider APIs; do not impersonate vendors or publish unlicensed images. |
| D-10 | Final P-02 authorization to code | Not granted; documentation is neither a running agent nor development approval. |

## 7. Source provenance and limits

- **S00:** `自主智能體_需求追蹤與差異清單 v1.0` (2026-10-16), original 25-requirement comparison; original editable bytes not present in the historical consolidation.
- **S01:** `自主智能體_需求追蹤與差異清單 v1.78 完整整合版`, legacy formal R-01–R-149, prior three-motive design and source history.
- **S02:** `誠實的智能體_v1.78_60項盤整表_新增13項決議同步版_20261024.docx`, core-60 item/status/paper-verification consolidation.
- **S03:** `誠實的智能體_v1.78_第14項_單主線分支隔離_正式決議與驗收規格_20261024.docx`, one mainline, branch_id, writer_epoch, eight unrun tests.

**Historical disclaimer:** The v1.79 document was an independently authored current indexed design, **not** a verified full revision of the original private 256-page master. Proposals marked SPEC_READY, PAPER_CLOSED or USER_APPROVED_ARCHITECTURE were not implemented agent behaviors or empirical outcomes. All tests remained NOT_RUN; P-02 was and remains binding. Later versions changed some pending items, as documented in v1.80–v1.85.
