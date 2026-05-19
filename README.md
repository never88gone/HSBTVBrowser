# Tanghulu Browser

[![TestFlight](https://img.shields.io/badge/TestFlight-Available-blue?logo=apple&logoColor=white)](https://testflight.apple.com/join/QWne6G6V)
[![Platform](https://img.shields.io/badge/Platform-tvOS-lightgrey?logo=apple)](https://developer.apple.com/tvos/)
[![License](https://img.shields.io/badge/License-Closed%20Source-red)](https://github.com/never88gone/HSBTVBrowser)
[![Telegram](https://img.shields.io/badge/Telegram-Join%20Chat-blue?logo=telegram)](https://t.me/tanghulutvos)

[简体中文](README_ZH.md) | **English** | [Türkçe](README_TR.md) | [Français](README_FR.md) | [日本語](README_JA.md) | [한국어](README_KO.md) | [Español](README_ES.md)

<p align="center">
  <img alt="Tanghulu" src="screenshot/Logo.png"/>
</p>

---

## 🌟 Introduction & Core Highlights

**Tanghulu Browser** is a **fully featured web browser and video playback tool deeply tailored for Apple TV (tvOS)**. We have re-engineered large-screen interaction to deliver an incredibly smooth, intuitive browsing experience customized for the Apple TV remote.

* 📺 **Uncompressed Big-Screen Streaming**: Effortlessly stream videos on **TikTok, Douyin, YouTube, Tencent Video, Bilibili**, and more directly on Apple TV.
* 🖱️ **Optimized Remote Gestures**: Supports four specialized control modes—**Click, Scroll, Touch, and Drag**—to resolve any precision and input challenges on TV browsers.
* ⚙️ **Powerful Custom Scripting**: Built-in **JavaScript Script Manager** allows uploading local JS files to auto-execute tasks like automated logins, customized full-screen adjustments, and much more.
* 🧭 **AI & Future-Proof Technologies**: Actively developing next-generation features, including LLM-driven voice navigation, real-time AI subtitle translations, and custom WebKit runtime optimizations.

> 💡 **If you find this project helpful, please give us a Star 🌟 at the top-right corner to show your support!**
> 
> 📌 Due to Apple ecosystem policy constraints, this repository will likely remain closed-source. Join our [Telegram Group](https://t.me/tanghulutvos) to get beta updates!

---

## 🗺️ Project Roadmap

We are moving fast to expand Tanghulu Browser's boundaries, including deep LLM integrations, on-device AI remote synergy, and next-gen TV experiences. Please read our [**Roadmap / Future Plans**](roadmap.md) to explore what's coming next!

---

## TestFlight URL

<https://testflight.apple.com/join/QWne6G6V>

## Operation Instructions

1. Double-click **[Play/Pause]** to display an advanced menu with more options
2. Long press **[Play/Pause]** to directly open the player in fullscreen mode
3. Click **[Play/Pause]** to control video playback/pause
4. Click **[Menu]** button to go back, or exit when on the root page
5. Click **[Left/Right]** buttons to control video fast-forward/rewind, or swipe left/right on the touch area (needs to be enabled in settings)
6. Click **[Up/Down]** buttons to scroll the page, or on some websites to navigate to previous/next video
7. Double-click the touch area to switch between cursor mode/scroll mode/touch mode/drag mode:
   - **Click Mode**: Cursor is displayed on the page, clicking the touch area triggers page click events. For pages using iframes, you can long press the iframe area to open it in a new window
   - **Scroll Mode**: Scroll the page by swiping up/down on the touch area or clicking up/down buttons
   - **Touch Mode**: Touch area clicks use mousedown/mouseup to implement clicks. Use this mode for buttons that can't be clicked in click mode, or for CAPTCHA pages. Scrolling implements mousemove, useful for pages that require mouse movement to display certain elements
   - **Drag Mode**: Long press the touch area to select an element to drag, then drag it
8. **Note**: If the current webpage is playing a video, **[Play/Pause]** will be intercepted by the system. The first click will pause the video, and long press/double-click operations will require another action

## Home

Note: The home page might display a clock to avoid Apple's review. When the clock is displayed, double-click the play button to access the actual home page.

Currently, there's only one tool: enter a URL to navigate to the corresponding webpage.

<p align="center">
  <img alt="Tanghulu Home" src="screenshot/home.png" />
</p>

## Favorites

Bookmarked pages will be displayed here.

## History

Browsing history will be displayed here.

## Settings

App-related settings are displayed here.

<p align="center">
  <img alt="Tanghulu Settings" src="screenshot/setting.png" />
</p>

## Browser

Using Douyin as an example, you can access Douyin from the home page and control the mouse position using the trackpad. Double-click the play button to bring up advanced options. Use up/down buttons to navigate to previous/next video.

<p align="center">
  <img alt="Tanghulu Browser" src="screenshot/browser.png" />
</p>

If the current page is playing a video, you can use left/right buttons to display the playback progress and adjust it. The progress bar is displayed at the top of the page.

<p align="center">
  <img alt="Video Playback Progress" src="screenshot/videoplayprocess.png" />
</p>

<p align="center">
  <img alt="CAPTCHA Drag Effect" src="screenshot/验证码拖动效果.gif" />
</p>

## Custom Features

You can upload local JavaScript files to the app to implement advanced custom features.

### Script Manager

Through the script manager, you can upload and manage custom JS script files.

<p align="center">
  <img alt="Script Manager" src="screenshot/scriptmanager.png" />
</p>

### Website Settings

In website settings, you can set custom scripts for specific websites to execute at the following times:

- **Custom Fullscreen**: Execute when entering fullscreen
- **Exit Fullscreen**: Execute when exiting fullscreen
- **After Loading**: Execute after page loading is complete

<p align="center">
  <img alt="Website Settings" src="screenshot/douyinsetting.png" />
</p>

### Custom Buttons

In the advanced menu, you can add custom buttons that execute corresponding JS scripts when clicked.

<p align="center">
  <img alt="Custom Buttons" src="screenshot/custombtn.gif" />
</p>

### Script Auto-Execution

You can write scripts to implement automatic login, automatic clicking, and other operations. For example, writing a script to automatically log in to Douyin.

<p align="center">
  <img alt="Script Auto-Execution" src="screenshot/自动脚本_final.gif" />
</p>

## Known Issues

Currently known bugs that cannot be resolved in the short term:

1. **MSE Video Playback Limitation**: Videos using MSE (Media Source Extensions) on platforms like iQiyi, Douyin Live, Migu Video, etc., cannot be played due to tvOS system restrictions and cannot be resolved in the short term
2. **Iframe Operation Limitation**: Some pages with embedded iframes may not be operable
3. **Playback Control Conflict**: When a video is playing on the page, the Play/Pause button is intercepted by the system and requires pausing the video first before using other functions

## Important Notes

### Memory Shortage Issues

If the page displays a memory shortage error, here are the reasons and solutions:

**Reasons:**

1. The latest Apple TV only has 4GB of memory, and older models have even less
2. Apple's memory is shared between RAM and VRAM. With modern TVs being 4K, VRAM consumes a significant amount of memory
3. tvOS 26's fluid glass effect consumes a lot of memory
4. The actual memory available to apps is very limited. Browsers are memory-intensive, especially when simulating a desktop environment. When webpages recognize the device as a desktop, memory usage becomes even more aggressive. This issue cannot be resolved in the short term
5. This app uses the system's browser engine. The browser does not forcefully close other apps when consuming memory. If other apps consume too much memory, the system will close them, which requires manual user intervention

**Solutions:**

1. Close other background applications
2. Restart the device
3. Disable the dynamic glass effect in tvOS 26 settings for Apple TV
4. Upgrade to a newer Apple TV model

## Release Notes

- [releases.md](https://github.com/never88gone/HSBTVBrowser/blob/main/releases.md?plain=1)

## Telegram Group

- <https://t.me/tanghulutvos>

<p align="center">
  <img alt="Telegram Group" src="screenshot/telegram_icon.png" />
</p>

## Acknowledgments

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
