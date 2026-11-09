# 自成之境 v2.36 Research Baseline and Development Handoff

2026-11-09 · P-02 isolated research

[繁體中文](README_ZH-TW.md) · [Current status](../../CURRENT_STATUS.md) · [v2.35 handoff](../v2.35/README_EN.md) · [Glossary](../../GLOSSARY.md)

This release builds on the v2.35 single-room and simulated-day tests and the original 65-state model's short collision tests. The new evidence covers 1-, 24-, and 72-hour post-impact runs, three separated impacts, interrupted body transactions, hypoxia and heat load, solver agreement, convergence, and fixed-form validity. The v2.35 delivery addendum already recorded C32-04. This release covers it alongside the ten subsequent items.

## Executed acceptance cases

W34-01 through W34-10 passed scoped tests for a fixed proxy in one room on one host, including 86,400 simulated seconds. The C32-03 short collision and C32-08 retry deduplication scored 37/37 and 32/32. The first C32-03 run using an absolute WORLD chemical-energy coordinate scored 24/36 and failed. The damping-heat deficit in the original equations is recorded as FAIL_EXPECTED. The results with an incremental chemical-energy coordinate and an external damping-heat contribution have their own scope.

| Case | Result | Checks in original report |
| --- | --- | ---: |
| C32-04 One hour after impact | PASS_WITH_SCOPE | 53/53 |
| C32-05 24 hours after impact | PASS_WITH_SCOPE | 61/61 |
| C32-06 72 hours after impact | PASS_WITH_SCOPE | 76/76 |
| C32-07 Separated collision ordering and dissipation | PASS_WITH_SCOPE | 60/60 |
| C32-09 Interruption before durable commit | PASS_WITH_SCOPE | 25/25 |
| C32-10 Interruption after commit and before receipt delivery | PASS_WITH_SCOPE | 26/26 |
| C32-11 Hypoxia, collisions, and donor nonnegativity | PASS_WITH_SCOPE | 340/340 |
| C32-12 Heat load and event-by-event heat accounting | PASS_WITH_SCOPE | 360/360 |
| C32-13 Matched BDF and Radau runs | PASS_WITH_SCOPE | 525/525 |
| C32-14 Step size, tolerance, and convergence | FAIL in both the original sweep and the follow-up | 132/133, 501/513 |
| C32-15 Q/S/M inertia and scale | PASS_WITH_SCOPE | 273/273 |

Each result applies to the tested version and scenario. Expected failures, numerical failures, and independent reruns are recorded separately.

## Paired long runs, events, and heat accounting

- **C32-04 through C32-06.** Two BDF settings used the same resting S-form proxy and WORLD receipt. Each setting ran a no-collision control, a collision with the original equations, and a collision with one passive damping-heat contribution. The original equations reproduced a heat deficit of about −0.000311111 J at 1, 24, and 72 hours after impact. The maximum original-ledger residual in the heat-compensated runs was about 3.54×10⁻⁶ J against a 2×10⁻⁵ J limit. At 72 hours, blood oxygen was about 72.48 times its initial inventory and tissue oxygen was about 58.92% of its initial inventory. The control also reproduced the distribution drift. Donor lower bounds, conservation, and distribution calibration are assessed separately.
- **C32-07.** Right, left, and right wall contacts committed once each at ticks 25, 265, and 865. Ordered and perturbed delivery produced byte-identical receipts and 1,108 state samples. The contacts dissipated about 7.466666667, 0.114302246, and 0.029170791 mJ, totaling about 7.610139703 mJ. Continuous damping accounted for about 0.379203793 mJ separately. Premature and conflicting requests were rejected, and identical retries returned the original receipts.
- **C32-09 and C32-10.** SIGKILL stopped the body adapter at specified points on a single host running SQLite WAL with FULL synchronization. Before commit, reopening showed durable revision 0 and no body effects, physical ledger entries, or body receipt. A retry committed after authoritative verification. After commit, reopening retrieved revision 1 and the original APPLIED receipt. Retries of committed events invoked the adapter zero times. Each case retained one durable effect and matched the uninterrupted reference states and receipt. The caller initially recorded a missing receipt as IN_DOUBT.
- **C32-11.** Oxygen delivery stopped from 900 to 2700 seconds, with three impacts spanning resupply. All 24 donor categories stayed nonnegative during interruption and recovery in the natural air-cut pair. The impact jumps changed none of those inventories. The original full-window checks also recorded four FAIL_NUMERICAL paths. The candidate held four artificial zero inventories at their verified zero derivatives and used a 0.1-second explicit start after resupply. A separate startup check addressed the natural sweat-film case. Recorded inventories on all five candidate paths were nonnegative.
- **C32-12.** The environment cycled through 25→41→25 °C with activity factor 1. The three impacts at 4498, 4500, and 4505 seconds added about 6.468619 mJ of instantaneous heat. Eighteen retries added zero heat. At 4500 seconds the temperature change affected continuous heat rates. The impact receipt accounted for the instantaneous heat jump at that time. Deliberately omitting and duplicating damping produced signed short-window residuals of about −0.379204 and +0.379204 mJ, both recorded as FAIL_EXPECTED.

