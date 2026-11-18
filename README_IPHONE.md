# Golf Course AI Simulator — iPhone 版 v1.2

這是針對 iPhone Safari 與「加入主畫面」使用情境調整的 PWA 網頁 App，不是已簽署、可直接安裝的 App Store `.ipa` 原生程式。

## iPhone 專用調整
- iPhone 直向操作與瀏海／Home Indicator 安全區。
- Apple Touch Icon 180×180、iOS Web App meta tags。
- PWA standalone 顯示模式及離線 App Shell。
- 相機優先要求後置鏡頭 `facingMode: environment`。
- 使用 `playsinline`，避免 iPhone Safari 將預覽強制切換成全螢幕播放器。
- 相機啟動錯誤提示改為 iPhone Safari 權限指引。
- 錄影格式依瀏覽器支援情況選擇 MP4／WebM；實際支援仍依 iOS 版本而定。
- 保留校正流程、球局紀錄、果嶺確認及雙模式推桿計分。

## 部署前提
必須把本資料夾「全部內容」部署到 HTTPS 靜態網站，例如 GitHub Pages、Netlify 或 Cloudflare Pages。只開啟本機 HTML 檔案、ChatGPT 內嵌預覽或其他 App 的內建瀏覽器，不適合用來測試 iPhone 相機權限。

## iPhone 安裝步驟
1. 在 iPhone 開啟 Safari。
2. 輸入部署後的 HTTPS 網址。
3. 點 Safari「分享」。
4. 選擇「加入主畫面」。
5. 若顯示「作為網頁 App」選項，保持開啟。
6. 點「加入」，再從 iPhone 主畫面點 Golf AI 圖示啟動。
7. 第一次使用攝影機時，按「啟動攝影機」並允許存取。

## 攝影機限制
- iPhone Safari 的網頁相機 API 不能保證固定 120fps 或 240fps；實際解析度與幀率由 iPhone 型號、iOS、Safari、光線及瀏覽器實作決定。
- 這版可以預覽及錄製一般校正影片，尚未接上 AI 球體偵測、逐格追蹤或真實距離估算模型。
- 若相機權限被拒絕，請到 iPhone「設定 → App → Safari → 相機」檢查權限（不同 iOS 版本選單名稱可能略有差異），並重新載入網站。
- 目前資料儲存在本機瀏覽器，沒有帳號或雲端同步。清除網站資料可能導致紀錄遺失，建議定期匯出 CSV。

## 版本
v1.2 iPhone-first PWA。
