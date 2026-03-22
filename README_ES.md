# Navegador Tanghulu

[![TestFlight](https://img.shields.io/badge/TestFlight-Disponible-blue?logo=apple&logoColor=white)](https://testflight.apple.com/join/QWne6G6V)
[![Platform](https://img.shields.io/badge/Plataforma-tvOS-lightgrey?logo=apple)](https://developer.apple.com/tvos/)
[![License](https://img.shields.io/badge/Licencia-Código%20Cerrado-red)](https://github.com/never88gone/HSBTVBrowser)
[![Telegram](https://img.shields.io/badge/Telegram-Unirse-blue?logo=telegram)](https://t.me/tanghulutvos)

[简体中文](README_ZH.md) | [English](README.md) | [Türkçe](README_TR.md) | [Français](README_FR.md) | [日本語](README_JA.md) | [한국어](README_KO.md) | **Español**

<p align="center">
  <img alt="Tanghulu" src="screenshot/Logo.png"/>
</p>

## Introducción

Un navegador para Apple TV. Llevaba tiempo usando un navegador en Apple TV pero encontré bastantes problemas operativos, así que hice algunas optimizaciones basadas en mi experiencia.

Puedes ver TikTok, Douyin, Tencent Video, Youku y otras plataformas de video en Apple TV. Se están adaptando más sitios web en el futuro.

Por razones políticas, este proyecto probablemente seguirá siendo de código cerrado.

> Ahora en Afdian (爱发电)

## URL de TestFlight

<https://testflight.apple.com/join/QWne6G6V>

## Instrucciones de Uso

1. Haz doble clic en **[Reproducir/Pausar]** para mostrar un menú avanzado con más opciones
2. Mantén presionado **[Reproducir/Pausar]** para abrir el reproductor en pantalla completa directamente
3. Haz clic en **[Reproducir/Pausar]** para reproducir o pausar el video
4. Haz clic en **[Menú]** para regresar, o salir si estás en la página principal
5. Haz clic en los botones **[Izquierda/Derecha]** para avanzar/retroceder, o desliza hacia la izquierda/derecha (debe activarse en configuración)
6. Haz clic en los botones **[Arriba/Abajo]** para desplazarte, o en algunas webs para ir al video anterior/siguiente
7. Haz doble clic en el área táctil para cambiar entre el Modo de Cursor / Modo de Desplazamiento / Modo Táctil / Modo de Arrastre:
   - **Modo de Clic**: Se muestra el cursor y puedes hacer clic. Para las páginas con iframes, puedes mantener el botón presionado en el iframe para abrirlo en otra ventana
   - **Modo de Desplazamiento**: Desplázate hacia arriba o abajo en la página
   - **Modo Táctil**: Excelente para botones donde el cursor no funciona bien
   - **Modo de Arrastre**: Mantén pulsado para arrastrar los elementos deseados
8. **Nota**: Durante la reproducción, el sistema toma control del botón de Reproducir/Pausar. El primer clic solo congelará la reproducción

## Inicio

Nota: La página de inicio podría mostrar un reloj en pantalla para evitar las duras políticas de revisión de Apple. Puedes hacer doble clic en el botón de reproducción en ese momento para acceder al inicio.

Actualmente sirve como una herramienta simple: inserta el link de la URL que quieres abrir.

<p align="center">
  <img alt="Tanghulu Inicio" src="screenshot/home.png" />
</p>

## Favoritos

Las páginas marcadas se mostrarán aquí.

## Historial

Tu historial saldrá aquí.

## Configuración

Configuraciones sobre la aplicación se muestran aquí.

<p align="center">
  <img alt="Tanghulu Configuración" src="screenshot/setting.png" />
</p>

## Navegador

Tomando a Douyin por ejemplo, puedes acceder a él de forma remota para controlar y usar la app.

<p align="center">
  <img alt="Tanghulu Navegador" src="screenshot/browser.png" />
</p>

La posición y la reproducción se pueden visualizar muy cómodamente a través de los atajos y botones.

<p align="center">
  <img alt="Video Playback Progress" src="screenshot/videoplayprocess.png" />
</p>

<p align="center">
  <img alt="Efecto CAptcha" src="screenshot/验证码拖动效果.gif" />
</p>

## Características Personalizadas

Puedes subir archivos de JS para conseguir personalización avanzada.

### Gestor de Scripts

Mediante la herramienta nativa, gestionas código de JS.

<p align="center">
  <img alt="Script Manager" src="screenshot/scriptmanager.png" />
</p>

### Configuración de Sitios Web

Puedes asignar configuraciones únicas según cada sitio web que visites:

- **Pantalla Completa Personalizada**
- **Salir Pantalla Completa**
- **Después de Cargar**

<p align="center">
  <img alt="Website Settings" src="screenshot/douyinsetting.png" />
</p>

### Botones Personalizados

Añade los botones y opciones extras sobre la interfaz para lanzar eventos rápidos de JS.

<p align="center">
  <img alt="Custom Buttons" src="screenshot/custombtn.gif" />
</p>

### Auto-Ejecución de Scripts

Para cosas como auto-logins y rutinas pesadas, automatízalo de una sola vez.

<p align="center">
  <img alt="Script Auto-Execution" src="screenshot/自动脚本_final.gif" />
</p>

## Problemas Conocidos

1. **Limitaciones MSE Video**: Fallará en algunos de ellos al estar limitados por tvOS
2. **Iframe**: Las interfaces dentro del embed podrían tener fallos aleatorios
3. **Conflictos Reproducción**: El control principal intercepta esto

## Notas Importantes

### Sobre la Escasez de Memoria

Fallos con problemas de RAM se deben a la limitación principal de los dispositivos y el renderizado 4K del software que abusan demasiado del cache del motor del browser de desktop. Para solventarlos mantén limpia las apps de detrás o usa los efectos gráficos más simples del sistema operativo tvOS 26.

## Registro de Cambios

- [releases.md](https://github.com/never88gone/HSBTVBrowser/blob/main/releases.md?plain=1)

## Grupo de Telegram

- <https://t.me/tanghulutvos>

<p align="center">
  <img alt="Telegram Group" src="screenshot/telegram_icon.png" />
</p>

## Agradecimientos

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
