# 🏠 個人 OS：入口 (Home)

> 「認識你自己。」—— 蘇格拉底

## 🧩 核心索引 (Core Index)

- [[01_MOCs/MOC-Identity|0. 身分與版本 (Identity)]]：我是誰、我現在在哪個階段
- [[01_MOCs/MOC-Identity|1. 核心問題 (Core Questions)]]：我最想解開的謎題
- [[01_MOCs/MOC-Identity|2. 性格特質 (Personality)]]：我的反應模式與優勢
- [[01_MOCs/MOC-Identity|3. 價值與目標 (Values & Goals)]]：我重視什麼
- [[01_MOCs/MOC-LifeStory|4. 人生故事 (Life Story)]]：我如何走到今天
- [[01_MOCs/MOC-LifeStory|5. 童年與家庭 (Childhood & Family)]]：根源的塑造
- [[01_MOCs/MOC-Systems|6. 關係地圖 (Relationship Map)]]：我與他人的互動
- [[01_MOCs/MOC-Systems|7. 行為系統 (Behavioral Systems)]]：習慣、拖延與工作流
- [[01_MOCs/MOC-Systems|8. 身心狀態 (Mind & Body)]]：情緒與能量管理

---

## 📊 儀表板 (Dashboard)

### 🌪️ 最近出現的模式 (Recent Patterns)
```dataview
TABLE domain, triggers, payoff_short_term, cost_long_term
FROM "30_SYSTEMS"
WHERE type = "pattern"
SORT file.ctime desc
LIMIT 5
```

### 👶 童年回憶按期別 (Childhood Memories)
```dataview
TABLE period, place, themes
FROM "20_LIFE_STORY"
WHERE type = "memory"
SORT period asc
```

### 👥 重要關係追蹤 (Key Relationships)
```dataview
TABLE relationship, closeness
FROM "30_SYSTEMS"
WHERE type = "person"
SORT closeness desc
```

### 🌡️ 最近的情緒與能量 (Recent Mood & Energy)
```dataview
TABLE mood, energy, themes
FROM "40_LOGS"
WHERE type = "daily"
SORT file.name desc
LIMIT 7
```

---
[[00_HOME/Tutorial|📖 使用指南]] | [[00_HOME/Examples|💡 實作範例]] | [[90_TEMPLATES/Prompts-Library|🧠 深度問句庫]]
