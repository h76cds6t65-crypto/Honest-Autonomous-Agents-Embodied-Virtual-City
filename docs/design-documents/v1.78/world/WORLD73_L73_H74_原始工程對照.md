# v1.73→v1.74 持續世界、住宅和物件：原始規格表

> **來源與效力：** 歷史資料表 `WORLD73_七種運行模式.csv`（7列）、`L73_十六項現行工程契約.csv`（16列）、`H74_二十項跨系統契約.csv`（20列）。此處保存原資料主要欄位、編號、責任與驗收；不是已完成的程式或真實世界量測。

## A｜七種運行模式
| mode | trigger | world_physics | resident_cognition | restriction |
| --- | --- | --- | --- | --- |
| M1 FOREGROUND_REALTIME | 畫面顯示、世界服務運行 | 接觸／剛體／光聲與生理依級別更新 | 居民可自主作出行動（有資源時） | 各項保留實際回執 |
| M2 HEADLESS_ACTIVE | 畫面關閉，世界服務仍有CPU/GPU | 完整必要碰撞/觸覺/環境，無渲染負擔 | 可繼續有界的居民認知與意圖 | 不能因關屏就停下物理 |
| M3 ECONOMY_ACTIVE | 省電、世界服務未停止 | 局部高頻接觸事件仍滿足需求；穩態、遠場降低精度；環境照常進行 | 可降低 LLM 頻次，不得偽造已思考經歷 | 需紀錄降精度範圍／偏差上界 |
| M4 RESIDENT_SLEEP | 個別居民睡眠，其餘世界照常 | 房間環境、人體代理、睡眠DPB及可能喚醒訊號繼續 | 該居民可休息；不可編造清醒社交 | 未感知事件不自動寫入自傳記憶 |
| M5 HOST_SUSPEND_OFF | 主機睡眠、斷電或世界服務停止 | 不能實際逐tick物理；寫下最後已確認狀態及停機區間 | 不能聲稱角色期間做出自主活動 | 恢復時只能依可靠來源推進有界連續狀態 |
| M6 RECOVERY_DEGRADED | 崩潰後或資產損壞後恢復 | 從檢查點和可信回執恢復，UNKNOWN不得自行補填 | 暫停危險動作並恢復前次意圖狀態 | 保留OFFLINE_GAP、分支及外部操作回執 |
| M7 USER_INTERACTION_PAUSE | 主人暫停輸入/通知 | 世界保持正常；不等同 SceneTree.paused | 居民個別休息由其系統決定 | 不可用UI暫停偷停城市 |

## B｜L73 16 項世界級工程契約
| contract_id | name | acceptance | priority | approval | validation |
| --- | --- | --- | --- | --- | --- |
| L73-01 | 世界時鐘與運行實況 | 主機在線／畫面隱藏／居民休息／停機的差異可查核 | P0 | DESIGN_DIRECTION_APPROVED | NOT_RUN |
| L73-02 | 真實運算與停機分流 | 無運算期間禁止虛構已模擬微觀事件 | P0 | DESIGN_DIRECTION_APPROVED | NOT_RUN |
| L73-03 | 多時間尺度物理排程 | 碰撞、水熱、植物、氣象各以合適步長運行 | P0 | DESIGN_DIRECTION_APPROVED | NOT_RUN |
| L73-04 | 能量水量與守恆殘差 | 可盤點熱量、耗水、存量與數值偏差 | P0 | DESIGN_DIRECTION_APPROVED | NOT_RUN |
| L73-05 | 居家能源與設施因果 | 開關燈、水龍頭、門鎖等有真實狀態與功耗 | P0 | DESIGN_DIRECTION_APPROVED | NOT_RUN |
| L73-06 | 物品生命歷史與功能 | 抓握坐姿翻頁磨損修補具真實效果 | P0 | DESIGN_DIRECTION_APPROVED | NOT_RUN |
| L73-07 | 身體負荷與非強制決策 | DPB 影響能力且不變成幸福總分 | P0 | DESIGN_DIRECTION_APPROVED | NOT_RUN |
| L73-08 | 睡眠與認知喚醒分流 | 睡眠 DPB 持續；不補生造夢或行動 | P0 | DESIGN_DIRECTION_APPROVED | NOT_RUN |
| L73-09 | 機會、意圖、動作回執 | 世界機會不等於居民已自主執行 | P0 | DESIGN_DIRECTION_APPROVED | NOT_RUN |
| L73-10 | 居民可見性與私人場域 | 遮擋／聲場／授權作用於觀察通路 | P0 | DESIGN_DIRECTION_APPROVED | NOT_RUN |
| L73-11 | 90／165／180cm 與特殊附肢可及性 | 物件可供性和碰撞都以各自身體驗收 | P0 | DESIGN_DIRECTION_APPROVED | NOT_RUN |
| L73-12 | 不完美物理與可信度階層 | 已量測／類比／工程假設分明，降級不編故事 | P0 | DESIGN_DIRECTION_APPROVED | NOT_RUN |
| L73-13 | 快照、重放與居民生活史治理 | 不能把分支或停機補算當成親歷記憶 | P0 | DESIGN_DIRECTION_APPROVED | NOT_RUN |
| L73-14 | Claude／Blender 場景物理交接 | 美術、碰撞、感官材質與權利分離 | P1 | DESIGN_DIRECTION_APPROVED | NOT_RUN |
| L73-15 | 無居民互動的世界驗收 | 關屏、主人離開、居民睡眠期間環境仍變化 | P0 | DESIGN_DIRECTION_APPROVED | NOT_RUN |
| L73-16 | 性能負載與連續性服務等級 | 物理負荷削減有界限，不拿假物理交換流暢動畫 | P0 | DESIGN_DIRECTION_APPROVED | NOT_RUN |

