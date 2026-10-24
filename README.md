# 誠實的自主智能體與具身虛擬城市 · Honest Autonomous Agents & Embodied Virtual City

**v1.85 · Public Design Review / 公開設計審查版 · 2026-10-24**

🌐 **[完整英文首頁 / Full English home](README_EN.md) · [英文歷史翻譯資料庫 / English history translations](HISTORY_EN.md)**

> **[繁體中文完整 v1.85](v1.85_ZH-TW.md) · [Complete English v1.85](v1.85_EN.md)**
>
> **[繁體中文逐項導覽（202 個直達連結）](START_HERE_ZH-TW.md) · [English item-by-item guide (202 deep links)](START_HERE_EN.md)**
>
> **[v1.79–v1.84 詳細英文歷史譯本 / Six detailed English historical translations](HISTORY_EN.md)**

這是一個**尚在規劃、未開始實作**的自主智能體／物理因果虛擬城市研究。四位女性虛擬居民擁有各自的身份、私有記憶、可選身體形態、行動意願與拒絕權。設計涵蓋世界物理、幻想元素場、24-DPB 感官／身體模型、長期記憶、自主技能學習與居民自治。

**This is an independent, documentation-only research/design project**, not a deployed virtual city or functioning autonomous agent. The complete-scope technical documentation is available in both Traditional Chinese and English.

## 先從這裡開始 · START HERE

