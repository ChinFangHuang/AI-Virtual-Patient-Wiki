# AI 虛擬病人 LLM Wiki：護理臨床思維訓練知識庫

> **建置狀態**：第三批 Ingest 完成（已驗證來源：**6/5 篇，全案 Ingest 門檻達成**）。本知識庫嚴格基於已取得之正式學術文獻全文撰寫，每項核心結論與數據均附可定位之文獻引用。

---

## 專案目的與讀者定位
- **專案主題**：AI 虛擬病人（Virtual Patient, VP）——探討大語言模型（LLM）扮演病人之技術原理，及其在訓練護理師與護理學生臨床判斷、檢傷問診、同理心溝通與健康評估之應用。
- **目標讀者**：新進護理師與護理學生。
- **核心特色**：兼顧 **AI 技術工程原理**（提示詞設計、防幻覺分層架構、參數校準、狀態記憶、領域微調模型、六大實作架構、多智慧體閉環、量化指標）與**護理臨床實務應用**（急症檢傷分類、術後照護、跨文化溝通、精神心理諮商、形成性回饋、認知負荷分析、傳統桌面模擬基準比較）。
- **教學聲明**：本知識庫為**護理教學知識庫**，非臨床決策支援系統（CDSS），不可作為真實病人個別診斷或醫療處置依據。

---

## Wiki 知識頁面目錄

