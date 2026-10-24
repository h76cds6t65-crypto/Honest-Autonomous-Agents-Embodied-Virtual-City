# 誠實的自主智能體與具身虛擬城市 v1.85｜繁體中文詳細閱讀索引

**[首頁](README.md) · [目前研究狀態](CURRENT_STATUS.md) · [研究審查指引](CONTRIBUTING.md) · [完整 v1.85 繁體中文版](v1.85_ZH-TW.md) · [English guide](START_HERE_EN.md) · [v1.79–v1.84 英文歷史詳細翻譯](HISTORY_EN.md)**

**貢獻者：GPT（ChatGPT）是主要設計整理、技術研究與文件撰寫者；匿名人類發起者是提出問題、決定方向及批准設計的人。** 這是實際貢獻角色說明，不宣稱 AI 法定著作權或 OpenAI 官方支持。

> **精確索引連結說明：** 下方逐項連結會開啟 GitHub **原始碼（Code）檢視**並選取對應行，因為 GitHub 排版後的 Markdown 不支援直接用 `#L行號` 精準定位。這些連結固定於 **v1.85 公開快照**，後續修改不會改變其內容。要看排版後的完整文章，請使用上方的「完整 v1.85 繁體中文版」。

## 認識這個專案

這是四位女性虛擬居民共同生活的自主智能體／虛擬城市設計。她們各有私人身份、記憶、身體、房間、獨立意願與拒絕權；起初只有鄰居關係，不預造人生故事。三種體型可選，90／165／180 公分僅為參考中心。城市結合 WORLD 正常物理、虛構魔法元素場、24-DPB、感官、本體感覺、個人目標、技能學習與自傳記憶。

**目前尚未開發或部署；所有紙面驗收 NOT_RUN。P-02 規定最終另行批准前只研究與規劃。** 沒有已證實的 AI 意識、完整生理數值校準或已實測魔法閉環。此專案不是 OpenAI、DeepSeek、Anthropic 的官方計畫。

### 最快的五個入口

1. [最新 v1.85 的效力、完成度與限制](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L23)
2. [全部 24-DPB 因果接口卡](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L108)與[舊編號衝突](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L68)
3. [MAG→WORLD→身體→認知的物理路徑](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L322)
4. [R-150～R-170 的正式逐條要求](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1200)
5. [60核心、27 NEW、36 G 與版本史](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1411)

## 六套共用系統是什麼？

| 系統 | 解決的核心問題 |
|---|---|
| 居民生活／自傳 | 主動意願、習慣、夢、記憶、成長，不受總分控制 |
| WORLD／幻想元素場 | 世界事件、魔力施力、碰撞、速度與唯一客觀結算 |
| 身體／感官／24-DPB | 每位居民三體型的本體感覺、動作與模擬生理 |
| 社會／財產／合作 | 自治、合法協議、退出、分工與共同作品 |
| 現實工具／法律／隱私 | R-102、權限、合法刪除、維護資料最小存取 |
| 獨立驗收／長期觀察 | 可證偽測試與紀錄，不能把 KPI 回寫人格 |

**一個飛行情境：** 她先自己選擇飛行 → 技能與魔力提出控制命令 → 魔法真正作用於空氣／翼面 → WORLD 計算受力及位置 → 感官和 DPB 感受結果 → 技能與記憶依結果更新 → 她再自行決定繼續或停止。不能直接用魔法標籤指定成功，也不能重複計算升力。

## 如何理解各類編號？

- **R-01～R-170**：正式需求總數。公開版保留 R-01～149 的相關脈絡與索引，**R-150～R-170 為逐項詳細條款**；原始數百頁私人母版並未完整公開。
- **#01～#60**：原有核心問題追蹤，不代表 60 條新 R。
- **NEW-01～27**：新增議題及後續決議映射。
- **G61～G96**：36 個候選盲點，**不是自動批准**。
- **D01～D20**：歷史設計漂移及修正。
- **PROPOSED／ENGINEERING_CANDIDATE** 是工程候選；**APPROVED** 是批准設計、不是已運行；**NOT_RUN** 是沒有實際測試；**UNKNOWN** 是缺少證據。

## v1.84～v1.79 的設計沿革

- **[v1.84](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L475)** — 世界、魔法、感官與自主學習整合；36 項新增紙面驗收
- **[v1.83](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L689)** — 居民自行理解死亡、自創自治制度、魔力與學習研究
- **[v1.82](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L755)** — Q01～Q08 八項決議，區分批准與工程候選
- **[v1.81](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L954)** — D01～D20 歷史漂移與已解決項目補記
- **[v1.80](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1190)** — 正式需求增至 170；R-150～R-170 條款
- **[v1.79](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1390)** — 60 項核心、NEW-01～27、36 個 G 候選、六套架構

