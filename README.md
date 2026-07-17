# cubicle-ai

**An enterprise AI literacy course for the cubicle worker — four self-contained interactive HTML presentations.**
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

四個檔案放在同一個資料夾，用瀏覽器直接開啟即可。建議課前把四份各開一個分頁、按 `F11` 全螢幕，現場用 `Ctrl+Tab` 切換。

### 快捷鍵

| 按鍵 | 功能 |
|------|------|
| `→` `←` `空白鍵` `點擊` | 翻頁 |
| `Home` / `End` | 跳到第一頁 / 最後一頁 |
| `1`–`9` | 直接跳頁 |
| `R` | 重播當前頁動畫 |
| `S` | 開關投影設定面板（字級 90–140%、高對比、安全邊距、減少動態） |
| `T` | 封面：顯示／隱藏倒數計時器 |
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

課程中的數據皆來自公開來源（查閱時間：2026 年）：

- **McKinsey** — 工作時間分配（郵件約 28%、會議約 23%、找資料約一天/週）；生成式 AI 可自動化 60–70% 工作活動
- **OpenAI Enterprise Usage Report** — AI 採用度前 5% 員工的訊息量是一般員工的 6 倍；「這個差距無關技術，是行為造成的」
- **Apple Research《The Illusion of Thinking》** 與 RAG 相關研究 — 乾淨資料 89% vs 雜訊資料 72% 準確度；脈絡半數以上無關時幻覺增加 18–48%
- **Anthropic**（2026/6/16，約 40 萬次 Claude Code 使用分析）— 領域專業比寫程式背景更能預測成功
- **Andrej Karpathy**（Sequoia Ascent 2026）— 「你可以外包你的思考，但你無法外包你的理解」

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
