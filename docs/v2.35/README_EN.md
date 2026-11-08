# 自成之境 v2.35 Development Baseline and Acceptance Handoff

November 8, 2026 · [Traditional Chinese](README_ZH-TW.md) · [Public status](../../CURRENT_STATUS.md) · [v2.34 acceptance criteria](../v2.34/README_EN.md)

自成之境 studies autonomous digital residents and their embodied world. Following the v2.34 sequence, local isolated tests covered one-room commits, recovery, and a simulated day. Separate tests then covered a short single collision and event deduplication on the original 65-state equations. Existing requirements govern resident identity, privacy, refusal, and memory provenance. Engineering checks measure test behavior. P-02 requires separate approval for formal resident development and deployment.

## One-room commits and observations

The analytical fixture uses one fixed-form research stand-in, a 120 tick/s clock, and single-host SQLite. One collision at tick 120 transfers impulses of −20 N·s to the stand-in and +20 N·s to the wall and its support, with 10 J of contact dissipation. The world version, receipt, and designated observation source persist in the same transaction. Observation projection keeps the source and actual write time.

| Test | Observed result | Checks |
| --- | --- | --- |
| W34-01 Single collision | One world effect, one original receipt, and one sourced synthetic observation. | 15/15 |
| W34-02 Retries and contention | Serial retries, eight competing processes, and concurrent retries and projection each produce one effect and one observation. | 48/48 |
| W34-03 Same ID with different content | Requests that change the tick, restitution, or read version are rejected. The original receipt and ledger remain retrievable. | 18/18 |
| W34-04 Interruption before commit | On reopening after termination, the uncommitted collision, receipt, and source are absent. A retry after checking the store applies one effect. | 16/16 |
| W34-05 Commit before reply loss | The caller records `IN_DOUBT`. Reopening recovers the original receipt and a retry returns the same bytes. | 12/12 |
| W34-06 Interruption before observation projection | Reopening finds the pending source. Projection writes one observation. Further reopens and projections add zero. | 16/16 |
| W34-07 Collision without a witness | The world effect and receipt exist. Observation sources and first-person memory records both total zero. | 14/14 |

Each row is `PASS_WITH_SCOPE`. Counts refer to that row's primary checks. Regression and control results are recorded separately.

## Simulated day and downtime

| Test | Observed result | Checks |
| --- | --- | --- |
| W34-08 Uninterrupted simulated day | Tick 0 through 10,368,000 represents 86,400 simulated seconds. Independent replay checks all 25 segments and 26 snapshots. | 20/20 |
| W34-09 Interruption before and after collision | Processes were terminated at ticks 60 and 120 in separate trials. Both resumed from their durable snapshots and reached the end of the simulated day. | 20/20 and 21/21 |
| W34-10 Continuous and recovered runs | All routes end at 1 m and 0 m/s with one collision, 10 J of dissipation, and one sourced observation. Each route retains its own versions, segmentation, and downtime records. | 39/39 for both archived and independently rerun inputs |

The simulated day uses an analytical contact followed by a stationary solution. Downtime wall-clock bounds, observation ticks, projection timestamps, and authoritative reconciliation times are recorded separately. Downtime records contain system facts. A deliberate change to the endpoint and observation category in a test copy caused the comparator to report both differences and exit with an error. That run is `FAIL_EXPECTED`.

## Short collision on the original 65-state model

| Test | Status and scope |
| --- | --- |
| C32-03 Single collision | `PASS_WITH_SCOPE`. Archived v2.14 equations and the v2.11 dependency were used for a six-second resting run in one S-form proxy. A committed receipt from a separate WORLD fixture triggered one jump at tick 121. Contact loss was about 0.00746667 J. The final run passed 37/37 checks. |
| C32-08 Same-event deduplication | `PASS_WITH_SCOPE`. The single, serial-retry, and four-writer contention cases each applied one jump. Each case's 722 full 65-state samples matched the archived C32-03 BDF trajectory with external damping heat byte for byte. A normal reopen recovered the original receipt. The run passed 32/32 checks. |

The first C32-03 attempt integrated the absolute world chemical-energy stock directly. It passed 24/36 checks and was recorded as `FAIL`. The follow-up used a coordinate relative to the initial stock and restored the absolute value when calling the original equations. Initial conditions, equations, and acceptance thresholds carried forward. The unmodified equations reproduced a damping-heat deficit of about 0.0003023 J after the collision, recorded as `FAIL_EXPECTED`. The separate branch that adds joint damping power to the core heat proxy had a maximum energy residual of about 3.54×10⁻⁶ J across the BDF run. The two collision paths and the failed diagnostic have separate evidence.

## Pending acceptance tests

C32-04, C32-05, and C32-06 cover 1, 24, and 72 hours after a collision, respectively. The checks address joint damping and heat, oxygen and ATP, conservation, and numerical stability. C32-09 and C32-10 cover actual process interruption before the original-model body commit and after commit but before delivery of the receipt. These five tests remain `NOT_RUN`. C32-01 and C32-02 cover the earlier resting baseline without collisions. The thermal-protection ATP, oxygen transport, and 24-DPB work retain the scoped evidence listed in v2.34. GitHub-hosted CI remains a candidate.

The suggested next test is the one-hour paired run in C32-04. Materials, organs, form changes, cross-host authority, and autonomous life have separate acceptance requirements.

This page reports public research results and their scope. Original inputs, execution logs, and rerun materials are preserved in their respective acceptance bundles. Asset publication and licensing follow their individual conditions. [Historical research](../v2.09/README_EN.md) · [Asset register](../../ASSETS.md) · [Publication scope](../v2.09/PUBLICATION_SCOPE.md)
