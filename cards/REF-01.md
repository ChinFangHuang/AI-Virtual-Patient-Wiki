# 證據卡：REF-01

## 基本資訊
- **REF ID**：REF-01
- **文獻完整名稱**：Large Language Model–Powered AI-Assisted Simulated Patient for Nursing Education: Quasi-Experimental Study
- **作者**：Max Chun Ming Chan, Danny Chun Kit Hung, Tyrone Tai-On Kwok, Janet Yuen Ha Wong
- **年份**：2026
- **文獻類型**：期刊原著論文（Original Paper）
- **出版刊物**：*JMIR Nursing* (Vol. 9, e98543)
- **DOI / 來源 URL**：[10.2196/98543](https://doi.org/10.2196/98543) / `https://nursing.jmir.org/2026/1/e98543`
- **取得範圍**：全文（Full text, 共 13 頁 PDF）
- **虛擬病人技術類別**：大語言模型生成式虛擬病人（LLM-Powered Simulated Patient, GPT-4o）

---

## 研究設計與對象
- **研究設計**：二階段研發與準實驗研究（Two-phase developmental study with quasi-experimental evaluation）
  - **Phase 1（2024年–2025年2月）**：臨床情境腳本開發、6 款候選大語言模型適配度篩選（Exploratory model-selection assessment）、生產原型建構。
  - **Phase 2（2025年2月–2026年2月）**：V1 系統教學試行（Cohort 2025, 11 場焦點座談，收集 226 位護理生質性回饋與系統日誌）、V2 系統工程精進、開發階段劇本忠實度評估（Script-fidelity evaluation）、V2 系統教學試行與可用性量表評估（Cohort 2026）。
- **研究對象與收案設定**：
  - 香港某應用型大學（Applied University）修讀急症護理理論課程之護理系大學生（Nursing undergraduates）。
  - 納入條件：具備可運行遊戲之行動裝置、首次使用 AI 護理模擬系統。
  - 排除條件：具備急診部門實習經驗者。
- **樣本數**：
  - 模型篩選測試：50 道標準化問診題 × 6 款模型，共 300 次評估。
  - 質性反饋焦點座談：2025 學年共 226 位學生參與 11 場座談。
  - 劇本忠實度評估：瘧疾（Malaria, 16 題×5 輪=80 次）與嗜中性白血球低下發燒（Neutropenic fever, 9 題×5 輪=45 次），V1 與 V2 各 125 次，共計 250 次生成回應。
  - 學生問卷評估：總計 393 名護理學生完成問卷（2025 年梯次 n=111，完成 V1 與 V2 組內自身前後對照；2026 年梯次 n=282，進行首次使用 V2 之組間比較）。男性佔 47.3% (186/393)，具臨時大學生護士（Temporary Undergraduate Nursing Student, TUNS）經驗者佔 29.0% (115/393)。

---

## 系統技術架構與介入方式
- **軟硬體架構**：
  - 前端：Unity 遊戲引擎開發之護理檢傷模擬遊戲（AI Triage Client），支援文字輸入與語音轉文字（Speech-to-Text, STT）輸入。
  - 後端：Microsoft Azure 雲端基礎架構，透過 Microsoft AI Foundry 託管與調用 GPT-4o 模型。
  - 語言與在地化：繁體中文字元，採用在地化廣東話語法（Cantonese syntax）模擬逼真急診檢傷對話。
- **分層防幻覺架構（Layered Hallucination Mitigation Architecture, V2 精進配置）**：
  1. **接地提示詞（Case-grounded prompt content）**：納入經臨床專家及醫管局（Hospital Authority）護理專家審查之標準案例劇本。
  2. **少樣本對話範例（Few-shot conversational exemplars）**：每個情境提供 2 至 3 組示範對話，界定回答語氣、風格與臨床範圍。
  3. **負向角色與隱藏資訊約束（Explicit negative role and hidden-information constraints）**：明確限制 AI 僅能扮演病人，禁止反客為主扮演護理師或醫師；嚴禁洩露診斷（Diagnosis）、檢傷級別（Triage category）、處置指引（Management information）或隱藏中繼資料。
  4. **對話工作階段記憶管理（Session-level conversation-history handling）**：單次檢傷歷程保留歷史對話，情境結案時自動清空，避免跨階段記憶污染。
  5. **生成參數校準（Calibrated generation settings）**：溫度參數（Temperature）由 0.5 降至 0.3；最大生成長度（Max tokens）設為 4000；頻率懲罰（Frequency penalty）與存在懲罰（Presence penalty）均設為 0。
  6. **雲端安全過濾器校正（Safety-filter adjustments）**：針對非英語系臨床對話調整 Azure 內容安全過濾器閥值，排除正常問診（如「點解你嚟睇醫生？／為什麼你來看醫生？」）遭誤判阻斷的問題。

---

## 主要測量指標與結果（含原文定位）
1. **探索性模型篩選評估（Phase 1, Table 1, p.7）**：
   - 評量 50 題標準問答之完全符合劇本率（Fully script-consistent）：
     - GPT-4o：45/50 (90.0%) —— 獲選為生產環境模型。
     - GPT-4：43/50 (86.0%)
     - Llama 3.1：39/50 (78.0%)
     - GPT-3.5-turbo：32/50 (64.0%)
     - DeepSeek-V2.5：23/50 (46.0%)
     - Amazon Titan：5/50 (10.0%)
2. **劇本不一致回應率（Script-Inconsistent Response Rate / 劇本偏離幻覺, Table 3, p.8）**：
   - **總體不一致率**：V1 基準配置為 78/125 (62.4%)，V2 精進配置大幅下降至 21/125 (16.8%)，絕對減少 45.6 個百分點。
   - **瘧疾案例**：V1 為 54/80 (67.5%)，V2 降至 15/80 (18.8%)，降低 48.7 個百分點。
   - **嗜中性白血球低下發燒案例**：V1 為 24/45 (53.3%)，V2 降至 6/45 (13.3%)，降低 40.0 個百分點。
3. **錯誤型態轉變分析（Primary Categories of Failure, Table 4, p.8）**：
   - **V1 最主要失誤**：角色置換（Role switching, 17/78, 21.8%）與矛盾症狀（Contradictory symptom, 16/78, 20.5%）。
   - **V2 精進效果**：洩露隱藏資訊（Hidden-information disclosure）由 7 次降為 0 次；未支持環境細節由 6 次降為 0 次；誤解問題為索取中繼資料由 5 次降為 0 次；角色置換降至 2 次。
   - **V2 最主要殘餘失誤**：未支持症狀（Unsupported symptom, 6/21, 28.6%）與不正確時間線（Incorrect timeline, 5/21, 23.8%）。
4. **系統可用性量表（SUS, 0–100 分, p.9）**：
   - **2025 梯次組內自身前後比較（n=111）**：V1 評分為 58.31 (SD 9.54)，V2 顯著上升至 62.65 (SD 11.66)（Mann-Whitney U=7324, Z=3.39, P<.001）。
   - **首次使用組間比較（2025 V1 n=111 vs 2026 V2 n=282）**：V1 評分為 58.31 (SD 9.54)，V2 顯著上升至 65.57 (SD 12.36)（U=10,566, Z=5.57, P<.001）。
5. **淨推薦值（Net Promoter Score, NPS, p.9）**：
   - 2025 梯次為 +36.6% (n=111)；2026 梯次為 +41.1% (n=282)，顯示學生對 V2 平台的滿意度與推薦意願高度正向。

---

## 研究限制與方法學注意事項
1. **非隨機對照設計**：採用準實驗前後測與世代比較，未設置傳統真人模擬或無 AI 對照組。
2. **問卷回收率落差可能造成選擇偏誤（Selection Bias）**：2025 梯次問卷回收率僅 49.1% (111/226)，而 2026 梯次達 95.3% (282/296)。
3. **測量指標侷限於自覺主觀指標**：成效指標為系統可用性（SUS）與推薦度（NPS），缺乏客觀臨床能力（Clinical competence）、客觀結構化臨床考試（OSCE）評分或真實臨床決策遷移（Transfer to practice）之量化數據。
4. **多項介入之共變效應**：V2 同時改動了提示詞、少樣本、參數、對話記憶與遊戲 UI，無法單獨離析出各項技術修改對降低幻覺的個別獨立貢獻。
5. **語言與在地化情境特異性**：研究聚焦於香港繁體中文廣東話檢傷環境，推廣至其他語言或不同專科情境時需重新校準。

---

## 核對紀錄與查核狀態
- **核對項目 1**：劇本不一致回應率總體由 V1 的 62.4% (78/125) 降至 V2 的 16.8% (21/125)，降幅 45.6 個百分點。（核對原文：Page 1 Abstract & Page 8 Table 3，完全一致）
- **核對項目 2**：V2 殘餘失誤主要類別為未支持症狀（6/21, 28.6%）及不正確時間線（5/21, 23.8%），而隱藏資訊洩露成功降為 0 次。（核對原文：Page 8 Table 4，完全一致）
- **核對項目 3**：SUS 評分首次使用組間比較（2025 V1 n=111 vs 2026 V2 n=282），由 58.31 (SD 9.54) 顯著提高至 65.57 (SD 12.36), P<.001。（核對原文：Page 9 SUS Outcomes 段落，完全一致）
- **查核狀態**：Verified（已通過原文全數據核對）
