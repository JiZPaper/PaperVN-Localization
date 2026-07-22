<p align="center">
  <a href="./README.md">English</a> ·
  <a href="./README.zh-Hans.md">简体中文</a> ·
  <strong>繁體中文</strong> ·
  <a href="./README.ja.md">日本語</a> ·
  <a href="./README.ko.md">한국어</a>
</p>

<p align="center">
  <img src="./docs/images/app-icon.png" width="112" alt="PaperVN App 圖示">
</p>

<h1 align="center">PaperVN</h1>

<p align="center">
  <strong>探索故事，掌握每一處細節，讓 VNDB 資料庫隨時保持同步。</strong>
</p>

<p align="center">
  專為探索視覺小說與記錄每一段遊玩旅程而打造的 iPhone 與 iPad 原生 VNDB 用戶端。
</p>

<p align="center">
  <sub>iPhone 與 iPad · iOS / iPadOS 26+ · SwiftUI · 5 種介面語言</sub>
</p>

<p align="center">
  <a href="./docs/images/screenshots/explore.png"><img src="./docs/images/screenshots/explore.png" width="250" alt="PaperVN 探索頁面"></a>
  <a href="./docs/images/screenshots/search.png"><img src="./docs/images/screenshots/search.png" width="250" alt="PaperVN 搜尋頁面"></a>
  <a href="./docs/images/screenshots/library.png"><img src="./docs/images/screenshots/library.png" width="250" alt="PaperVN 資料庫頁面"></a>
</p>

<p align="center"><sub>探索 · 搜尋 · 資料庫</sub></p>

## 深入每部作品背後的故事

從簡要概覽一路深入真正重要的細節：劇情簡介、標籤、截圖、發行版本、製作公司、製作人員、相關作品與外部連結。角色頁面則將角色特徵、聲優與登場作品集中呈現在同一處。

<p align="center">
  <a href="./docs/images/screenshots/visual-novel-details.png"><img src="./docs/images/screenshots/visual-novel-details.png" width="360" alt="PaperVN 的視覺小說詳情"></a>
  <a href="./docs/images/screenshots/character-details.png"><img src="./docs/images/screenshots/character-details.png" width="360" alt="PaperVN 的角色詳情"></a>
</p>

<p align="center"><sub>視覺小說詳情 · 角色詳情</sub></p>

## 依你的方式瀏覽

搜尋視覺小說與角色，並自由組合語言、平台、篇幅、評分與開發狀態等篩選條件。沒有特定搜尋目標時，也可從標籤、角色特徵、發行版本、製作人員、製作公司等分類開始探索。

<p align="center">
  <a href="./docs/images/screenshots/tags.png"><img src="./docs/images/screenshots/tags.png" width="360" alt="在 PaperVN 中瀏覽 VNDB 標籤"></a>
</p>

<p align="center"><sub>標籤與分類瀏覽</sub></p>

## 讓資料庫隨時保持最新

連接你的 VNDB 帳號，即可整理資料庫，並更新遊玩狀態、遊玩版本、評分，以及開始或完成日期。語言、外觀、搜尋與內容安全偏好設定也都能隨時調整。

<p align="center">
  <a href="./docs/images/screenshots/edit-library-entry.png"><img src="./docs/images/screenshots/edit-library-entry.png" width="360" alt="在 PaperVN 中編輯 VNDB 資料庫項目"></a>
  <a href="./docs/images/screenshots/settings.png"><img src="./docs/images/screenshots/settings.png" width="360" alt="PaperVN 使用者與設定頁面"></a>
</p>

<p align="center"><sub>編輯資料庫項目 · 自訂你的 PaperVN</sub></p>

## 功能亮點

- 根據你的 VNDB 資料庫提供個人化探索，所有計算皆在裝置本機完成。
- 支援納入、排除、符合任一與符合全部模式的複合搜尋篩選條件。
- 提供色情或暴力圖片的顯示控制，並可選擇模糊劇透內容、評分與簡介。
- 支援簡體中文、繁體中文、英文、日文與韓文介面，並提供標題語言偏好與裝置端劇情簡介翻譯。
- 支援截圖預覽、縮放、分享及儲存至「照片」。

## 系統需求

- iOS 26.0+ 或 iPadOS 26.0+
- 從原始碼建置時需要 Xcode 26+
- 網際網路連線

## 從原始碼建置

1. 使用 Xcode 26 或更高版本開啟 `PaperVN.xcodeproj`。
2. 選取 `PaperVN` scheme。
3. 選擇執行 iOS 26+ 的模擬器或裝置，然後執行 App。
4. 若要在實體裝置上執行，請在 Signing & Capabilities 中選擇自己的開發團隊；必要時也請更改 Bundle Identifier。

命令列建置：

```bash
xcodebuild \
  -project PaperVN.xcodeproj \
  -scheme PaperVN \
  -sdk iphonesimulator \
  -configuration Debug \
  CODE_SIGNING_ALLOWED=NO \
  build
```

## 連接你的 VNDB 帳號

無須登入即可瀏覽、探索與搜尋公開資料。如要讀取及編輯資料庫，則需要你自己的 VNDB Token：

1. 前往 VNDB 的 [My Profile → Applications](https://vndb.org/u/tokens) 頁面。
2. 建立 Token，並授予 `listread` 與 `listwrite` 權限。
3. 將 Token 貼到 PaperVN 的使用者頁面中。

PaperVN 會將 Token 儲存在 iOS 鑰匙圈中。切勿分享 Token；若意外外洩，請立即前往 VNDB 撤銷並重新建立。

## 採用技術

- Swift、SwiftUI、Combine 與 Swift Concurrency
- URLSession、Codable 與 [VNDB Kana API](https://api.vndb.org/kana)
- Keychain、Translation、StoreKit 2、Photos 與 SafariServices
- Swift Testing 與 XCTest
- 不依賴任何第三方 Swift Package

## 資料來源與免責聲明

PaperVN 透過 [VNDB Kana API](https://api.vndb.org/kana) 取得視覺小說的中繼資料與圖片。相關資料受 [VNDB Data License](https://vndb.org/d17) 與 API 使用條款規範。

PaperVN 是非官方第三方專案，與 [VNDB](https://vndb.org/) 並無關聯，也未獲得 VNDB 的認可。
