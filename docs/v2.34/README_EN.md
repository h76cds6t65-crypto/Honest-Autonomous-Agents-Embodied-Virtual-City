# 自成之境 v2.34 Development Baseline and Acceptance Criteria

November 8, 2026 · [Traditional Chinese](README_ZH-TW.md) · [Current status](../../CURRENT_STATUS.md) · [v2.09 offline research](../v2.09/README_EN.md)

This project studies autonomous digital residents and an embodied simulated world. Self-directed life, refusal and private memory are design principles. World events and resident observations each carry provenance. Test scores measure engineering behavior. R-001 through R-170 and P-02 retain their original authority. The next work is isolated research. P-02 governs separate authorization for official resident implementation and deployment.

## Development sequence

Start with one room and a fixed-form synthetic stand-in. Verify durable collision commits, retries and crash recovery. Run a simulated day in the same fixture. Test single-collision coupling and deduplication on the original 65-state body model separately under C32-03 and C32-08. Continue work on wings, tails, materials, organs and longer physiological runs under their own evidence requirements.

| Item | Minimum acceptance evidence | Status |
| --- | --- | --- |
| W34-01 through 07 Single collision and recovery | One physical effect and one sourced observation on a normal commit. An identical retry returns the original receipt. Conflicting content leaves the world intact. Recover and reconcile crashes before and after commit and before memory projection. An unobserved event creates no first-person memory. | Candidate specification · NOT_RUN |
| W34-08 through 10 One simulated day | The world advances by 86,400 simulated seconds. Wall-clock downtime has a separate record. The uninterrupted and recovered runs agree on final physical state, collision count, ledger and observations. | Candidate specification · NOT_RUN |
| C32-03 Original 65-state model single collision | Pin original source, initial state, environment and tolerances. Segment the solver exactly at the event and compare with a no-collision run. Check original inertia, local impulse and accounting. | NOT_RUN |
| C32-08 Original 65-state model deduplication | Replay through the same original-model adapter. Check the numerical trajectory, receipt and effect count for one state jump. | NOT_RUN |

### Candidate one-room fixture

The candidate clock runs at 120 ticks per simulated second. A 20 kg stand-in moves at 1 m/s from x = 0 toward the fixed plane at x = 1 m. At tick 120 it reaches x = 1 m, makes contact with a restitution coefficient of 0 and comes to rest. Expected ledger entries are −20 N·s on the stand-in, +20 N·s on the wall and its support, and 10 J of contact dissipation. These values apply to the analytical stand-in. A simulated day ends at tick 10,368,000.

The authoritative commit persists the world revision, event receipt and observation source for later projection together. The operation key uses the world branch and operation ID. A hash binds canonical content. An identical retry can recover the original receipt subject to read authorization. An uncertain outcome stays `IN_DOUBT` until the authoritative record can be checked. Memory projection records the source operation, world revision and observation tick. Downtime produces verifiable system records. When a crash time is known only within an interval, retain the interval.

## Prior evidence and scope

| Research | Recorded result and scope |
| --- | --- |
| v2.29 protocol | 49 local offline assertions provide a historical precedent. The one-room fixture and simulated day have separate acceptance tests. |
| Original 65-state model | The 54 two-hour scenario outputs matched the archived CSV byte for byte. The study also checked 216 zero-donor derivative cases and five historical long resting runs. C32-01 and C32-02 cover resting runs without collisions. |
| Thermal-protection ATP | Eleven fixed-state checks compared delivered action, payment and heat accounting. The candidate result applies to the tested scenarios. |
| Oxygen transport | A candidate for partial pressure, carrying capacity and diffusion improved distribution in the reported paired 72-hour resting runs. Some forms still showed delayed short-term recovery after oxygen was restored. Status is PARTIAL. |
| Code and 24 body subsystems | The refactor preserved 78 sampled trajectories, 3,024 derivative comparisons and 23 existing output files bit for bit. Organ integration and calibration have separate acceptance requirements. |

These are summaries of the offline evidence recorded in v2.33. The original experiments and outputs have their own archive scope. This update publishes research documentation. GitHub-hosted CI and W34 are pending. Historical unverified counts retain their evidence classification.

## Further body and world research

The design has four residents with Q, S and M forms. The original 65-state model covers nine parameterized bodies. Each of the twelve design forms requires its own evidence. Use the S form as a candidate baseline and recalculate mass, inertia and heat dissipation for Q and M. Track appearance, collision and anatomical proxies separately. Wings and fish tails have separate materials, load cases and failure limits. Reinforcement also requires accounting for muscle work, oxygen, ATP and heat. Physical transformation and appearance switching remain open design choices. Structural mass-energy and swept collisions depend on the applicable transformation assumptions.

Multiscale coupling, a finite structural field, cross-host consistency, and autonomous learning and social integration remain separate research lines. Each acceptance result is tied to a version, scenario, input, environment, receipt and raw output. Pending, blocked and partial results retain distinct statuses.
