# 證據卡：REF-06

## 基本資訊
- **REF ID**：REF-06（原訂 REF-05 改編號）
- **文獻完整名稱**：Large Language Model-Based Virtual Patient Simulations in Medical and Nursing Education: A Review
- **作者**：Young-Woo Jo, Myungeun Lee, Hyung-Jeong Yang
- **年份**：2025
- **文獻類型**：期刊綜述論文（Integrative / Scoping Review）
- **出版刊物**：*Applied Sciences* (2025, Vol. 15, 11917)
- **DOI / 來源 URL**：[10.3390/app152211917](https://doi.org/10.3390/app152211917) / `https://doi.org/10.3390/app152211917`
- **取得範圍**：全文（Full text, 共 24 頁 PDF）
- **虛擬病人技術類別**：大語言模型虛擬病人（LLM-Based Virtual Patient Simulations, 涵蓋單智慧體、多智慧體、知識圖譜與閉環自適應系統）

---

## 研究設計與納入範疇
- **研究設計**：遵循 PRISMA 流程架構執行之大語言模型醫護虛擬病人系統性文獻綜述。
- **文獻檢索與篩選**：
  - 檢索 Google Scholar, PubMed, Web of Science, Scopus 四大資料庫（2023 年 1 月至 2025 年 6 月）。
  - 初篩 378 篇，全文章節檢核 72 篇，最終納入 **40 篇發表於 2023–2025 年之同儕審查研究與會議論文** [Page 3–4, Fig 1]。
- **涵蓋領域**：醫學（Medicine）、護理（Nursing）與跨專業健康照護教育。

---

## 核心技術實作與分類架構（Six Implementation Categories, p.4–5, Fig 2）
本綜述將 LLM 虛擬病人系統歸納為**六大實作範式**：
1. **LLM 臨床劇本自動生成（Scenario Generation, 8 篇, 20%）**：利用多階段反饋或 Agentic 工作流快速產製多樣化教案（如 Barra et al. 整合多模型將開發時間縮短 70–80% 至 4.5 分鐘）[Page 5–6, Table 1]。
2. **簡易提示詞驅動系統（Simple Prompt-Based VP, 9 篇, 22%）**：僅憑基礎角色指令與案例描述驅動，建置成本低但容易產生腳本外幻覺（高達 56.4%）與角色漂移 [Page 6–7, Table 2]。
3. **迭代回饋與自動評分系統（Iterative Feedback & Automated Scoring, 8 篇, 20%）**：結合量規（如 MIRS, SPIKES, 3E）進行即時文字反思與評分，評分一致性達 Cohen's κ ≈ 0.83，但存在過度寬鬆正面（Overly positive）之評估偏誤 [Page 7–9, Table 3]。
4. **擬真度與動態自適應系統（Realism- and Adaptability-Enhanced Systems, 6 篇, 15%）**：
   - 結合多模態化身、語音與社交機器人（Borg et al. 證實機器人擬真度顯著優於電腦 P=.04）[Page 10, Table 4]。
   - **Adaptive-VP 閉環架構（Lee et al., 2025）**：首創評估、自適應調整、對話生成與安全監控四模組閉環，根據學生表現動態調整病患不滿度與態度，角色忠實度顯著提升（P=.043）[Page 10–11]。
5. **知識驅動與多智慧體混合系統（Knowledge-Driven & Multi-Agent Hybrids, 4 篇, 10%）**：
   - 劃分知識層（KG/EHR）、編排層（多 Agent 驗證）與生成層。
   - **EvoPatient（Du et al., 2024）**：病患 Agent 與多科醫師 Agent 透過有向無環圖（DAG）雙向協同演化 [Page 11–12]。
   - **CureFun（Li et al., 2024）**：透過 ERRG 流程將新資訊「持續寫回案例圖譜（Continuous write-back）」，徹底維持長對話情境一致性 [Page 12–13]。
   - **AIPatient（Yu et al., 2024）**：結合 6 個專業 Agent 與 Reasoning-RAG，問答準確率達 94.15% [Page 12–13]。
6. **心理健康與諮商專業系統（Mental Health- and Counseling-Oriented Systems, 5 篇, 13%）**：
   - 注入認知行為治療（CBT）與動機式晤談（MI）理論模型，模擬抗拒、矛盾與情緒波動（如 Patient-Ψ, SimPatient, PSYCHE）[Page 13–15, Table 6]。

---

## 評估方法學與可量化指標（Evaluation Metrics, p.17–18）
針對過往醫療 LLM 評估過度依賴主觀或缺乏重測信度的缺陷，本綜述建立了**客觀可重現的數學評估指標**：
1. **臨床表徵識別準確率（Recognition Accuracy, RA）**：$RA = \frac{1}{N}\sum_{i=1}^{N} C_i$（$C_i$ 代表是否正確識別關鍵臨床線索或生命徵象）[Equation 1]。
2. **指令與約束遵循率（Instruction-following Effective Rate, ER）**：$ER = \frac{1}{N}\sum_{i=1}^{N} F_i$（$F_i$ 代表是否遵循劇本與負向角色約束）[Equation 2]。
3. **綜合加權準確率（Aggregated Accuracy, AA）**：$AA = \frac{\sum_{i=1}^{N} w_i A'_i RA_i ER_i}{\sum_{i=1}^{N} w_i}$（整合各題難度權重 $w_i$ 與專家核可推理準確率 $A'_i$）[Equation 3]。
4. **LLM-as-a-Judge（模型自評裁判）偏差警訊**：指出以 GPT-4 擔任裁判時雖與人類評分相關性 >80%，但存在**位置偏差（Position bias）、冗長偏差（Verbosity bias）與自強化偏差（Self-reinforcement bias）**，必須透過隨機洗牌（Order-shuffled）與多評審集成來修正 [Page 18]。

---

## 倫理治理與研究限制（Page 19–20）
1. **多數研究屬初步原型**：受試樣本偏小（多為 15–28 人），缺乏多中心對照試驗與客觀 OSCE 轉化驗證。
2. **資料治理規範落後**：35 篇（87.5%）使用研究者自編小資料集，欠缺標準化與共享機制；使用真實病歷需遵循歐盟 AI 法案（EU AI Act）、WHO 衛生 LLM 指引與 NIST AI 風險管理框架，確保去識別化與人類可追溯審計（Human oversight & traceable audit）[Page 16, 20]。

---

## 原文核對紀錄（至少 3 項）
- **核對項目 1**：系統性回顧 40 篇發表於 2023–2025 年之研究，確立六大實作架構分類（劇本生成 20%、提示詞 VP 22%、自動評分 20%、擬真自適應 15%、知識多智慧體 10%、心理健康 13%）。（核對原文：Page 1 Abstract & Page 4–5 Fig 2，完全一致）
- **核對項目 2**：提出 RA、ER 與加權綜合準確率 AA（整合難度權重、特徵識別與約束遵循）之可重現數學評估公式。（核對原文：Page 17 Equations 1–3，完全一致）
- **核對項目 3**：LLM-as-a-Judge 評審與人類評分相關性 >80%，但存在位置偏差、冗長偏差與自強化偏差，需透過洗牌與集成修正。（核對原文：Page 18，完全一致）
- **查核狀態**：Verified（已通過原文全數據核對）
