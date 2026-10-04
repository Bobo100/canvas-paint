# Canvas-Paint

用 React + HTML Canvas 做的線上小畫家。

**Demo:** <https://bobo100.github.io/canvas-paint/>

## 狀態

2023 年的練習作品，已不再加新功能。

## 功能

- 工具：筆刷、畫框框
- 選擇顏色、調整粗細(1–8)
- 返回(undo)、復原(redo)、清除

已知問題:

- 按過「清除」之後 redo 不會有作用，但按鈕外觀沒有變成停用。
- `npm audit` 仍有漏洞，全部在 Create React App 的 build／測試工具鏈(webpack-dev-server、jest、svgo 等),不會進到部署的靜態檔。CRA 已停止維護，要清掉只能改用 Vite 之類的工具。

## 本機執行與部署

```bash
npm install
npm start          # http://localhost:3000
npm run deploy     # build 後推到 gh-pages 分支(GitHub Pages)
```

技術:Create React App、React 18、TypeScript、SCSS。
