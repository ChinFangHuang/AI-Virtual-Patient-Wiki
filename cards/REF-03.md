# 證據卡：REF-03

## 基本資訊
- **REF ID**：REF-03
- **文獻完整名稱**：Effects of generative artificial intelligence (GenAI) patient simulation on perceived clinical competency among global nursing undergraduates: a cross-over randomised controlled trial
- **作者**：Tai Chun John Fung, Siu Ling Chan, Choi Fung Mabel Lam, Chung Yan Lam, Christopher Chi Wai Cheng, Man Hin Lai, Cheuk Chun Joseph Ho, Siu Lun Au, Lok Yi Mak, Sophia Hu, Supapak Phetrasuwan, Jumpee Granger, Jung Min Yoon, Gulzar Malik, Clara Cabrera Moreno, Man Hei Patrick Kwok, Chia-Chin Lin
- **年份**：2025
- **文獻類型**：期刊原著研究論文（Original Research Article）
- **出版刊物**：*BMC Nursing* (2025) 24:934
- **DOI / 來源 URL**：[10.1186/s12912-025-03492-0](https://doi.org/10.1186/s12912-025-03492-0) / `https://link.springer.com/article/10.1186/s12912-025-03492-0`
- **取得範圍**：全文（Full text, 共 15 頁 PDF）
- **虛擬病人技術類別**：生成式人工智慧虛擬病人（專有醫學微調大語言模型，GenAI Patient Simulation）

---

## 研究設計與對象
- **研究設計**：跨國、雙臂交叉隨機對照試驗（Cross-over randomised controlled trial, RCT），設有 1 週洗除期（One-week washout period）。
- **收案地點與對象**：
  - 來自全球 6 個國家／地區（香港、台灣、泰國、西班牙、南韓、澳洲）共 6 所大學護理學院之一至三年級護理系大學生。
  - 受試者被分為 3 人一組之次群組，以 1:1 隨機分派至兩組：
    - **Group A (n=22)**：先接受 360° 虛擬實境（360° VR）影片模擬，經 1 週洗除期後，交叉接受 GenAI 生成式病人模擬。
    - **Group B (n=22)**：先接受 GenAI 生成式病人模擬，經 1 週洗除期後，交叉接受 360° VR 影片模擬。
  - 總樣本數 N=44（Group A=22, Group B=22），流失率為 0%（0% dropout rate）。
  - 受試者平均年齡 21.0 歲 (SD 1.24)，女性佔 84.1% (37/44)；大一佔 4.5%、大二佔 34.1%、大三佔 61.4%；73.6% (28/44) 具臨床實習經驗，20.5% (9/44) 具臨時大學生護士（TUNS）經驗，18.2% (8/44) 曾受過 GenAI 訓練（Table 1, p.7）。兩組基線特徵無顯著差異（P>0.05）。

---

## 系統技術架構與教學介入設計
- **技術架構**：
  - 專有醫學大語言模型（Specialized LLM）：香港大學護理學院與 0xmd Inc. (Hong Kong) 共同合作研發微調，以臨床病歷數據庫、醫學文獻與護理案例進行特定領域訓練（Domain-specific fine-tuning）[Page 5]。
  - 整合護理理論架構：
    1. **NANDA-I 護理診斷分類架構**：提供標準化診斷評分規準 [Page 5]。
    2. **Maslow 需求層次理論（Maslow’s Hierarchy of Needs）**：訓練 AI 辨識護理處置的優先順序（如生理需求必須優先於心理社會需求）[Page 6]。
    3. **3D 反思解說模型（3D Debriefing Model）**：引導模擬後的結構化討論，涵蓋情緒宣洩（Defusing）、表現發現（Discovering）與深化應用（Deepening）三階段 [Page 4, 7]。
- **臨床模擬案例（兩組使用相同案例內容）**：
  - **T1 案例**：急性肺炎（Acute Pneumonia, 25 歲男性 Peter）[Page 4–5]。
  - **T2 案例**：急性闌尾炎術後（Acute Appendicitis post-appendectomy, 38 歲男性 Ken Chan，具肝硬化徵兆與生活壓力背景）[Page 5]。
- **介入程序**：每次模擬 60 分鐘，隨後進行 60 分鐘實體面對面反思解說；GenAI 組另獲 AI 產生的個人化即時表現評分與回饋 [Page 4, 7]。

---

## 測量工具與指標
1. **臨床能力問卷（Clinical Competence Questionnaire, CCQ）**：47 題，5 點李克特量表（總分 47–235 分），包含護理專業行為（NP, 16 題）、一般表現（GP, 13 題）、核心護理技能（CNS, 12 題）與進階護理技能（ANS, 6 題）。Cronbach's α 為 0.98 [Page 3]。
2. **文化覺知量表（Cultural Awareness Scale, CAS）**：36 題，7 點量表（總分 36–252 分），涵蓋一般教育經驗（GEE）、認知覺知（CA）、研究議題（RI）、互動行為舒適度（BOCWI）與病患照護議題（PCOCI）。信度 0.91 [Page 3]。
3. **醫學生醫療人工智慧準備度量表（MAIRS-MS）**：22 題，5 點量表（總分 22–110 分），涵蓋認知（Cognition）、能力（Ability）、願景（Vision）與倫理（Ethics）。Cronbach's α 為 0.88 [Page 3]。
4. **模擬有效性工具修正版（Simulation Effectiveness Tool – Modified, SET-M）**：19 題，3 點量表，評估簡報、學習、信心與解說 [Page 4]。

---

## 主要研究結果與關鍵量化數據（含原文定位）
1. **自覺臨床能力（CCQ）組間與前後差異（Table 3, p.10）**：
   - 在第一階段介入後（T1），先接受 GenAI 的 Group B 在 CCQ 總分之提升幅度為 **47.68 分** (95% CI: 36.68, 58.68, P<.001)，顯著高於接受 360° VR 的 Group A 之 **24.95 分** (95% CI: 13.96, 35.95, P<.001)；**組間差異顯著達 16.59 分 (95% CI: 2.77, 30.41, P=0.020)**。
   - 次向度分析顯示，Group B 在「一般表現（GP）」改善幅度顯著高於 Group A（組間差 5.68 分, 95% CI: 2.72–8.64, P<.001）；在「核心護理技能（CNS）」亦顯著更優（組間差 6.36 分, 95% CI: 2.08–10.65, P=0.005）。
   - 在 T2 交叉後，兩組均維持顯著成長，最終總能力趨於相當（組間差 2.41 分, P=0.727）。
2. **醫療 AI 準備度（MAIRS-MS）顯著進展（Table 3, p.10）**：
   - Group B 接受 GenAI 後（T0 到 T1）提升 **30.18 分** (95% CI: 23.35, 37.01, P<.001)，顯著高於 Group A 在 T2 接受 GenAI 後的提升幅度 **16.64 分** (95% CI: 9.80, 23.47, P<.001)；**組間差異顯著達 12.09 分 (95% CI: 4.43, 19.75, P=0.003)**。
   - 其中「認知（Cognition）」（組間差 6.14 分, P<.001）與「能力（Ability）」（組間差 4.18 分, P=0.043）子量表具統計顯著優勢。
3. **模擬有效性（SET-M）高度肯定（Table 2, p.8）**：
   - 75.0% (33/44) 受試學生強烈同意反思解說（Debriefing）促進了其學習。
   - 68.2% (30/44) 強烈同意模擬讓自己對護理評估技能更有信心。
   - 72.7% (32/44) 強烈同意模擬增強了以實證為基礎進行照護的信心。

---

## 研究限制與方法學審查（特別注意事項）
1. **重要界線：成效指標全數為「自覺能力（Perceived Competence）」**：
   - 原文第 13 頁特別警示：「所有測量均透過自陳問卷評估學生的自覺能力，而非客觀之實際臨床表現（All measures assess perceived competence rather than actual clinical performance through self-report questionnaires）。」自評信心不必然與真實臨床技能呈正相關，**絕對不得直接等同於臨床客觀照護成效** [Page 13]。
2. **樣本數相對有限（Modest sample size, n=44）**：
   - 雖然交叉設計與零流失率維持了統計檢定力，但將樣本細拆至 6 個國家與 3 個年級時無法進行更深入的次群組統計分析，外推性受限 [Page 13]。
3. **語言潛在干擾**：
   - 全數問卷均以英文進行，雖然各參與學校均以全英語授課，但非母語學生可能在文化覺知問卷的理解上存在細微語義偏差 [Page 13]。

---

## 原文核對紀錄（至少 3 項）
- **核對項目 1**：T1 時 CCQ 總分改善，Group B (47.68) 顯著大於 Group A (24.95)，組間差異為 16.59 分 (95% CI: 2.77, 30.41, P=0.020)。（核對原文：Page 1 Abstract & Page 10 Table 3，完全一致）
- **核對項目 2**：MAIRS-MS AI 準備度改善，Group B (30.18) 顯著高於 Group A (16.64)，組間差異為 12.09 分 (95% CI: 4.43, 19.75, P=0.003)。（核對原文：Page 1 Abstract & Page 10 Table 3，完全一致）
- **核對項目 3**：SET-M 中 75.0% 學生強烈同意解說促進學習，68.2% 強烈同意提升評估技能信心。（核對原文：Page 8 Table 2，完全一致）
- **查核狀態**：Verified（已通過原文全數據核對）
