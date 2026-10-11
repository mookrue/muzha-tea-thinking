# 一種茶，怎麼在木柵落地？──歷史思考練習

教學內容改作自 OER Project〈[Historical Thinking Skills Guide](https://www.oerproject.com/OER-Materials/OER-Media/HTML-Articles/Teacher-Resources/Historical-Thinking-Skills-Guide)〉（CC BY 4.0）。

> **警語：** 本網站的資料出處尚未經人工逐一檢核。網站中的提問與引導，是依據 OER Project〈[Historical Thinking Skills Guide](https://www.oerproject.com/OER-Materials/OER-Media/HTML-Articles/Teacher-Resources/Historical-Thinking-Skills-Guide)〉的教材內容提供；網站的目的是把這些歷史思考教學內容具體化、互動化，用來展示歷史思考的流程，不是可信的歷史推論。網站只使用了有限的資料，因此只呈現這段歷史的部分樣貌。

用木柵鐵觀音的真實史料，讓學生**自己一步一步**練習歷史學家的六種思考方法。整個網站只有一個 `index.html`，不需要伺服器，也不需要帳號，打開就能用。

## 六個任務

| 任務 | 技能 | 內容 |
|---|---|---|
| 1 | 史料考證 Sourcing | 用 HAPPY 五問考證 1908 年《漢文臺灣日日新報》的茶市報導 |
| 2 | 脈絡化 Contextualization | 用漏斗把「1895 年鐵觀音來到木柵」放回時代 |
| 3 | 因果 Causation | 排出長期、中期、短期原因，看自動產生的因果圖，用 ADE 判斷重要性 |
| 4 | 延續與變遷 CCOT | 在「延續↔變遷 × 正面↔負面」看板上放便利貼 |
| 5 | 論點檢驗 Claim Testing | 用直覺、權威、邏輯、證據檢驗一個 AI 給的錯誤年份 |
| 6 | 比較 Comparison | 木柵鐵觀音 vs 坪林包種茶 |

設計原則：

- **一頁一個重點**：相關的小題放在同一頁，每個任務 3–5 頁，畫面上方有進度條。
- **點選為主**：選答案、排卡片、放便利貼，幾乎不用打字；每個任務最後有一題選填的反思。
- **立刻看到理由**：每次點選後，馬上顯示引導說明，可以改答案。
- **自動記錄**：進度和答案存在學生自己的瀏覽器（localStorage），可以隨時離開再回來。「練習筆記」頁可以一鍵複製全部紀錄，用來交作業。
- **不需要 AI、不收集資料**：網站沒有後端，不會把學生的作答傳到任何地方。

## 資料搜尋方式

一手史料主要透過臺鵠 TAIHU 人文知識探勘系統（臺大數位人文研究中心）以提問方式查得；二手資料則透過 Google、華藝線上圖書館（Airiti Library）及臺灣博碩士論文知識加值系統查得。以上只做了單輪搜尋，尚未全面轉換關鍵字，因此並未找到完整的相關資料。

## 製作與分工

本網站由**國立政治大學圖書館**與 AI 助理 **Claude**（Anthropic）合作製作，於 2026 年 10 月使用 Claude Opus 5.5（medium）完成。

| | 國立政治大學圖書館 | Claude |
|---|---|---|
| 教學設計 | 訂定教學目標與整體方向、選定案例（木柵鐵觀音、坪林包種茶）、決定任務形式（自學、以點選為主） | 依指示提出任務流程與互動設計 |
| 素材與史料 | 提供 OER Project 原始工具、回饋表與課程活動；從資料庫檢索並提供報紙、方志等史料全文；提供研究文獻 | 從提供的資料與公開資料中整理史實、照錄史料、追查註腳出處 |
| 製作 | 決定內容取捨 | 撰寫網站程式、題目與回饋文字、README 與說明文字 |
| 品質檢查 | 提出查核要求，確認爭議處理方式（例如「大庭茶商公會」的解讀、保留或移除引用文獻） | 逐句引用查核、爭議用語檢視、與 OER 原版對照，並留有內部查核紀錄（未公開） |

> **注意：** 本網站已使用自訂的引用查核 skill（citation-verification）讓 Claude 自我檢核，然而資料出處的正確性尚未經人工逐一查證。表中的「品質檢查」是 Claude 的自我檢核，不等於人工查證。

網站中的引導說明是教學判斷，不是史料本身。如發現錯誤，歡迎告知國立政治大學圖書館。

## 授權與出處

- 練習設計改作自 OER Project 的歷史思考技能指南 [Historical Thinking Skills Guide](https://www.oerproject.com/OER-Materials/OER-Media/HTML-Articles/Teacher-Resources/Historical-Thinking-Skills-Guide)、工具（Sourcing、Contextualization、Causation、Comparison）、回饋表（Sourcing、Contextualization、CCOT、Comparison）與課程活動（Causation、CCOT、Claim Testing），工具與回饋表以 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) 授權。本網站已翻譯為繁體中文、改為逐步點選形式，並換成臺灣在地案例。
- 網站中引用的史料與研究，其著作權屬原作者或原出版單位。網站只節錄短篇幅並註明出處，供教學使用。詳見 `LICENSE.md`。
