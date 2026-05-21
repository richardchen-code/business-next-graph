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

## 注意事項

- **Public Repo**：所有檔案公開可見。**禁止放未發布稿件、API key、客戶資料、財報內部數據**。
- **CDN 快取**：改完 HTML 後 1–5 分鐘 GitHub Pages 才刷新；需強制刷新 URL 後加 `?v=YYYYMMDD`。
- **GitHub Pages 設定**：Settings → Pages → Source 選 `main` branch、`/` (root)。
