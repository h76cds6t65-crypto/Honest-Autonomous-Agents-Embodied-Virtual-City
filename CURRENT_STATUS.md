# 現行設計狀態 / Current Design Status

> **最新公開研究規格 / Latest public research specification [v2.34 繁體中文](docs/v2.34/README_ZH-TW.md) · [v2.34 English](docs/v2.34/README_EN.md)** (2026-11-08)
>
> v2.34 先驗收一房間碰撞的提交、重送與恢復，再驗一個模擬日。W34-01 單次碰撞已通過本機限定範圍驗收。其餘 W34 及原版 65D 的 C32-03、08 仍待跑。 / v2.34 starts with one-room collision commits, retries and recovery, followed by a simulated day. W34-01 passed with local scope. The remaining W34 tests and C32-03/C32-08 are NOT_RUN.
>
> **歷史離線研究 / Earlier offline research: [v2.09 繁體中文](docs/v2.09/README_ZH-TW.md) · [v2.09 English](docs/v2.09/README_EN.md)** (2026-10-27) — [中文公式](docs/v2.09/EQUATIONS_ZH-TW.md) / [English equations](docs/v2.09/EQUATIONS_EN.md) · [中文驗收](docs/v2.09/VALIDATION_ZH-TW.md) / [English validation](docs/v2.09/VALIDATION_EN.md) · [歷史技術沿革](docs/v2.09/HISTORY_ZH-TW.md) / [English history](docs/v2.09/HISTORY_EN.md).
>
> v2.09 documents scoped **offline** math/geometry findings and explicit failures. The earlier v1.85 materials below remain a historical public design baseline, not the latest experimental state. Private Word/ZIP files, personal information and unlicensed artwork are not distributed. P-02 remains active.


**誠實的自主智能體與具身虛擬城市 / Honest Autonomous Agents & Embodied Virtual City**  
**v2.34 development specification · 2026-11-08 · P-02 isolated research**

[首頁 Home](README.md) · [English home](README_EN.md) · [中文 v1.85](v1.85_ZH-TW.md) · [English v1.85](v1.85_EN.md) · [English history](HISTORY_EN.md)

## v2.34 目前開發狀態 / Current development status

| 研究 / Research | 狀態 / Status |
| --- | --- |
| 一房間單次碰撞 / One-room single collision | W34-01 · PASS_WITH_SCOPE（本機 15/15 / 15 of 15 local checks） |
| 重送與故障恢復 / Replay and fault recovery | W34-02–07 · NOT_RUN |
| 一個模擬日及停機留痕 / One simulated day and downtime records | W34-08–10 · NOT_RUN |
| 原版 65D 單次碰撞與去重 / Original 65-state collision and deduplication | C32-03 and C32-08 · NOT_RUN |
| 原版無碰撞、ATP、氧與 24 DPB / No-collision baseline, ATP, oxygen and 24-DPB work | 離線證據，按各自場景與範圍 / Scoped offline evidence |

**W34-01 本機驗收**　2026 年 11 月 8 日，在單機 SQLite 固定替身情境，第 120 tick 留下一次持久碰撞與一筆有來源的合成觀察。替身衝量為 −20 N·s，牆與支座為 +20 N·s，接觸耗散為 10 J。正常重開後可查回原回執與觀察來源。

**W34-01 local acceptance**　On November 8, 2026, the fixed stand-in in a single-host SQLite fixture recorded one durable collision at tick 120 and one sourced synthetic observation. The stand-in impulse was −20 N·s, the wall and support impulse was +20 N·s, and contact dissipation was 10 J. A normal reopen recovered the original receipt and observation provenance.

[v2.34 開發順序與驗收](docs/v2.34/README_ZH-TW.md) · [v2.34 Development sequence and acceptance](docs/v2.34/README_EN.md)

## 1. v1.85 歷史設計範圍 / Historical v1.85 design scope

