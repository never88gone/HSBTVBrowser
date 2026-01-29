# 糖葫芦浏览器

**简体中文** | [English](README.md)

<p align="center">
  <img alt="糖葫芦" src="screenshot/Logo.png"/>
</p>

## 简介

Apple TV 上使用的浏览器。目前自己一直在用 Apple TV 上使用起飞了浏览器，但是发现有些操作存在一些问题，自己参考后做了一些操作上的优化。

可以在 Apple TV 上观看 TikTok、抖音、腾讯视频、优酷等视频平台，更多网站正在适配中。

因为政策的原因，这个估计只能闭源。

> 入驻了爱发电

## TestFlight 地址

https://testflight.apple.com/join/QWne6G6V

## 操作说明

1. 双击【播放/暂停】可显示包含更多选项的高级菜单
2. 长按【播放/暂停】可以直接打开播放器全屏播放视频
3. 点击【播放/暂停】可以控制视频的播放暂停
4. 点击【菜单】按钮可返回，或在根页面上退出
5. 点击【左/右】按钮可以控制视频的快进，向左向右滑动触控区域可以控制视频的快进（需要到设置中打开）
6. 点击【上/下】按钮可以控制页面往下滚动，部分网页可以控制视频的上翻/下翻操作
7. 双击触摸区域，可以实现光标模式/滚动模式/触摸模式/拖动模式的切换：
   - **点击模式**：光标显示在页面上，点击触摸区域后实现页面的点击事件，部分页面采用的是 iframe 内嵌页面，可以长按 iframe 区域，新开窗口打开 iframe
   - **滚动模式**：通过触摸区域的上下滑动，点击上下按钮，实现页面的滚动
   - **触摸模式**：触摸区域点击使用 mousedown、mouseend 实现点击，页面上的按钮需要使用点击模式点不中，有些验证码页面可以尝试使用，滚动实现 mousemove，有些需要滑动鼠标才能显示的页面可以尝试使用
   - **拖动模式**：长按触摸区域选择需要拖动的元素，实现元素的拖动
8. 注意：如果当前网页正在播放视频，【播放/暂停】会被系统拦截，点击第一下会暂停视频，长按、双击操作都需要再次操作

## 首页

这里需要注意，首页有可能是个时钟，是为了避免 Apple 审核。当首页显示时钟的时候需要双击播放按钮，就会出现当前首页。

目前只有一个工具，输入 URL，会跳转到对应的网页上。

<p align="center">
  <img alt="糖葫芦首页" src="screenshot/home.png" />
</p>

## 收藏

收藏的页面会显示到这里。

## 历史

浏览历史记录会显示到这里。

## 设置

App 的相关设置会显示在这里。

<p align="center">
  <img alt="糖葫芦设置" src="screenshot/setting.png" />
</p>

## 浏览器

以抖音为例子，首页进入抖音，可以通过触摸板控制鼠标位置，双击播放按钮，可以弹出高级选项，上下按钮可以上一个、下一个视频。

<p align="center">
  <img alt="糖葫芦浏览器" src="screenshot/browser.png" />
</p>

如果当前页面正在播放视频，可以通过左右按键显示播放进度，并且可以调整进度，进度栏显示在页面的顶部。

<p align="center">
  <img alt="视频播放进度" src="screenshot/videoplayprocess.png" />
</p>

<p align="center">
  <img alt="验证码拖动效果" src="screenshot/验证码拖动效果.gif" />
</p>

## 自定义玩法

可以将本地上传的 JavaScript 文件上传到 App 中，实现高级自定义功能。

### 脚本管理器

通过脚本管理器，可以上传和管理自定义 JS 脚本文件。

<p align="center">
  <img alt="脚本管理器" src="screenshot/scriptmanager.png" />
</p>

### 网站设置

在网站设置中，可以为特定网站设置自定义脚本，设置在以下时机执行：

- **自定义全屏**：进入全屏时执行
- **退出全屏**：退出全屏时执行
- **加载完成后**：页面加载完成后执行

<p align="center">
  <img alt="网站设置" src="screenshot/douyinsetting.png" />
</p>

### 自定义按钮

在高级菜单中，可以添加自定义按钮，点击按钮即可执行对应的 JS 脚本。

<p align="center">
  <img alt="自定义按钮" src="screenshot/custombtn.gif" />
</p>

## 已知问题

目前已知短期无法解决的 Bug：

1. **MSE 视频播放限制**：爱奇艺、抖音直播、咪咕视频等使用 MSE（Media Source Extensions）播放的视频，由于 tvOS 系统限制，目前无法播放，短期内难以解决
2. **Iframe 操作限制**：部分使用 iframe 内嵌的页面可能无法正常操作
3. **播放控制冲突**：当页面正在播放视频时，Play/Pause 按键会被系统拦截，需要先暂停视频才能使用其他功能

## 注意事项

### 内存不足问题

如果页面显示内存不足，以下是原因与解决办法：

**原因：**

1. 最新款的 Apple TV 只有 4GB 内存，旧款的内存更少
2. Apple 的内存是内存与显存共用的，现在电视都是 4K 分辨率，显存占用了大量内存
3. tvOS 26 的液态玻璃效果非常占用内存
4. 实际 App 能用的内存很有限，浏览器又是个吃内存的大户，特别是模拟成电脑时，网页端识别为电脑端后，内存使用更激进。所以这个问题目前暂时无法解决
5. 当前 App 使用的是系统的浏览器内核，浏览器占用内存时并不会强制关闭其他应用。如果其他应用占用内存过多，系统会主动关闭其他应用，这需要用户手动操作

**解决办法：**

1. 关闭后台其他应用
2. 重启设备
3. 在 tvOS 26 的设置中关闭 Apple TV 的动态玻璃效果
4. 升级到新款 Apple TV

## 更新日志

- [releases.md](https://github.com/never88gone/HSBTVBrowser/blob/main/releases.md?plain=1)

## Telegram 群组

- [https://t.me/tanghulutvos](https://t.me/tanghulutvos)

<p align="center">
  <img alt="Telegram 群组" src="screenshot/telegram_icon.png" />
</p>

## 致谢

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
