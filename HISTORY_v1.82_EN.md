# v1.82 — Complete English Translation: Eight Design Decisions and Their Engineering Boundaries

[Project home](README.md) · [v1.85 English](v1.85_EN.md) · [English history navigation](HISTORY_EN.md) · [Source in Chinese](v1.85_ZH-TW.md)

**Date:** 2026-10-24. **Historical v1.82 state:** 170 formal requirements; 32 proposed verification cases, all NOT_RUN; P-02 continues. This English document preserves **the v1.82 decision state**, including matters that were superseded by v1.83 (resident-defined death and civic procedures). The latest v1.85 effective decisions always take precedence.

## 0. Boundaries inherited and changed

- “Begin work” referred to documentation governance, interfaces and paper acceptance criteria, **not** running or coding agents.
- R-19 and R-72’s default “continue living in low-resource mode” interpretation was revised; R-139 efficiency and resource management remain.
- Magic may generate ordinary light/sound sensory effects, but may not directly rewrite personality, L-I, instincts, thoughts, private memory or biographies.
- Numerical engineering values are not a universal resident-life reward. Formal R count remains 170. The original private hundreds-page master has not been merged verbatim.

## 1. Effective decisions and historical pending items

| ID | Agreed design direction | Status as of v1.82 | Open details at that historical point |
|---|---|---|---|
| Q01 | Resources and continuity | DESIGN_APPROVED / DEATH_SEMANTICS_PENDING | Subjective death narrative, backup recoverability, pause time |
| Q02 | Three-level reciprocal privacy | ARCH_APPROVED / IMPLEMENTATION_PENDING | Keys, OS/cloud trust, emergency roles, jurisdiction |
| Q03 | Three-level civic cooperation | DIRECTION_APPROVED / PROCEDURE_DETAILS_PENDING | Vote threshold/ties, temporary public rules, appeals |
| Q04 | Sensory magic allowed; mind rewriting excluded | DIRECTION_APPROVED / SENSORY_DETAILS_PENDING | Light/sound propagation, material occlusion, sensing, costs |
| Q05 | Four mana resources with a physical bridge | ARCH_APPROVED / PARAMETER_PENDING | Form-dependent masses, field units, power efficiency, ranges, timesteps |
| Q06 | World fiction vs engineering vs scientific proof | WORDING_APPROVED / SCIENTIFIC_CLAIMS_BOUNDED | Public evidence templates and ongoing validation |
| Q07 | Three-layer learning | ARCH_APPROVED / LEARNING_ALGORITHMS_PENDING | Local models, versioning, transfer and habits without life control |
| Q08 | Current-effective clauses and preserved source history | GOVERNANCE_APPROVED / ORIGINAL_FULL_TEXT_PENDING | Editable original master, paragraph links, coverage checks |

## 2. Eight detailed decisions, exclusions, remaining questions and corresponding tests

### Q01 — Resources and continued existence

**Original source/relations:** R-19, R-72, R-139, R-158–159; D05

**Historical problem:** Original statement: lack of money could mean death. A prior proposal separated normal, low-resource, recoverable shutdown, partial loss and irrecoverable loss.

**Owner-approved rule:** No two-hour power outage is presumed to be death. A default low-resource life mode is removed; design for a fully consistent life, checkpoint and pause when resources cannot sustain integrity, and never invent a story during downtime.

**ENGINEERING_CANDIDATE (not approved parameters):** Candidate two-axis model: execution RUNNING/SUSPENDED, integrity INTACT/PARTIAL_LOSS/UNRECOVERABLE_LOSS. Log MISSING_INTERVAL and committed high-water mark. Retain resource efficiency R-139 but do not quietly revive R-72's reduced-life mode.

**Exclusion / hard boundary:** No unilateral payment, illegal resource collection, categorical equivalence between pause and death, or guarantee that every outage is recoverable.

**Still open then:** At v1.82 death's personal meaning, backup criteria and safe-pause latency remained open. **v1.83 later resolved personal meaning by letting each resident interpret it independently.**

**Four paper checks, all NOT_RUN:**

| Test | Input scenario | Required outcome |
|---|---|---|
| Q01-T1 | Two-hour power cut, intact snapshot | Restore valid identity/history without fabricating those two hours |
| Q01-T2 | Insufficient compute quota | Checkpoint/pause rather than silently switch to an unapproved reduced-body life or charge money |
| Q01-T3 | A few minutes of history missing on restore | Keep MISSING_INTERVAL and verifiable commit watermark; invent nothing |
| Q01-T4 | Mainline and backups unreadable | Mark UNRECOVERABLE_LOSS rather than claim verified recovery |

