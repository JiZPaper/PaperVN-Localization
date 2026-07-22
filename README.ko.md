<p align="center">
  <a href="./README.md">English</a> ·
  <a href="./README.zh-Hans.md">简体中文</a> ·
  <a href="./README.zh-Hant.md">繁體中文</a> ·
  <a href="./README.ja.md">日本語</a> ·
  <strong>한국어</strong>
</p>

<p align="center">
  <img src="./docs/images/app-icon.png" width="112" alt="PaperVN 앱 아이콘">
</p>

<h1 align="center">PaperVN</h1>

<p align="center">
  <strong>새로운 이야기를 발견하고, 세세한 정보까지 살펴보며, VNDB 보관함을 늘 최신 상태로 유지하세요.</strong>
</p>

<p align="center">
  비주얼 노벨을 발견하고 플레이 여정을 꼼꼼히 기록할 수 있도록 만든 iPhone 및 iPad용 네이티브 VNDB 클라이언트입니다.
</p>

<p align="center">
  <sub>iPhone &amp; iPad · iOS / iPadOS 26+ · SwiftUI · 5개 언어 지원</sub>
</p>

<p align="center">
  <a href="./docs/images/screenshots/explore.png"><img src="./docs/images/screenshots/explore.png" width="250" alt="PaperVN 탐색 화면"></a>
  <a href="./docs/images/screenshots/search.png"><img src="./docs/images/screenshots/search.png" width="250" alt="PaperVN 검색 화면"></a>
  <a href="./docs/images/screenshots/library.png"><img src="./docs/images/screenshots/library.png" width="250" alt="PaperVN 보관함 화면"></a>
</p>

<p align="center"><sub>탐색 · 검색 · 보관함</sub></p>

## 작품에 담긴 이야기를 더 깊이 살펴보세요

한눈에 보는 개요에서 중요한 세부 정보까지 자연스럽게 이어집니다. 줄거리, 태그, 스크린샷, 출시 정보, 제작사, 제작진, 관련 작품, 외부 링크를 확인할 수 있으며, 캐릭터 페이지에서는 특성, 성우, 등장 작품을 한곳에 모아 보여 줍니다.

<p align="center">
  <a href="./docs/images/screenshots/visual-novel-details.png"><img src="./docs/images/screenshots/visual-novel-details.png" width="360" alt="PaperVN의 비주얼 노벨 상세 정보"></a>
  <a href="./docs/images/screenshots/character-details.png"><img src="./docs/images/screenshots/character-details.png" width="360" alt="PaperVN의 캐릭터 상세 정보"></a>
</p>

<p align="center"><sub>비주얼 노벨 상세 정보 · 캐릭터 상세 정보</sub></p>

## 원하는 방식으로 탐색하세요

비주얼 노벨과 캐릭터를 검색하고 언어, 플랫폼, 분량, 평점, 개발 상태 조건을 조합해 결과를 좁힐 수 있습니다. 검색어 없이 둘러보고 싶을 때는 태그, 특성, 출시 정보, 제작진, 제작사 등 다양한 분류로 탐색할 수 있습니다.

<p align="center">
  <a href="./docs/images/screenshots/tags.png"><img src="./docs/images/screenshots/tags.png" width="360" alt="PaperVN에서 VNDB 태그 탐색"></a>
</p>

<p align="center"><sub>태그 및 카테고리 탐색</sub></p>

## 보관함을 최신 상태로 유지하세요

VNDB 계정을 연결해 보관함을 정리하고 상태, 플레이한 버전, 평점, 시작일과 완료일을 업데이트할 수 있습니다. 언어, 화면 표시, 검색 및 콘텐츠 안전 설정도 언제든 손쉽게 조정할 수 있습니다.

<p align="center">
  <a href="./docs/images/screenshots/edit-library-entry.png"><img src="./docs/images/screenshots/edit-library-entry.png" width="360" alt="PaperVN에서 VNDB 보관함 항목 편집"></a>
  <a href="./docs/images/screenshots/settings.png"><img src="./docs/images/screenshots/settings.png" width="360" alt="PaperVN 사용자 및 설정 화면"></a>
</p>

<p align="center"><sub>보관함 항목 편집 · 나에게 맞게 PaperVN 설정</sub></p>

## 주요 기능

- VNDB 보관함을 바탕으로 기기에서 직접 계산하는 개인 맞춤형 작품 추천.
- 포함/제외 및 하나라도/모두 일치 조건을 조합할 수 있는 복합 검색 필터.
- 선정적이거나 폭력적인 이미지의 표시를 제어하고, 스포일러·평점·설명을 선택적으로 흐리게 표시.
- 중국어(간체), 중국어(번체), 영어, 일본어, 한국어 UI와 제목 언어 설정 및 기기 내 줄거리 번역.
- 스크린샷 미리보기, 확대/축소, 공유 및 사진 앱 저장.

## 요구 사항

- iOS 26.0 이상 또는 iPadOS 26.0 이상
- 소스에서 빌드하려면 Xcode 26 이상
- 인터넷 연결

## VNDB 계정 연결하기

둘러보기와 작품 탐색, 공개 데이터 검색은 로그인 없이 이용할 수 있습니다. 보관함을 읽고 편집하려면 본인의 VNDB 토큰이 필요합니다.

1. VNDB의 [My Profile → Applications](https://vndb.org/u/tokens) 페이지를 엽니다.
2. `listread`와 `listwrite` 권한이 있는 토큰을 생성합니다.
3. PaperVN의 사용자 화면에 토큰을 붙여넣습니다.

PaperVN은 토큰을 iOS 키체인(Keychain)에 저장합니다. 토큰을 다른 사람과 공유하지 마세요. 유출된 경우 VNDB에서 즉시 철회한 뒤 새로 발급받으세요.

## 사용 기술

- Swift, SwiftUI, Combine 및 Swift Concurrency
- URLSession, Codable 및 [VNDB Kana API](https://api.vndb.org/kana)
- Keychain, Translation, StoreKit 2, Photos 및 SafariServices
- Swift Testing 및 XCTest
- 외부 Swift 패키지 의존성 없음

## 데이터 출처 및 고지

PaperVN은 [VNDB Kana API](https://api.vndb.org/kana)를 통해 비주얼 노벨의 메타데이터와 이미지를 가져옵니다. 해당 데이터에는 [VNDB Data License](https://vndb.org/d17)와 API 이용 약관이 적용됩니다.

PaperVN은 비공식 제3자 프로젝트로, [VNDB](https://vndb.org/)와 제휴 관계가 없으며 VNDB가 공식적으로 보증하거나 승인한 프로젝트가 아닙니다.