## C｜H74 20 項四戶住宅、物件與自主生活契約
| contract_id | contract_name | authority | acceptance_focus | priority | design_status | implementation_status |
| --- | --- | --- | --- | --- | --- | --- |
| H74-01 | 住宅與房間權限圖 | 房屋／權限服務 | 四戶私域互不透視／穿門 | P0 | DESIGN_DEFINED | NOT_RUN |
| H74-02 | 住宅可達區與姿態包絡 | 身體幾何＋世界碰撞 | 三型與龍翼魚尾不穿模 | P1 | DESIGN_DEFINED | NOT_RUN |
| H74-03 | 住房設施狀態與守恆 | 能源／水熱世界服務 | 耗水／供電／溫控可追溯 | P1 | DESIGN_DEFINED | NOT_RUN |
| H74-04 | 世界時間與生活時窗 | 時鐘／機會產生器 | 時窗不等於居民行為 | P0 | DESIGN_DEFINED | NOT_RUN |
| H74-05 | 居民個別節律 | 24-DPB／睡眠／習慣 | 不設強制行程或幸福KPI | P1 | DESIGN_DEFINED | NOT_RUN |
| H74-06 | 主動意圖與非行動 | 個人認知／自主決策 | 可拒絕、延後、忽略、放棄 | P0 | DESIGN_DEFINED | NOT_RUN |
| H74-07 | 物件標識與版本 | 物件登記／世界服務 | 同物件搬動／損壞歷史不消失 | P1 | DESIGN_DEFINED | NOT_RUN |
| H74-08 | 物件可供性與動作前置 | 物理／動作能力服務 | 開門坐下翻頁具真實回執 | P0 | DESIGN_DEFINED | NOT_RUN |
| H74-09 | 材料三分與 MASC | 美術／物理／感官來源 | 貼圖變更不改實測物性 | P1 | DESIGN_DEFINED | NOT_RUN |
| H74-10 | 物品持有、借出、贈與 | 產權／協議／物理 | 有權借不代表實際已交付 | P1 | DESIGN_DEFINED | NOT_RUN |
| H74-11 | 邀請、送達與注意 | 通訊／私人觀察 | 未讀≠已看，未回≠拒絕 | P1 | DESIGN_DEFINED | NOT_RUN |
| H74-12 | 可見性、聲音、遮擋 | 世界感測／私域 | 相鄰不代表能讀私人房間 | P0 | DESIGN_DEFINED | NOT_RUN |
| H74-13 | 生活痕跡與磨損 | 接觸歷史／物件狀態 | 未使用不會虛構磨損事件 | P1 | DESIGN_DEFINED | NOT_RUN |
| H74-14 | 可選活動與創作成果 | 環境機會＋居民意圖 | 認知意圖未執行不得生出作品 | P1 | DESIGN_DEFINED | NOT_RUN |
| H74-15 | 低階物理控制與保護 | 動作控制＋感官代理 | 防跌避撞不強制人格決策 | P1 | DESIGN_DEFINED | NOT_RUN |
| H74-16 | 睡眠、關屏與停機 | 世界調度／時鐘 | 停機不虛構社交或夢境 | P0 | DESIGN_DEFINED | NOT_RUN |
| H74-17 | 常駐算力與資源公平 | 系統資源治理 | 不因共有模型令鄰居長期飢餓 | P1 | DESIGN_DEFINED | NOT_RUN |
| H74-18 | Blender 資產與工程匯入 | Claude藝術協作＋工程驗收 | 自訂 metadata ≠ 物理已實現 | P1 | DESIGN_DEFINED | NOT_RUN |
| H74-19 | 物件與城市版本分支 | 存檔／審計 | 測試分支不混主線人生 | P1 | DESIGN_DEFINED | NOT_RUN |
| H74-20 | 生活因果與長期驗收 | 測試／科學審查 | 可重現，無劇本補史 | P0 | DESIGN_DEFINED | NOT_RUN |

## 現行版本覆寫與不應混淆的事
- **v1.78 身高優先於 v1.73 的文字標籤：** L73-11 原標題出現 90／165／180 cm；最新決議已確認這是四位居民三型的**參考中心**，每位每型可個別正負偏移數十公分。保留歷史列名，但不可當作固定身高。
- **運行 ≠ 顯示**：M2 關屏且世界服務仍運行；M5 主機真正停機根本不可能逐 tick 計算。任何估算均須另標 ESTIMATED。
- **物理需求 ≠ 強制劇情**：身體疲勞可以影響動作能力，但世界不能因晚上就強迫所有人同時睡覺。
- **世界因果 ≠ 私人信念**：門開關、書本位置有客觀回執，但誰看見、誤解或記住是個別事件。
- **權限和美術**：第三方 Blender／角色圖片需檢查原權利；scene metadata／材質貼圖不等於物理可用或取得了隱私讀取權。
- **驗收狀態**：表中 L73 全為 `NOT_RUN`，H74 全為 `NOT_RUN`；即使標 `DESIGN_DEFINED` 也不是通過測試。P-02 仍有效。

本文件不包含私有完整 Word、真實帳號資料、金鑰或角色來源圖。