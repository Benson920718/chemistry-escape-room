# 零號實驗室｜化學知識解謎密室逃脫

一款以研究室封鎖為背景的互動式化學解謎網站。玩家須在 30 分鐘內完成六道知識謎題，逐關解除鎖定。

## 玩法
1. 按「進入實驗室」開始 30 分鐘倒數。
2. 閱讀研究線索與資料卡，輸入答案。
3. 答對後查看化學概念解說，再前往下一關。
4. 每題最多查看兩層提示；遊戲狀態保存在目前瀏覽器。

六關主題：原子序、pH 酸鹼性、反應式平衡、密度與浮沉、物理／化學變化、分子式原子數。

## 技術
- HTML5、CSS3、原生 JavaScript。
- 無需 npm、資料庫、伺服器或第三方套件。
- localStorage 儲存個人遊戲進度。
- 響應式版型，支援桌面與行動裝置。

## 本機預覽
直接以瀏覽器開啟 `index.html`，或在專案目錄執行：
```bash
python -m http.server 8000
```
然後開啟 `http://localhost:8000`。

## Cloudflare Pages 部署
1. Cloudflare Dashboard → Workers & Pages → Create application → Pages。
2. Connect to Git → 選擇 `Benson920718/chemistry-escape-room`。
3. Production branch：`main`。
4. Framework preset：`None`；Build command：留空；Build output directory：`.`。
5. 儲存並部署。網站首頁位於 repository 根目錄的 `index.html`。

## 文件
- `docs/PROJECT_PLAN.md`：專案目標、學習關卡、技術規格與驗收清單。
- `_headers`：基本安全回應標頭。

> 本作品為教育用途模擬解謎，不是實驗操作指南；請勿在現實中混合未知化學品。
