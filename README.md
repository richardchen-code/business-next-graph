# Business Next Graph

《數位時代》互動視覺配件托管庫，由 [visual-asset](https://github.com/terrylee-lang/BN_next/blob/main/visual-asset.md) Skill 自動產出 HTML 互動配件並托管於此。

- 線上預覽：https://richardchen-code.github.io/business-next-graph/
- 配件嵌入文章時使用 iframe，src 指向上述網域

## 目錄結構

```
business-next-graph/
├── .nojekyll          # 必要：避免 Jekyll 忽略 _assets/
├── index.html         # 首頁卡片牆（陸續加入配件後維護）
├── 2026/              # 配件 HTML 依年份分類
│   └── MM-主題-kebab-case.html
└── _assets/
    ├── base.css       # 共用樣式（累積到 3-4 個配件後抽出）
    └── logos/         # 自托管 logo（如需高解析度）
```

## 配件命名規範

`<年份>/<MM-主題-kebab-case>.html`

例：`2026/05-layoffs-tracker.html`、`2026/06-openai-revenue-breakdown.html`

## 配件清單

| 日期 | 配件 | 檔案 |
|---|---|---|
| 2026 / 07 / 14 | 阿姨經濟 1 / 3：43.2 歲，25 年沒變的「阿姨」認知 | `2026/07-auntie-economy-perception.html` |
| 2026 / 07 / 14 | 阿姨經濟 2 / 3：熟齡女性的 4 個行為轉變 | `2026/07-auntie-economy-spending-shift.html` |
| 2026 / 07 / 14 | 阿姨經濟 3 / 3：15 兆美元，被隱形的熟齡女性商機 | `2026/07-auntie-economy-15trillion.html` |
| 2026 / 06 / 05 | AI 已經變成最好聊的同事 | `2026/06-ai-replacing-coworker-interactions.html` |
| 2026 / 05 / 21 | 宜得利 vs 無印良品市值黃金交叉 | `2026/05-nitori-vs-muji-timeline.html` |

## 注意事項

- **Public Repo**：所有檔案公開可見。**禁止放未發布稿件、API key、客戶資料、財報內部數據**。
- **CDN 快取**：改完 HTML 後 1–5 分鐘 GitHub Pages 才刷新；需強制刷新 URL 後加 `?v=YYYYMMDD`。
- **GitHub Pages 設定**：Settings → Pages → Source 選 `main` branch、`/` (root)。
