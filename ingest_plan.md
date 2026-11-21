# 分批 Ingest 執行計畫

## 目標、界線、驗收
- **最少 5 篇不同文獻**；來源清單見 `raw/source_manifest.csv`。候選不等於已 ingest。
- 每批「取得原始可讀資料 → 擷取可定位內容 → 證據卡 → Wiki 條目 → 原文比對 → 紀錄/commit」。
- 若只能讀摘要，依摘要限定整理；原文的具體統計數據必須有可核位置。
- 區分：①LLM 生成式病人；②更廣義桌面/VR 虛擬病人；不可將後者成效直接歸因於 LLM。

## 第一批：REF-01、REF-02（2 篇）已完成
- REF-01 (Chan et al., 2026, JMIR Nursing)：護理檢傷模擬、分層防幻覺架構、V1/V2 腳本不一致率（62.4% 降至 16.8%）、SUS 與 NPS 評估。
- REF-02 (Jiang et al., 2026, JMIR)：醫療教育生成式虛擬病人系統性回顧（15 篇實證研究、3 篇 RCT、教育理論缺口與 JBI 偏誤風險）。
- 已分別建立 `cards/REF-01.md` 與 `cards/REF-02.md`，並完成 Wiki 初始 6 大主題頁面。

## 第二批：REF-03、REF-04（2 篇）已完成
- REF-03 (Fung et al., 2025, BMC Nursing)：跨 6 國 6 校護理學生交叉 RCT（n=44），比較 GenAI 病人模擬與 360° VR 影片模擬之自覺臨床能力（CCQ）與 AI 準備度（MAIRS-MS）。
- REF-04 (Zeng et al., 2026, BMC Nursing)：護理學生對 LLM 虛擬病人前置期待、功能需求、UTAUT 信任動態與應用邊界之質性實證研究。
- 已分別建立 `cards/REF-03.md` 與 `cards/REF-04.md`，並完成 Wiki 6 大主題頁面深度增修。

## 第三批：REF-05、REF-06（2 篇）執行中
- **編號調整與納入歷程紀錄**：
  - 原訂第二批備選之桌面虛擬病人統合分析文獻（Zhao et al., 2026, Nurse Education in Practice）於第二批讓位給最新護理生質性研究（REF-04）。現依使用者指示正式編為 **REF-05**，作為傳統非生成式桌面模擬的「基準比較證據（Baseline Comparator）」，提供教育成效之橫向對照，**嚴格禁止直接歸因於 LLM**。
  - 原計畫中的 MDPI Applied Sciences LLM 綜述（Jo et al., 2025）順延改編號為 **REF-06**，深入補充 LLM 虛擬病人六大技術實作架構、多智慧體閉環系統、知識圖譜整合與量化評估指標。
- **REF-05 (Zhao et al., 2026, Nurse Education in Practice)**：
  - 篇名：*Effect of desktop virtual patient simulation on clinical reasoning skills of nursing students: A systematic review and meta-analysis*（DOI: [10.1016/j.nepr.2026.104822](https://doi.org/10.1016/j.nepr.2026.104822)）。
  - 重點：納入 24 篇研究、1,875 名護理學生之統合分析；探討臨床推理技能（SMD = 0.42）、知識（SMD = 2.40）與自信心（SMD = 0.39）之成效，以及混合教學與小組學習之優勢。
- **REF-06 (Jo et al., 2025, Applied Sciences)**：
  - 篇名：*Large Language Model-Based Virtual Patient Simulations in Medical and Nursing Education: A Review*（DOI: [10.3390/app152211917](https://doi.org/10.3390/app152211917)）。
  - 重點：回顧 40 篇文獻，歸納六大技術實作分類、知識圖譜/RAG 架構、評估量化指標（RA, ER, AA）與倫理審計標準。
- 分別建立 `cards/REF-05.md`、`cards/REF-06.md`，並增修 Wiki 6 大主題頁面。
- 逐篇核對至少 3 項關鍵結果與原文定位，通過後記錄於 `wiki/log.md`。

## 最終 Wiki → 簡報 Graph
1. 檢索 Wiki，列出需要的教學概念；來源數 >=5（目前達 6 篇完整來源）。
2. 檢查主題覆蓋率：定義、技術、臨床情境、回饋、證據、限制。
3. 建立證據卡、產出 `outline.md`，大綱檢查不足則返回檢索。
4. 逐頁寫簡報草稿；每頁重要論點要引用 Wiki REF；來源錯誤退回該頁或證據卡。
5. 輸出 `deck.html`（8–15 頁），跑連結/引用/頁數/渲染檢查與獨立 AI 忠實度審查。
6. 每一局部問題最多 3 輪，保存紀錄；通過後再交件。

## 記錄格式
每次：日期時間｜批次｜REF ID｜原文取得範圍｜完成 Wiki 條目｜核對段落｜問題｜修正｜重新檢查｜結論｜git commit（如有）。
