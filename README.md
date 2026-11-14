# cubicle-ai

**An enterprise AI literacy course for the cubicle worker — four self-contained interactive HTML presentations, plus a references page.**
Designed for non-technical office staff and managers. Content in Traditional Chinese.

---

## 這是什麼

一套為企業內訓設計的 AI 入門課程，對象是**每天和文件、郵件、報告為伍，但沒有技術背景的辦公室同仁與主管**。

四個檔案都是**單一 HTML**，用瀏覽器打開就能播放，不需要安裝任何東西、不需要網路（字型有系統備援）、不需要 PowerPoint。

課程主軸很簡單：

> 乏味的留給 AI，重要的留給你。

---

## 課程結構

| 檔案 | 內容 | 頁數 |
|------|------|------|
| `course_cover_final.html` | 封面 · 蟲洞動畫，可當進場待機畫面 | — |
| `ai_intro_presentation.html` | **Part 1 · 認識 AI** — Why / What / Who / When | 11 |
| `ai_understand_you.html` | **Part 2 · 讓 AI 懂你** — 需求表達、餵對資料、建立素材庫 | 8 |
| `ai_apply_examples.html` | **Part 3 · 應用實例** — 痛點辨識、情境題抽獎機、收尾 | 3 |
| `references.html` | **參考資料** — 每個數字的原始出處（附對應頁面連結）、延伸閱讀、修訂紀錄 | — |
| `index.html` | 課程首頁（GitHub Pages 入口） | — |

設計上四份走一條「逐漸明亮的深色曲線」：封面純黑 → Part 1 靛青 → Part 2 青綠 → Part 3 亮天藍，連續播放時色調會自然推進。

---

## 使用須知

本專案是**企業 AI 素養內訓教材**，設計給講師在實體課程中使用，**非隨插即用的成品**——建議依你的受眾、公司環境、可用的 AI 工具調整內容後再上場。

課程中部分資訊具時效性，使用前請自行核實更新，包括但不限於：

- AI 廠商版圖（如「三巨頭」的指涉對象、市場份額，這塊變動很快）
- 引用的統計數據與研究報告（發布時間、方法論可能已有更新版本）
- 特定產品功能、定位或命名（AI 產品迭代速度快，簡報中提及的功能可能已更新或更名）

以上內容以查閱當下（2026 年）的公開資訊為準，不代表持續維護或即時更新。

---

## 使用方式

所有檔案放在同一個資料夾，用瀏覽器直接開啟即可（線上版：<https://alphag60229.github.io/cubicle-ai/>）。建議課前把四份各開一個分頁、按 `F11` 全螢幕，現場用 `Ctrl+Tab` 切換。

每份簡報左上角有章節導覽列（滑過才會變亮，投影時可按 `H` 隱藏），每章最後一頁左下角有「下一章」連結，封面上的三個站點也可以直接點進該章。

網址後加 `#p頁碼` 可直接開到指定頁，例如 `ai_understand_you.html#p6`；翻頁時網址會自動更新，方便把特定頁面傳給同事。

### 快捷鍵

| 按鍵 | 功能 |
|------|------|
| `→` `←` `空白鍵` `點擊` | 翻頁 |
| `Home` / `End` | 跳到第一頁 / 最後一頁 |
| `1`–`9` | 直接跳頁 |
| `R` | 重播當前頁動畫 |
| `S` | 開關投影設定面板（字級 90–140%、高對比、安全邊距、減少動態） |
| `T` | 封面：顯示／隱藏倒數計時器 |
| `H` | 顯示／隱藏左上角章節導覽列 |
| `Esc` | 關閉圖片放大（Part 2）／題目編輯視窗（Part 3） |
| `Enter` | Part 3 抽獎機：抽一題 |

投影設定會記在瀏覽器裡，下次開啟自動套用。

### 封面

- **倒數計時器**：⚙ 設定 → 輸入分鐘 → 開始。最後一分鐘會轉紅提示，歸零顯示「即將開始」。
- **QR Code**：⚙ 設定 → 上傳圖片，顯示在左下角，可自訂說明文字，會存在瀏覽器裡。

### Part 3 情境題抽獎機

內建 10 題辦公室痛點情境（PowerShell 建資料夾、Excel 函數與 VBA、Draw.io 流程圖、HTML 批次壓縮工具、簡報翻譯、會議記錄、週報範本、Q&A 機器人、請假信）。

- 點「抽一題」隨機抽出，單次課程中不重複
- 抽到的題目附範例 Prompt，可一鍵複製
- 抽過的題號會列出，點了可重看
- 「✏ 編輯題目」可現場改題目（存在瀏覽器），或用「匯出題目」把內容複製成程式碼片段，貼回原始碼永久保存

要直接改預設題目，開啟 `ai_apply_examples.html`，找到檔案裡的 `DEFAULT_QUESTIONS` 區塊修改即可。這也是這份教材設計成可持續擴充的地方——場景、痛點、產業案例都可以自行替換。

---

## 引用的研究與資料

完整出處、原文連結、可信度標註與「出現在哪一頁」都整理在 [`references.html`](references.html)。摘要如下（查閱時間：2026 年 11 月）：

- **Part 1** — Brynjolfsson 等《Generative AI at Work》（NBER 2023）；Dell'Acqua 等《Navigating the Jagged Technological Frontier》（HBS × BCG 2023）；GitHub Copilot 對照實驗（2022）；OpenAI《The state of enterprise AI》（2025/12）；McKinsey《The social economy》（2012）；HBR《Stop the Meeting Madness》（2017）；Microsoft Learn（Copilot 中的 Anthropic 模型）
- **Part 2** — Microsoft Learn（Copilot Chat 模式選單）；Google《Prompting guide 101》（PTCF）；Microsoft Support（GCSE）；Apple《GSM-Symbolic》（ICLR 2025）
- **Part 3** — Anthropic《Agentic coding and persistent returns to expertise》（2026/6/16）；Andrej Karpathy @ Sequoia AI Ascent 2026（引述）

---

## 更新紀錄

### 2026-11 · 內容查證與互連

- 替換查無出處的數據：Part 1 四個匿名企業案例、Part 2 的 89% / 72% 與「幻覺 +18–48%」（原標 Apple《The Illusion of Thinking》，該論文無此數據）
- 修正引用錯誤：OpenAI 6 倍是「使用量」不是「產出量」、年份為 2025/12；HBR 23 是「小時／週、主管」不是 23%；Karpathy 那句話為引述
- 更新 2026 現況：Copilot 已可在模型選單切換 Claude；補上 Copilot 英文介面模式名稱與 Microsoft 官方 GCSE 架構
- 新增互連：章節導覽列、章末下一章、封面站點可點、`#p頁碼` 深層連結、`references.html`
- 修正：Part 2 深色背景下看不見的副標、頁碼點、開關；Part 3 Prompt 含引號時「複製」按鈕失效、編輯內容未跳脫 HTML

逐項對照見 [`references.html#changelog`](references.html#changelog)。

---

## 製作說明

- 簡報由 HTML / CSS / 原生 JavaScript 手寫，無任何框架與相依套件
- 封面蟲洞動畫與 Part 2 的示意圖片由 Google Gemini 輔助生成
- 中文字型使用 Google Fonts（Noto Sans TC），並內建系統字型備援（微軟正黑體 / 蘋方 / 黑體），離線環境仍可正常顯示

---

## 授權

本專案採用 [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/) 授權。

你可以自由地使用、修改、再散布，包含商業用途，只要標示原作者。

作者：[AlphaG60229](https://github.com/AlphaG60229)
