# 引力遊樂場 · Gravity Playground

**版本：v1.0.0** · **共同創作：Tonny（@tonnychiulab）× OpenAI GPT-6 Astra**

讓宇宙亂一下。用滑鼠或手指攪動 2,800 顆星塵，在星環、漩渦與光之海之間切換。

**[直接開玩 →](https://tonnychiulab.github.io/gravity-playground/)**

不需登入、不需安裝。單一 HTML 檔，使用原生 JavaScript 與 Canvas 2D，沒有外部套件、字型或圖片依賴；下載後也能離線玩。

## 共同創作與模型

這是一個由人類與 AI 協作完成的互動作品。

- **[Tonny（@tonnychiulab）](https://github.com/tonnychiulab)**：發起專案、提出需求與創作方向，決定公開發布及共同署名。
- **OpenAI GPT-6 Astra（AI 協作者）**：協作完成視覺設計、程式實作、瀏覽器驗證與部署設定。
- **本次開發環境標示的模型識別碼**：`openai-codex/gpt-6-astra`。

模型資訊記錄的是開發時使用的 AI；網頁執行時不會呼叫模型或 AI API，也不需要 API key。AI 協作署名不代表 OpenAI 官方出品或背書。

## 版本紀錄

### v1.0.0

首個編號版本，對應 Git 標籤 [`v1.0.0`](https://github.com/tonnychiulab/gravity-playground/tree/v1.0.0)。

- 三種粒子模式：星環、漩渦、光之海。
- 滑鼠與觸控擾動、爆發、強度調整、暫停及重置。
- PNG 畫布匯出、鍵盤操作與減少動態效果支援。
- 公開 GitHub Pages 網站、操作文件，以及頁面版本號與人類／AI 共同署名。

## 怎麼玩

| 操作 | 效果 |
| --- | --- |
| 移動滑鼠 | 吸引附近的粒子 |
| 在畫布上按住並拖曳 | 推開粒子、攪動星塵 |
| 放開 | 粒子逐漸回到原本的形態 |
| 來一場大爆發 | 讓粒子向外散開，並開始播放 |
| 擾動強度滑桿 | 調整游標作用力與爆發強度 |
| 暫停／繼續 | 凍結或恢復動畫 |
| 重置 | 回到星環模式，將強度恢復為 65% |
| 存成桌布 | 匯出目前畫布的 PNG，不包含介面文字；尺寸依當前視窗與像素密度而定 |

手機和平板可在畫布空白處按住拖曳。暫停時若要繼續攪動，先按「繼續」。

### 三種模式

- **星環**：暖金色環狀星塵。
- **漩渦**：薄荷綠螺旋星流。
- **光之海**：冰藍色起伏波面。

### 快捷鍵

| 按鍵 | 功能 |
| --- | --- |
| `1` / `2` / `3` | 切換星環／漩渦／光之海 |
| `Space` | 暫停或繼續 |
| `R` | 重置 |

焦點位於按鈕或滑桿上時，保留控制元件原生鍵盤操作，不觸發全頁快捷鍵。若系統啟用「減少動態效果」，頁面預設暫停，可自行按「繼續」或「來一場大爆發」開始播放。切換到其他分頁時會停止繪製，回到頁面後依原先播放狀態恢復。

## 本機開啟

下載本 repo 的 ZIP 並解壓縮，雙擊 `index.html` 即可。

也可以使用 Git：

```sh
git clone https://github.com/tonnychiulab/gravity-playground.git
cd gravity-playground
```

接著用現代瀏覽器開啟 `index.html`。不需要 `npm install`、建置步驟或後端伺服器。

## GitHub Pages

網站由 GitHub Pages 發布，來源為 **`main` 分支的根目錄 `/`**，入口檔案是 `index.html`。

更新檔案並推送至 `main` 後，GitHub 會重新部署。部署狀態可在 repo 的 **Actions** 或 **Settings → Pages** 查看；推送完成不代表網站已立即更新，請等部署成功。

## 檔案

- `index.html`：完整介面、樣式與粒子模擬。
- `README.md`：遊玩與部署說明。
