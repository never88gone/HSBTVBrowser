# 糖葫芦浏览器

<p align="center">
  <img alt="糖葫芦" src="screenshot/Logo.png"/>
</p>
appletv的上使用的浏览器   
目前自己一直在用appletv 上使用起飞了浏览器，但是发现有些操作存在一些问题，自己参考后做了一些操作上的优化。
因为政策的原因，这个估计只能闭源。</p>
testflight地址 
-  [https://testflight.apple.com/join/QWne6G6V](https://testflight.apple.com/join/QWne6G6V)
<br>

部分操作说明<br>
1:双击【播放/暂停】可显示包含更多选项的高级菜单<br>
2:长按【播放/暂停】可以直接打开播放器屏播放视频<br>
3:点击【播放/暂停】可以控制视频的播放暂停<br>
4:点击【菜单】按钮可返回，或在根页面上退出<br>
5:点击【左/右】按钮可以控制视频的快进<br>
6:点击【上/下】按钮可以控制页面往下滚动，部分网页可以控制视频的上翻/下翻操作<br>
7:双击触摸区域，可以实现光标模式/滚动模式/触摸模式的切换</p>
【光标模式】光标显示在页面上，点击触摸区域后 实现页面的点击事件<br>
【滚动模式】通过触摸区域的上下滑动，实现页面的滚动<br>
【触摸模式】触摸区域点击后实现mousedown，滚动实现mousemove，抬起后实现mouseend，有些验证码页面可用，部分页面【光标模式】的点击无效时候可以使用。<br>

# 首页
这里需要注意，首页有可能是个时钟，是为了避免apple审核，当时首页显示时钟的时候需要双击播放按钮，就会出现当前首页
目前只有一个工具，输入url，会跳转到对应的网页上
<p align="center">
  <img alt="糖葫芦" src="screenshot/home.png" />
</p>
# 收藏
收藏的页面会显示到这里
# 历史
浏览历史记录会显示到这里
# 设置
app的相关设置会显示在这里
<p align="center">
  <img alt="糖葫芦" src="screenshot/setting.gif" />
</p>
# 浏览器
以抖音为例子,首页进入抖音，可以通过触摸板控制鼠标位置，双击播放按钮，可以弹出高级选项，上下按钮可以上一个、下一个视频。
<p align="center">
  <img alt="糖葫芦" src="screenshot/browser.gif" />
</p>
如果当前页面正在播放视频，可以通过左右按键显示播放进度，并且可以调整进度，进度栏显示在页面的顶部。
<p align="center">
  <img alt="糖葫芦" src="screenshot/videoplayprocess.png" />
</p>
# releases
-  [releases.md](https://github.com/never88gone/HSBTVBrowser/blob/main/releases.md?plain=1)

### Telegram Group
-  [https://t.me/tanghulutvos](https://t.me/tanghulutvos)
### Links

- [debugly/fsplayer](https://github.com/debugly/fsplayer)
- [ikishorek/TVVLCKit](https://github.com/ikishorek/TVVLCKit)
- [SnapKit/Masonry](https://github.com/SnapKit/Masonry)
- [jsonmodel/jsonmodel](https://github.com/jsonmodel/jsonmodel)
- [CocoaLumberjack/CocoaLumberjack](https://github.com/CocoaLumberjack/CocoaLumberjack)
- [SDWebImage/SDWebImage](https://github.com/SDWebImage/SDWebImage)
- [zattoo/TvOSSlider](https://github.com/zattoo/TvOSSlider)
-  [lechium/KBBulletinView](https://github.com/lechium/KBBulletinView)
-  [zattoo/TvOSSlider](https://github.com/zattoo/TvOSSlider)
-  [vtourraine/VTAcknowledgementsViewController](https://github.com/vtourraine/VTAcknowledgementsViewController)
-  [AliSoftware/Reusable](https://github.com/AliSoftware/Reusable)
-  [nicklockwood/GZIP](https://github.com/nicklockwood/GZIP)
-  [AliSoftware/Reusable](https://github.com/AliSoftware/Reusable)
-  [robbiehanson/CocoaAsyncSocket](https://github.com/robbiehanson/CocoaAsyncSocket)
-  [SwiftyJSON/SwiftyJSON](https://github.com/SwiftyJSON/SwiftyJSON)
-  [yichengchen/swifter](https://github.com/yichengchen/swifter)
-  [mattt/Ono](https://github.com/mattt/Ono)
-  [yichengchen/ATV-Bilibili-demo](https://github.com/yichengchen/ATV-Bilibili-demo)
-  [steventroughtonsmith/tvOSBrowser](https://github.com/steventroughtonsmith/tvOSBrowser)