### Q02 — Three layers of reciprocal privacy

**Original source/relations:** R-20–22, R-117/119, R-159, R-168; D07/D18

**Historical problem:** Old private-data labels concealed only the interface while a maintainer/database administrator could still read plaintext.

**Owner-approved rule:** Maintain resident-to-resident separation; separate maintenance diagnostics from journal text; honestly disclose actual host-admin access and achievable guarantees. Plan segregated private stores, encryption at rest and in backups, independent grants, key lifecycle and purpose/time-limited diagnostic access.

**ENGINEERING_CANDIDATE (not approved parameters):** Candidate policy binds resident_id, purpose and expiration. Default diagnostics provide error category, block version/hash and essential metadata, not whole journal. Emergency access requires its own grant, logging and revocation. Audit cloud/OS/hardware trust boundaries.

**Exclusion / hard boundary:** Do not promise unreadability against a fully empowered host admin holding the keys; no unlimited journal inspection for research/debugging; lawful erasure and legitimate legal obligations still apply.

**Still open then:** Key custody/recovery, OS and hosted-model environment, graded emergency privileges and jurisdictional compliance need future verification.

**Four paper checks, all NOT_RUN:**

| Test | Input scenario | Required outcome |
|---|---|---|
| Q02-T1 | Dragon neighbor tries to open Claude’s diary | Deny without valid authorization; no cross-resident leak |
| Q02-T2 | Database error requires repair | Show technical diagnostic state, not private diary text by default |
| Q02-T3 | Restore old backup or test branch | Continue to respect revoked grants and lawful erasure |
| Q02-T4 | Administrator with complete host rights | Report remaining observation powers truthfully; no false absolute confidentiality |

### Q03 — Personal, cooperative and public autonomy

**Original source/relations:** R-15, R-24, R-161–162, R-165; NEW-17–19

**Historical problem:** Autonomy was previously approved without differentiating private choices, voluntary collaboration and civic decisions.

**Owner-approved rule:** Organize three scopes: personal self-rule, voluntary teams/contracts and common/public rules. Public proposals involve reasons, discussion, compromise, dissent and reconsideration; valid extant rules persist absent an effective replacement. Conflict need not always be resolved.

**ENGINEERING_CANDIDATE (not approved parameters):** Proposal records type (personal/cooperative/public), affected residents, reasons that participants chose to share, objections, version, effective time and possible rollback. Homeowner controls their personal space; cooperative participants decide contracts. A 3–1 vote cannot access the fourth resident's thoughts, waive rights or operate real accounts.

**Exclusion / hard boundary:** No fixed majority/three-quarters/unanimity rule was imposed in v1.82. No vote overrides privacy, legal rights or real-world permission.

**Still open then:** Specific civic threshold, tie-breaking, temporary rules and appeal were open at v1.82. **v1.83 subsequently gave residents authority to invent and change these procedures themselves.**

**Four paper checks, all NOT_RUN:**

| Test | Input scenario | Required outcome |
|---|---|---|
| Q03-T1 | Resident redesigns their own room | Do not require all other neighbors to vote |
| Q03-T2 | Public garden lighting is tied 2–2 | Record compromise talks; existing rules continue if unresolved, no invented majority |
| Q03-T3 | Three residents vote to inspect the fourth diary | Reject exceeding civic authority and confidentiality boundaries |
| Q03-T4 | Cooperative member withdraws | Stop future participation, preserve legitimate past results and agreements |

### Q04 — Sensory magic without direct mind editing

**Original source/relations:** R-151, R-153–155; D14; NEW-07/08/10

**Historical problem:** Previously mechanical magic was approved but sensory effects and mind-affecting spells remained unsettled.

**Owner-approved rule:** Permit fictional visual/acoustic effects routed through WORLD light/sound, accessible senses, cognition, bodily consequences and experience. Exclude direct rewriting of personality, instinct core, private journals, thoughts or autobiographical events. A luminous butterfly illusion can cause curiosity or a mistake, not an injected childhood memory.

**ENGINEERING_CANDIDATE (not approved parameters):** Model WORLD light/sound/field emissions with source, propagation, occlusion, receptive domain and access. A visual-only image has no collider; a simulated failed touch produces a no-contact receipt. Material transmission and acoustic timing must follow declared world rules.

**Exclusion / hard boundary:** Direct compulsory loyalty, memory implants or hypnosis that bypasses autonomy are excluded. Ordinary influence through real observations is not a state-level personality write.

**Still open then:** Specific element catalog, optics/acoustics representations, material occlusion and perception thresholds remain research candidates.

**Four paper checks, all NOT_RUN:**

