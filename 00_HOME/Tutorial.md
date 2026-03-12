# 🚀 個人 OS：使用指南 (User Guide)

> 「這不是一個筆記庫，這是一個與自己對話的動態系統。」

這套系統的設計初衷是為了讓你從「碎片化」的經驗中，歸納出「系統化」的自我認知。以下是如何使用這套系統的教學。

---

## 🛠️ 第一步：安裝必備插件 (Prerequisites)
為了讓儀表板自動運作，請確保你的 Obsidian 安裝並啟用了以下插件：
1. **Dataview**: 核心插件，用於自動彙整筆記（如 `Index.md` 中的表格）。
2. **Templater**: 讓模板套用更自動化，並自動填入日期。

---

## 📋 模板與屬性 (Templates & Properties)

系統透過 **屬性 (Properties)** 來標記筆記的身分，讓 Dataview 能自動幫你歸納。

### 核心屬性說明 (Key Properties)
- `type`: **筆記類型**。這是系統最重要的「身分證」，決定筆記會出現在哪個儀表板。
- `tags`: **階層式標籤**。用於視覺化分類與快速搜尋。
- `themes`: **生命主題**。連結如 `[[Theme/安全感]]`，幫助你發現跨時空的生命模式。
- `people`: **人物連結**。連結如 `[[Person/父親]]`，追蹤特定關係的互動。

### 模板體系一覽 (Template Ecosystem)

| 層次 (Layer) | 模板名稱 (Template) | 關鍵屬性 (Properties) | 寫作時機 (When) |
| :--- | :--- | :--- | :--- |
| **捕捉層** | `Template-Daily` | `type: daily`, `mood`, `energy` | 每天記錄情緒、身體訊號與自動想法。 |
| | `Template-FreeWriting` | `type: free_writing` | 感到混亂、壓力大時的大腦傾倒。 |
| **分析層** | `Template-Memory` | `type: memory`, `period`, `place` | 深入挖掘具體回憶及其帶來的規則。 |
| | `Template-Pattern` | `type: pattern`, `domain`, `triggers` | 拆解反覆出現的行為模式（如拖延）。 |
| | `Template-Person` | `type: person`, `relationship`, `closeness` | 分析與重要他人的互動與界線。 |
| **核心層** | `Template-Value` | `type: value`, `importance` | 定義核心價值觀及其願付代價。 |
| | `Template-TurningPoint` | `type: turning_point`, `period` | 記錄並重新詮釋人生的重大轉捩點。 |
| **回饋層** | `Template-Weekly` | `type: weekly`, `energy_avg`, `mood_avg` | 每週總結，發現模式並檢視規則。 |

---

## 📝 寫作時機與位置 (When & Where to Write)

根據你的**意圖 (Intent)** 選擇合適的寫作位置：

| 情境 (Scenario) | 寫作位置 (Where) | 做法 (How) | 目的 (Purpose) |
| :--- | :--- | :--- | :--- |
| **隨手捕捉當下** | `40_LOGS/` | 建立日期筆記，套用 `Daily` 模板 | 捕捉原始數據，不需考慮分類 |
| **深度考古與填空** | 直接打開對應頁面 | **直接在頁面的引導問題下寫答案** | 建立穩定的自我地圖 |
| **建立獨立「卡片」** | `20_LIFE_STORY/` 或 `30_SYSTEMS/` | 建立新筆記，套用對應模板 | 建立可被自動彙整的「原子化資產」 |
| **感到混亂/壓力大** | `40_LOGS/` | 建立新筆記，套用 `FreeWriting` 模板 | 大腦傾倒 (Brain Dump)，清空空間 |

---

## 🏷️ 標籤體系 (Tagging System)
為了讓分類更精確，系統採用「階層式標籤 (Nested Tags)」：

- `#log/daily`: 每日記錄
- `#story/memory`: 生命回憶
- `#system/pattern`: 行為模式
- `#identity/value`: 核心價值
- (更多詳見各模板預設標籤)

---

## 🔗 如何連結與歸納 (Linking & Organizing)

### 1. 連結 (Link) —— 建立神經網路
- **主題連結**: 在任何筆記中使用 `[[Theme/主題]]`（例如 `[[Theme/安全感]]`）。
- **跨頁連結**: 如果你在寫回憶時發現與某個性格特質有關，請直接連結過去（例如 `這件事反映了我的 [[Personality-BigFive|神經質特質]]`）。

### 2. 歸納 (Organize) —— 自動化儀表板
- **自動歸納**: 只要你在獨立卡片中正確填寫了 `type` 屬性，它們就會自動出現在 `Index.md` 或各個 MOC 的 Dataview 表格中。
- **雙向連結 (Backlinks)**: 打開 Obsidian 右側的「反向連結」面板，你可以看到目前這頁被哪些筆記提到過。

---

## 💡 使用心法 (Mindset)
- **不要急於填滿**: 這是一個長期的系統，不是一份作業。
- **誠實優先**: 這是寫給你自己看的，越誠實，系統就越強大。
- **動態更新**: 你的價值觀、目標、甚至是對回憶的看法都會改變。

---

## 🎨 關係圖視覺化 (Graph View Visualization)
為了讓你的生命地圖更直觀，建議在 Graph View 的 **Groups** 中設置以下顏色規則：

- `tag:#log` -> **灰色** (日常流動)
- `tag:#story` -> **藍色** (過去的敘事)
- `tag:#system` -> **紅色** (運作中的系統)
- `tag:#identity` -> **金色/黃色** (核心身分)
- `[[Theme/]]` -> **紫色** (跨越時空的生命主題)

---

## 🛠️ 故障排除與常見問題 (FAQ)
- **Q: 為什麼 Index.md 的表格是空的？**
  - A: 請檢查是否安裝了 Dataview 插件，且你的筆記 Properties 中是否有正確的 `type`。
- **Q: 我該如何處理舊的筆記？**
  - A: 慢慢將它們搬移到對應的資料夾，並加上 `type` 屬性。

---
*最後更新: 2026-03-12*
