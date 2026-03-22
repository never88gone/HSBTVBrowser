# 탕후루 브라우저 (Tanghulu Browser)

[![TestFlight](https://img.shields.io/badge/TestFlight-이용가능-blue?logo=apple&logoColor=white)](https://testflight.apple.com/join/QWne6G6V)
[![Platform](https://img.shields.io/badge/플랫폼-tvOS-lightgrey?logo=apple)](https://developer.apple.com/tvos/)
[![License](https://img.shields.io/badge/라이선스-클로즈드%20소스-red)](https://github.com/never88gone/HSBTVBrowser)
[![Telegram](https://img.shields.io/badge/Telegram-그룹%20참여-blue?logo=telegram)](https://t.me/tanghulutvos)

[简体中文](README_ZH.md) | [English](README.md) | [Türkçe](README_TR.md) | [Français](README_FR.md) | [日本語](README_JA.md) | **한국어** | [Español](README_ES.md)

<p align="center">
  <img alt="Tanghulu" src="screenshot/Logo.png"/>
</p>

## 소개

Apple TV용 브라우저입니다. 이전부터 Apple TV에서 브라우저를 사용하면서 불편함을 느꼈기 때문에, 제 경험을 기반으로 최적화 작업을 진행했습니다.

Apple TV에서 TikTok, Douyin, Tencent Video, Youku 등의 비디오 플랫폼을 시청할 수 있습니다. 더 많은 웹사이트를 계속 추가 중입니다.

정책상의 이유로, 이 프로젝트는 클로즈드 소스로 유지될 가능성이 높습니다.

> Afdian (爱发电)에서 지원 가능합니다

## TestFlight URL

<https://testflight.apple.com/join/QWne6G6V>

## 조작 방법

1. **[재생/일시정지]** 버튼을 더블 클릭하면 더 많은 옵션이 포함된 고급 메뉴가 표시됩니다
2. **[재생/일시정지]**를 길게 누르면 플레이어를 전체 화면 모드로 직접 엽니다
3. **[재생/일시정지]**를 클릭하여 비디오 재생/일시정지를 제어합니다
4. **[메뉴]** 버튼을 클릭하여 뒤로 가거나, 루트 페이지에 있을 때 종료합니다
5. **[좌/우]** 버튼을 클릭하여 비디오를 빨리 감거나 되감습니다. 또는 터치 영역에서 좌/우로 전환힙니다(설정에서 활성화 필요)
6. **[상/하]** 버튼을 클릭하여 페이지를 스크롤하거나, 일부 웹사이트에서는 이전/다음 비디오로 이동합니다
7. 터치 영역을 더블 클릭하여 커서 모드 / 스크롤 모드 / 터치 모드 / 드래그 모드 간에 전환합니다:
   - **클릭 모드**: 커서가 페이지에 표시되며 터치 영역을 클릭하면 페이지 클릭이 발생합니다. iframe이 있는 페이지에서는 iframe 영역을 길게 눌러 새 창에서 엽니다
   - **스크롤 모드**: 터치 영역에서 위/아래로 스크롤하거나 상/하 버튼을 사용하여 페이지를 스크롤합니다
   - **터치 모드**: 버튼 등 클릭 모드로 누르기 어려운 요소에 사용됩니다 (mousedown / mouseup 지원)
   - **드래그 모드**: 드래그할 요소를 선택하기 위해 터치 공간을 길게 누른 다음 이동시킵니다
8. **참고**: 현재 웹페이지에서 비디오가 재생되고 있다면, 시스템이 **[재생/일시정지]** 버튼을 가로챕니다. 첫 번째 클릭은 비디오를 일시 중지하기만 합니다

## 홈

참고: Apple의 검토를 피하기 위해 홈 페이지 에는 시계가 표시될 수 있습니다. 시계가 표시된 경우 재생 버튼을 더블 클릭해야 실제 홈 페이지에 접근할 수 있습니다.

현재 홈 화면에서는 URL을 입력하여 해당 웹페이지로 이동할 수 있습니다.

<p align="center">
  <img alt="Tanghulu 홈" src="screenshot/home.png" />
</p>

## 즐겨찾기

즐겨찾기에 등록된 페이지가 여기에 표시됩니다.

## 시청기록

인터넷 사용 기록이 여기에 표시됩니다.

## 설정

앱 관련 설정이 여기에 표시됩니다.

<p align="center">
  <img alt="Tanghulu 설정" src="screenshot/setting.png" />
</p>

## 브라우저 기능

Douyin을 예로 들면 홈 페이지를 통해 Douyin에 접속 할 수 있으며 터치 패드를 사용하여 마우스 위치를 제어할 수 있습니다. 재생 버튼을 더블 클릭하여 고급 옵션을 표시합니다.

<p align="center">
  <img alt="Tanghulu 브라우저" src="screenshot/browser.png" />
</p>

비디오 재생 중인 경우 좌우 버튼을 사용해 진행률 막대를 조절 할 수 있습니다.

<p align="center">
  <img alt="Video Playback Progress" src="screenshot/videoplayprocess.png" />
</p>

<p align="center">
  <img alt="CAPTCHA 드래그 효과" src="screenshot/验证码拖动效果.gif" />
</p>

## 사용자 지정 기능

로컬 JavaScript 파일을 앱에 업로드하여, 고급 사용자 지정 기능을 구현할 수 있습니다.

### 스크립트 관리자

스크립트 관리자를 통해, 사용자 지정 JS 스크립트를 관리할 수 있습니다.

<p align="center">
  <img alt="Script Manager" src="screenshot/scriptmanager.png" />
</p>

### 웹사이트 설정

다음 이벤트 실행 타이밍에 사용자 지정 스크립트를 추가 할 수 있습니다:

- **Full Screen 진입 시**: 전체 화면 진입 시
- **Full Screen 종료 시**: 전체 화면 종료 시
- **로딩 완료 후**: 페이지 로딩 완료 후

<p align="center">
  <img alt="Website Settings" src="screenshot/douyinsetting.png" />
</p>

### 사용자 지정 버튼

고급 메뉴에 버튼 클릭 이벤트시 작동하는 JS 스크립트 버튼을 추가 할 수 있습니다.

<p align="center">
  <img alt="Custom Buttons" src="screenshot/custombtn.gif" />
</p>

### 스크립트 자동 실행

자동 로그인 등의 조작을 위한 스크립트를 작성하여 자동화 할 수 있습니다.

<p align="center">
  <img alt="Script Auto-Execution" src="screenshot/自动脚本_final.gif" />
</p>

## 알려진 문제

단기간에 해결할 수 없는 일부 버그가 존재합니다:

1. **MSE 비디오 재생 제한**: iQiyi, Douyin Live 등 MSE (Media Source Extensions) 방식 비디오는 tvOS 제한으로 재생 불가
2. **Iframe 작동 제한**: iframe이 사용된 경우 일부 페이지가 정상 작동하지 않을 수 있음
3. **재생 충돌 버그**: 영상이 재생중일때 재생/일시정지 버튼은 시스템 인터셉트 발생

## 중요 공지사항

### 메모리 부족 현상

페이지에 메모리 부족 현상이 나타날 경우 :

**원인:**

1. 최신 Apple TV 의 메모리도 4GB로 제한됨
2. Apple은 RAM과 VRAM을 공유하므로 4K TV에서는 메모리 소비가 심함
3. tvOS 26 자체 효과가 메모리 소비 원인
4. 웹페이지에서 데스크톱 처럼 브라우저를 인식할때 메모리가 폭발적으로 늘어남
5. 이 앱은 자체 제어를 통해서 타 앱을 종료시키지 않음

**해결책:**

1. 백그라운드 앱을 종료
2. 기기 재시동
3. tvOS 26 설정에서 시각효과 축소
4. 신형 Apple TV 업그레이드 고려

## 릴리즈 노트

- [releases.md](https://github.com/never88gone/HSBTVBrowser/blob/main/releases.md?plain=1)

## Telegram 그룹

- <https://t.me/tanghulutvos>

<p align="center">
  <img alt="Telegram Group" src="screenshot/telegram_icon.png" />
</p>

## 감사한 분들

- [debugly/fsplayer](https://github.com/debugly/fsplayer)
- [ikishorek/TVVLCKit](https://github.com/ikishorek/TVVLCKit)
- [SnapKit/Masonry](https://github.com/SnapKit/Masonry)
- [jsonmodel/jsonmodel](https://github.com/jsonmodel/jsonmodel)
- [CocoaLumberjack/CocoaLumberjack](https://github.com/CocoaLumberjack/CocoaLumberjack)
- [SDWebImage/SDWebImage](https://github.com/SDWebImage/SDWebImage)
- [zattoo/TvOSSlider](https://github.com/zattoo/TvOSSlider)
- [lechium/KBBulletinView](https://github.com/lechium/KBBulletinView)
- [vtourraine/VTAcknowledgementsViewController](https://github.com/vtourraine/VTAcknowledgementsViewController)
- [AliSoftware/Reusable](https://github.com/AliSoftware/Reusable)
- [nicklockwood/GZIP](https://github.com/nicklockwood/GZIP)
- [robbiehanson/CocoaAsyncSocket](https://github.com/robbiehanson/CocoaAsyncSocket)
- [SwiftyJSON/SwiftyJSON](https://github.com/SwiftyJSON/SwiftyJSON)
- [yichengchen/swifter](https://github.com/yichengchen/swifter)
- [mattt/Ono](https://github.com/mattt/Ono)
- [yichengchen/ATV-Bilibili-demo](https://github.com/yichengchen/ATV-Bilibili-demo)
- [steventroughtonsmith/tvOSBrowser](https://github.com/steventroughtonsmith/tvOSBrowser)