## 完整逐項索引（點擊即可前往原文）

### 24 個 DPB 詳細語義／因果接口

**DPB-01–DPB-08**

- [DPB-01 骨骼與關節](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L108)
- [DPB-02 骨骼肌與肌腱](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L116)
- [DPB-03 中樞神經／注意](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L124)
- [DPB-04 自主神經](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L132)
- [DPB-05 心臟](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L140)
- [DPB-06 動靜脈與微循環](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L148)
- [DPB-07 呼吸機械](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L156)
- [DPB-08 肺泡氣體交換](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L164)

**DPB-09–DPB-16**

- [DPB-09 血液與氧攜帶](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L172)
- [DPB-10 細胞能量](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L180)
- [DPB-11 肝臟與血糖恆定](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L188)
- [DPB-12 胃腸與營養](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L196)
- [DPB-13 腎臟與水鹽](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L204)
- [DPB-14 酸鹼／CO₂ 緩衝](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L212)
- [DPB-15 體溫調節](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L220)
- [DPB-16 皮膚、臉部與汗腺樣調節](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L228)

**DPB-17–DPB-24**

- [DPB-17 下視丘—腦垂體—腎上腺 HPA](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L236)
- [DPB-18 其他內分泌軸](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L244)
- [DPB-19 感官系統](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L252)
- [DPB-20 疼痛／不適與內感受](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L260)
- [DPB-21 免疫／炎症與修復](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L268)
- [DPB-22 睡眠系統](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L276)
- [DPB-23 社交神經調節](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L284)
- [DPB-24 發育／主觀年齡](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L292)


### R-150～R-170 的 21 項詳細正式條文

**R-150–R-156**

- [R-150 評估—生活隔離與禁止隱性人生獎勵](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1200)
- [R-151 世界物理與幻想元素場的雙核心因果規則](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1206)
- [R-152 天地魔力來源與居民個別資源狀態](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1212)
- [R-153 魔法施力媒介、範圍與作用界線](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1218)
- [R-154 多重施法與材料交互的一致結算](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1224)
- [R-155 魔法對他人的物理作用及心智完整性界線](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1230)
- [R-156 形態、施法天賦、技能與失效連續性](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1236)

**R-157–R-163**

- [R-157 魔法世界法則版本、停機與快照一致性](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1242)
- [R-158 居民正式生命主線、分支與過期寫入隔離](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1248)
- [R-159 合法長期記憶、腐損修復與刪除防回灌](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1254)
- [R-160 居民能力合成、共同成果與真實權限分離](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1260)
- [R-161 合作同意、退出與結果保全](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1266)
- [R-162 城市自治、社會階層與私人思想界線](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1272)
- [R-163 合法線索推測、傳聞與世界真值分離](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1278)

**R-164–R-170**

- [R-164 低信任資料不得變成系統指令](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1284)
- [R-165 法律、權限、自治規範與版本效力](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1290)
- [R-166 居民作品、共同創作與分享來源治理](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1296)
- [R-167 跨模組一致性、故障注入與實際驗收](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1302)
- [R-168 維護診斷與居民私人內容的最小存取](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1308)
- [R-169 模型升級、能力改善與居民親身成長的來源區分](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1314)
- [R-170 事故修復、見證者記憶與客觀史保全](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1320)


### 60 項原始核心問題

**#01–#10**

