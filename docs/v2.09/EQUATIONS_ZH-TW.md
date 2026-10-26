# v2.09 數學規格、守恆、回饋與 DAE（繁體中文）

[English](EQUATIONS_EN.md) · [主文件](README_ZH-TW.md)

**證據類型：離線縮減數學模型，不是已完成的 24-DPB 或校準生物模型。** 時間單位為秒；kg、mol、J、W 分開處理。本附錄記錄能從 v2.09 研究程式核對的實際方程與尚未完成的物理約束。

## 1. 權威身體與共用世界

對居民 i、形態 f∈{Q,S,M}：
\[
\dot{\mathbf x}_{i,f}=F_f(\mathbf x_{i,f},\mathbf w,\mathbf u_i,\boldsymbol\theta_{i,f}),\quad
\dot{\mathbf w}=G(\mathbf w,\{\mathbf x_j\},e_{\rm external}).
\]
身體/環境的質量或能量交換必須有相反方向的權威收支。世界儲水量不因居民換體型而縮放。24-DPB 模組只提出物理通量，不能各自更新不同版本的血氧、水量或 ATP 真值。普通 mana 與 O02 的形態結構質能分開。

v2.07 的 53 維縮減求解器包含 26 化學庫存、5 能量庫存、8 感測/控制量與 14 累積稽核計數器。v2.09 對其中 28 個內部動態座標取雅可比，發現 7 個近中性模態，五個局部零敏感度輸入是 H2O@blood、Na@ecf、K@ecf、Cl@ecf、ATP_J。**53 維≠53 種生理機制；新 9D 試驗未取代原 53D。**

## 2. 九身體＋六 WORLD 狀態

\[
\mathbf y=[B,I,N_{Na},N_K,N_{Cl},E_{\rm ATP},u_f,u_r,u_m,
W_w,N_{Na,w},N_{K,w},N_{Cl,w},E_{w,\rm chem},E_{w,\rm heat}]^\top.
\]

B,I,Ww 為 kg 水；N 為 mol；E 為 J；u 無量綱。細胞內水**在此模型是固定剖面參數**，不是動態庫存。候選：
\[
m=(6.49,40.00,51.93)\ \mathrm{kg},\ W_{\rm body}=.60m,\ 
B_0=.08W_{\rm body},\ I_0=.28W_{\rm body},\
W_{\rm ICF}=.64W_{\rm body}.
\]
\[
N_{Na,0}=.14I_0,\ N_{K,0}=.004I_0,\ N_{Cl,0}=.105I_0\ \mathrm{mol};
\quad E_{\rm ATP,0}=8000(m/40)^{.78}\ \mathrm J;\ u_0=(1,1,1).
\]
各形態獨立試驗皆採 **相同 WORLD**：1000 kg 水、Na/K/Cl 各 300 mol、世界化學能 10^10 J、環境熱 0 J。候選 60% 體水比例及質量並非各物種實測，離子濃度是研究代理而非生理校準。

## 3. 水量連續交換（直接與 WORLD 對帳）

令 \(b=B/B_\ast,\ e=I/I_\ast\)；Q/S/M 的 \(k_b=(1/400,1/650,1/790)\ \mathrm{s^{-1}}\)；基本入水率 \(q_w=(6,27,31)\times10^{-6}\ \mathrm{kg/s}\)。
\[
J_{I\rightarrow B}=B_\ast k_b(1-b)-4\times10^{-6}(u_f-1)\quad[\mathrm{kg/s}],
\]
\[
J_{\rm in}=q_w,\qquad J_{\rm urine}=q_w\max(.1,u_r)\max(.1,u_f)^{.2}\max(.1,e)^{.7}.
\]
\[
\dot B=J_{I\rightarrow B},\quad
\dot I=-J_{I\rightarrow B}+J_{\rm in}-J_{\rm urine},\quad
\dot W_w=-J_{\rm in}+J_{\rm urine}.
\]
故 \(\dot B+\dot I+\dot W_w=0\)。**這只是三庫存的守恆；不包含動態 ICF、呼吸蒸發、流汗或多居民同時競爭。** 完整汗膜需 ECF→汗膜，之後分成蒸發與滴落，鹽分要跟隨液態滴落，蒸發潛熱另計。

## 4. Na/K/Cl 配對交換

各離子 a∈{Na,K,Cl}，候選 \(c=(.14,.004,.105)\ \mathrm{mol/kg}\)、\(q_s=(1.5,6.5,7.7)\times10^{-8}\ \mathrm{mol/s}\)、濃度敏感指數 \(\beta=(.20,.65,.24)\)：
\[
J_{a,\rm in}=q_s(c_a/.14),\quad
J_{a,\rm out}=J_{a,\rm in}\max(.1,u_r)\max(.1,u_f)^{.2}
\max(.2,N_a/N_{a,\ast})^{\beta_a},
\]
\[
\dot N_a=J_{a,\rm in}-J_{a,\rm out},\quad
\dot N_{a,w}=-\dot N_a.
\]
因此每種離子 \(N_a+N_{a,w}\) 守恆。**全局淨電荷守恆不等於各隔室電中性**；反離子、膜電位、蛋白緩衝等尚未建成真正代數約束。

## 5. ATP／世界化學能／環境熱總帳

