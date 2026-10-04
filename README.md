# Canvas-Paint

用 React + HTML Canvas 做的線上小畫家。

**Demo:** <https://bobo100.github.io/canvas-paint/>

## 狀態

2023 年的練習作品，已不再加新功能。

## 功能

- 工具：筆刷、畫框框
- 選擇顏色、調整粗細(1–8)
- 返回(undo)、復原(redo)、清除

已知問題：按過「清除」之後 redo 不會有作用，但按鈕外觀沒有變成停用。

## 本機執行與部署

```bash
npm install
npm run dev        # http://localhost:3000/canvas-paint/
npm run lint
npm run build      # 輸出到 dist/
```

部署:push 到 `main` 後由 GitHub Action([.github/workflows/main.yml](.github/workflows/main.yml))build 並把 `dist/` 推到 `gh-pages` 分支;PR 只跑 build 當檢查。

需要 Node.js 20.19 以上。

技術:Vite、React 19、TypeScript、SCSS。
