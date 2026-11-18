# Golf Course AI Simulator — Mobile PWA v1.1

## 這一版的手機功能
- 手機優先版面與底部導覽列
- 支援直向操作、較大的觸控按鈕及 iPhone 安全區
- 優先使用手機後置鏡頭預覽
- PWA manifest、主畫面圖示及 Service Worker
- 支援 Android Chrome 安裝；iPhone/iPad 可透過 Safari「分享 → 加入主畫面」
- 原有校正、球局紀錄、果嶺確認及雙模式推桿計分保留

## 部署
將整個資料夾內容上傳至 GitHub Pages、Netlify 或其他 HTTPS 靜態網站服務。不要只上傳 index.html；manifest、sw.js 和 icons 必須一起上傳。

## 手機安裝
- Android：Chrome 開啟 HTTPS 網址 → 選單 →「安裝應用程式」或「加入主畫面」。
- iPhone：Safari 開啟 HTTPS 網址 → 分享 →「加入主畫面」。

## 攝影機注意
攝影機只會在使用者按下啟動並授權後開啟。瀏覽器必須透過 HTTPS（或 localhost）提供頁面。手機瀏覽器取得的實際 FPS 依裝置、瀏覽器與光線條件而定；此版本不是原生 120/240fps 相機控制，也尚未串接 AI 球體追蹤模型。

## 本機測試
在資料夾內執行 `python -m http.server 8000`，桌面開啟 `http://localhost:8000`。手機正式測試請部署至 HTTPS 網址。
