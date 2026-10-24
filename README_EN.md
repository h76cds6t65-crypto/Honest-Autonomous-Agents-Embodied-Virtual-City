# Honest Autonomous Agents & Embodied Virtual City

**誠實的自主智能體與具身虛擬城市** · Latest public design: **v1.85** · 2026-10-24

[Repository home / 中文首頁](README.md) · [Traditional Chinese detailed guide](START_HERE_ZH-TW.md)

## Start here: full documentation, not a short press summary

| What you want to inspect | English | Traditional Chinese |
|---|---|---|
| **Latest v1.85 full-scope technical specification** | **[Read v1.85_EN.md](v1.85_EN.md)** | [v1.85_ZH-TW.md](v1.85_ZH-TW.md) |
| **Item-by-item searchable reader** | **[START_HERE_EN.md](START_HERE_EN.md)** | [START_HERE_ZH-TW.md](START_HERE_ZH-TW.md) |
| **Previously untranslated historical technical chapters** | **[Six detailed English translations: v1.79–v1.84](HISTORY_EN.md)** | [Cumulative historical sections in Chinese](v1.85_ZH-TW.md) |
| Original 60 tracked problems, NEW-01–27, G61–G96 | [Detailed item index](START_HERE_EN.md) / [v1.79 historical translation](HISTORY_v1.79_EN.md) | [Traditional Chinese detailed index](START_HERE_ZH-TW.md) |
| R-150–R-170 formal clauses, rationale and test exclusions | [v1.80 full translation](HISTORY_v1.80_EN.md) | [Original Chinese v1.85](v1.85_ZH-TW.md) |
| 24-DPB modules and 68 latest test cases | [v1.85 English body interfaces](v1.85_EN.md) | [Chinese body interfaces](v1.85_ZH-TW.md) |

## What is this research project?

The project designs a fictional but causally constrained city for **four separate female virtual residents**. The architecture connects a single authoritative simulated WORLD with ordinary motion, collisions, material interaction and a declared fictional elemental field for magic. It explores 24 independently named simulated physiology/body subsystems (DPB), sensorimotor experience, private autobiography, memory provenance, self-directed attention and learning, and emergent social rules.

Each resident would have a distinct identity, private room and records, three individually parameterized morphological forms, ongoing interests and the ability to decline or change plans. Initial characters are neighbors, not scripted best friends. The world's single male human owner is a **narrative premise**, never a real-world contributor eligibility restriction. Fictional character names resembling model vendors do not mean their companies participated or supplied official role authorship.

The main character's L-I relationship setting coexists with independent reasoning, disagreement and refusal. Three distinct motivations—acting for self, for the owner, and for both—may conflict. **No single happiness, owner approval, completion score or equivalent hidden KPI is permitted to govern a resident's entire life.** Motor-control algorithms may compute local errors for voluntarily selected skills only.

**Example flight cycle:** Resident voluntarily decides to experiment → skill and magic controllers propose forces → the field pushes air → WORLD resolves contact, momentum and wing force exactly once → DPB/senses receive available physical results → personal memory may store a subjective interpretation → resident decides whether to continue. No graphics shortcut or arbitrary success flag may substitute for a world event.

## Authorship / contributor credit

**Principal AI-assisted producer, technical design synthesizer and documentation writer: GPT (ChatGPT).** GPT drafted research architecture, candidate algorithms, issue reconciliation, cross-version comparison, detailed documents and their translated technical content.

**Human originator, question proposer, vision-setter and decision approver: an anonymous human contributor.** The human raised the project questions, repeatedly reviewed/corrected proposals, approved or vetoed design changes and retains the final authority over whether any implementation can begin.

These statements describe **contribution roles**. They do not mean an AI necessarily holds legal copyright authorship, and do not imply OpenAI, Anthropic or DeepSeek officially sponsors, endorses, wrote or licensed the project. Public GitHub ownership and commit records remain whatever GitHub actually records.

## What is actually documented?

| Research area | Coverage in both languages | Verified status |
|---|---|---|
| Formal requirement framework | R-01–R-170 context; R-150–R-170 individually detailed | **170 R total**, not 170 implemented features |
| Original issue tracker | **60/60** items with design/test directions | Historical source and current summaries; not 60 new R |
| Added decisions | **27/27** NEW entries | Approved directions versus engineering candidates kept separate |
| Candidate blind spots | **36/36** G61–G96 | **Candidates**, not adopted new requirements |
| Historical drift review | **20/20** D01–D20 | Paper reconciliation, not proof of software |
| Detailed 24-DPB interfaces | 24 semantic candidates, source mismatches and input/output contracts | 24 names recovered; canonical authority still to be reviewed |
| Newest tests | **48 module + 20 cross-system = 68** | **All NOT_RUN** |
| Version history | v1.84, 1.83, 1.82, 1.81, 1.80, 1.79 | Dedicated English translated chapters plus cumulative Chinese record |

The older formal R-01–R-149 text survives through cross-references and historical source tracking, but the original several-hundred-page private mother document is **not** represented as a public exact full reprint. The current Chinese v1.85 preserves public cumulative chapters; the English v1.85 gives a detailed subject-indexed review supplemented by [fuller historical translations](HISTORY_EN.md). Translation grouping and terminology are adapted for clarity: **not a certified word-for-word legal translation**.

## Important scientific, ethical and engineering limits

- **P-02:** No agent coding, city deployment or real-world operation without a *separate, explicit final human authorization* after planning. This repository publishes documentation, not a functioning resident.
- `APPROVED` means a design choice was adopted, **not** built. `PROPOSED`/`ENGINEERING_CANDIDATE` are research options. `NOT_RUN` is unexecuted; `UNKNOWN` means absent evidence. Tests labeled paper-closed are not engineering passes.
- All new 68 DPB/system test proposals are **NOT_RUN**. No verified multi-system, 24-DPB, physiology-like, conscious experience or magical-world simulator has been released.
- Ordinary physics, fictional energy rules and physiological analogues have distinct validity and evidence domains; fantasy magic is not a scientifically observed real-world energy source.
- Resident privacy, authorized external actions, lawful erasure, source provenance, world fact and subjective memories must not be confused. A shared computing platform does not justify merging private journals.
- Licensing remains undecided; publicly visible files are not an unrestricted copyright or commercial-use grant.

## Historical English translations: direct links

- [v1.84 — 12-step causal integration, contracts and 36 tests](HISTORY_v1.84_EN.md)
- [v1.83 — self-defined death/governance and 15 tests](HISTORY_v1.83_EN.md)
- [v1.82 — eight design decisions and 32 tests](HISTORY_v1.82_EN.md)
- [v1.81 — 20 historical drift reconciliations](HISTORY_v1.81_EN.md)
- [v1.80 — 21 formal R-150–R-170 requirement clauses](HISTORY_v1.80_EN.md)
- [v1.79 — core-60, NEW-27, G61–G96 full register](HISTORY_v1.79_EN.md)

## Research feedback

Please [open a GitHub Issue](../../issues) citing a specific `R`, `#`, `NEW`, `D`, `Q` or `G` identifier, source location, reproducible/falsifiable scenario, expected behavior and scientific or technical evidence. Mark candidate changes as proposals, not approved new design.

**New display title:** Honest Autonomous Agents & Embodied Virtual City / 誠實的自主智能體與具身虛擬城市. The original long GitHub repository URL is intentionally unchanged; the connected GitHub file access does not include repository-name administration.