1. [1. AI 虛擬病人基礎概念](file:///c:/Users/Fang/Desktop/AI_Virtual_Patient_LLM_Wiki/wiki/01_concepts.md)
   - 虛擬病人（VP）的醫學定義與演進歷程（從 PLATO 分支劇本、桌面 D-VPS、360° VR 影片到生成式 AI）
   - 傳統桌面模擬 D-VPS（低成本、低認知負荷、避免 VR 眩暈）vs 360° VR vs LLM 生成式虛擬病人技術比較
   - 護理臨床教學引進生成式模擬的教學價值與心理安全感
   - 護理學生共識：虛擬病人作為「課堂至臨床實習之輔助過渡工具」，不能取代真實病患接觸與教師引導
2. [2. LLM 技術原理與防幻覺架構](file:///c:/Users/Fang/Desktop/AI_Virtual_Patient_LLM_Wiki/wiki/02_technical_principles.md)
   - 大語言模型對話生成機制、API 串接與專有醫學微調模型運作原理
   - LLM 虛擬病人六大技術實作架構分類（劇本生成、提示詞驅動、自動評分、擬真自適應、知識多智慧體、心理健康）
   - 臨床模擬核心威脅：腳本不一致幻覺、角色漂移、隱藏資訊洩露與 AI 過度迎合偏誤
   - 分層防幻覺架構（Layered Hallucination Mitigation Architecture）：接地提示詞、少樣本範例、負向角色約束、記憶管理、參數校準（溫度調至 0.3）與雲端安全過濾器調校
   - 次世代高階架構：多智慧體閉環動態自適應系統（Adaptive-VP）、圖譜持續寫回機制（CureFun）與協同演化（EvoPatient）
   - 模型客觀量化評估公式（臨床識別率 RA、指令遵循率 ER、加權綜合準確率 AA）
3. [3. 護理臨床情境模擬與多元互動設計](file:///c:/Users/Fang/Desktop/AI_Virtual_Patient_LLM_Wiki/wiki/03_clinical_scenarios.md)
   - 急診護理檢傷分類模擬案例（瘧疾境外移入感染、嗜中性白血球低下發燒）
   - 跨國護理情境模擬：急性肺炎氣道評估與闌尾炎術後生活衛教
   - 傳統桌面虛擬病人經典案例庫（vSim 等 24 篇研究之內外兒科應用）
   - 高階心理健康與精神專科諮商模擬（Patient-Ψ 認知行為治療、SimPatient 動機式晤談、PSYCHE 精神會談）
   - 多模態影像同步系統（MedDiT 圖文生成）
   - 護理學生期待：多元專科案例（內外婦兒）、不配合病患模擬，以及「寫實化身與卡通風格切換」以降低焦慮
4. [4. AI 回饋與教學機制](file:///c:/Users/Fang/Desktop/AI_Virtual_Patient_LLM_Wiki/wiki/04_feedback_mechanisms.md)
   - 護理模擬演練中的反思解說（Debriefing）與結構化回饋核心地位
   - 回饋機制跨技術演進：傳統桌面 D-VPS 程序化回饋 vs LLM 語意深度量規（SPIKES, MIRS, 3E）與多模型集成投票
   - 結構化 3D 解說模型（Defusing, Discovering, Deepening）與 SET-M 評估
   - 馬斯洛需求層次理論（Maslow’s Hierarchy）於臨床優先序評分演算法之應用
   - 學生期望之閉環學習系統（階梯化難度 → 即時回饋 → 補救指引 → 針對弱點重複練習）
   - LLM-as-a-Judge（模型評審）之偏差警訊（位置偏差、冗長偏差、自強化偏差）與認知負荷理論分析
5. [5. 研究成效與實證文獻比較](file:///c:/Users/Fang/Desktop/AI_Virtual_Patient_LLM_Wiki/wiki/05_evidence_comparison.md)
   - 實證研究全貌與方法學梯度（統合分析基準 vs 隨機對照試驗 vs 準實驗 vs 質性研究）
   - 傳統桌面虛擬病人（D-VPS）統合分析基準成效（Zhao et al., 2026, 24 篇, N=1,875）：臨床推理（SMD=0.42）、知識（SMD=2.40）、自信心（SMD=0.39）顯著提升；混合教學與小組學習更優（**特別註明：此為傳統模擬成效，不可直接歸因於 LLM**）
   - 生成式 AI 虛擬病人隨機對照試驗（RCT）之核心量化實證（跨國護理交叉 RCT、臨床決策、眼科問診、一般病史採集）
   - 護理準實驗實證數據（V1 到 V2 腳本不一致率顯著降低 45.6 個百分點、SUS 可用性提升）
   - 護理學生採納動態與信任機制（基於 UTAUT 理論之分析）
   - 嚴格方法學界線：自覺能力提升絕不等於臨床病人照護成效，警惕 AI 過度迎合誘發之「虛假自信」
6. [6. 臨床應用挑戰與未來發展](file:///c:/Users/Fang/Desktop/AI_Virtual_Patient_LLM_Wiki/wiki/06_ethics_limitations.md)
   - 臨床正確性隱患與隱蔽性殘餘錯誤型態（未支持症狀 28.6%、時間線錯誤 23.8%）
   - 人文關懷與深層同理心的本質極限：實體臨場張力與眼神肢體撫慰不可替代
   - 國際 AI 倫理法規遵循（歐盟 AI Act、WHO 衛生 LLM 指引、NIST 風險管理框架）
   - 病歷資料隱私、去識別化、本地模型部署（Local Deployment）與倫理治理
   - 系統可用性瓶頸（語音延遲造成認知過載）與安全過濾器誤判阻斷
   - 評量工具標準化（OSCE）需求與未來展望（AI Triage 3.0 學生自主生成情境、跨會話長期記憶、動態生理表徵連動）

---

## 來源文獻清單（全案已完成驗證：6 篇）
- **[REF-01]** Chan MCM, Hung DCK, Kwok TTO, Wong JYH. Large Language Model–Powered AI-Assisted Simulated Patient for Nursing Education: Quasi-Experimental Study. *JMIR Nursing* 2026;9:e98543. [DOI: 10.2196/98543](https://doi.org/10.2196/98543). [詳細證據卡](file:///c:/Users/Fang/Desktop/AI_Virtual_Patient_LLM_Wiki/cards/REF-01.md)
- **[REF-02]** Jiang J, Ye MZ, Kwok TTO, Wong JYH. GenAI-Supported Virtual Patients in Health Care Education: Systematic Review. *Journal of Medical Internet Research* 2026;28:e82756. [DOI: 10.2196/82756](https://doi.org/10.2196/82756). [詳細證據卡](file:///c:/Users/Fang/Desktop/AI_Virtual_Patient_LLM_Wiki/cards/REF-02.md)
- **[REF-03]** Fung TCJ, Chan SL, Lam CFM, et al. Effects of generative artificial intelligence (GenAI) patient simulation on perceived clinical competency among global nursing undergraduates: a cross-over randomised controlled trial. *BMC Nursing* 2025;24:934. [DOI: 10.1186/s12912-025-03492-0](https://doi.org/10.1186/s12912-025-03492-0). [詳細證據卡](file:///c:/Users/Fang/Desktop/AI_Virtual_Patient_LLM_Wiki/cards/REF-03.md)
- **[REF-04]** Zeng J, Zhu X, Liu X, Li S, Shen S, Zhang Q, Cao S. Undergraduate nursing students’ perceptions, needs, and expectations regarding large language model–based virtual patients: a qualitative study. *BMC Nursing* 2026;25:826. [DOI: 10.1186/s12912-026-04942-z](https://doi.org/10.1186/s12912-026-04942-z). [詳細證據卡](file:///c:/Users/Fang/Desktop/AI_Virtual_Patient_LLM_Wiki/cards/REF-04.md)
- **[REF-05]** Zhao L, Yan H, Liu L, et al. Effect of desktop virtual patient simulation on clinical reasoning skills of nursing students: A systematic review and meta-analysis. *Nurse Education in Practice* 2026;93:104822. [DOI: 10.1016/j.nepr.2026.104822](https://doi.org/10.1016/j.nepr.2026.104822). [詳細證據卡](file:///c:/Users/Fang/Desktop/AI_Virtual_Patient_LLM_Wiki/cards/REF-05.md)
- **[REF-06]** Jo YW, Lee M, Yang HJ. Large Language Model-Based Virtual Patient Simulations in Medical and Nursing Education: A Review. *Applied Sciences* 2025;15:11917. [DOI: 10.3390/app152211917](https://doi.org/10.3390/app152211917). [詳細證據卡](file:///c:/Users/Fang/Desktop/AI_Virtual_Patient_LLM_Wiki/cards/REF-06.md)
