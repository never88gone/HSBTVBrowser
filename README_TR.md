# Tanghulu Tarayıcı

[![TestFlight](https://img.shields.io/badge/TestFlight-Mevcut-blue?logo=apple&logoColor=white)](https://testflight.apple.com/join/QWne6G6V)
[![Platform](https://img.shields.io/badge/Platform-tvOS-lightgrey?logo=apple)](https://developer.apple.com/tvos/)
[![License](https://img.shields.io/badge/Lisans-Kapalı%20Kaynak-red)](https://github.com/never88gone/HSBTVBrowser)
[![Telegram](https://img.shields.io/badge/Telegram-Gruba%20Katıl-blue?logo=telegram)](https://t.me/tanghulutvos)

[简体中文](README_ZH.md) | [English](README.md) | **Türkçe** | [Français](README_FR.md) | [日本語](README_JA.md) | [한국어](README_KO.md) | [Español](README_ES.md)

<p align="center">
  <img alt="Tanghulu" src="screenshot/Logo.png"/>
</p>

## Giriş

Apple TV için bir tarayıcı. Bir süredir Apple TV'de başka bir tarayıcı kullanıyordum, ancak bazı operasyonel sorunlar buldum, bu yüzden kendi deneyimlerime göre bazı optimizasyonlar yaptım.

Apple TV'de TikTok, Douyin, Tencent Video, Youku ve diğer video platformlarını izleyebilirsiniz. Daha fazla web sitesi uyarlanıyor.

Politika nedenlerinden dolayı, bu muhtemelen kapalı kaynak olarak kalacaktır.

> Şimdi Afdian'da (爱发电)

## TestFlight URL

<https://testflight.apple.com/join/QWne6G6V>

## Kullanım Talimatları

1. Daha fazla seçenek içeren gelişmiş bir menüyü görüntülemek için **[Oynat/Duraklat]** düğmesine çift tıklayın
2. Oynatıcıyı tam ekran modunda doğrudan açmak için **[Oynat/Duraklat]** düğmesine uzun basın
3. Videoyu oynatmak/duraklatmak için **[Oynat/Duraklat]** düğmesine tıklayın
4. Geri gitmek veya kök sayfadayken çıkmak için **[Menü]** düğmesine tıklayın
5. Videoyu hızlı ileri/geri sarmak için **[Sol/Sağ]** düğmelerine tıklayın veya dokunmatik alanda sola/sağa kaydırın (ayarlardan etkinleştirilmesi gerekir)
6. Sayfayı kaydırmak veya bazı web sitelerinde önceki/sonraki videoya gitmek için **[Yukarı/Aşağı]** düğmelerine tıklayın
7. İmleç modu / kaydırma modu / dokunma modu / sürükleme modu arasında geçiş yapmak için dokunmatik alana çift tıklayın:
   - **Tıklama Modu**: İmleç sayfada görüntülenir, dokunmatik alana tıklamak sayfa tıklama olaylarını tetikler. iframe kullanan sayfalar için, yeni bir pencerede açmak üzere iframe alanına uzun basabilirsiniz.
   - **Kaydırma Modu**: Dokunmatik alanda yukarı/aşağı kaydırarak veya yukarı/aşağı düğmelerine tıklayarak sayfayı kaydırın
   - **Dokunma Modu**: Dokunmatik alan tıklamaları, tıklamaları uygulamak için mousedown/mouseup kullanır. Tıklama modunda tıklanamayan düğmeler veya CAPTCHA sayfaları için bu modu kullanın. Kaydırma mousemove uygular, belirli öğeleri görüntülemek için fare hareketi gerektiren sayfalar için kullanışlıdır
   - **Sürükleme Modu**: Sürüklemek için bir öğe seçmek üzere dokunmatik alana uzun basın, ardından sürükleyin
8. **Not**: Geçerli web sayfası bir video oynatıyorsa, **[Oynat/Duraklat]** sistem tarafından yakalanır. İlk tıklama videoyu duraklatacak ve uzun basma / çift tıklama işlemleri başka bir eylem gerektirecektir

## Ana Sayfa

Not: Apple'ın incelemesinden kaçınmak için ana sayfa bir saat gösterebilir. Saat görüntülendiğinde, gerçek ana sayfaya erişmek için oynat düğmesine çift tıklayın.

Şu anda sadece bir araç var: ilgili web sayfasına gitmek için bir URL girin.

<p align="center">
  <img alt="Tanghulu Ana Sayfa" src="screenshot/home.png" />
</p>

## Favoriler

Yer işareti eklenmiş sayfalar burada görüntülenecektir.

## Geçmiş

Tarama geçmişi burada görüntülenecektir.

## Ayarlar

Uygulamayla ilgili ayarlar burada görüntülenir.

<p align="center">
  <img alt="Tanghulu Ayarlar" src="screenshot/setting.png" />
</p>

## Tarayıcı

Örnek olarak Douyin'i kullanırsak, ana sayfadan Douyin'e erişebilir ve izleme dörtgenini kullanarak fare konumunu kontrol edebilirsiniz. Gelişmiş seçenekleri açmak için oynat düğmesine çift tıklayın. Önceki/sonraki videoya gitmek için yukarı/aşağı düğmelerini kullanın.

<p align="center">
  <img alt="Tanghulu Tarayıcı" src="screenshot/browser.png" />
</p>

Geçerli sayfa bir video oynatıyorsa, oynatma ilerlemesini görüntülemek ve ayarlamak için sol/sağ düğmelerini kullanabilirsiniz. İlerleme çubuğu sayfanın üstünde görüntülenir.

<p align="center">
  <img alt="Video Oynatma İlerlemesi" src="screenshot/videoplayprocess.png" />
</p>

<p align="center">
  <img alt="CAPTCHA Sürükleme Efekti" src="screenshot/验证码拖动效果.gif" />
</p>

## Özel Özellikler

Gelişmiş özel özellikler uygulamak için yerel JavaScript dosyalarını uygulamaya yükleyebilirsiniz.

### Komut Dosyası Yöneticisi

Komut dosyası yöneticisi aracılığıyla özel JS kod dosyalarını yükleyebilir ve yönetebilirsiniz.

<p align="center">
  <img alt="Komut Dosyası Yöneticisi" src="screenshot/scriptmanager.png" />
</p>

### Web Sitesi Ayarları

Web sitesi ayarlarında, aşağıdaki zamanlarda yürütülmek üzere belirli web siteleri için özel komut dosyaları ayarlayabilirsiniz:

- **Özel Tam Ekran**: Tam ekrana girerken yürüt
- **Tam Ekrandan Çık**: Tam ekrandan çıkarken yürüt
- **Yüklendikten Sonra**: Sayfa yüklemesi tamamlandıktan sonra yürüt

<p align="center">
  <img alt="Web Sitesi Ayarları" src="screenshot/douyinsetting.png" />
</p>

### Özel Düğmeler

Gelişmiş menüde, tıklandığında ilgili JS komut dosyalarını yürüten özel düğmeler ekleyebilirsiniz.

<p align="center">
  <img alt="Özel Düğmeler" src="screenshot/custombtn.gif" />
</p>

### Komut Dosyası Otomatik Yürütme

Otomatik oturum açma, otomatik tıklama ve diğer işlemleri uygulamak için komut dosyaları yazabilirsiniz. Örneğin, Douyin'e otomatik olarak giriş yapmak için bir komut dosyası yazmak.

<p align="center">
  <img alt="Komut Dosyası Otomatik Yürütme" src="screenshot/自动脚本_final.gif" />
</p>

## Bilinen Sorunlar

Kısa vadede çözülemeyen bilinen hatalar:

1. **MSE Video Oynatma Sınırlaması**: iQiyi, Douyin Live, Migu Video vb. platformlarda MSE (Media Source Extensions) kullanan videolar, tvOS sistem kısıtlamaları nedeniyle oynatılamaz ve kısa vadede çözülemez
2. **Iframe İşlem Sınırlaması**: Gömülü iframe'lere sahip bazı sayfalar çalıştırılamayabilir
3. **Oynatma Kontrolü Çatışması**: Sayfada bir video oynatılırken, Oynat/Duraklat düğmesi sistem tarafından yakalanır ve diğer işlevleri kullanmadan önce videoyu duraklatmayı gerektirir

## Önemli Notlar

### Bellek Yetersizliği Sorunları

Sayfa bellek yetersizliği hatası gösteriyorsa, bunun nedenleri ve çözümleri:

**Nedenler:**

1. En son Apple TV'de sadece 4GB bellek vardır ve daha eski modellerde daha az bellek bulunur
2. Apple'ın belleği RAM ve VRAM arasında paylaşılır. Modern TV'lerin 4K olmasıyla VRAM önemli miktarda bellek tüketir
3. tvOS 26'nın akışkan cam efekti çok fazla bellek tüketir
4. Uygulamalar için mevcut gerçek bellek çok sınırlıdır. Tarayıcılar, özellikle masaüstü ortamını simüle ederken bellek yoğundur. Web sayfaları cihazı bir masaüstü olarak algıladığında, bellek kullanımı daha da agresif hale gelir. Bu sorun kısa vadede çözülemez
5. Bu uygulama sistemin tarayıcı motorunu kullanır. Tarayıcı bellek tüketirken diğer uygulamaları zorla kapatmaz. Diğer uygulamalar çok fazla bellek tüketirse, sistem onları kapatır ve bu da manuel kullanıcı müdahalesi gerektirir

**Çözümler:**

1. Diğer arka plan uygulamalarını kapatın
2. Cihazı yeniden başlatın
3. Apple TV için tvOS 26 ayarlarında dinamik cam efektini devre dışı bırakın
4. Daha yeni bir Apple TV modeline yükseltin

## Sürüm Notları

- [releases.md](https://github.com/never88gone/HSBTVBrowser/blob/main/releases.md?plain=1)

## Telegram Grubu

- <https://t.me/tanghulutvos>

<p align="center">
  <img alt="Telegram Grubu" src="screenshot/telegram_icon.png" />
</p>

## Teşekkür

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
