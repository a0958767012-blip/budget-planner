# 錢去哪了？月預算分配器

輸入每月收入，把錢分成「需要、想要、儲蓄」三類，對照 50/30/20 法則，追蹤實際花費與超支提醒，並用終值（FV）公式預測每月儲蓄的長期成長。純靜態網站，無需建置。

## 功能
- 學生／上班族範例，一鍵帶入
- 50/30/20、60/20/20、70/20/10 與自訂法則
- 預計 vs 實際花費、超支提醒、圓環圖
- 儲蓄成長預測（FV = PMT × [(1+r)ⁿ − 1] ÷ r）
- 資料只存在使用者自己的瀏覽器（localStorage）
- 內建「使用說明」，支援深色模式與手機

## 專案結構
```
index.html   網站本體（必須在倉庫最上層）
_headers     Cloudflare 安全標頭
README.md
LICENSE
.gitignore
```

## 部署到 Cloudflare Pages
1. Workers & Pages → Create → Pages → Connect to Git，選擇此倉庫。
2. Framework preset：None；Build command：留空；Build output directory：留空（或 `/`）。
3. Save and Deploy，取得 xxx.pages.dev 網址。

## 備註
- 配色（宇治抹茶）：靜息米白 #F6F7EC、抹茶綠 #7A8864、苔綠 #677D6A、深森綠 #40534C。
- 使用 Google Fonts，載入不到時改用系統字型。
- 本工具僅為試算與記帳輔助，不構成投資建議。