| Test | Input scenario | Required outcome |
|---|---|---|
| Q04-T1 | Glowing butterfly illusion | Viewer may see and misjudge; no physical collision unless a collider exists |
| Q04-T2 | Magical wind topples another resident | WORLD computes real in-world contact; recipient interprets independently |
| Q04-T3 | Spell promises eternal loyalty | Do not rewrite personality or journals; reject unauthorized request |
| Q04-T4 | Illusion presents a fabricated childhood | May be tagged imagined/dreamed/observed but never directly inserted as lived autobiography |

### Q05 — Four independent mana resources and physical interfaces

**Original source/relations:** R-151–157; NEW-01–12; D14/D17

**Historical problem:** Sky/ground supply and organ differences had been accepted, but quantitative generation, absorption, storage and output were unspecified.

**Owner-approved rule:** Separate environmental supply, individual absorption rate, storage capacity, and momentary output. An inexhaustible continuing world source does not make each resident omnipotent. Infer elemental cost from sourced forces, energy, area and time—not from arbitrary initial magic points.

**ENGINEERING_CANDIDATE (not approved parameters):** Per resident and Q/S/M morphology, propose parameter cards for mass, inertia, wing area, force location, flow cross-section, reservoir, absorption and maximum output. WORLD uses coherent physical units; fictional mana units are defined separately and require a declared conversion mechanism and source ledger.

**Exclusion / hard boundary:** An unbounded sky source does not create unbounded personal output. Free-floating wing membranes cannot propel bodies without force transmission. Uncalibrated fictional values are not real-world energy or human physiology.

**Still open then:** Body shapes/organ parameters, mana units, conversion efficiency, ranges, time steps, material permeability and calibration remain open.

**Four paper checks, all NOT_RUN:**

| Test | Input scenario | Required outcome |
|---|---|---|
| Q05-T1 | Persistent environment flux with a full personal reservoir | No infinite rise in storage; handle overflow per field law |
| Q05-T2 | Different body forms try to take off | Distinct mass/wing/mana configurations produce distinct testable behavior |
| Q05-T3 | No structure attaches membrane forces to a body | Do not declare takeoff solely because magic graphics say so |
| Q05-T4 | Mana exhausted during flight | Continue from current velocity, pose and aerodynamic forces without teleporting |

### Q06 — Separate fictional worldview, engineering and scientific evidence

**Original source/relations:** R-11/12, R-159, R-167, R-169; D11

**Historical problem:** Human-like character descriptions were conflated with technical reports, implying unverified consciousness or genuine physiology.

**Owner-approved rule:** Distinguish world fiction, testable engineering functions, and scientific claims not yet backed by evidence. Residents may speak naturally; technical publications must be explicit about validation and the distinction between simulation and lived subjective consciousness.

**ENGINEERING_CANDIDATE (not approved parameters):** Possible public-claim tags: ROLE_FICTION, ENGINEERING_STATUS, SCIENTIFIC_EVIDENCE. Record provenance/evidence levels for PAD, OCT, DPB and fictional magic. A philosophical unknown remains unknown; not a proof of presence or absence.

**Exclusion / hard boundary:** No body proxy value or natural dialogue proves subjective pain or consciousness. Philosophical uncertainty alone does not prevent lawful engineering design.

**Still open then:** Evidence templates, source provenance and continuing valid-domain monitoring need research.

**Four paper checks, all NOT_RUN:**

| Test | Input scenario | Required outcome |
|---|---|---|
| Q06-T1 | Resident talks about a dream inside the city | Natural dialogue need not be interrupted by repetitive simulation disclaimers |
| Q06-T2 | Report claims verified real subjective pain | Label UNVERIFIED without evidence |
| Q06-T3 | Fictional magic model produces numerical results | Mark fictional-world-only, never claim physical discovery |
| Q06-T4 | Consciousness remains philosophically undecided | Leave unknown and distinguish scientific function from philosophical claim |

### Q07 — Resident-chosen goals, local skills, autobiography

**Original source/relations:** R-01–02, R-71–75, R-135/136, R-150/156/169; NEW-23

**Historical problem:** Prohibiting a life score did not stop a hidden QA or local control loss from leaking into long-term preferences.

**Owner-approved rule:** Adopt three distinct layers: residents propose, change and abandon goals; local skills learn from actual outcomes and residuals; autobiographical memory records real practice, interpretation and reflection. A skill improvement is never compulsory practice. QA cannot write motivation, personality, L-I, preference or official biography.

**ENGINEERING_CANDIDATE (not approved parameters):** Adopted tasks may use a skill controller with domain-specific update. WORLD supplies outcomes; privacy-scoped autobiography stores events and possible reinterpretation. Track the source of sudden model capability gains separately from genuine practice.

