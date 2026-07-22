<p align="center">
  <strong>English</strong> ·
  <a href="./README.zh-Hans.md">简体中文</a> ·
  <a href="./README.zh-Hant.md">繁體中文</a> ·
  <a href="./README.ja.md">日本語</a> ·
  <a href="./README.ko.md">한국어</a>
</p>

<p align="center">
  <img src="./docs/images/app-icon.png" width="112" alt="PaperVN app icon">
</p>

<h1 align="center">PaperVN</h1>

<p align="center">
  <strong>Discover stories. Understand every detail. Keep your VNDB library in sync.</strong>
</p>

<p align="center">
  A native VNDB client for iPhone and iPad, built for discovering visual novels and keeping track of every journey.
</p>

<p align="center">
  <sub>iPhone &amp; iPad · iOS / iPadOS 26+ · SwiftUI · 5 interface languages</sub>
</p>

<p align="center">
  <a href="./docs/images/screenshots/explore.png"><img src="./docs/images/screenshots/explore.png" width="250" alt="PaperVN Explore screen"></a>
  <a href="./docs/images/screenshots/search.png"><img src="./docs/images/screenshots/search.png" width="250" alt="PaperVN Search screen"></a>
  <a href="./docs/images/screenshots/library.png"><img src="./docs/images/screenshots/library.png" width="250" alt="PaperVN Library screen"></a>
</p>

<p align="center"><sub>Explore · Search · Library</sub></p>

## See the story behind every title

Move naturally from a quick overview to the details that matter: synopsis, tags, screenshots, releases, producers, staff, related titles, and external links. Character pages bring traits, voice actors, and appearances together in one place.

<p align="center">
  <a href="./docs/images/screenshots/visual-novel-details.png"><img src="./docs/images/screenshots/visual-novel-details.png" width="360" alt="Visual novel details in PaperVN"></a>
  <a href="./docs/images/screenshots/character-details.png"><img src="./docs/images/screenshots/character-details.png" width="360" alt="Character details in PaperVN"></a>
</p>

<p align="center"><sub>Visual novel details · Character details</sub></p>

## Browse on your terms

Search visual novels and characters, then combine language, platform, length, rating, and development-status filters. Browse by tags, traits, releases, staff, producers, and more when you want to explore without a query in mind.

<p align="center">
  <a href="./docs/images/screenshots/tags.png"><img src="./docs/images/screenshots/tags.png" width="360" alt="Browse VNDB tags in PaperVN"></a>
</p>

<p align="center"><sub>Tags and category browsing</sub></p>

## Keep your library current

Connect your VNDB account to organize your library and update status, played release, rating, and start or finish dates. Language, appearance, search, and content-safety preferences stay close at hand.

<p align="center">
  <a href="./docs/images/screenshots/edit-library-entry.png"><img src="./docs/images/screenshots/edit-library-entry.png" width="360" alt="Edit a VNDB library entry in PaperVN"></a>
  <a href="./docs/images/screenshots/settings.png"><img src="./docs/images/screenshots/settings.png" width="360" alt="PaperVN user and settings screen"></a>
</p>

<p align="center"><sub>Edit a library entry · Make PaperVN yours</sub></p>

## Highlights

- Personalized discovery based on your VNDB library, calculated locally on device.
- Compound search filters with include, exclude, any, and all matching modes.
- Controls for sexual or violent imagery, plus optional blurring for spoilers, ratings, and descriptions.
- Simplified Chinese, Traditional Chinese, English, Japanese, and Korean interfaces, with title-language preferences and on-device synopsis translation.
- Screenshot preview, zoom, sharing, and saving to Photos.

## Requirements

- iOS 26.0+ or iPadOS 26.0+
- An internet connection

## Connect your VNDB account

Browsing, discovery, and public-data search work without signing in. Reading and editing your library requires your own VNDB Token:

1. Open VNDB's [My Profile → Applications](https://vndb.org/u/tokens) page.
2. Create a Token with the `listread` and `listwrite` permissions.
3. Paste it into the User screen in PaperVN.

PaperVN stores the Token in the iOS Keychain. Never share it; revoke and replace it from VNDB immediately if it is exposed.

## Built with

- Swift, SwiftUI, Combine, and Swift Concurrency
- URLSession, Codable, and the [VNDB Kana API](https://api.vndb.org/kana)
- Keychain, Translation, StoreKit 2, Photos, and SafariServices
- Swift Testing and XCTest
- No third-party Swift package dependencies

## Data source and disclaimer

PaperVN retrieves visual-novel metadata and images through the [VNDB Kana API](https://api.vndb.org/kana). The data is subject to the [VNDB Data License](https://vndb.org/d17) and the API usage terms.

PaperVN is an unofficial third-party project. It is not affiliated with or endorsed by [VNDB](https://vndb.org/).
