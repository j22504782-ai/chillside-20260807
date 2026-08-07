# 專案紀錄

更新日期：2026-08-07  
專案類型：靜態單頁網站

## 專案概覽

此專案目前以 `index.html` 建立一個 Bootstrap 5 的示範首頁。頁面包含導覽列、圖片輪播（Carousel）與一個主標題；沒有本機 CSS、JavaScript、套件設定檔或建置流程。

## 檔案結構

```text
website/
├── index.html          # 網站首頁與全部頁面結構
├── images/
│   ├── 1.jpg           # 輪播第 1 張圖片（800 × 534）
│   ├── 2.jpg           # 輪播第 2 張圖片（960 × 635）
│   └── 3.jpg           # 輪播第 3 張圖片（577 × 346）
└── .vscode/            # VS Code 工作區設定資料夾
```

## 技術與相依項目

- HTML5
- Bootstrap 5.0.2 CSS（由 jsDelivr CDN 載入）
- Bootstrap 5.0.2 Bundle（含 Popper，由 jsDelivr CDN 載入）

頁面需要網路連線才能取得 Bootstrap 的樣式與互動功能。

## 頁面內容

1. 導覽列：顯示 `Navbar` 品牌與 Home、Features、Pricing、Disabled 項目。
2. 圖片輪播：使用 Bootstrap Carousel，依序載入 `images/1.jpg`、`images/2.jpg`、`images/3.jpg`。
   - 第 1 張停留 10 秒。
   - 第 2 張停留 2 秒。
   - 第 3 張採用 Bootstrap 預設間隔。
3. 頁面標題：顯示 `Hello, world!`。

## 維護注意事項

- `lang` 目前設定為 `en`；若網站內容改為中文，建議同步改成 `zh-Hant`。
- `<title>`、導覽文字、輪播標題與說明目前皆為 Bootstrap 預設示範文字，正式上線前應替換成網站實際內容。
- 輪播圖片尺寸比例不一致，顯示時可能造成版面高度變動；建議統一圖片比例或加入固定高度與 `object-fit: cover` 樣式。
- 圖片的 `alt` 目前為 `...`，建議改為能描述圖片內容的替代文字，以改善無障礙性與 SEO。
- 專案尚未有自訂 CSS；視覺調整可新增 `css/style.css`，並於 `index.html` 引入。

## 本機預覽

可直接在瀏覽器開啟 `index.html`，或使用 VS Code 的 Live Server 類型工具啟動本機伺服器進行預覽。

## Github推送地址
USER NAME:j22504782.ai
專案名稱：chillside-20260807
HTTPS:https://github.com/j22504782-ai/chillside-20260807.git
SSH:git@github.com:j22504782-ai/chillside-20260807.git