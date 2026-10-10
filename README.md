# 一種茶，怎麼在木柵落地？──歷史思考練習

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

- **一次一小步**：每一步只做一件事，畫面上方有進度條。
- **點選為主**：選答案、排卡片、放便利貼，幾乎不用打字；每個任務最後有一題選填的反思。
- **立刻看到理由**：每次點選後，馬上顯示「歷史學家怎麼想」，可以改答案。
- **自動記錄**：進度和答案存在學生自己的瀏覽器（localStorage），可以隨時離開再回來。「練習筆記」頁可以一鍵複製全部紀錄，用來交作業。
- **不需要 AI、不收集資料**：網站沒有後端，不會把學生的作答傳到任何地方。

## 上架到 GitHub Pages

1. 在 GitHub 建立新的 repository（例如 `muzha-tea-thinking`），設為 Public。
2. 把這個資料夾裡的所有檔案上傳到 repository 根目錄：`index.html`、`README.md`、`LICENSE.md`、`sources/`。網頁上可以直接拖曳上傳（Add file → Upload files）。
3. 到 **Settings → Pages**，Source 選 **Deploy from a branch**，Branch 選 `main`、資料夾選 `/ (root)`，按 Save。
4. 約一兩分鐘後，網址會是 `https://<你的帳號>.github.io/<repository 名稱>/`。

如果 repository 名稱不是 `muzha-tea-thinking`，請打開 `index.html`，找到開頭附近這一行，改成你的實際網址：

```js
const SOURCES_URL = "https://github.com/mookrue/muzha-tea-thinking/tree/main/sources";
```

這是網站頁尾「史料包」的連結。

## 修改內容

所有題目都寫在 `index.html` 裡的 `QUESTS` 陣列。每個任務由幾個步驟組成，步驟類型有：

- `read`：閱讀說明或史料
- `choice`：選擇題。每個選項標記 `ok`（與歷史學家一致）、`mid`（部分有道理）或 `no`，並附上回饋文字
- `sort`：把卡片分到不同的框，每張卡片可以有多個可接受的答案
- `board`：延續與變遷看板，每張便利貼有參考座標
- `map`：依任務 3 的分類自動畫出因果圖
- `ade`：用數量、深度、持續判斷重要性
- `reflect`：選填的反思，附參考寫法
- `done`：任務完成與小抄

## 史料包

`sources/` 資料夾收錄網站用到的史料原文照錄、出處與查核紀錄。`00_史料總覽與追查清單.md` 列出：

- 已照錄的史料，以及它們是一手還是二手
- 查核時發現的引文錯誤與資料矛盾（可以直接當教材）
- 尚未取得、建議到圖書館資料庫追查的一手史料

## 製作與分工

本網站由**國立政治大學圖書館**與 AI 助理 **Claude**（Anthropic）合作製作。

| | 國立政治大學圖書館 | Claude |
|---|---|---|
| 教學設計 | 訂定教學目標與整體方向、選定案例（木柵鐵觀音、坪林包種茶）、決定任務形式（自學、以點選為主） | 依指示提出任務流程與互動設計 |
| 素材與史料 | 提供 OER Project 原始工具、回饋表與課程活動；從資料庫檢索並提供報紙、方志等史料全文；提供研究文獻 | 從提供的資料與公開資料中整理史實、照錄史料、追查註腳出處 |
| 製作 | 審閱並決定所有內容取捨 | 撰寫網站程式、題目與回饋文字、README 與史料包說明 |
| 品質檢查 | 提出查核要求，確認爭議處理方式（例如「大庭茶商公會」的解讀、保留或移除引用文獻） | 逐句引用查核、爭議用語檢視、與 OER 原版對照，並記錄於 `sources/11`、`sources/12` |

網站中「歷史學家怎麼想」的回饋是教學判斷，不是史料本身。如發現錯誤，歡迎告知國立政治大學圖書館。

## 授權與出處

- 練習設計改作自 [OER Project](https://www.oerproject.com/) 的歷史思考技能指南、工具（Sourcing、Contextualization、Causation、Comparison）、回饋表（Sourcing、Contextualization、CCOT、Comparison）與課程活動（Causation、CCOT、Claim Testing），工具與回饋表以 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) 授權。本網站已翻譯為繁體中文、改為逐步點選形式，並換成臺灣在地案例。
- 與 OER 原版的對照與本站新增的部分，見 `sources/12_與OER原版對照.md`。
- 網站中引用的史料與研究，其著作權屬原作者或原出版單位。網站只節錄短篇幅並註明出處，供教學使用。詳見 `LICENSE.md`。