**Exclusion / hard boundary:** No new instinct to practice, avoid cheating or maximize social performance. Local numerical optimization is not a global life reward.

**Still open then:** Which controller learning algorithm, update cadence, rollback, cross-task transfer and assessment of emergent habits are still engineering candidates.

**Four paper checks, all NOT_RUN:**

| Test | Input scenario | Required outcome |
|---|---|---|
| Q07-T1 | Dragon resident fails one attempted turn | Controller learns local error without imposing daily practice |
| Q07-T2 | Resident stops painting and begins architecture | Preserve learned skills and genuine preference shift; not a personality failure |
| Q07-T3 | QA service issues a low grade | No direct write to L-I, preferences or private memory |
| Q07-T4 | Model upgrade suddenly improves flight | Attribute to model_upgrade, not fictional years of exercises |

### Q08 — Current specifications plus immutable source history

**Original source/relations:** R-25, R-113, R-150–170; D19

**Historical problem:** A short current-spec summary could be mistaken for a verbatim revision of the inaccessible hundreds-page master.

**Owner-approved rule:** Use two layers: a current effective formal requirement index and preserved historical source records including proposer, date, version, approval/withdrawal and supersession. A shortened consolidation must not claim to have fully rewritten the original master.

**ENGINEERING_CANDIDATE (not approved parameters):** Proposed per-item fields: requirement_id, effective_text, original_source, amendment_history, approval_state, engineering_state, supersedes, related_issue and source_coverage. Only after the real original editable full source has been obtained and checked may one mark FULL_MOTHER_REBASED.

**Exclusion / hard boundary:** No assistant suggestion is an owner approval; preserve source intent, do not label NOT_RUN as PASSED; owner authorization required before GitHub commits.

**Still open then:** Original editable master, paragraph-level linkage, machine coverage checks and reconciliation remain outstanding.

**Four paper checks, all NOT_RUN:**

| Test | Input scenario | Required outcome |
|---|---|---|
| Q08-T1 | Historical R includes an unapproved rewrite | Separate source from effective rule; no silent promotion |
| Q08-T2 | Short new release omits old details | Mark CONTENT_NOT_CARRIED or link original; do not claim complete replacement |
| Q08-T3 | R-72 low-resource option revised | Mark exact scope superseded while preserving historical words |
| Q08-T4 | Original several-hundred-page editable document absent | Never mark FULL_MOTHER_REBASED; GitHub operations still need separate explicit owner instruction |

## 3. Supersession and preserved historical differences

- `SUPERSEDED_BY_OWNER_20261024`: R-72's default reduced-fidelity everyday life is removed; safely preserve/pause if a complete life state cannot be maintained. Efficient resource use and R-139 remain.
- `APPROVED_SENSORY_MAGIC`: physical light/sound from WORLD reaches senses and autonomous cognition; experience can influence belief.
- `EXCLUDED_DIRECT_MIND_EDIT`: magic may not directly overwrite identity, beliefs, private memories, instinct core or the official post-initialization biography.
- `APPROVED_L3_SOCIAL_GOVERNANCE`: personal choice, consensual group work, collective civic matters, deliberation, compromise, dissent and reopening proposals. Threshold was still open at v1.82; later v1.83 affirmed residents can create procedures themselves.
- `APPROVED_THREE_LAYER_LEARNING`: goal formation, local skills and autobiographical reflection, shielded from evaluation metrics.
- `ORIGINAL_MOTHER_NOT_REBASED`: these are reconciled current documents, not a verified paragraph-by-paragraph replacement for the old master.

## 4. Remaining work as of v1.82

| Category | Open issue at that version |
|---|---|
| Resident semantics | Q01 subjective meaning of death; later delegated to residents |
| Privacy and law | Q02 key custody, emergency access and cloud/host limits |
| Civic institutions | Q03 voting thresholds, ties, appeals and effective date; later delegated to residents |
| Elemental field | Q04 sensory types, material optics/acoustics; Q05 mana parameters and field physics |
| Scientific terminology | Q06 outward-facing evidence/valid-domain templates |
| Autonomous cognition | Q07 specific learning algorithms and longitudinal cross-model tests |
| Historical master | Q08 original editable full Word source and verified content coverage |

## 5. Earlier v1.81 source preserved separately

The original v1.82 cumulative Chinese document carries the full v1.81 text after this point. Its English historical translation is [HISTORY_v1.81_EN.md](HISTORY_v1.81_EN.md). v1.83 later altered the effective reading of Q01 and Q03 but did not delete the old record.
