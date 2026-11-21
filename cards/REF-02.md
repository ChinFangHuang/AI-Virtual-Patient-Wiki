# 證據卡：REF-02

## 基本資訊
- **REF ID**：REF-02
- **文獻完整名稱**：GenAI-Supported Virtual Patients in Health Care Education: Systematic Review
- **作者**：Juming Jiang, Megan Zichen Ye, Tyrone Tai-On Kwok, Janet Yuen Ha Wong
- **年份**：2026
- **文獻類型**：系統性文獻回顧（Systematic Review）
- **出版刊物**：*Journal of Medical Internet Research* (Vol. 28, e82756)
- **DOI / 來源 URL**：[10.2196/82756](https://doi.org/10.2196/82756) / `https://www.jmir.org/2026/1/e82756`
- **取得範圍**：全文（Full text, 共 26 頁 PDF）
- **虛擬病人技術類別**：生成式人工智慧虛擬病人（GenAI-Supported Virtual Patients）

---

## 研究設計與納入範疇
- **研究設計**：依循 PRISMA 2020 準則與無統合分析綜合報告指引（SWiM）執行之系統性回顧。
- **文獻檢索與篩選**：
  - 檢索 5 大學術資料庫：CINAHL、MEDLINE、Embase、Scopus、Web of Science Core Collection（自資料庫建立至 2026 年 3 月 19 日）。
  - 初步檢索獲得 2860 篇文獻，去重複後篩選 1885 篇，全文評估 107 篇，最終納入 15 篇符合條件之實證研究。
- **總樣本數與學科分佈**：
  - 15 篇研究總參與者共 645 人（N=645，各篇樣本數自 6 人至 145 人不等）。
  - 涵蓋醫護相關專業領域：護理（Nursing）、醫學（Medicine）、藥學（Pharmacy）、放射醫事（Radiography）、第一線緊急救護員（Medical first-responder）。
- **納入研究之設計類型**：
  - 隨機對照試驗（RCT）：3 篇（20%）。
  - 準實驗研究（Quasi-experimental）：6 篇（40%）。
  - 橫斷面研究（Cross-sectional）：6 篇（40%，含 1 篇概念驗證觀察性研究）。
  - 質性與量化研究方法分佈：9 篇為純量化研究，6 篇採量化與質性混合方法（Mixed-methods）。

---

## 系統技術架構與設計特徵綜整（Table 2, p.7–13）
1. **互動模態（Modalities）**：
   - 輸入方式（Input）：文字輸入佔 11 篇、口語語音輸入佔 5 篇、文字/語音混合佔 1 篇。
   - 輸出方式（Output）：純文字回應佔 9 篇、語音合成回應佔 5 篇、文字與語音雙重呈現佔 1 篇。
2. **虛擬化身（Avatar）設計**：
   - 具身化身（3D-embodied avatar）：6 篇（包含結合 VR 頭戴裝置、結合實體安妮模型之混合實境、Furhat 社交機器人臉部投影等）。
   - 無化身（Nonembodied）：9 篇（純文字對話視窗或純語音介面）。
3. **底層 AI 模型分佈**：
   - OpenAI GPT 系列佔壓倒性多數：共 13 篇（86.7%）使用 ChatGPT、GPT-3.5、GPT-4、GPT-4 Turbo 或 GPT-4o。
   - 微調開源模型：1 篇使用微調之百川模型（Fine-tuned Baichuan-13B-Chat）。
   - 多模型家族橫向比較：1 篇（Yu et al., 2025）同時評估 Anthropic Claude 系列（Haiku、Sonnet、Opus）、GPT 系列與開源模型（DeepSeek-V3 671B、Qwen3-32B、LLaMA-3 70B）。
4. **教育理論與教學策略整合現況（Educational Theories）**：
   - **高度缺乏理論支持**：15 篇中僅 3 篇（20%）明確宣告引用教育理論或教學設計架構（Kim et al. 運用 AI 教學設計模型與科技接受模型；Luo et al. 運用 Kolb 經驗學習圈與 Calgary-Cambridge 溝通架構；Chinwong et al. 運用戒菸諮商 5As 架構）。其餘 12 篇（80%）均未提及任何教育理論。

---

## 主要評估成果與研究結果（Table 3 & Results, p.14–19）
1. **評估面向分佈**：
   - 使用者知覺評估（User Perceptions）：14 篇評估了可用性、滿意度、互動擬真感、沉浸感或學習感受。
   - 學習與技能成效評估（Learning Outcomes）：11 篇評估了客觀技能或臨床成效，包括客觀操作表現（Performance, 7 篇）、溝通技巧（Communication skills, 4 篇）、臨床推理（Clinical reasoning, 3 篇）。
2. **對照組與隨機對照試驗（RCT）之實證發現**：
   - 共有 6 篇研究設立對照組（5 篇與傳統教學或無 AI 控制組比較，1 篇比較純 AI 對話 vs AI 對話+回饋）。
   - 3 篇 RCT 均證實生成式虛擬病人具備顯著學習增益：
     - **臨床決策表現（Brügge et al., 2024, RCT, n=21）**：AI 對話搭配結構化回饋組在建立臨床脈絡與資訊收集的評分顯著高於純對話控制組。
     - **眼科病史採集能力（Luo et al., 2025, RCT, n=26）**：介入組之病史採集評分（MHTA score）顯著優於控制組（平均 64.62 vs 54.12 分，平均差 10.50 分，95% CI 4.66–16.33, P<.001），且在同理心表現上亦顯著較佳。
     - **醫學問診表現（Yu et al., 2025, 交叉 RCT, n=20）**：在情感真實感（4.37 vs 3.74, P<.01）、技術可靠性（4.39 vs 3.79, P<.01）與臨床推理技能（4.41 vs 3.97, P<.05）上，AI 虛擬病人表現達到或超越真人標準化病人（Human-Simulated Patients, H-SPs）。

---

## 偏誤風險評估與文獻限制（Risk of Bias via JBI, p.6, p.21）
1. **研究品質呈現顯著落差**：
   - 3 篇 RCT 因隨機分派、隱匿分組與盲法結果評估嚴謹，偏誤風險評為「低至中低度風險（Low to moderate risk）」。
   - 其餘 12 篇準實驗與橫斷面研究偏誤風險普遍偏高（「中度至高度風險」）。
2. **主要方法學限制**：
   - **缺乏對照組與前後測**：9 篇研究（60%）無對照組，亦未在介入前後測量相同變項。
   - **樣本數偏小且為單一機構便利抽樣**：多篇樣本僅 6 至 28 人。
   - **缺乏評量工具信效度**：15 篇中高達 13 篇（86.7%）未報告評估工具的信度或效度檢驗（僅 2 篇有報告）。
   - **過度依賴主觀自評與短期效益**：大部分研究依賴學生自覺問卷，且介入時間極短（5 篇單次少於 10 分鐘，7 篇僅為單次互動），完全缺乏長期追蹤（Longitudinal follow-up）與真實臨床遷移證據。

---

## 技術挑戰與教育邊界（Limitations, p.19–21）
1. **非語言與動態臨床表徵不足**：3D 化身多數呈現僵直靜態，無法即時呈現細微疼痛面容、視線眼神或肢體語言，亦無法動態模擬生命徵象惡化（如呼吸音變化）。
2. **缺乏長期工作階段記憶**：目前虛擬病人多為「單次無狀態」互動，無法記住跨日或跨週的前期互動脈絡，限制了真實世界「縱向追蹤病情演變」之訓練。
3. **幻覺與醫療正確性隱憂**：LLM 內建之偏差或生成合乎語法但醫學錯誤的症狀，若未加設防護欄，將誤導初學者建立錯誤臨床心智模型。
4. **認知負荷問題**：技術故障、語音延遲或 AI 偏離情境迫使學生進行技術除錯（Troubleshooting），增加了額外認知負荷（Extraneous cognitive load），干擾臨床推理的基模建構。

---

## 核對紀錄與查核狀態
- **核對項目 1**：納入 15 篇研究（總受試者 N=645），包含 3 篇 RCT、6 篇準實驗與 6 篇橫斷面研究。（核對原文：Page 1 Abstract & Page 5 Study Characteristics，完全一致）
- **核對項目 2**：底層模型中 OpenAI GPT 系列佔 13 篇，僅 3 篇研究明確結合教育理論架構，13 篇未報告測量工具信效度。（核對原文：Page 1 Abstract, Page 13 Educational Strategies & Page 19，完全一致）
- **核對項目 3**：眼科病史採集 RCT（Luo et al., 2025, n=26）中，介入組 MHTA 分數顯著高於控制組 10.50 分（64.62 vs 54.12, 95% CI 4.66–16.33, P<.001）。（核對原文：Page 16 Table 3，完全一致）
- **查核狀態**：Verified（已通過原文全數據核對）