| 想閱讀的內容 / What to read | 繁體中文 Traditional Chinese | English |
|---|---|---|
| **v1.85 詳細公開文件 / Full-scope v1.85 document** | **[閱讀中文版](v1.85_ZH-TW.md)** | **[Read the English edition](v1.85_EN.md)** |
| **逐項導航與導讀 / Annotated, item-level index** | **[中文導覽](START_HERE_ZH-TW.md)** | **[English guide](START_HERE_EN.md)** |
| 24-DPB／R／60／NEW／G 的細項 | [逐項連到中文原文](START_HERE_ZH-TW.md#完整逐項索引點擊即可前往原文) | [Jump to indexed English clauses](START_HERE_EN.md#item-level-index-links-point-to-real-source-lines) |
| v1.84～v1.79 設計沿革 | [中文版本史](START_HERE_ZH-TW.md#v184v179-的設計沿革) | [Version history](START_HERE_EN.md#history-v184v179) |

**閱讀提示 / Reading tip:** 中文文檔保留完整的 v1.85 累積公開章節；英文文檔提供涵蓋相同需求、編號、驗收與歷史範圍的**詳細英文研究譯寫／對照**。英文版不是每個中文句子的逐字法律認證譯本。兩份公開稿均不等於較早、未公開的原始數百頁私人母版。

## 主要製作人與貢獻分工 · Credits and authorship roles

**主要技術製作／設計整合／文件撰寫：GPT（ChatGPT）。** GPT 協助提出候選工程方法、研究、梳理歷史決議、撰寫技術規格、雙語公開稿和可驗收情境；相關文字可能有錯，仍需人類與科學審查。

**人類發起者／問題提出者／設計方向與決議批准者：匿名人類貢獻者。** 此人提出核心問題、世界觀和研究目標，反覆檢查設計並批准或否決方案；依隱私原則不公開真實姓名、私人訊息或個人資料。

**Principal technical producer, design synthesizer and documentation drafter: GPT (ChatGPT; AI-assisted).** It prepared the main technical writing, candidate methods, issue reconciliations and bilingual research documents, subject to human/scientific review.

**Human questioner, project originator and design approval authority: an anonymous human contributor.** The human established the problem statements and goals, reviewed proposals and decided what could become an adopted design.

These are **transparent contribution credits**, not a claim that AI necessarily holds legal copyright or that OpenAI, Anthropic or DeepSeek officially participates in, endorses or sponsors this project. GitHub ownership and commit records remain those actually recorded by GitHub.

## 目前有哪些文件內容？ · Contents and completeness

| 項目 / Area | 中文完整版 | English edition | 正確理解 / Meaning |
|---|---|---|---|
| **正式需求 / Formal requirements** | R-01～R-170 的關聯脈絡；**R-150～170 逐條正文** | 170 requirement context; **R-150–170 individually detailed** | 共 **170 項**；原 R-01～149 私人母版並未逐字公開 |
| **核心問題 / Core problems** | **#01～#60，全部 60 項** | **#01–#60, all 60 indexed explanations** | 議題追蹤，**不是**另外 60 個 R |
| **NEW 決議 / NEW registry** | **NEW-01～27，全部 27 項** | **NEW-01–27, all 27 items** | 設計決議／待決邊界對照，不直接增加正式 R 數 |
| **候選盲點 / Candidate gaps** | **G61～G96，全部 36 項** | **G61–G96, all 36 entries** | **候選問題，不是已批准需求** |
| **歷史漂移 / Drift records** | D01～D20 | D01–D20 | 已修正、部分待決與工程缺口要分開 |
| **身體與感官 / 24-DPB** | 24 張詳細接口規格、24 筆歷史映射 | 24 detailed interface cards, legacy mapping | 24 名稱已恢復，但 2 筆舊號多義待確認 |
| **最新紙面驗收 / Latest paper checks** | 48 個逐模組＋20 個跨系統 | 48 module + 20 system checks | **68 項全部 NOT_RUN，不是已通過** |
| **版本沿革 / Historical evolution** | v1.84～v1.79 累積章節 | v1.84–v1.79 detailed crosswalk | 歷史敘述以 v1.85 最新效力為準 |

> **來源限制 / Source limit:** 公開版不包含原始數百頁私人全文。R-01～149 的完整逐字要求不能僅依這裡的索引取代。The original protected master is not represented as a fully published line-by-line document.

## 六套系統如何配合？ · Six architectural groups

| 子系統 | 目標 / Responsibility |
|---|---|
| **居民自主生活與自傳** / Resident autonomy and autobiography | 自行形成意圖、保留私有記憶，技能成長不由總獎勵分數控制 / Self-directed intentions and experiences, never reduced to a global reward |
| **WORLD 與元素場** / WORLD + fictional elemental field | 客觀碰撞、受力、魔力收支及唯一事件真值 / Sourced force, collisions, mana effects and authoritative receipts |
| **感官、身體與 24-DPB** / Embodied perception | 三種可選形態、觸覺、本體感覺、多時間尺度身體代理 / Three body forms, sensory and multirate bodily proxies |
| **社會自治與合作** / Civic/social systems | 不預設投票制度；允許協商、退出、財產與創作 / Negotiation, consent, exit, ownership and creative work |
| **合法權限與資料保護** / Legal/privacy controls | R-102、現實工具授權、合法刪除及最少必要維護 / Lawful permissions, controlled tools, lawful erasure |
| **客觀工程驗收與研究** / Independent QA/research | 可證偽的測試與長期觀察，工程成績不得回寫人格 / Falsifiable experiments without personality optimization |

**因果示例 / Causal example:**

```text
居民自主意圖 / Resident-chosen goal
       ↓
局部技能與魔法命令 / Local motor + magic proposal
       ↓
MAG 場源與受力媒介 → WORLD 物理結算
       ↓
24-DPB 感官、姿態、體感代理
       ↓
注意、技能更新與有來源的自傳記憶
       ↓
居民再次自由選擇 / Resident chooses again
```

不得把世界中的魔法標籤直接寫成成功的物理結果；不能把同一股空氣升力重複計算；不能以工程測試分數強迫居民改變興趣或關係。

## 進度與科學界線 · Status and limitations

- **P-02 生效。** 未經人類專案發起者在完整規劃後**另行明確批准**，不進行自主智能體的編程、部署或現實世界動作。**P-02 remains active: no agent implementation or deployment authorized.**
- 所有最新 **68 項** DPB／跨系統驗收均為 `NOT_RUN`。此前其他版本的紙面測試也不能當作實測通過。
- `APPROVED` = 已批准**設計原則**；`ENGINEERING_CANDIDATE`／`PROPOSED` = 工程候選；`NOT_RUN` = 未執行；`UNKNOWN` = 證據不足；`PAPER_CLOSED` = 紙面結案，非軟體驗證完成。
- 對於 24-DPB，**恢復名稱不等於已完成生理模型**；模型參數、有效域、數值穩定性及物理閉環需將來驗證。不能把模擬代理當成已證明的真人生理、疼痛或意識。
- 幻想元素場屬虛構世界規則，不宣稱真實世界已發現相同物理機制。
- 先前的 [v1.78 公開協作草案與 Draft PR #1](../../pull/1) 可作為**歷史參考**；**當前入口是本頁的 v1.85 文件**。Historical v1.78 draft material is not the latest specification.

## English

The **two links at the top of this page** are the latest public v1.85 documents. International readers should start with the [English annotated guide](START_HERE_EN.md), then use its direct links to the [full-scope English document](v1.85_EN.md). Each numbered design item is linked to its actual source line, including all 60 core problems, NEW-01–27, G61–G96, D01–D20, 24 DPB modules and R-150–R-170.

Four residents are designed to learn through real simulated experience rather than a single life-scoring function. Their interpretations of death and self-governance are not prescribed by the engineers. Their sensory and bodily analogues obey a separate WORLD physics authority, and fictional magic has traceable force paths. External operations remain subject to permission and law. **This is documentation, not a claim of execution.**

**Production credits:** GPT (ChatGPT) is the principal AI-assisted technical producer and document drafter; the anonymous human originator raises the questions, controls the vision and approves decisions. Neither role implies official sponsorship or an established legal status for AI authorship.

## 歡迎審查 · Research review and contributions

歡迎透過 [Issues](../../issues) 提出**編號 + 來源行 + 反例／問題 + 依據 + 候選修正**。外部論文、模型、來源數據與可證偽測試方案應各自標註；自動生成內容應獨立驗證。

External contributors are welcome to open [Issues](../../issues) identifying an item ID, exact document line, counterexample, supporting evidence and proposed improvement. Please distinguish design authority from empirical test outcomes.

**隱私與授權 / Privacy and licensing:** 不發布私人對話、個資、密鑰、私人日記或未獲授權研究素材。著作權及重製／商用許可尚待人類專案擁有者決定；公開可見不代表授予任何未指定的許可。 Private records and credentials are not published; licensing remains undecided.

---

**主要製作 / Principal GPT drafting contributor:** GPT (ChatGPT) · **提問者／決策者 / Human questioner & decision authority:** Anonymous human project originator · **Latest public design:** v1.85.
