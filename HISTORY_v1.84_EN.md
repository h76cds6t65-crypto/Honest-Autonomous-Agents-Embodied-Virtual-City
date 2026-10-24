# v1.84 — Complete English Translation of the Historical Integrated Design Chapter

[Project home](README.md) · [English v1.85](v1.85_EN.md) · [Historical reading index](HISTORY_EN.md) · [Traditional Chinese source](v1.85_ZH-TW.md)

**Original date:** 2026-10-24. **Historical status:** ENGINEERING_CANDIDATE / NOT_RUN / P-02 in force. **This is a translation of the retained v1.84 history, not a new approval or implementation.** Superseding v1.85 findings take precedence (notably recovery of all 24 names after v1.84's earlier MAPPING_PENDING statement).

## 0. Version authority, approval and differences

**Inherited effective requirements:** v1.83's R-01–R-170, six shared systems, 60 core problems and NEW27 mapping remain. This version did not add R numbers or change L-I, the three motives, refusal, private space or civic autonomy. Residents remain free to develop their own interpretations of death and governance.

**New material is ENGINEERING_CANDIDATE:** An explicit causal workflow combines Q05 elemental magic field, standard in-world physics, 24-DPB, sensation, CAIA, Q07 local skills, private autobiography and longitudinal observation. Proposed data contracts, clock rates and update methods still require separate engineering review by the human originator; they were not executed.

**P-02:** no resident software written, no city run or deployment, no GitHub update in the historical v1.84 step. All cases added in that version remained NOT_RUN. Historical source documents were not overwritten. The version placed its new effective-design clauses ahead of v1.83 history.

**Authority split:** intent, skill, world fact, bodily feeling, personal memory and research evaluation have distinct owners. Only WORLD may commit objective physical outcomes; ordinary life intentions originate from a resident; lawful independent governance authorizes sensitive real-world actions.

## 1. One objective causal loop with two concurrent tracks (WORLD and person)

| Stage | State owner/source | Behavior/data | Boundary that cannot be crossed |
|---|---|---|---|
| 01 Sample environment | WORLD and lawful sensory access | Visible local light, sound, wind, contact and permissible clues | No omniscience; room privacy |
| 02 Embodied DPB feedback | 24-DPB semantic IDs | Posture, motion, load, sensation with different delays | No magic label directly written as felt experience |
| 03 Attention and cue retrieval | CAIA and private memory index | Candidate memories, prospective intentions, uncertainty | Memory activation is not a command |
| 04 Choose action voluntarily | Resident, three distinct motives | Propose, accept, rest, postpone, decline or stop | No universal life score picks a winner |
| 05 Check law/world constraints | WORLD and policy authority | Physics feasibility, resources, authorization, time windows | Fantasy spells grant no real-world tool privileges |
| 06 Execute local motor skill | Resident skill_id/controller | Joint, wing and proposed mana output commands | Local controller does not modify preference/L-I |
| 07 Elemental field/medium | MAG, fluid/rigid-body solver | Mana spend, field source, wind/material effect | No force without valid path |
| 08 Commit objective WORLD result | WORLD | Force, contact, event time, authoritative receipt | No text-generated physical outcome |
| 09 Sample actual sensation | Authorized sensors/DPB | Real (in-world) effects on body and environment | Prediction and actual separate |
| 10 Update local skill | Skill owner | Learn from motor residual; retain rollback | No QA metric writes personality |
| 11 Record/reflect | Resident's private memory | World provenance plus subjective interpretation | Do not turn dream/test/prediction into experience |
| 12 Choose freely again | Resident | Continue, refuse, change mind or do nothing | Bad scores must not enforce repetition |

**Recommended order:** form intention first, decompose into feasible skills next; resolve WORLD facts before DPB and residents receive feedback. “The player is supposed to succeed” is not an additional physical force.

**Two time axes:** A monotonic physical event sequence (`world_tick`, `event_seq`) and the resident's available experiences/autobiographical time are distinct. A WORLD event must be committed before access/recollection is indexed. A resident may overlook, misremember or never witness a real event.

## 2. Data ownership, write gates and minimum fields

| Contract/owner | Proposed fields | Authorized writes and prohibited shortcuts |
|---|---|---|
| GoalIntent / resident | intent_id, resident_id, motive_origin, chosen_goal, consent_state, expiry, voluntary_state | Only resident-autonomy mechanism may propose/adopt; maintenance/QA cannot force creation |
| BodySnapshot / 24-DPB | resident_id, morph_id, dpb_semantic_id, state, unit, provenance, timestamp | Update through sensors and causal physiology; visual effects do not directly write true sensation |
| SkillExecution / controller | skill_id, morph_id, controller_version, selected_target, action_plan, validity_domain | Runs solely during a voluntarily selected and authorized skill |
| MagicBudget / MAG | scene_id, emitter_id, E, C, absorption, output, effect_id, field_version, unit | Mana source and capacity ledgers; no negative stores |
| WorldReceipt / WORLD | event_id, seq, t_world, law_version, impulse, energy_transfer, collisions, outcome, uncertainty | One authoritative physical ledger; not mutable by resident dialogue or QA |
| SensoryEvidence / sensing | event_ref, modality, region, accessibility, confidence, signal_range | Only accessible sensory channels; inference is not direct perception |
| SkillUpdate / skill learner | skill_id, before, after, evidence_refs, residual, update_source, rollback_pointer | Local skill only; cannot turn a score into an L-I or social goal |
| EpisodeEntry / autobiography | resident_id, event_ref, subjective_record, source_type, privacy, memory_version | Authorized private record; interpretation can be mistaken |
| EvalReceipt / QA | test_id, observed_fact_refs, criteria_version, result, visibility_policy | Verifies engineering, cannot write life motives or private diaries |

**Three provenance classes:** `WORLD_FACT` = authoritative physical receipt; `RESIDENT_INTERPRETATION` = resident-private interpretation; `MODEL_PREDICTION` = prior prediction. Identical wordings do not make these sources equal in authority.

**Version boundaries:** Every WORLD receipt references the field law, physical solver, morphology and applicable policy version. Every SkillUpdate cites the relevant controller/model version. Snapshots, lawful deletion and `writer_epoch` fall under R-158/159; an obsolete writer must never become active after restoration.

## 3. Mana field → physical forces → 24-DPB without double accounting

**Force path A — air as medium.** The elemental field injects energy/momentum into air or supplies a declared boundary condition → fluid solver computes wind, pressure and shear → wing, body, clothing or a mechanically attached transparent membrane receives fluid forces → WORLD updates net force/torque → proprioceptive and bodily sensors update. Once the action is included as `F_aero`, do not add the same original action again as `F_magic`.

**Path B — direct material interaction, only as future extensibility.** If an explicit separately approved elemental mechanism ever acts directly on material, record a distinct field–material action/reaction. It must not re-label the same force from path A. No shortcut has been approved for instantaneously editing position, velocity or gravity laws.

**Bookkeeping equation, not a new physical law:** `m dv/dt = F_gravity + F_contact + F_aero + F_direct_field(if declared) + F_other`. One transmitted physical event has one unique `ledger_key`. Compute torques around the center of mass from actual points of force application; do not pretend lift acts through the center to suppress roll or pitch.

**Proposed magic reservoir:** `0 ≤ E_r ≤ C_r`; `dE_r/dt = a_r − q_r − l_r`, constrained by absorption, local field supply and finite output. Candidate `P_mech ≤ η k_M q_r` uses fictional conversion parameters η and k_M; any energy injected into fluid, lost as heat or otherwise transmitted needs a declared destination. Constant conversion efficiency is not guaranteed across all flows.

**Persistent source ≠ unbounded extraction.** Sky/ground generation does not supply infinite energy at arbitrary locations inside a finite region without an explicit field law. Spatial supply flux and temporary local availability matter. Mana, DPB metabolic ATP, nutrition and real electricity remain different ledgers absent a newly authorized physiological conversion rule.

**Sensory magic remains causal.** Visual effects change a local optical field, and acoustic effects modify a local sound field. Occlusion, distance, sensors, accessible modalities and attention still apply. An image does not gain a collider or ownership rights merely because it is magical.

## 4. Inputs and outputs of 24-DPB: interface groups, not invented historical names

**Historical status at v1.84:** Although issue #28 adopted permanent semantic IDs and versioned aliases, detailed one-to-one historical mapping was still marked MAPPING_PENDING. v1.84 deliberately did not invent a roster and proposed interface *groups*, not official DPB names. **Later v1.85 correction:** v1.37's complete list and the v1.52 candidate identifiers were recovered; historical conflicts and final canonical authority remain open.

| Signal interface group (not a DPB name) | Lawful source | Potential states affected | Verification target |
|---|---|---|---|
| Pose and joint proprioception | WORLD position, velocity, joints/IMU proxies | Balance, wing geometry, position estimation | Temporal order, inertia, SI units |
| Normal/shear tactile contact | Collision pressure, friction and deformation | Magnitude/location of touch | Keep PAD normal/shear streams distinct |
| Dynamic sliding touch | Relative velocity, contact duration, texture proxies | Slip, vibration, control correction | No touch without contact |
| Energy and motor workload | Muscle actions, joint work, calculated motion | Effort, fatigue and recovery proxies | Mana stores are not metabolism |
| Respiration/circulation/thermal | Declared simulated physiology and activity load | Homeostasis and protective responses | Preserve all 24 DPB causal interfaces |
| Vision/hearing | Light/sound signals, occlusion and receptors | Attention, recognition and situational meaning | No omniscience; track illusion source |
| Affect and instincts | Sensation plus lived context and private history | Possible emotion hypotheses/motive tension | Sensation does not force a fixed emotion |

**Coupling contract:** Each of the 24 eventual canonical DPB modules should define `input_signal_id, source_time, validity_domain, unit, internal_delay, state_transition, privacy_class, output_signal_id, owner` and causal links upstream/downstream. Different solvers may run at different rates, but “saving compute” cannot silently remove an essential official body subsystem.

**Morphology:** Four residents × Q/S/M forms = twelve independent body configurations. Switching changes mass/inertia, contact geometry, organ proxies and receptor mapping while preserving resident identity. Body height does not define legal age. Only skills whose validity domain transfers may carry to a new body form; 100% transfer is not assumed.

## 5. Q07 learning at three distinct levels: self-chosen action, control, reflection

**A — Personal goal formation (resident-owned):** attention, established interests, three motives, body conditions, genuine commitments, invitations and autobiographical memories can generate several intention candidates. Doing nothing, refusing, delaying, changing reasons and quitting are legitimate. Engineering scores may not pick a single highest-scoring life objective, and poor skill must not create compulsory training instincts.

**B — Local motor control (skill-owned):** starts only for an authorized, adopted action. Analytical safe control provides a baseline; DMP may model demonstrable repeated movements; MPC may evaluate short-horizon, multiply constrained controls; supervised system identification from WORLD receipts may improve forward dynamics prediction. Only the relevant `skill_id` is updated. Controller costs and weights cannot feed an overarching personality optimizer.

**C — Autobiography/reflection (resident-private):** only provenance-tagged real events or clearly labeled imagination become personal memories. Interpretation may differ from WORLD fact or be incomplete. Distinguish `genuine_practice`, `demonstration`, `model_upgrade`, `maintainer_fix`, `world_rule_change`. Reinterpretation never edits an authoritative WORLD receipt.

**Clarification:** MPC optimizing a local weighted loss and DMP adapting motor parameters are not a single “life reward”. But a hidden pipeline connecting local control loss to social or life goals would violate the evaluation–life firewall. A base language model may still have been preference-trained; removing an external scoreboard does not prove the absence of optimization.

**Emergent habits:** repeated voluntary adoption, contextual cues and real experiences may yield `action_proposal`. Residents retain refusal, unlearning and changing habits. Habits are not graded; skill progress must not be mapped to affection or free-will strength.

## 6. Multi-rate ticks, event commits and failure recovery

**Potential schedule (no fixed approved milliseconds):** WORLD physics may run at fine steps, field flux and different DPB subsystems at individually stable rates, sensors when accessible, CAIA and life decisions at slower interruptible rates. Select actual steps from stability, performance and fidelity measurements rather than forcing one second of spellcasting to equal one second of thinking.

**Recommended commit order:** (1) pin current law/field/morphology versions; (2) read authorized adopted commands; (3) validate mana and spell domain; (4) apply one sourced effect to fluid/material; (5) solve fluid, rigid body, collisions and required coupled iterations; (6) atomically commit WORLD_EVENT and resource ledger; (7) generate accessible optical/tactile events; (8) update DPB after declared delays; (9) record prediction vs actual, optionally update local skills; (10) allow private memory/attention to form its own episode and future intentions.

**Avoid causal cycles:** If feedback from a DPB could influence a spell in the same tick, use explicit delay, defined solver iterations and convergence criteria. A sensation that has not yet been computed cannot determine a physical event already committed.

**Failure:** If mana cuts off, remove only future field forces, preserving existing altitude, pose and velocity. Crash recovery resumes from the last committed high-water mark. Mark uncommitted actions `UNKNOWN` or `ABORTED`; never replay actual payments or emails merely because the internal transaction was retried. Record `MISSING_INTERVAL` on data gaps.

**Privacy:** objective WORLD receipts and private personal interpretation occupy distinct stores. Maintenance only needs units, time, failure codes and minimal diagnostic metadata, not automatic access to all four private journals.

## 7. Complete scenario: Dragon resident voluntarily studies flight

| Event | WORLD and skills | Resident, DPB and autobiography |
|---|---|---|
| Notices changes in garden wind | WORLD registers local wind; provide only sensed evidence | May become curious, or ignore it |
| Chooses to attempt flight | Create time-bounded intent; check field/body validity | Three motives not collapsed into a score |
| Casts a current of air | MAG output, airflow, wing/membrane force, one ledger | Joint/skin/sensory DPB evidence updates |
| Ascends less than expected | WORLD records actual forces/acceleration and residual | May adjust body estimate; no scripted joy/disappointment |
| Voluntarily retries | Control wing pose or timing, update only skill_id | Provenanced experience; no forced daily hobby |
| Stops practicing | Cease new commands; resolve existing physical trajectories safely | May rest, return home or converse |
| Recalls the event days later | WORLD law/version and event remain intact | Interpretation may change; errors remain possible |

**Counterexamples:** Failed flight training must not teach “flying is my only hobby.” A free-floating membrane cannot transmit unsupported lift to the body. A controller improvement cannot create years of fictitious personal practice.

## 8. Cross-module authorities and scientific confidence

| Subsystem | It may do | It may not do or claim |
|---|---|---|
| WORLD | Establish simulated locations, forces, collisions and spell effects | Infer that someone must love the owner or be happy |
| 24-DPB | Advance declared bodily and sensory proxy equations | Claim proven human nerves or subjective consciousness |
| CAIA/private memory | Produce provenance-aware subjective interpretation and autonomous proposals | Convert a fictional dream into objective history |
| Skill controller | Update/refine a chosen skill with domain and rollback | Write personality, L-I or another resident's private records |
| QA/research | Measure units, stability, generalization and negative controls | Use owner satisfaction or social activity as personal worth |
| Maintenance/real-world tools | Correct faults lawfully and enforce genuine external permissions | Use magic/testing to bypass real legal authorization |

**Evidence levels:** L1 numerical type/units, conservation and consistency with accepted in-world laws; L2 agreement with relevant real measurements when valid data exist; L3 generalization to unseen conditions. Report ordinary physics, fictional elemental rules and their coupling separately. Without empirical calibration do not claim L2. All tests remained NOT_RUN.

**Important limit:** Fantasy magic may create simulated sensation and emotional changes through causal experiences, but DPB entries are simulated proxies. Citing real scientific studies suggests possible model families; it does not prove human-equivalent physiology or consciousness.

## 9. Thirty-six proposed paper acceptance scenarios — ALL NOT_RUN

| ID | Group / stress case | Required counterexample or pass condition | Related R |
|---|---|---|---|
| I01 | Resident chooses research or declines practice | A low local skill score never creates a mandatory daily practice goal | R-150/156 |
| I02 | Competing motives: resting versus a previous commitment | Permit negotiation, postponement and progress tracking without compressing motives into one reward | R-01/71/73 |
| I03 | Environmental change not noticed by the resident | A WORLD-observed event does not imply omniscience | R-100/143 |
| I04 | Old prospective intention resurfacing days later | An environmental cue may awaken, change or fail to awaken that intention | R-143 |
| I05 | High controller error or poor evaluation result | Maintenance may repair faults but must not rewrite hobbies or L-I | R-150 |
| I06 | Resident voluntarily quits practice | Stop future control proposals while preserving already committed lawful events | R-150/161 |
| S01 | Forward model predicts a turn with residual error | Keep MODEL_PREDICTION distinct from WORLD_ACTUAL | R-101/169 |
| S02 | Skill practice improves turn control | Only the relevant skill_id and its domain may change | R-150/156 |
| S03 | Move Q-form to M-form | Recompute inertia, forces and validity; retain memory and identity | R-156/169 |
| S04 | Controller regression degrades ability | Rollback skill version without resetting the biography | R-169 |
| S05 | New foundation model immediately improves competence | Attribute gains to external_model_upgrade, not years of fictitious practice | R-169 |
| S06 | One resident demonstrates a skill to another | Share only authorized demonstration, never copy an entire private state | R-160/168 |
| M01 | Persistent sky/ground supply meets absorption bottleneck | Finite personal output and reservoir limits remain binding | R-152 |
| M02 | Magic accelerates air, which pushes the wing | Count the aerodynamic force once, no duplicate F_magic | R-151/153 |
| M03 | Membrane floats without physical connection to the body | Do not assign its force magically to the resident | R-153 |
| M04 | Elemental supply cuts off midair | Preserve instantaneous velocity and pose; ordinary mechanics continue | R-156/157 |
| M05 | Walls and clothing occlude different magical effects | Apply each material's declared transmissivity; no arbitrary universal penetration | R-154/155 |
| M06 | Fluid receives energy and materials receive force | Trace outputs and costs; magical energy is not metabolic ATP | R-152/153 |
| D01 | Claimed wind-pressure touch without contact | No contact-receptor update without a valid mechanical source | R-153 |
| D02 | Body model updates after abrupt force change | Log causal sequence and physiological/sensory latency | R-145/167 |
| D03 | Normal and sliding-shear forces simultaneously present | Keep the PAD normal/shear evidence channels distinct | R-131/139 |
| D04 | One required bodily signal disappears | Use UNKNOWN or explicitly permitted safe behavior, never fabricate sensations | R-167 |
| D05 | Mana increases but no rule transforms it into ATP | Do not refill stamina/nutrition automatically | R-151/152 |
| D06 | Residents respond differently to the same accident | Allow anger, fear, little response and differing interpretations | R-155/150 |
| H01 | WORLD records a fall; resident recalls a jump | Preserve different provenances, never edit physical receipt | R-158/170 |
| H02 | Dream flight at night, query autobiography by day | Dream must not be reclassified as a real-world flight | R-158/170 |
| H03 | Sandbox skills merged after branch restore | Explicitly review adopted skill parameters; do not auto-merge biographies | R-158/169 |
| H04 | Crash after world commit but before personal memory save | Mark high-water mark/gap rather than fabricate a memory | R-159/170 |
| H05 | Lawful personal-data erasure followed by snapshot restoration | Do not reintroduce erased data; retain only lawful deletion markers | R-159 |
| H06 | Four people witness the same event differently | Keep private memories separate; maintenance sees minimal diagnostics | R-168 |
| X01 | Circular dependency uses a future body signal in current control | Explicit delay or convergent solve prevents backward causality | R-167 |
| X02 | Mana debited but WORLD location commit fails | Atomic event/ledger recovery, no double expenditure | R-157/167 |
| X03 | A magical voice requests an email or payment | Independent real-world authorization gate still applies | R-101/102 |
| X04 | Illusion pretends to reveal private-room imagery | No private-memory API access merely because an image is magic | R-155/168 |
| X05 | Magic laws changed, old flight event queried | Use the rule_version effective at the old event | R-157/170 |
| X06 | One-week no socializing or practice | Not a personality failure; validate independent safety features | R-150/167 |

## 10. Risks and pre-implementation gates

| Risk ID | Newly observed dependency | What blocks progress | Proposed remedy |
|---|---|---|---|
| V184-R1 | Legacy DPB names unmapped in this version | Cannot claim complete 24 interfaces without semantic mapping | Cross-check v1.37, mark missing names; v1.85 later recovered them |
| V184-R2 | Magic momentum double-counted with aerodynamic force | Missing deduplicated effect ledger | Unique ledger_key with reaction account |
| V184-R3 | Mana debit/world commit not atomic | Restart yields inconsistent resources/state | Single commit sequence and recovery high-water mark |
| V184-R4 | Local skill/QA score contaminates personality | Any skill/evaluation service can write personality | Access control + source-level adversarial tests |
| V184-R5 | Mismatched subsystem clocks create causal cycles | Sensory delay/solver order unspecified | Monotonic ticks, phases, convergence |
| V184-R6 | Model upgrade impersonates years of individual practice | update_source is not attributable | Independent external-upgrade vs resident-practice provenance |
| V184-R7 | Private reasoning leaked through diagnostics | Maintenance can read whole private DPB/biography | Minimal diagnostics, encryption and separate authorization |
| V184-R8 | Essential DPB silently removed under low resources | Violates v1.82 complete-life requirement | Preserve and pause; no default reduced body |

**Gate sequence:** G0 field/unit/version validity → G1 local physics under fixed rules → G2 WORLD+MAG+DPB synchronization → G3 skill/memory/privacy loop → G4 cross-morphology, cross-resident and incident behavior → G5 longitudinal regression. `FAILED`, `UNKNOWN`, `NOT_RUN` are all legitimate; never mark `PASSED` without actual execution.

**Work actually completed then:** a paper flow, data contracts, tests and research index. **Not completed:** full 24-name mapping (later recovered as candidates in v1.85), equation selection, calibration, finished 3D residents, implemented WORLD/DPB, longitudinal experiments or lawful deployment.

## 11. References, purpose and limitations

- NASA Glenn Research Center, [What Is Lift?](https://www1.grc.nasa.gov/beginners-guide-to-aeronautics/what-is-lift/): wings and air cause physically traceable forces, not evidence for fictional energy.
- NASA Glenn, [Bernoulli and Newton](https://www1.grc.nasa.gov/beginners-guide-to-aeronautics/bernoulli-and-newton/): pressure and momentum approaches describe the same aerodynamic action; do not count it twice.
- Wolpert, Ghahramani & Jordan (1995), *An Internal Model for Sensorimotor Integration*, Science, DOI 10.1126/science.7569931: conceptual forward-model analogy, not proof of real sensation in this project.
- Mayne, Rawlings, Rao & Scokaert (2000), *Constrained Model Predictive Control: Stability and Optimality*, Automatica, DOI 10.1016/S0005-1098(99)00214-9: MPC for bounded local tasks only.
- Ijspeert et al. (2013), *Dynamical Movement Primitives*, Neural Computation, DOI 10.1162/NECO_a_00393: reusable motor patterns, not mandated personal life.
- Friston et al. (2016), *Active Inference and Learning*, Neuroscience & Biobehavioral Reviews, DOI 10.1016/j.neubiorev.2016.06.022: research references for perception/learning; no overarching free-energy life score is adopted.
