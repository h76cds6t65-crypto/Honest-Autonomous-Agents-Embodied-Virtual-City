# v2.09 Detailed Equations, Conservation, Feedback and DAE (English)

[繁體中文](EQUATIONS_ZH-TW.md) · [Active specification](README_EN.md)

**Evidence: offline reduced mathematical experiments, not completed 24-DPB or calibrated biology.** Time is measured in seconds; kg, mol, J and W carry distinct dimensions. These equations reflect the actual specified pilot and its known missing physical constraints.

## 1. Authoritative body and shared WORLD

For resident i and form f∈{Q,S,M}:
\[
\dot{\mathbf x}_{i,f}=F_f(\mathbf x_{i,f},\mathbf w,\mathbf u_i,\theta_{i,f}),\quad
\dot{\mathbf w}=G(\mathbf w,\{\mathbf x_j\},e_{\rm external}).
\]
Any material/energy transfer between a body and WORLD requires an equal, opposite ledger entry. World resource inventories do not scale with body size. The 24-DPB modules propose directed fluxes rather than rewriting separate versions of the same inventory. Ordinary mana and the O02 morphology structural-energy reservoir are different accounts.

The inherited reduced 53-dimensional solver has 26 chemical inventories, five energy inventories, eight sensor/controller states and 14 cumulative audit counters. In a 28-coordinate internal Jacobian, seven modes are near-neutral; five zero-sensitivity input coordinates are H2O@blood, Na@ecf, K@ecf, Cl@ecf, ATP_J. **53 dimensions are not 53 physiological mechanisms; a new 9D pilot has not repaired the inherited 53D.**

## 2. Nine body and six WORLD states

\[
\mathbf y=[B,I,N_{Na},N_K,N_{Cl},E_{\rm ATP},u_f,u_r,u_m,
W_w,N_{Na,w},N_{K,w},N_{Cl,w},E_{w,\rm chem},E_{w,\rm heat}]^\top.
\]
B, I, Ww are kg of water; N are mol; E are J; u are dimensionless. Intracellular water is a **fixed profile** in this nine-body-state experiment, not a dynamic stock.

Candidate initialization:
\[
m=(6.49,40.00,51.93)\ {\rm kg},\ W_{\rm body}=.60m,\quad
B_0=.08W_{\rm body},\ I_0=.28W_{\rm body},\ W_{\rm ICF}=.64W_{\rm body}.
\]
\[
(N_{Na},N_K,N_{Cl})_0=(.14,.004,.105)I_0\quad {\rm mol};\quad
E_{\rm ATP,0}=8000(m/40)^{.78}\ \mathrm J,\quad u_0=(1,1,1).
\]
All independent Q/S/M trials use identical WORLD stocks: water 1000 kg, Na/K/Cl 300 mol each, world chemical energy 10^10 J, heat 0 J. These mass and ion partitions are research surrogates, not measured species-specific physiology or fully electrically neutral plasma.

## 3. Water flow and equal/opposite WORLD ledger

Let b=B/B*, e=I/I*, and use k_b=(1/400,1/650,1/790) s^-1 plus baseline q_w=(6,27,31)×10^-6 kg/s for Q/S/M.
\[
J_{I\to B}=B_*k_b(1-b)-4\times10^{-6}(u_f-1)\quad [\mathrm{kg/s}],
\]
\[
J_{\rm in}=q_w,\quad J_{\rm urine}=q_w\max(.1,u_r)\max(.1,u_f)^{.2}\max(.1,e)^{.7}.
\]
\[
\dot B=J_{I\to B},\quad \dot I=-J_{I\to B}+J_{\rm in}-J_{\rm urine},\quad
\dot W_w=-J_{\rm in}+J_{\rm urine}.
\]
Then \(\dot B+\dot I+\dot W_w=0\). This certifies conservation only for the **defined three-stock water pilot**; dynamic ICF, sweat, breathing, food intake and concurrent residents are absent. A full sweat-film system needs ECF→film generation, separate evaporation and dripping, transported salts and evaporation latent heat.

## 4. Paired Na/K/Cl transfer

For ion a∈{Na,K,Cl}, candidate c=(.14,.004,.105) mol/kg, q_s=(1.5,6.5,7.7)×10^-8 mol/s and sensitivity β=(.20,.65,.24):
\[
J_{a,\rm in}=q_s(c_a/.14),\quad
J_{a,\rm out}=J_{a,\rm in}\max(.1,u_r)\max(.1,u_f)^{.2}
\max(.2,N_a/N_{a,*})^{\beta_a},
\]
\[
\dot N_a=J_{a,\rm in}-J_{a,\rm out},\quad
\dot N_{a,w}=-\dot N_a.
\]
Hence each ion's body+world total is conserved. **Global ionic/charge conservation is not local electroneutrality.** Counterions, membrane potentials and buffering remain unimplemented constraints.

## 5. ATP–WORLD chemical energy–environment heat ledger

