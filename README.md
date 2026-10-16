# LINE 貼圖工作室

用 AI 生成或上傳圖片，加上文字、去背、套邊框，整理成符合 LINE Creators Market 規格的貼圖套件 ZIP。

**線上使用**：https://kftseng2oo1.github.io/line-sticker/

## 主要功能
- **🤖 AI 生成**
  - Claude SVG：選角色（貓咪、柴犬、熊熊、青蛙、兔兔…）、畫風、常用語，生成向量貼圖
  - Stability AI：上傳照片轉成新海誠、皮克斯 3D、吉卜力、水彩、浮世繪、賽博龐克等風格
- **📁 上傳圖片**：自動縮放到貼圖尺寸，可用 remove.bg 去背，套用邊框
- 文字可橫排或直排，也可不加字
- **🗂 管理貼圖**：分套件管理，每套 8 張，累計最多 40 張
- **📦 匯出 ZIP**，可複製圖片或分享到 LINE

## 技術與依賴
- 單檔 HTML PWA（`index.html` 內含全部 HTML/CSS/JS），`manifest.json` + `sw.js` 提供安裝到主畫面與離線快取。
- 後端：`arcar.kftseng2oo1.workers.dev`（Claude、`/sd/t2i`、`/sd/i2i`）
- 去背：`api.remove.bg`（需 API Key）；JSZip（cdnjs）

## 相關 repo
- [cut](https://github.com/kftseng2oo1/cut)：把整張貼圖表格裁成單張
- [Cmt](https://github.com/kftseng2oo1/Cmt)：LINE 動態貼圖編輯器
