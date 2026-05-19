# Navigateur Tanghulu (Tanghulu Browser)

[![TestFlight](https://img.shields.io/badge/TestFlight-Disponible-blue?logo=apple&logoColor=white)](https://testflight.apple.com/join/QWne6G6V)
[![Platform](https://img.shields.io/badge/Plateforme-tvOS-lightgrey?logo=apple)](https://developer.apple.com/tvos/)
[![License](https://img.shields.io/badge/Licence-Source%20Fermée-red)](https://github.com/never88gone/HSBTVBrowser)
[![Telegram](https://img.shields.io/badge/Telegram-Rejoindre-blue?logo=telegram)](https://t.me/tanghulutvos)

[简体中文](README_ZH.md) | [English](README.md) | [Türkçe](README_TR.md) | **Français** | [日本語](README_JA.md) | [한국어](README_KO.md) | [Español](README_ES.md)

<p align="center">
  <img alt="Tanghulu" src="screenshot/Logo.png"/>
</p>

---

## 🌟 Caractéristiques Clés & Présentation

**Tanghulu Browser** est un **navigateur web et un outil de lecture vidéo complet, profondément optimisé pour l'Apple TV (tvOS)**. Nous avons repensé l'interaction sur grand écran pour offrir une navigation extrêmement fluide et intuitive, entièrement adaptée à la télécommande Apple TV.

* 📺 **Streaming sur Grand Écran** : Regardez facilement des vidéos sur **TikTok, Douyin, Tencent Video, Youku, Bilibili**, et plus encore, directement sur l'Apple TV.
* 🖱️ **Gestes Tactiles Optimisés** : Gère quatre modes de contrôle spéciaux—**Clic, Défilement, Tactile et Déplacement**—pour résoudre les problèmes de précision sur écran TV.
* ⚙️ **Scripts Personnalisés JavaScript** : Intègre un puissant **Gestionnaire de Scripts** permettant d'uploader des fichiers JS pour automatiser des connexions, basculer en plein écran personnalisé, etc.
* 🧭 **Technologies & Innovations Futures** : Nous développons activement la navigation vocale intelligente par IA, la traduction automatique de sous-titres de vidéo en temps réel et la personnalisation de WebKit !

> 💡 **Si ce projet vous a aidé, n'hésitez pas à lui attribuer une étoile 🌟 en haut à droite ! Votre soutien nous encourage énormément à continuer à l'optimiser !**
> 
> 📌 En raison des politiques d'Apple, le projet restera probablement fermé. Rejoignez notre [Groupe Telegram](https://t.me/tanghulutvos) pour tester les versions bêta !


---

## 🗺️ Feuille de Route du Projet (Roadmap)

We are moving fast to expand Tanghulu Browser's boundaries, including deep LLM integrations, on-device AI remote synergy, and next-gen TV experiences. Please read our [**Roadmap / Future Plans**](roadmap.md) to explore what's coming next!

---

## URL TestFlight

<https://testflight.apple.com/join/QWne6G6V>

## Instructions d'Utilisation

1. Double-cliquez sur **[Lecture/Pause]** pour afficher un menu avancé avec plus d'options
2. Appuyez longuement sur **[Lecture/Pause]** pour ouvrir directement le lecteur en mode plein écran
3. Cliquez sur **[Lecture/Pause]** pour contrôler la lecture/pause de la vidéo
4. Cliquez sur le bouton **[Menu]** pour revenir en arrière ou pour quitter la page principale
5. Cliquez sur les boutons **[Gauche/Droite]** pour avancer ou reculer la vidéo, ou balayez vers la gauche/droite sur la zone tactile (doit être activé dans les paramètres)
6. Cliquez sur les boutons **[Haut/Bas]** pour faire défiler la page, ou sur certains sites pour passer à la vidéo précédente/suivante
7. Double-cliquez sur la zone tactile pour basculer entre le mode curseur / mode défilement / mode tactile / mode déplacement :
   - **Mode Clic** : Le curseur est affiché à l'écran, cliquer sur la zone tactile déclenche des événements de clic. Pour les pages utilisant des iframes, vous pouvez appuyer longuement sur la zone iframe pour l'ouvrir dans une nouvelle fenêtre
   - **Mode Défilement** : Faites défiler la page en glissant vers le haut/bas sur la zone tactile ou en cliquant sur les boutons haut/bas
   - **Mode Tactile** : Les clics de la zone tactile utilisent mousedown/mouseup. C'est idéal pour les boutons qui ne peuvent pas être cliqués en mode clic ou pour les pages de CAPTCHA. Le défilement simule un mouvement de souris (mousemove)
   - **Mode Déplacement** : Appuyez longuement sur la zone tactile pour sélectionner un élément, puis glissez pour le déplacer
8. **Remarque** : Si la page web actuelle lit une vidéo, le bouton **[Lecture/Pause]** sera intercepté par le système. Le premier clic mettra la vidéo en pause, un autre essai sera nécessaire pour les autres opérations

## Accueil

Remarque : La page d'accueil pourrait afficher une horloge pour éviter l'examen strict d'Apple. Lorsque l'horloge s'affiche, double-cliquez sur le bouton de lecture pour accéder à la véritable page d'accueil.

Actuellement, il n'y a qu'un seul outil : entrer une URL pour accéder à la page correspondante.

<p align="center">
  <img alt="Tanghulu Accueil" src="screenshot/home.png" />
</p>

## Favoris

Les pages ajoutées en favoris seront affichées ici.

## Historique

L'historique de navigation sera affiché ici.

## Paramètres

Les paramètres liés à l'application sont affichés ici.

<p align="center">
  <img alt="Tanghulu Paramètres" src="screenshot/setting.png" />
</p>

## Navigateur

En prenant l'exemple de Douyin, vous pouvez accéder à Douyin depuis la page d'accueil et contrôler la position de la souris avec le pavé tactile. Double-cliquez sur le bouton de lecture pour ouvrir les options avancées. Utilisez les boutons haut/bas pour passer à la vidéo précédente/suivante.

<p align="center">
  <img alt="Tanghulu Navigateur" src="screenshot/browser.png" />
</p>

Si la page en cours lit une vidéo, vous pouvez utiliser les boutons gauche/droite pour afficher la progression. La barre de progression est affichée en haut de la page.

<p align="center">
  <img alt="Progression de la Vidéo" src="screenshot/videoplayprocess.png" />
</p>

<p align="center">
  <img alt="Effet de Glissement CAPTCHA" src="screenshot/验证码拖动效果.gif" />
</p>

## Fonctionnalités Personnalisées

Vous pouvez uploader des fichiers JavaScript locaux dans l'application pour implémenter des fonctionnalités personnalisées avancées.

### Gestionnaire de Scripts

À l'aide du gestionnaire de scripts, vous pouvez uploader et gérer vos fichiers JS.

<p align="center">
  <img alt="Gestionnaire de Scripts" src="screenshot/scriptmanager.png" />
</p>

### Paramètres de Site

Dans les paramètres de site, vous pouvez définir des scripts pour s'exécuter à des moments précis :

- **Plein écran personnalisé** : S'exécute en entrant en mode plein écran
- **Quitter le plein écran** : S'exécute en quittant le mode plein écran
- **Après le chargement** : S'exécute après la fin du chargement de la page

<p align="center">
  <img alt="Paramètres de Site" src="screenshot/douyinsetting.png" />
</p>

### Boutons Personnalisés

Ajoutez des boutons personnalisés dans le menu avancé, qui exécuteront des scripts JS lorsque cliqués.

<p align="center">
  <img alt="Boutons Personnalisés" src="screenshot/custombtn.gif" />
</p>

### Auto-exécution de Scripts

Rédigez des scripts pour implémenter la connexion automatique ou d'autres automatisations. Par exemple, automatiser la connexion à Douyin.

<p align="center">
  <img alt="Auto-exécution de Scripts" src="screenshot/自动脚本_final.gif" />
</p>

## Problèmes Connus

Bugs connus impossibles à résoudre à court terme :

1. **Limitation de Lecture Vidéo MSE** : Les vidéos utilisant MSE (Media Source Extensions) sur les plateformes comme iQiyi, Douyin Live ne peuvent être lues en raison des restrictions système de tvOS
2. **Limitations des Iframe** : Certaines pages avec des iframes intégrés peuvent ne pas fonctionner
3. **Conflit de Contrôle de Lecture** : Lorsqu'une vidéo est lue, le bouton Lecture/Pause est intercepté par le système et nécessite une pause manuelle avant toute autre action

## Notes Importantes

### Problèmes de Mémoire

Si la page affiche une erreur de mémoire insuffisante, voici les raisons et les solutions :

**Raisons :**

1. L'Apple TV la plus récente ne possède que 4 Go de mémoire.
2. La mémoire est partagée entre la RAM et la VRAM, qui consomme beaucoup pour l'affichage 4K.
3. L'effet visuel en verre de tvOS 26 consomme beaucoup.
4. Les navigateurs sont très gourmands en mémoire, en particulier en version "ordinateur de bureau".
5. L'application ne force pas la fermeture d'autres apps.

**Solutions :**

1. Fermer d'autres applications en arrière-plan
2. Redémarrer l'appareil
3. Désactiver les effets de verre dynamiques dans tvOS 26
4. Migrer vers une Apple TV plus récente

## Notes de Version

- [releases.md](https://github.com/never88gone/HSBTVBrowser/blob/main/releases.md?plain=1)

## Groupe Telegram

- <https://t.me/tanghulutvos>

<p align="center">
  <img alt="Groupe Telegram" src="screenshot/telegram_icon.png" />
</p>

## Remerciements

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
