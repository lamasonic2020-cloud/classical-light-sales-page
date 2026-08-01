# 唐芯｜線上成交年訂閱社群 — 銷售頁

單頁靜態銷售頁，純 HTML／CSS，無需建置流程。

## 本機預覽

直接用瀏覽器開 `index.html` 即可；或啟一個本機伺服器：

```bash
python3 -m http.server 8000
# 開 http://localhost:8000
```

## 部署到 GitHub Pages

1. 在 GitHub 建一個新 repo，把這個資料夾裡的所有檔案推上去（含 `.nojekyll`）。
2. Repo → Settings → Pages → Source 選 `Deploy from a branch`，Branch 選 `main` / `/ (root)`。
3. 幾分鐘後即可在 `https://<帳號>.github.io/<repo>/` 看到頁面。

自訂網域：在 Pages 設定填入網域，並在專案根目錄新增一個 `CNAME` 檔（內容為你的網域）。

## 檔案結構

```
index.html                 整頁內容（所有文案都在這裡，直接改）
support.js                 頁面執行環境
image-slot.js              可拖放圖片的預留框元件
uploads/                   照片素材
_ds/classical-.../         Classical 設計系統（styles.css 為所有色彩／字級變數）
```

## 上線前待補

- [ ] 見證截圖 ×3、授課／直播工作照、LINE QR — 目前是預留框，換成 `<img src="...">` 即可
- [ ] 所有「預約 1 對 1 諮詢」按鈕的 `href="#final-cta"` → 改成實際 LINE 連結
- [ ] 頁尾 Instagram 連結
- [ ] 關於唐芯區塊的企業內訓客戶名稱
- [ ] 加上 GA4 或 Meta Pixel 追蹤碼（貼在 `</head>` 前）

## 調整外觀

色彩、字級、間距全部走 `_ds/classical-.../styles.css` 最上方的 CSS 變數，改那裡就會全頁一致更新。