| 項目 / Area | 文件涵蓋 / Documented | 執行狀態 / Status |
|---|---|---|
| 正式需求 / Formal requirements | **R-01–R-170 = 170** | Approval is not implementation |
| R-01～149 | Referenced via history and issues; original private master **not public** | `SOURCE_COVERAGE_PARTIAL` |
| 核心問題 / Core problems | **60** entries (#01–#60) | Paper review, not new R |
| NEW 決議 / NEW decisions | **27** entries (NEW-01–27) | Some parameters pending |
| 候選盲點 / Candidate gaps | **36** (G61–G96) | `CANDIDATE`, not formal R |
| 歷史偏差 / Drift reconciliation | **20** (D01–D20) | Paper resolution, not tested code |
| 身體代理 / 24-DPB | 24 semantic/causal cards, recovered historical names | Some aliases ambiguous; no empirical calibration |
| v1.85 逐模組驗收 / Module checks | **48** proposed tests | **ALL NOT_RUN** |
| v1.85 跨系統驗收 / System checks | **20** proposed tests | **ALL NOT_RUN** |
| 較早測試 / Older historical checks | v1.84: 36; v1.83: 15; v1.82: 32; 144 previously located paper cases | **NOT_RUN**; do not sum as passes |
| 虛擬居民程式 / Working agents | No completed operational agent, WORLD/DPB simulator or scientific validation | `NOT_IMPLEMENTED` |

**重要 / Important:** Chinese v1.85 retains public cumulative chapters. English v1.85 and [six English historical translations](HISTORY_EN.md) provide substantial detail, **not an externally certified word-for-word equivalent**. The original hundreds-page private mother document and the full R-01–149 original clauses are not publicly reproduced.

## 2. 標籤定義 / Status glossary

| 標籤 | 中文 | English |
|---|---|---|
| `OWNER_APPROVED` / `APPROVED` | 人類已批准設計；**不等於已實作** | Design adopted, not implemented |
| `SPEC_READY` / `PAPER_CLOSED` | 紙面條文或歷史問題結案；**不是測試通過** | Paper/specification disposition, not a passed test |
| `ENGINEERING_CANDIDATE` / `PROPOSED` | 可再審查的算法、參數、方案 | Candidate, not a committed implementation |
| `NOT_RUN` | 測試未執行 | Acceptance test has not run |
| `NOT_IMPLEMENTED` | 功能尚未建成 | Function not implemented |
| `UNKNOWN` / `NOT_CALIBRATED` | 無充分數據或校準 | Evidence or calibration unavailable |
| `SUPERSEDED` | 後來批准的新決議取代舊說法，歷史仍保留 | Superseded, retained as historical evidence |

**測試編號注意 / Test ID namespace:** v1.85 的跨模組測試使用 `S01–S20`；但歷史 v1.84 的三層學習測試也使用 `S01–S06`。引用時必須寫 **`v1.85/S01`** 或 **`v1.84/S01`** 並附來源版本，**不能把同名編號當同一測試，也不能多算通過數**。 / Historical versions reuse some S-numbers; always qualify test IDs by version.

**歷史差異 / Historical example:** v1.82 still debated subjective death meaning, but v1.83 lets residents define it themselves. v1.84 lacked the complete 24-module name map, while v1.85 recovered candidate names; neither development means a physiological simulation has been tested.

## 3. 不可破壞的既有原則 / Existing boundaries

- **P-02:** 完整規劃後，**另行取得人類發起者明確批准**才可開發／部署自主智能體。文件整理不是批准開發。 / Separate final human authorization is necessary before agent coding/deployment.
- **自主生活 / No global life reward:** 禁止幸福、服從、主人滿意或局部 KPI 的隱性總分控制人格、意願、L-I 或人生史。局部技能測量不等於居民必須練習。
- **因果與真值 / Causality:** 幻想元素場 → WORLD 受力／光聲 → 24-DPB 感官 → 私人認知與記憶；不能用動畫指定成功或直接改寫思想。
- **隱私與法律 / Privacy and law:** 真實工具權限和居民私域獨立，合法刪除不得從備份回灌；這是**待實作架構**，不宣稱已能保證絕對技術隱私。
- **科學證據 / Evidence:** 24-DPB 代理與虛構魔法不構成人類生理、主觀意識或新現實物理定律的實證。

## 4. 原 v1.86 候選審查事項 / Historical v1.86 review candidates

**以下不是新 R，也不是授權實作 / These are proposed review priorities, not requirements or coding approval.**

1. **24-DPB semantic closure:** input/output, units, delays, validity domains, and two mixed historical aliases.
2. **MAG→WORLD→DPB→cognition:** single-accounted force, reachable senses, clock ordering, private experience provenance and negative controls.
3. **Q07 autonomous learning:** freely chosen goals, local motor updates, autobiography, and a firewall against QA scores modifying life choices.
4. **Q05 mana parameters:** define quantities/units/supply/absorption/storage/output from mechanics, without inventing pre-approved constants.
5. **Long-term history and resilience:** legitimate main writer, checkpoint recovery, lawful erasure non-resurrection, and model-upgrade attribution.
6. **Honest verification:** preserve distinct `NOT_RUN`, `UNKNOWN`, `FAILED` until real tests are authorized and performed.

## 5. 貢獻與署名 / Review and attribution

[中文導覽](START_HERE_ZH-TW.md) · [English guide](START_HERE_EN.md) · [Contribution guidance](CONTRIBUTING.md) · [GitHub Issues](../../issues)

**Credits:** GPT（ChatGPT）是主要技術設計整合、文件與譯寫協助者；匿名人類發起者提出問題、確立方向及批准決議。這不是 AI 法定著作權的認定，也不代表 OpenAI、DeepSeek 或 Anthropic 官方參與。

**License / 授權：** 現階段未制定全面重製與商業使用許可，公開閱讀不代表取得未聲明的許可。
