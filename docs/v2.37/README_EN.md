# 自成之境 v2.37 Research Baseline and Development Handoff

2026-11-17 · P-02 isolated research

[繁體中文](README_ZH-TW.md) · [Public status](../../CURRENT_STATUS.md) · [v2.36 research baseline](../v2.36/README_EN.md) · [Glossary](../../GLOSSARY.md)

v2.37 follows Section 8 of v2.36 with executed evidence for C32-16 wing and fish-tail root loading, C32-17 revocation across synchronization points, and C32-18 candidate physical morphing during contact. Earlier one-room, original 65-state event persistence, and paired long-run evidence remains in v2.35 and v2.36. Both the original C32-14 sweep and the follow-up retain their overall `FAIL`.

The first Q-form v48 test round and its 18 November replay cover the original model’s scale, mesh overlaps, and single-room receptor results. [Test results](Q_DRAGON_V48_TESTS_EN.md) · [Model and reference images](../../assets/q-dragon/v48/)

## Results

| Acceptance item | Original run and archive replay | Scope |
| --- | --- | --- |
| C32-16 Wing and fish-tail roots | 413/413 each, `PASS_WITH_SCOPE` | Separate passive, slowly loaded, small-deflection beam proxies for fixed Q/S/M forms. |
| C32-17 Revocation across sync points | 947/947 each, `PASS_WITH_SCOPE` | Multiple processes on one host, one SQLite WORLD authority, and one fixed proxy body. |
| C32-18 Physical morphing and impact | 120,941/120,941 each, `PASS_WITH_SCOPE` | Axisymmetric ellipsoid, fixed wall, piecewise-linear deformation, and declared mass exchange at the center of mass. |

Counts come from the individual offline acceptance runs. They include step-by-step ledger checks, rejection conditions, and controls. Checks within a case share its inputs and evidence.

### C32-16 Local forces and material limits

The S-form wing under one uniformly distributed air load reached its candidate limit at 51.21 N, with a root bending moment of 15.36 N·m and torque of +2.30 N·m. Slow wingtip contact first reached the 5% deflection threshold at 20.83 N. An increasing load toward the S-form fish-tail tip in water reached its candidate stress limit at 22.05 N, with root bending and torsional moments of 7.35 and −1.54 N·m. Of 105 load cases, 21 exceeded the limits. Seven additional fast-loading cases were rejected. All 12 nominal results for a 15% thicker tail radius lay outside the slenderness limit.

The reconstructed first run returned 398/407, `FAIL`. Nine distributed-load cases missed the strain-energy threshold, and SciPy ignored `max_step_s`. The corrected run refined the mesh and checked actual solver steps. Each round reproduced its own 21 evidence files byte-for-byte. Actual materials, wing membrane, tail fin, tissues, and organs require calibration. Peak-force acceptance requires a contact force history and a mapping from the original joint axis to each local root.

### C32-17 Effective revocation and event recovery

WORLD ran at 120 Hz with body snapshots at 10 Hz. The authority used commit order for events in the same tick. Five authorized effects at ticks 118–122 persisted. After revocation at tick 123, the ten new requests through tick 132 were all rejected. A passive wall impact still occurred at tick 124.8, dissipating 4.6875 J. Four SIGKILL points exercised persistence and retry. A retry of a committed event returned its original receipt.

The epoch-only control returned 6/8, `FAIL`, after committing a 2 N·s unauthorized impulse following revocation. The candidate checks an effective new grant, its scope and time window, and source revision. An archive replay with fresh keys matched 34/34 main and 4/4 control evidence files at the logical level. Actual actuators, multi-host authority, and production key governance have separate outstanding acceptance work.

### C32-18 Deformation, conservation, and swept contact

Q→S, S→M, and M→Q each changed mass and inertia on both sides of impact. The solver used instantaneous inertia, surface velocity, and contact location to compute the impulse. The audit combined the body, structural field, wall, and support to check rest energy, mechanical energy, linear momentum, and angular momentum about the same fixed origin. All residuals were zero in the declared rational model. Ordinary mana had a separate ledger.

The 52 cases ran at 120, 240, and 480 Hz for 156 runs, including 33 expected rejections. In a 120 Hz expansion–contraction case, the free trajectory had 0.6 mm clearance at both endpoints. The sweep found contact at 2.5 ms. Endpoint overlap alone missed it. Another control double-counted about 0.939544 J of wall heat. Binary64 subtraction of totals including rest energy rounded the difference to zero. The independent mechanical ledger detected the discrepancy. The archive replay reproduced six primary evidence files byte-for-byte.

Physical morphing remains a design decision. Full acceptance would need three-dimensional mass distributions, sweeps with arbitrary rotation and deformation, multiple contacts, materials, organ continuity, and finite structural-field transport. Appearance swaps follow the original design conditions.

## Development handoff

- The next fixed-form integration can use one room, one actuator, and a known contact force history to connect authorization provenance, receipts, and local loading and sensing. On 19 November the fixed v48 Q-form left wingtip completed this integration and restart replay in one guided contact fixture. Material and organ calibration remain open. [Left-wingtip wall contact](Q_DRAGON_V48_TESTS_EN.md#single-room-left-wingtip-wall-contact)
- C32-14 retains the overall `FAIL` outcomes at 132/133 and 501/513. The single-impact WORLD oxygen tolerance, BDF clock stalls, and the original long-run oxygen distribution each retain their own evidence and criteria.
- Joint operation of WORLD, MAG, the original 65-state model, and 24-DPB, as well as multi-host consistency, follow their own evidence and approval conditions. P-02 uses isolated research scenarios.