Candidate baseline powers P=(4.1,19.4,24.8) W for Q/S/M, surrogate yield η=.4, activity multiplier a(t):
\[
P_{\rm gen}=P\max(.2,u_m),\quad P_{\rm use}=Pa(t);
\]
\[
\dot E_{\rm ATP}=P_{\rm gen}-P_{\rm use},\quad
\dot E_{w,\rm chem}=-P_{\rm gen}/\eta,\quad
\dot E_{w,\rm heat}=P_{\rm gen}(1/\eta-1)+P_{\rm use}.
\]
Thus all three derivatives sum to zero. This is a **three-account energy identity**, not oxygen/glucose/CO2/ATP stoichiometry, mechanical work, calibrated physiology or a magic-energy model. The efficiency η is assumed, not measured.

## 6. Delayed bounded flow, renal and metabolic controls

Define clip(x,l,h)=min(h,max(l,x)):
\[
u_{f,*}=\operatorname{clip}(1+.6(1-b)+.14(1-e),.45,1.6),
\]
\[
u_{r,*}=\operatorname{clip}(1+1.0(e-1)+.25(N_{Na}/N_{Na,*}-1)
+.18(N_K/N_{K,*}-1)-.10(N_{Cl}/N_{Cl,*}-1),.2,1.5),
\]
\[
u_{m,*}=\operatorname{clip}(1+1.2(1-E_{\rm ATP}/E_{\rm ATP,*}),.4,1.7);
\]
\[
\dot u_f=(u_{f,*}-u_f)/\tau_f,\quad
\dot u_r=(u_{r,*}-u_r)/\tau_r,\quad
\dot u_m=(u_{m,*}-u_m)/\tau_m.
\]
Time constants Q/S/M: flow (45,70,85) s, renal (560,900,1150) s, metabolic (75,135,165) s. Ablation pins an actuator target to 1. **Causal influence is not the same as beneficial feedback**; some disabled-flow tests improve a limited six-hour normalized deviation metric.

## 7. Resting equilibrium and seven neutral modes

\[
F_b(x_b^*;w,\theta)=0,\qquad
J_{ij}=\left.\frac{\partial F_{b,i}}{\partial x_{b,j}}\right|_{x_b^*}.
\]
The inherited 53D/28-internal-coordinate analysis finds seven modes with |λ|<10^-10 s^-1 and largest real part ≈3.06×10^-16 s^-1. This **does not prove** asymptotic stability. The separate nine-state pilot's maximum real parts are Q ≈-2.423×10^-8 s^-1 and S ≈-1.704×10^-8 s^-1; corresponding slow modes take **years**, not necessarily useful daily-life compensation. External/world audit totals can change while body stocks are at a steady state.

## 8. Algebraic pH example is not a solved physiological DAE

For candidate ECF water E:
\[
N_X=N_{Na}+N_K-N_{Cl}-N_{HCO3},\quad N_{HCO3}=.024E.
\]
Assume pCO2=40 mmHg, pKa=6.10, CO2 solubility .0307 mmol/(L mmHg), and kg≈L:
\[
pH=6.10+\log_{10}\left[\frac{1000N_{HCO3}/E}{.0307pCO2}\right].
\]
Across three forms and three ECF multipliers, nine algebraic residuals were zero, with illustrative pH ≈7.39. The untracked anion X is a **charge-balance proxy**. Actual DAE \(\ F(t,y,\dot y)=0\ \) requires ammonium, phosphate, protein buffers, oxygen-carrier equilibria, renal acid handling, local electrical neutrality and consistent initial conditions. **SUNDIALS IDA was not run.**

## 9. Q→S structural mass-energy, momentum and sampled collision

\[
m_b(\alpha)=6.49+33.51\alpha\ \mathrm{kg},\
\Delta m_{\rm field}=-33.51\alpha\ \mathrm{kg},\
\Delta E_{\rm field}=-33.51\alpha c^2,\quad c=299792458\ \mathrm{m/s}.
\]
For assumed exchange speed v=.30 m/s, \(\Delta p_b=+33.51\alpha v\), \(\Delta p_{\rm field}=-33.51\alpha v\); angular changes at r=(.2,.1,0) m are ΔL=r×Δp and must cancel in the external ledger. This is a **bookkeeping illustration**, not a physically validated magic field.

With corresponding mesh connectivity:
\[
\mathbf v_i(\alpha)=(1-\alpha)\mathbf v_{i,Q}+\alpha\mathbf v_{i,S}.
\]
21 discrete Q→S samples include **seven** heights exceeding a 1.4 m ceiling, first α≈.70. This is not certified continuous swept collision. Organ positions, blood/fluid transfer, shape-change rate and safe abort conditions are still unresolved.

## 10. Numerical protocol, dimensions, failures and authority

SciPy BDF candidate tolerances: rtol=2×10^-8, atol=10^-9, max_step=900 s; mixed kg/mol/J variables ultimately need per-variable absolute tolerances. Stress protocol: 0–1h rest, 1–9h activity multiplier 1.30 (**28,800 seconds exactly**), 9–72h recovery. Three forms each have rest24, fluid24, feedback_off24 and stress72, yielding **12 independently integrated experiments**. The reduced model's global water/ion/energy checks do not establish validated 53D, fully calibrated 24-DPB, working rigs or WORLD×MAG integration.

No physiology score may override resident identity, personal memory, refusal rights or lawful data controls.