形態候選功率 \(P=(4.1,19.4,24.8)\ \mathrm W\)、能量效率 \(\eta=.4\)，活動倍數 a(t)：
\[
P_{\rm gen}=P\max(.2,u_m),\quad P_{\rm use}=Pa(t);
\]
\[
\dot E_{\rm ATP}=P_{\rm gen}-P_{\rm use},\quad
\dot E_{w,\rm chem}=-P_{\rm gen}/\eta,\quad
\dot E_{w,\rm heat}=P_{\rm gen}(1/\eta-1)+P_{\rm use}.
\]
故 \(\dot E_{\rm ATP}+\dot E_{w,\rm chem}+\dot E_{w,\rm heat}=0\)。這是**指定三帳代理能量守恆**，不是已建立真實 ATP/O2/CO2/葡萄糖計量或機械功及魔力交換；效率也不是校準參數。

## 6. 三個有限增益、有延遲的控制器

設 \(\operatorname{clip}(x,l,h)=\min(h,\max(l,x))\)：
\[
u_{f,*}=\operatorname{clip}(1+.6(1-b)+.14(1-e),.45,1.6),
\]
\[
u_{r,*}=\operatorname{clip}(1+1.0(e-1)+.25(N_{Na}/N_{Na,*}-1)
+.18(N_K/N_{K,*}-1)-.10(N_{Cl}/N_{Cl,*}-1),.2,1.5),
\]
\[
u_{m,*}=\operatorname{clip}(1+1.2(1-E_{\rm ATP}/E_{\rm ATP,*}),.4,1.7).
\]
\[
\dot u_f=(u_{f,*}-u_f)/\tau_f,\quad
\dot u_r=(u_{r,*}-u_r)/\tau_r,\quad
\dot u_m=(u_{m,*}-u_m)/\tau_m.
\]
Q/S/M 的 \(\tau_f=(45,70,85)\) s、\(\tau_r=(560,900,1150)\) s、\(\tau_m=(75,135,165)\) s。單一消融實驗把相應目標固定為 1。**有因果影響不代表補償有效**：部分短期案例關閉 flow 反而讓偏離量減小，故仍須健康有效域、恢復時間和跨器官損益驗證。

## 7. 固定點與七個近中性模態

\[
F_b(x_b^\ast;\mathbf w,\theta)=0,\qquad
J_{ij}=\left.\partial F_{b,i}/\partial x_{b,j}\right|_{x_b^\ast}.
\]
舊 53D 的 28 內部座標中有 7 個 \(|\lambda|<10^{-10}\ \mathrm{s^{-1}}\)；最大實部約 \(3.06\times10^{-16}\ \mathrm{s^{-1}}\)。不能據此宣稱漸近穩定。新 9D 模型 Q 最大實部 \(-2.423\times10^{-8}\ \mathrm{s^{-1}}\)，S \(-1.704\times10^{-8}\ \mathrm{s^{-1}}\)：意味最慢模態**數年級**，不能直接當合理生理補償。定常「身體狀態」不要求世界熱帳、尿液累計帳停止增加。

## 8. 酸鹼代數示例，不冒稱完整 DAE

令 E 為 ECF 水量：
\[
N_X=N_{Na}+N_K-N_{Cl}-N_{HCO3},\quad N_{HCO3}=.024 E.
\]
若 \(pCO2=40\ \mathrm{mmHg}\)、\(pK_a=6.10\)、\(\alpha_{CO2}=.0307\ \mathrm{mmol/(L\,mmHg)}\)，在 kg≈L 假設下：
\[
pH=6.10+\log_{10}\left[\frac{1000N_{HCO3}/E}{.0307\,pCO2}\right].
\]
三形態×三種 ECF 倍率＝9 組代數殘差為零、示例 pH 約 7.39。X 是**未追蹤陰離子代理**，不是已驗證物種。真正 DAE 須符合 \(F(t,y,\dot y)=0\)，並完整處理 NH4+、磷酸、蛋白緩衝、氧載體、腎臟排酸、局部電中性及一致初值。**本次未使用 IDA**。

## 9. Q→S 結構場質能與動量連續帳

\[
m_b(\alpha)=6.49+33.51\alpha\ {\rm kg},\
\Delta m_{\rm field}=-33.51\alpha\ {\rm kg},\
\Delta E_{\rm field}=-33.51\alpha c^2,
\quad c=299792458\ {\rm m/s}.
\]
速度設例 \(v=.30\ \mathrm{m/s}\)，則 \(\Delta p_b=+33.51\alpha v\)、\(\Delta p_{\rm field}=-33.51\alpha v\)。在共同交換點 r=(.2,.1,0) m 的角動量差為 \(\Delta L=r\times\Delta p\)，身體與場交換反號。這是**對帳範例，不是魔法場實驗證明**。

Q/S 同名 17 部件的拓撲相同，故可作候選頂點插值：
\[
\mathbf v_i(\alpha)=(1-\alpha)\mathbf v_{i,Q}+\alpha\mathbf v_{i,S}.
\]
21 個離散取樣，在天花板 1.4 m 情境 **7 個不合格**，首次 α≈.70。離散取樣不等於完整 swept collision；器官容積、血液/水鹽分配、實際變形速度、碰撞中止仍未知。

## 10. 求解、單位、失敗與效力

SciPy BDF 候選設定：rtol=2×10^-8、atol=10^-9、max_step=900s。混合 kg/mol/J 狀態未來需逐變數容許值。長時情境：0–1h 靜息、1–9h 負荷 a=1.30（精確 28,800s）、9–72h 恢復；Q/S/M 各 rest24、fluid24、feedback_off24、stress72 共 **12 組**獨立求解。測試所示水/離子/能量守恆，僅適用這個縮減模型；九形態白模、Rig、53D 完整閉環、24-DPB 和 WORLD×MAG 仍未驗證。

不得以單一生理數值取代居民人格、記憶、拒絕權及依法刪除義務。