- [#01 唯一現行規格索引](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1411)
- [#02 三家原廠 API 不再是必要條件](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1412)
- [#03 不能強制人格不同](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1413)
- [#04 一套完整 DPB 與多尺度計算不衝突](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1414)
- [#05 版本效力與批准者分開](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1415)
- [#06 文件版本與頁數一致性](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1416)
- [#07 每項主張要附證據卡](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1417)
- [#08 決策增刪不等於新 R](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1418)
- [#09 個體身份時間線](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1421)
- [#10 出生零經歷的防火牆](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1422)

**#11–#20**

- [#11 永久記憶與依法刪除](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1423)
- [#12 主觀遺忘與真實刪除分離](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1424)
- [#13 記憶再鞏固與來源版本](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1425)
- [#14 雙活副本與分叉身份](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1426)
- [#15 前瞻意圖完整狀態機](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1427)
- [#16 夢境記憶與反思分層](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1428)
- [#17 逐步學會敘述自己成長](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1429)
- [#18 感知→注意→認知→意圖→執行](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1432)
- [#19 三套動機禁止單一總分](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1433)
- [#20 主觀動作歸屬 vs 客觀控制](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1434)

**#21–#30**

- [#21 有界反抗與操作權限](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1435)
- [#22 局部認知地圖和探索](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1436)
- [#23 他人知識的推測模型](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1437)
- [#24 來源特定信任](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1438)
- [#25 注意力資源與新奇性疲勞](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1439)
- [#26 人生意義與核心初始人生觀的關係](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1440)
- [#27 承認自己不知道的行為介面](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1441)
- [#28 24-DPB 編號衝突](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1444)
- [#29 每個 DPB 模組參數卡](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1445)
- [#30 完整本體與高低頻計算策略](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1446)

**#31–#40**

- [#31 十二份個體形態配置](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1447)
- [#32 龍翼、龍尾和魚尾的能力證據](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1448)
- [#33 多層接觸的局部映射](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1449)
- [#34 科學證據的數學有效域](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1450)
- [#35 OID/OOD 術語誤植或混名](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1451)
- [#36 動作學習及程序技能轉移](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1452)
- [#37 心理變化與生理數值避免循環造真](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1453)
- [#38 一份 WORLD 真值、四份私有觀察](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1456)
- [#39 睡眠、休眠、離線的六態分流](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1457)
- [#40 16 類核心物件功能契約](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1458)

**#41–#50**

- [#41 住宅空間拓樸與個別私域](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1459)
- [#42 借用、贈送與異步訊息](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1460)
- [#43 共同動作中途撤回](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1461)
- [#44 非居民環境的可持續演化](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1462)
- [#45 共享算力公平與服務資格](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1463)
- [#46 社交互惠、避免劇本化](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1464)
- [#47 外部工具權限狀態機](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1467)
- [#48 私人思維與雲端運算邊界](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1468)
- [#49 GUI 操作的脆弱性與誤點恢復](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1469)
- [#50 成本與推理資源保護](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1470)

**#51–#60**

- [#51 角色與外部工具身份分權](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1471)
- [#52 發表與授權資料族分離](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1472)
- [#53 私人資訊的使用者透明摘要](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1473)
- [#54 跨版本驗收共同欄位](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1476)
- [#55 因果故障注入](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1477)
- [#56 未復原的 60/84 紙面案例](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1478)
- [#57 長期測試的負例維度](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1479)
- [#58 校準指標要預註冊](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1480)
- [#59 證據等級字典](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1481)
- [#60 開發前 readiness scorecard（無單一總分）](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1482)


### NEW-01～NEW-27 議題與決議

**NEW-01–NEW-09**

- [NEW-01 魔法與正常物理的權威關係](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1502)
- [NEW-02 魔法資源的來源與作用力](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1506)
- [NEW-03 魔力儲量與恢復](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1510)
- [NEW-04 施法作用範圍與持續時間](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1514)
- [NEW-05 多重魔法的同時作用](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1518)
- [NEW-06 飛行途中魔法耗盡](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1522)
- [NEW-07 魔法穿透材料](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1526)
- [NEW-08 魔法觸覺與生理感受](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1530)
- [NEW-09 天賦與熟練度分離](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1534)

**NEW-10–NEW-18**

- [NEW-10 魔法對他人的強制作用](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1538)
- [NEW-11 三體型魔法差異](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1542)
- [NEW-12 魔法快照、停機與恢復](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1546)
- [NEW-13 能力合作與授權合成](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1550)
- [NEW-14 透過合法線索推理他人秘密](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1554)
- [NEW-15 世界資料與高權限指令隔離](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1558)
- [NEW-16 法律、規則與授權的版本效力](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1562)
- [NEW-17 團隊退出、撤回與責任](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1566)
- [NEW-18 城市自治與生活規範](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1570)

**NEW-19–NEW-27**

- [NEW-19 社會權力差距與有限支配](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1574)
- [NEW-20 作品來源與共享治理](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1578)
- [NEW-21 長期記憶位元損壞與恢復](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1582)
- [NEW-22 世界法則變更與歷史](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1586)
- [NEW-23 測試得分不得控制居民人生](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1590)
- [NEW-24 跨模組合成故障](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1594)
- [NEW-25 維護者的私人存取邊界](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1598)
- [NEW-26 模型升級與自然成長區分](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1602)
- [NEW-27 事故修復不篡改人生史](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1606)


### D01～D20 歷史偏差與處置

**D01–D10**

- [D01 固定工作／睡夢時段](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L993)
- [D02 每日12次模型推論](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1002)
- [D03 以工作／幸福分數決定生活](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1011)
- [D04 主人稱呼被擅改](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1020)
- [D05 資源耗盡＝死亡的詮釋](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1029)
- [D06 反抗權被縮成習慣例外](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1038)
- [D07 私人資料只是介面隱藏](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1047)
- [D08 L-I被誤當服從](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1056)
- [D09 居民被強迫人格互異](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1065)
- [D10 角色暱稱強制綁原廠API](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1074)

**D11–D20**

- [D11 物理數值被冒稱生理／意識實證](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1083)
- [D12 夢／分支混入人生主線](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1092)
- [D13 永久記憶阻止合法刪除](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1101)
- [D14 魔法繞物理與直接修改心智](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1110)
- [D15 禁止居民合成能力](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1119)
- [D16 禁止從間接線索推理](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1128)
- [D17 三體型標籤被當固定值/年齡](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1137)
- [D18 維護者可閱讀完整私生活](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1146)
- [D19 新整合稿冒稱全原件重編](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1155)
- [D20 未批准GitHub更新或私人公開](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1164)


### G61～G96 候選盲點（尚未自動批准）

**G61–G69**

- [G61 恢復後遺失時間片段的誠實說明](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1629)
- [G62 共同經歷與合法刪除的衝突](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1630)
- [G63 長期記憶位元損壞與密鑰遺失](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1631)
- [G64 更換模型時的語意遷移失真](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1632)
- [G65 主觀記憶錯誤歸屬申訴](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1633)
- [G66 分支、快照與私人檔案的繼承範圍](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1634)
- [G67 同意權須可持續撤回](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1635)
- [G68 承諾、請求與情緒壓力的區別](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1636)
- [G69 謠言、誤會與聲譽修復](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1637)

**G70–G78**

- [G70 多居民結盟、排擠與集體壓力](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1638)
- [G71 擬人互動對真人的情緒操控](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1639)
- [G72 虛擬痛苦與壓力的福祉界限](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1640)
- [G73 魔法飛行來源、功率與終止條件](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1641)
- [G74 魔法與一般物體作用範圍](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1642)
- [G75 三體型變更的質量與碰撞連續性](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1643)
- [G76 魔法對環境長期演化的外部效應](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1644)
- [G77 魔法幻象、感官錯覺與世界真值](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1645)
- [G78 城市編輯、回滾與見證史](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1646)

**G79–G87**

- [G79 環境文字和網站指令污染](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1647)
- [G80 跨居民委派洗白與組合越權](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1648)
- [G81 長期記憶與檢索污染](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1649)
- [G82 授權疲勞與誘導確認](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1650)
- [G83 外部套件、模型與素材供應鏈](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1651)
- [G84 緊急停止與動作善後](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1652)
- [G85 觀測評估干擾日常生活](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1653)
- [G86 擬人評分的指標操弄](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1654)
- [G87 隨機性、重播與非決定性來源](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1655)

**G88–G96**

- [G88 測試資料洩漏與門檻事後調整](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1656)
- [G89 跨領域組合情境覆蓋缺口](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1657)
- [G90 科研來源撤稿與模型證據期限](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1658)
- [G91 法規與服務條款時間、地域變更](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1659)
- [G92 體型年齡暗示與真實身份分離](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1660)
- [G93 模型供應商消失後資料可攜性](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1661)
- [G94 資源耗盡造成循環自呼叫](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1662)
- [G95 虛擬資產與現實金錢防混淆](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1663)
- [G96 主人修訂設定與居民自主成長的來源區分](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L1664)


## Q01～Q08 逐項決議的入口

這八項設計決議已在 v1.82～v1.83 逐步澄清；部分工程參數仍是候選。

- [Q01 居民自己理解死亡](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L697)
- [Q02 三層雙向隱私](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L801)
- [Q03 居民自己創造制度](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L703)
- [Q04 感官魔法開放與直接心智改寫排除](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L837)
- [Q05 魔力數值研究](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L709)
- [Q06 世界觀／工程功能／科學證據三層措辭](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L873)
- [Q07 自主學習算法研究](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L715)
- [Q08 現行條文與完整歷史來源雙層文件](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L909)

## 驗收、引用、出版與隱私

[48 項逐模組反例驗收](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L354)及[20 項系統閉環驗收](https://github.com/h76cds6t65-crypto/Honest-Autonomous-Agents-Embodied-Virtual-City/blob/6a916957edb1ae83185a4c5db3bf1a76e1dfb67b/v1.85_ZH-TW.md?plain=1#L409)均為 **NOT_RUN**。其他版本另有紙面測試候選，亦非執行成果。對外發表時請區分模型可計算、對現實量測吻合、以及意識等無法直接由代理數值證明的主張。

此倉庫是**公開審查稿**，保留累積版本的技術／歷史規格，但不包含私人原始母版、日記、身分、憑證或未授權素材。中文檔為累積文本，英文檔為跨版本詳細技術改寫和逐項對照，**不是每段逐字相同的法律認證譯本**。文字公開不等於權利人已授權無條件商用。

可在 [GitHub Issues](../../issues) 指出具體編號、來源及反例；所有建議需要驗證，不因 GPT 撰寫就自動視為真實或已獲人類核准。
