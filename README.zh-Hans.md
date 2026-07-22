<p align="center">
  <a href="./README.md">English</a> ·
  <strong>简体中文</strong> ·
  <a href="./README.zh-Hant.md">繁體中文</a> ·
  <a href="./README.ja.md">日本語</a> ·
  <a href="./README.ko.md">한국어</a>
</p>

<p align="center">
  <img src="./docs/images/app-icon.png" width="112" alt="PaperVN App 图标">
</p>

<h1 align="center">PaperVN</h1>

<p align="center">
  <strong>发现故事，读懂细节，让 VNDB 资料库始终同步。</strong>
</p>

<p align="center">
  一款为 iPhone 和 iPad 打造的原生 VNDB 客户端，帮你发现视觉小说，也记录每一段游玩旅程。
</p>

<p align="center">
  <sub>iPhone 与 iPad · iOS / iPadOS 26+ · SwiftUI · 5 种界面语言</sub>
</p>

<p align="center">
  <a href="./docs/images/screenshots/explore.png"><img src="./docs/images/screenshots/explore.png" width="250" alt="PaperVN 探索页面"></a>
  <a href="./docs/images/screenshots/search.png"><img src="./docs/images/screenshots/search.png" width="250" alt="PaperVN 搜索页面"></a>
  <a href="./docs/images/screenshots/library.png"><img src="./docs/images/screenshots/library.png" width="250" alt="PaperVN 资料库页面"></a>
</p>

<p align="center"><sub>探索 · 搜索 · 资料库</sub></p>

## 看见每部作品背后的故事

从作品概览自然深入到真正重要的细节：简介、标签、截屏、发行版本、会社、制作人员、相关作品与外部链接。角色页面则把特征、声优和登场作品集中在一处。

<p align="center">
  <a href="./docs/images/screenshots/visual-novel-details.png"><img src="./docs/images/screenshots/visual-novel-details.png" width="360" alt="PaperVN 视觉小说详情页面"></a>
  <a href="./docs/images/screenshots/character-details.png"><img src="./docs/images/screenshots/character-details.png" width="360" alt="PaperVN 角色详情页面"></a>
</p>

<p align="center"><sub>视觉小说详情 · 角色详情</sub></p>

## 按你的方式浏览

搜索视觉小说和角色，再组合语言、平台、篇幅、评分与开发状态等筛选条件。没有明确目标时，也可以从标签、特征、发行版本、制作人员和会社等分类开始探索。

<p align="center">
  <a href="./docs/images/screenshots/tags.png"><img src="./docs/images/screenshots/tags.png" width="360" alt="在 PaperVN 中浏览 VNDB 标签"></a>
</p>

<p align="center"><sub>标签与分类浏览</sub></p>

## 让资料库始终跟上进度

连接 VNDB 账号后，你可以整理资料库，并更新游玩状态、游玩版本、评分以及开始或结束日期。语言、外观、搜索与内容安全偏好也都触手可及。

<p align="center">
  <a href="./docs/images/screenshots/edit-library-entry.png"><img src="./docs/images/screenshots/edit-library-entry.png" width="360" alt="在 PaperVN 中编辑 VNDB 资料库条目"></a>
  <a href="./docs/images/screenshots/settings.png"><img src="./docs/images/screenshots/settings.png" width="360" alt="PaperVN 用户与设置页面"></a>
</p>

<p align="center"><sub>编辑资料库条目 · 打造你的 PaperVN</sub></p>

## 功能亮点

- 根据你的 VNDB 资料库生成个性化发现内容，推荐计算在设备本地完成。
- 支持“包含、排除、任意、全部”等匹配方式的复合搜索筛选。
- 可控制色情或暴力图片的显示，并选择模糊剧透、评分与简介。
- 支持简体中文、繁体中文、英语、日语和韩语界面，并提供标题语言偏好与设备端简介翻译。
- 支持作品截屏预览、缩放、分享及保存到照片。

## 系统要求

- iOS 26.0+ 或 iPadOS 26.0+
- 从源码构建时需要 Xcode 26+
- 网络连接

## 连接你的 VNDB 账号

浏览、探索和搜索公开数据不需要登录。读取与编辑资料库需要你自己的 VNDB Token：

1. 打开 VNDB 的 [My Profile → Applications](https://vndb.org/u/tokens) 页面。
2. 创建一个 Token，并授予 `listread` 与 `listwrite` 权限。
3. 在 PaperVN 的用户页面中粘贴 Token。

PaperVN 使用 iOS Keychain 保存 Token。请不要分享 Token；如果意外泄露，请立即前往 VNDB 撤销并重新创建。

## 技术实现

- Swift、SwiftUI、Combine 与 Swift Concurrency
- URLSession、Codable 与 [VNDB Kana API](https://api.vndb.org/kana)
- Keychain、Translation、StoreKit 2、Photos 与 SafariServices
- Swift Testing 与 XCTest
- 无第三方 Swift Package 依赖

## 数据来源与声明

PaperVN 通过 [VNDB Kana API](https://api.vndb.org/kana) 获取视觉小说资料与图片。相关数据遵循 [VNDB Data License](https://vndb.org/d17) 及其 API 使用条款。

PaperVN 是非官方第三方项目，与 [VNDB](https://vndb.org/) 不存在隶属关系，也未获得 VNDB 的官方背书。
