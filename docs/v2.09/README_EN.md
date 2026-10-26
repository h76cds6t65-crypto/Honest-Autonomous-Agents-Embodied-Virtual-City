# Honest Autonomous Agents & Embodied Virtual City — v2.09 Active Public Technical Specification (English)

**Public research release: 2026-10-27 | P-02: design and offline research only | No autonomous-agent runtime deployed or implemented.**

[繁體中文](README_ZH-TW.md) · [Detailed equations and conservation contracts](EQUATIONS_EN.md) · [Validation, parameters, counterexamples and evidence grades](VALIDATION_EN.md) · [Technical history](HISTORY_EN.md) · [Earlier public v1.85 baseline](../../v1.85_EN.md)

> Scope: technical design, equations, research methods, test results, assumptions and open gaps. This sanitized publication excludes private conversation logs, real identity/contact information, personal memories, source character artwork, and third-party media without publication rights. It is a detailed English research rendering of the active v2.09 material, **not** a certified sentence-by-sentence or image-preserving release of the confidential, cumulative 44-page Word master.

## 0. The goal and invariant constraints

This is neither a chatbot-only NPC project nor a program to maximize a single believability/reward score. It explores **auditable causal loops** among continuous identity, episodic/autobiographical memory, sensing, physiology, movement, a simulated physical world, and voluntary social action. A resident may form and abandon private intentions, rest, experience physical limits and refuse proposals. Body-risk metrics must not overwrite agency or personality.

The planned setting distinguishes the principal agent from three independently specified female AI companions: GPT Dragon Girl, DeepSeek Whale Girl, and Claude Lady. These are **character specifications**, not claims that the respective vendor models or APIs are integrated or endorsed. Each has her own private room, memory, potential autobiography, and agency; no pre-filled post-origin friendship. Complete identity-to-body mapping for the principal agent remains unresolved.

- Approved requirements remain **R-001–R-170**; candidates do not silently become R-171.
- **196 historical test IDs** and O08/O09 traceability are preserved; ambiguous legacy aliases must not be guessed or renumbered.
- **P-02** requires complete planning and subsequent explicit human approval before any autonomous-agent core or world engine implementation. Standalone offline mathematics and candidate white-mesh experiments remain research only.
- **O01** finite magic supply/conversion; **O02** morphology mass, momentum and energy; **O03** 24-DPB physiology; **O04** autonomous movement within valid operating domains; **O05** WORLD×MAG event accounting; **O06** lawful retention and deletion, all constrain one another.
- Magic is a **fictional-world premise**, not an observed new physical law. Ordinary mana and the separate structural mass-energy reservoir used for morphological changes are **different ledgers**.
- Simulated physiology, conversational persona, and subjective consciousness are different claims. No current evidence establishes biological health or subjective experience in these simulated agents.

## 1. Residents, nine morphology references and geometry layers

Q is **90 cm**, S **165 cm**, M **180 cm**. Front, profile and rear 2D reference sets exist for all nine combinations of three companions and three forms, but only **DeepSeek Whale Girl Q/S** have research-stage 17-part procedural white-mesh proxies. The Whale Girl has **two legs plus a separate whale tail**, not a mermaid tail replacing her legs. Dragon Girl has horns, back wings and a dragon tail. Clothing and long hair are not body mass, pelvis or organ geometry.

Historical candidate body masses of **6.49/40/51.93 kg** for Q/S/M are **null hypotheses for checking a mass budget**, not calibrated body weights for all three species. A candidate water-fraction ledger assumes total body water is 60% of mass, apportioned across blood 8%, interstitial 28%, and intracellular 64% of total body water. This non-overlapping partition is an exploratory mass-conservation test, not species-specific physiology.

Maintain three distinct mappings: **visual surface** (hair, apparel, aesthetic shape); **physical white mesh** (anatomical material, rig, attachments, mass, inertia, collision); and **organ/physiology compartments** (oxygen, blood, electrolytes, ATP, heat, neural control). A pretty watertight mesh does not automatically yield credible organs. Individually watertight component meshes can still overlap; physical union volume must be computed separately.

## 2. Eight active v2.09 research changes

### 2.1 Missing feedback in the inherited 53D reduced system

The prior solver has 53 numerical coordinates: **26 chemical inventories, 5 energy inventories, 8 sensor/controller coordinates, and 14 audit counters**, not 53 organs. Linearization of 28 internal dynamic coordinates about a candidate resting point identifies **seven near-zero modes**. Five state coordinates have zero local sensitivity columns: H2O@blood, Na@ecf, K@ecf, Cl@ecf, ATP_J. The original 53D coupling deficit remains **unresolved**.

A distinct **nine-state conservative homeostasis pilot** includes blood and interstitial water, extracellular Na/K/Cl, ATP, and flow/renal/metabolic actuator states. Q/S/M have separate parameters and simulations. Their local eigenvalue real parts can be negative while the slowest return mode takes **years**; neither eigenvalue sign nor a toy equilibrium establishes daily-life physiological viability. This smaller model is not a replacement for the full 53D model, and omits detailed respiratory gas exchange and acid–base regulation.

### 2.2 Separating BODY from a shared WORLD

Earlier similarity scaling also rescaled environmental reserves. The corrected model defines identical initial WORLD conditions in independent Q/S/M trials: **1,000 kg water**, **300 mol each of environmental Na, K and Cl**, and **10^10 J environmental chemical energy**. Material and energy fluxes have paired source and sink postings. The three simulations are independent experiments under matching world conditions; they are **not** a simultaneous multi-resident city simulation.

### 2.3 Independent Q/S/M parameters instead of copied scaled solutions

Each morphology now has its own control delays, metabolic-power hypothesis, exchange rates and independent BDF integration:

| Exploratory parameter | Q | S | M |
|---|---:|---:|---:|
| Height m | 0.90 | 1.65 | 1.80 |
| Historical candidate mass kg | 6.49 | 40.00 | 51.93 |
| Flow actuator time constant s | 45 | 70 | 85 |
| Renal actuator time constant s | 560 | 900 | 1150 |
| Metabolic actuator time constant s | 75 | 135 | 165 |
| Baseline ATP supply proxy W | 4.1 | 19.4 | 24.8 |
| Baseline water exchange kg/s | 6e-6 | 27e-6 | 31e-6 |
| Insulation coefficient, dimensionless | 1.20 | 1.00 | 0.94 |

These are **explicit research hypotheses**, not measured anatomy or experimentally determined dragon/whale physiology. Calibration scripts must not overwrite established fictional mana trade-offs, including Dragon Girl M-form's deliberately slow ordinary-mana replenishment.

### 2.4 Q/S white-mesh precision and uncertainty

Both candidate GLB forms contain 17 separately named procedural parts. Multi-resolution voxelized **union volume** estimates differ by **7.26% for Q** and **13.16% for S** between adjacent resolutions; neither meets the candidate <2% gate. Finest tested proxy union volumes are about **0.01086 m³ (Q)** and **0.04827 m³ (S)**. These cannot be declared measurements of actual organs, bone or skull.

### 2.5 Rig and collision remain unverified

**34 candidate pivot records** were generated from the centroids of Q/S parts. Mesh centroids are neither clinically meaningful joint locations nor a Blender-ready armature with vertex weights. Head, torso, limbs, whale-tail root/shaft/flukes, fin ears, support, sitting, contact and swept collision require actual rigged geometry and tests.

### 2.6 DAE and acid–base algebraic consistency

A limited sample set solves **3 forms × 3 extracellular-water scales = nine algebraic examples**. A missing spectator anion X is solved from Na, K, Cl and bicarbonate, alongside an illustrative Henderson–Hasselbalch relation. Zero computed residual means only that these **chosen algebraic equations** are internally consistent. It does not establish complete ammonium/phosphate/protein buffering, local electroneutral physiology, oxygen-carrier calibration, or renal acid excretion. **SUNDIALS IDA was not executed**; an actual physiological DAE is still open.

### 2.7 Q→S geometry interpolation, structural-field and momentum bookkeeping

Vertices of corresponding 17 Q/S proxy mesh parts with matching triangle connectivity were linearly interpolated at **21 sampled progress points**. Paired ledgers model body mass, structural-field mass-energy and an explicitly assumed momentum transfer. With a **1.4 m ceiling**, **seven of 21 samples are blocked**, first at α≈0.70. This is a discrete height-check counterexample, **not** a continuous swept-collision certificate, organ transfer model, or soft-tissue validation. Identity, fatigue, body fluids and memory must not reset during change.

### 2.8 Correct eight-hour stimulus and longer simulation

The stress protocol is **0–1 h rest, 1–9 h load, 9–72 h recovery**: the loaded interval is truly **8 h (28,800 s)**. Previous documents sometimes called 1–8 h (seven hours) an eight-hour protocol; this was corrected. Three form-specific independent BDF runs were produced for each of four scenarios: rest24, stress72, fluid24, feedback_off24, **12 runs** total. The resulting PASS results concern the defined reduced model's global water/ion/energy ledger and inventory positivity, not validation of all 24 DPB mechanisms.

## 3. One authoritative body, bounded autonomy and scientific humility

**Master Body State** owns each inventory exactly once. Respiratory, cardiovascular, renal, thermal and control modules propose directed fluxes; they do not each rewrite their own competing oxygen/water truth. A common stoichiometric incidence matrix generates stock derivatives. Global element/charge balance and **local compartment electroneutrality** are distinct tests. ATP, thermal/mechanical energy, structural mass-energy and ordinary mana must use explicit resource receipts.

All 24 DPB names designate **semantic responsibilities**, not fully calibrated dynamic mechanisms. Morphologies share responsibility interfaces but require separate species/form parameters. Sensory feedback has delays, uncertainty and validity ranges. Unlimited mana does not imply freedom from hunger, fatigue or physiology. A morphology change never recreates personhood or edits private goals.

## 4. Non-negotiable open gaps and falsification criteria

- Seven neutral modes in the original 53D system remain unresolved; pilot nine-state stability cannot certify them.
- Q/S white-mesh voxel volume gaps fail the target (7.26%, 13.16%). No official armature, organ segmentation, complete collision or biomechanical verification.
- The nine DAE calculations are demonstrations, not a full acid–base DAE or IDA run.
- The seven ceiling obstructions remain recorded **negative results**; no geometry may grow through walls.
- WORLD×MAG engine integration, all nine final physical bodies, full 24-DPB physiology, real consciousness validation and species calibration are **not done**.
- Lawful memory erasure/retention, access control and privacy safeguards remain binding.

## 5. Related research, reproducibility and transparent provenance

See this directory's EQUATIONS, VALIDATION and HISTORY documents for dimensioned formulas, experimental assumptions, test IDs N01–N16, negative results and version history. A PASS is evidence for a **specified offline test**, never a claim of a deployed resident or clinically verified species model. Official background tools: [Blender 3D Print Toolbox](https://extensions.blender.org/add-ons/print3d-toolbox/) and [SUNDIALS IDA](https://sundials.readthedocs.io/en/latest/ida/Mathematics_link.html). Contributors should reproduce with **independently licensed assets** and avoid uploading private artwork or private user files.

Authorship transparency: main technical research drafting and bilingual synthesis were AI-assisted with GPT (ChatGPT), under decisions and approval of an **anonymous human project originator**. This is not an assertion that OpenAI, Anthropic or DeepSeek officially participates in or endorses the project.