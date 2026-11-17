# Q-form Dragon v48 Test Baseline

[繁體中文](Q_DRAGON_V48_TESTS_ZH-TW.md) · [v2.37 research baseline](README_EN.md) · [Asset register](../../ASSETS.md)

On 2026-11-17 the project owner selected `GPT_Dragon_Q_G1_v48_Dressed.blend` as the shared Q-form dragon test model. The Q reference height is 0.90 m. The model provides measurable rest geometry, rig poses, wing and tail deformation, contacts, and garment overlap. The model's SHA-256 is `e9ce3129973ee9b9070bcd2d4540383a36a1f75d943670a9abb0b7f1f2b08f03`. Use a working copy and record the source and export hashes per run.

## Evidence available

- All 417 package checksums matched. A local open attempt with Blender 4.3.2 failed with a header compatibility error. The handoff calls for Blender 5.2.3. Opening and rerendering in that version and the following acceptance runs are pending.
- The delivery records list 80 bones. Recounting the archived checks gives 22,242 garment-overlap points in the specified seated v47 pose and 134 in v48, all at the bodice lower edge. The tail still has 702 overlap points in that pose. The 120° knee-bend garment count rose from 6,200 to 6,355, a useful extreme-pose regression. These are counts for the archived mesh and sampling method.
- The garments use rig-driven pose correctives. Cloth simulation is disabled in the delivery settings. The tests track appearance, moving geometry, collision shapes, and sensory responses as distinct evidence.

## Acceptance plan

| Stage | Test | Evidence |
| --- | --- | --- |
| Open | Blender 5.2.3, dependencies, and reference renders | Record the build, dependency and driver warnings, and matched front, side, back, three-quarter, and seated renders. Inspect eyes, hair, wing membranes, ruffles, and tail root. |
| Scale and axes | Feet, origin, laterality, rig, and 0.90 m reference | Freeze the neutral pose and measuring landmarks. Record character height and accessory envelopes, wing and tail landmarks, and local axes. Verify units, transforms, and floor height after export. |
| Rig and mesh | Standing, sitting, gait, crouch, arm raises, wing folding, and tail sway | Keep keyframes and intermediate frames. Check weights, joint continuity, flips, discontinuities, and finite data. Test unilateral movement on each side. |
| Garments | Standing, half seated, 90° seated, both one-leg poses, extreme bends, and arm raise | Reproduce the 134-point check with the same sampling inputs. Report depth, location, and visible area per piece. Keep the 100° hip and 120° knee controls and test concurrent tail sway. |
| Export | Candidate GLB round trip | Compare the same sampled poses after import. Verify transforms, joints, materials, expressions, pose correctives, garment layers, and masks in the target runtime. |
| Colliders | Torso, limbs, wings, and tail tied to the same rig | Compare collision coverage against the visible model in standing, seated, wing-fold and tail-sway poses. Record false and missed coverage, continuity from root to tip, and contact layers. |
| WORLD | Floor, wall, desk edge, and thin-obstacle sweeps inside one room | Record the earliest contact, point, normal, opposing impulses, and dissipation. Test isolated wingtip or tail-tip contact, mirrored sides, and contact between separated samples. Retain the former fixed proxy as a control. |
| Load paths | Wing roots and dragon tail root | Measure contact lever arms and signed `r × F` from a specified load history. Exercise different points on the wings. Record sections and material assumptions and calibrate the dragon tail separately. |
| Mass properties | Q-form center of mass and inertia candidates | State the segment mass and density assumptions, calculate the full inertia tensor, and compare with C32-15's fixed-axis fixture. Check the response to known impulses and mirrored inputs. |
| Authority | Fixed Q form, one actuator, one known contact history | At 120 Hz WORLD and 12-tick body snapshots, test commit order, revocation, old receipts, passive contact, and restarts. Trace thrust, reaction, and dissipation to the committed event. |
| Sensing | Contact-to-24-DPB test interface | Verify side, location, timestamp, source event, and receptor receipt for left and right wings, tail root, soles, no contact, and retries. Use the existing oxygen, ATP, and heat ledgers when adding active or thermal loads. |
| Endurance | Mixed poses, multiple contacts, replay, and cost | Repeat standing, sitting, rising, wing and tail motion, and walk-stop cycles. Save misses, false contacts, step cost, memory, replay error, and interruption checkpoints. |

Begin with opening, neutral scale, and standing, seated, wing, and tail pose replay. With the fixed-form axes and collision shapes measured, connect WORLD to a receptor in one room with one actuator and a traceable contact. Define the acceptance criteria before each run. Material properties, physiological coupling, and propulsion require their own calibration evidence. S/M geometry and the physical morphing decision follow their existing research tracks.

## Model and reference images

The v48 handoff records that the head uses adapted geometry from `animeGirlBase.blend`. Redistribution and derivative permissions for that source model and the underlying source art used for the six generated reference views are pending verification. The [asset register](../../ASSETS.md) records filenames, fingerprints, and publication status.

## References

[C32-15 Fixed-form inertia and speed bounds](../v2.36/README_EN.md) · [C32-16 through C32-18 offline evidence](README_EN.md) · [Blender 5.2 glTF export manual](https://docs.blender.org/manual/en/5.2/addons/scene_gltf2.html) · [Blend file compatibility](https://developer.blender.org/docs/release_notes/compatibility/)
