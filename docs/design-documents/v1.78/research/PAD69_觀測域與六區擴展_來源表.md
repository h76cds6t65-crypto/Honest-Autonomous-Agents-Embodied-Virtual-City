# v1.69 PAD 科學觀測域、數值及六種身體擴展先決條件

> **來源**：`PAD69_觀測與適用域.csv`（5 列）與 `PAD69_身體擴展次序.csv`（6 列）。數值和狀態均保留原始版本，這些數字是**論文中報告的刺激條件或資料集目錄規模，不是本專案取得原始資料後的量測結果**。目前研究暫緩。

## A｜五個不同可觀測域
| ID | Stimulus | PublishedDataset | Observable | Precondition | NextGate | CurrentStatus |
| --- | --- | --- | --- | --- | --- | --- |
| PAD-A | 正向壓入 | 論文列載荷0–3.5 N、0.5 N階梯；Flat OCT目錄 | 2D局部位移/輪廓/估計應變 | 力—幀時序對齊；載荷；原始像素解析度/座標；跨受試者留出 | A1文件—A5實驗驗證，逐關卡 | LITERATURE_CHECKED; RAW_NOT_DOWNLOADED |
| PAD-B | 切向剪切/黏滑 | 論文報滑動約0.8 mm/s、行程約7.6 mm | 局部追蹤點剪切、黏著/滑移起始 | 切向載入實際可讀性需核驗；如缺力僅比較位移 | B1—B5；承接A的校驗方法 | LITERATURE_CHECKED; RAW_NOT_DOWNLOADED |
| PAD-C | 動態局部變形 | OCT約10Hz，2D視野 | 低頻形變時序 | 高頻訊號需另一類同步資料；5Hz近邊界仍需慎重 | C1—C5；不可假造高頻真值 | DOMAIN_LIMITED; RAW_NOT_DOWNLOADED |
| PAD-D-H | 真人指腹滑動 | 真人振動/力/運動公開研究（歷史基線） | 波形、PSD、運動學 | 皮下受器真值未知，來源和欄位待複驗 | D1—D5，人體專屬域 | CATALOG_ONLY; RAW_NOT_DOWNLOADED |
| PAD-D-R | 人工探頭滑動 | Cluster 118類表面，5速、8方向、2力量 | 人工探頭加速度/力量/聲音 | 非真人皮膚，版本授權有差異 | D1—D5，人工探頭專屬域 | PUBLISHED; RAW_NOT_DOWNLOADED |

## B｜六種身體區域及中介層的先決證據
| ID | BodyRegion | ScienceLimit | AdditionalEvidence | Status |
| --- | --- | --- | --- | --- |
| X-01 | 手掌 | 延伸無毛皮膚，但厚度與受器/掌紋不同 | 皮膚厚度、荷載、位移獨立校驗 | PHYSIOLOGY_PRIOR_REQUIRED |
| X-02 | 腳底 | 承重、剪切、粗糙度與足底不同接觸條件 | 站姿荷重與局部壓力分布獨立驗證 | PLANTAR_DATA_REQUIRED |
| X-03 | 衣物隔層 | 纖維/厚度/編織/濕度中介力學與熱交換 | 雙層布-皮接觸試驗以及實測材料參數 | INTERFACE_UNCALIBRATED |
| X-04 | GPT龍尾 | 爬行動物等真實類比僅提供宏觀接觸假說 | 特殊表面等效模量/尾部關節與局部形變 | NONHUMAN_RECEPTOR_UNKNOWN |
| X-05 | GPT翼膜 | 薄膜張力/氣流/折疊形變與神經未知 | 薄膜力學及安全碰撞測試 | NONHUMAN_RECEPTOR_UNKNOWN |
| X-06 | DeepSeek魚尾 | 魚類鰭條柔性/水動力/尾柄力矩，和腿部並存 | 水流、鰭面變形及乾地觸碰 | NONHUMAN_RECEPTOR_UNKNOWN |

## C｜外部來源與權利：本次沒有直接上傳任何研究資料
- PAD-A/B/C 的原始 OCT 研究與資料庫：Corniani et al., eLife，https://doi.org/10.7554/eLife.93554；Dryad，https://doi.org/10.5061/dryad.0vt4b8hbz。本專案截至該版**尚未取得原始 OCT 影像／逐幀力資料**。
- PAD-D-H / PAD-D-R 的研究來源、採集設備與授權應依實際下載版本再核對；原表的材料、速度與方向數不能直接當作人體感覺生理真值。
- 影像、聲學波形或神經資料均未在此上傳。此處是專案自行整理的研究設計表格；授權狀態須依原始網站的實際條款另行確認。
- **不確定性**：表中的 10 Hz 是先前文獻描述的近似採樣速度。Nyquist 近邊界的可靠性需配合原始影像時間戳、頻帶與反混疊程序處理。
- **幻想附肢**：龍尾、翼膜、魚尾的等效材料力學可研究，卻沒有可直接當成真人神經受器真值的數據。

所有表格的 `RAW_NOT_DOWNLOADED`、`UNKNOWN` 和 `UNCALIBRATED` 均不得改成 `VALIDATED`。P-02 仍然有效。