## Solvers and convergence limits

C32-13 matched BDF and Radau on initial conditions, events, tolerances, and step caps. The heat-load and natural air-cut runs included 24 and 72 hours after the last scheduled impact. The maximum scaled difference over 65 states was about 1.63×10⁻⁸ against a 2×10⁻⁶ limit. Without the guard, the artificial zero-inventory BDF run recorded tissue oxygen and ATP at about −1.79×10⁻²² mol and −5.55×10⁻²³ J around 0.61 ms after resupply. Radau's recorded donor values were nonnegative. Accepted steps and dense midpoints preserve this SOLVER_DEPENDENT_STRICT_ZERO difference. With the same guard, both solvers recorded nonnegative values for all 24 donor categories.

All 16 evaluable refinement ladders in C32-14 reduced their maximum scaled differences at each level. The 72-hour heat-load and natural air-cut runs passed the fine-to-finest and cross-solver finest-level comparisons. The overall result remains FAIL.

| Unmet criterion | Evidence |
| --- | --- |
| Coarse skin-heat ledger | The heat-load BDF residual was −0.0125994 J against a 0.01 J limit. |
| Single-impact WORLD oxygen | Eight absolute differences exceeded 2×10⁻⁹ mol. The maximum was 3.2159732655×10⁻⁹ mol. |
| Clock in the artificial zero-inventory case | Four fine or finest BDF runs stopped with the absolute clock. All four completed in the elapsed-time comparison. |
| Mechanism of the stops | The smallest accepted steps with the elapsed clock still exceeded the original step floor. Four mechanism checks failed. |

## Fixed-form inertia and scale

C32-15 used one wall and a passive single-axis joint in a fixed form, with zero pre-impact angle and angular velocity. Nine original proxies passed the common case at restitution 0.2, lever arm 5 mm, and impact speed 0.020 m/s. The height-scaled figures below apply to the Q/S/M forms of one proxy family.

| Form | Height (m) | Mass (kg) | Single-axis inertia (kg·m²) | Scaled lever arm (mm) | Speed ceiling (m/s) | First limiting condition |
| --- | ---: | ---: | ---: | ---: | ---: | --- |
| Q | 0.90 | 6.49 | 0.00473447 | 2.727 | 0.05629 | Angular velocity |
| S | 1.65 | 40.00 | 0.03500000 | 5.000 | 0.03402 | Subsequent angle |
| M | 1.80 | 51.93 | 0.04664039 | 5.455 | 0.02668 | Subsequent angle |

All forms passed at 98% of their ceilings and had out-of-domain results at 102%. At restitution 0.2, avoiding renewed contact requires lever arms below about 12.061/12.755/12.838 mm and compliance with the corresponding speed ceilings. In all three forms, out-of-domain cases showed a contact point crossing the wall again after the center of mass separated. Three-dimensional bodies and organs need their own mass distributions, centers of mass, inertia tensors, local axes, and materials.

## Development handoff

| Order | Pending case | Acceptance question |
| --- | --- | --- |
| 1 | C32-16 · NOT_RUN | Establish local torque, material, and load validity for the wing root and fish-tail root separately. Retain near-limit and out-of-domain controls. |
| 2 | C32-17 · NOT_RUN | Check whether revocation across synchronization points blocks new thrust in accordance with the authorization epoch and effective ordering. |
| 3 | C32-18 · NOT_RUN | If continuous physical morphing is selected, check mass-energy, inertia, momentum, and swept contact. |

The C32-14 oxygen precision and rejected-step cause remain separate investigations. Oxygen distribution, 24-DPB calibration, multiscale coupling, structural-field validity, cross-host governance, and resident perception and learning each retain their own acceptance criteria. P-02 applies to isolated research and specifications. Resident implementation and deployment follow their established authorization conditions. [Publication scope](../v2.09/PUBLICATION_SCOPE.md)
