---
title: How to Use Multiline Comments in Lua with EmEditor Text Editor
date: 2025-02-02T19:38:23.129Z
updated: 2025-02-09T03:22:17.068Z
tags:
  - product
categories:
  - emeditor
thumbnail: https://thmb.techidaily.com/410d74b9604f670385408a643dcb6acbafd048141ccf91d45ea026a8c7847004.jpg
---

## How to Use Multiline Comments in Lua with EmEditor Text Editor

Viewing 3 posts - 1 through 3 (of 3 total)

* Author  
Posts
* May 11, 2010 at 1:28 pm [#8445](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/3b865294c7b9edf6a1955ec9513cdacb?s=80&d=identicon&r=g)MattG](https://www.emeditor.com/forums/users/MattG/ "View MattG's profile")  
Participant  
Hi!  
 I am in the evaluation of EmEditor, and it is definitive my Favorite at the moment.  
 One thing I am not getting to work, I imported a ESY-Lua from the Library, checked the Highlight(2) -> Comments  
 Begin: –\[\[
 End: \]\]  
 So if I open my lua-file and check if Tools->Select Configuration my Lua-config is active, I still get no multiline highlight for that comment-block only the first line.  
 I compared this with a simple C-File  
 /\*  
 foo  
 foo foo  
 \*/  
 is correctly highlighted and the Config is the same.  
 any clues, or is it a Bug of the 9.13, which is the Eval-Version  
 Cheers  
 Matthias  
May 11, 2010 at 4:24 pm [#8446](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/a0a6377144ed3636f985d87303f65ed2?s=80&d=identicon&r=g)Yutaka Emura](https://www.emeditor.com/forums/users/yemura/ "View Yutaka Emura's profile")  
Keymaster  
Hello Matthias,  
 Thank you for trying EmEditor Professional!  
 I reproduced your issue, and the problem was the Line Comment (–) has more priority than multiline comment (–\[\[…\]\]). If you remove the string (–) from Line Comment text box in the Highlight (2) tab of configuration properties, it works. I am not sure if I can correct this behavior at this moment.  
 If you want both types of comments highlighted, instead of specifying — in the Highlight (2) tab, you can add — in the Highlight (1) tab, check “Highlight Right Side”, and select your favorite color (1 – 10). You will also need to remove the already defined keyword (-) from the list.  
 I hope this helps.  
 Please don’t hesitate to ask me if you have further questions.  
 Thank you,  
May 12, 2010 at 11:13 am [#8448](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/3b865294c7b9edf6a1955ec9513cdacb?s=80&d=identicon&r=g)MattG](https://www.emeditor.com/forums/users/MattG/ "View MattG's profile")  
Participant  
Hi!  
 Nice Idea!  
 Yes it helps, I understand its a bit difficult with that  
 –\[\[….\]\]  
 and — stuff.  
 Hehe… still my favorite editor  
 Cheers  
 Matthias
* Author  
Posts

Viewing 3 posts - 1 through 3 (of 3 total)

* You must be logged in to reply to this topic.

<ins class="adsbygoogle"
     style="display:block"
     data-ad-format="autorelaxed"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="1223367746"></ins>

<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="8358498916"
     data-ad-format="auto"
     data-full-width-responsive="true"></ins>

<span class="atpl-alsoreadstyle">Also read:</span>
<div><ul>
<li><a href="https://desktop-recording.techidaily.com/new-screencasting-guide-what-is-and-how-to/"><u>[New] Screencasting Guide What Is and How To</u></a></li>
<li><a href="https://win-web3.techidaily.com/1728508774813-windows-11-23h2/"><u>未经支持的硬件上运行 Windows 11 23H2版本 - 安装指南 | 多项途径解析</u></a></li>
<li><a href="https://win-help.techidaily.com/6windows-pc/"><u>重建歷史：用6種不同技術自Windows PC中恢復網頁存查記錄</u></a></li>
<li><a href="https://solve-latest.techidaily.com/1724313404874-cookiebot-enabled-enhance-your-sites-analytics-and-conversions/"><u>Cookiebot-Enabled: Enhance Your Site's Analytics & Conversions</u></a></li>
<li><a href="https://win-web3.techidaily.com/effortless-guide-moving-your-garageband-ringtones-onto-your-iphone/"><u>Effortless Guide: Moving Your GarageBand Ringtones Onto Your iPhone</u></a></li>
<li><a href="https://ios-unlock.techidaily.com/how-to-change-your-apple-id-password-on-your-apple-iphone-11-pro-max-by-drfone-ios/"><u>How To Change Your Apple ID Password On your Apple iPhone 11 Pro Max</u></a></li>
<li><a href="https://change-location.techidaily.com/how-to-fix-android-app-not-installed-error-on-google-pixel-8-quickly-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>How to Fix Android App Not Installed Error on Google Pixel 8 Quickly? | Dr.fone</u></a></li>
<li><a href="https://buynow-marvelous.techidaily.com/innovative-auto-encryption-unravelers-2024-outlook/"><u>Innovative Auto Encryption Unravelers, 2024 Outlook</u></a></li>
<li><a href="https://win-web3.techidaily.com/recuperacion-de-archivos-desde-la-nube-una-guia-rapida-y-sencilla/"><u>Recuperación De Archivos Desde La Nube: Una Guía Rápida Y Sencilla</u></a></li>
<li><a href="https://fox-place.techidaily.com/smart-techniques-for-extracting-video-content-from-telegram-channels/"><u>Smart Techniques for Extracting Video Content From Telegram Channels</u></a></li>
<li><a href="https://win-web3.techidaily.com/step-by-step-guide-to-cloning-your-hdd-to-an-m2-ssd-seamlessly/"><u>Step-by-Step Guide to Cloning Your HDD to an M.2 SSD Seamlessly</u></a></li>
<li><a href="https://win-web3.techidaily.com/step-by-step-guide-recovering-information-from-a-non-bootable-laptops-hard-drive/"><u>Step-by-Step Guide: Recovering Information From a Non-Bootable Laptop's Hard Drive</u></a></li>
<li><a href="https://win-web3.techidaily.com/stop-your-downloads-from-disappearing-on-windows-11-with-these-4-effective-fixes/"><u>Stop Your Downloads From Disappearing on Windows 11 with These 4 Effective Fixes!</u></a></li>
<li><a href="https://solve-luxury.techidaily.com/top-5-free-mp3-editors-for-windows-11-users-effortless-audio-trimming/"><u>Top 5 Free MP3 Editors for Windows 11 Users: Effortless Audio Trimming</u></a></li>
<li><a href="https://fox-zaraz.techidaily.com/wiedergewonnene-kontrolle-uber-ihr-eclipse-entwicklungsprojekt-wiederherstellung-geloschter-projekte-mit-vier-praktischen-methoden/"><u>Wiedergewonnene Kontrolle Über Ihr ECLIPSE-Entwicklungsprojekt: Wiederherstellung Gelöschter Projekte Mit Vier Praktischen Methoden</u></a></li>
<li><a href="https://win-web3.techidaily.com/wiedergutmachung-bei-fehlender-wiederherstellungsumgebung-auf-dem-pc-mit-windows-11-tipps-and-tricks/"><u>Wiedergutmachung Bei Fehlender Wiederherstellungsumgebung Auf Dem PC Mit Windows 11 - Tipps & Tricks</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/97ydpSmzTJw?si=tFcelmtQX4u-b3u5" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

