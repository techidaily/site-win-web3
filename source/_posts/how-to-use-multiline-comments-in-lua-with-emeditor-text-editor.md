---
title: How to Use Multiline Comments in Lua with EmEditor Text Editor
date: 2024-11-01T22:28:03.429Z
updated: 2024-11-03T18:39:41.191Z
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
<li><a href="https://article-tips.techidaily.com/new-leading-the-way-in-high-res-display-technology-for-2024/"><u>[New] Leading the Way in High-Res Display Technology for 2024</u></a></li>
<li><a href="https://remote-screen-capture.techidaily.com/updated-2024-approved-in-depth-look-apowersofts-pc-screenshare-technology/"><u>[Updated] 2024 Approved In-Depth Look Apowersoft's PC Screenshare Technology</u></a></li>
<li><a href="https://facebook-video-footage.techidaily.com/updated-the-ultimate-guide-to-quieter-youtube-videos/"><u>[Updated] The Ultimate Guide to Quieter YouTube Videos</u></a></li>
<li><a href="https://howto.techidaily.com/7-fixes-for-unfortunately-phone-has-stopped-on-honor-90-lite-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>7 Fixes for Unfortunately, Phone Has Stopped on Honor 90 Lite | Dr.fone</u></a></li>
<li><a href="https://win-web3.techidaily.com/iumsiowvueacjewkoeapkosplusmpluswvhjrmlbdmja7kuk3lv4pnoazku7blpifku73op6plhrpmlrnmoygi/"><u>针对服务提供商:数据中心硬件备份解决方案</u></a></li>
<li><a href="https://win-web3.techidaily.com/automatisches-erstellen-von-windows-backups-mit-truenas-eine-einfache-anleitung/"><u>Automatisches Erstellen Von Windows-Backups Mit TrueNAS: Eine Einfache Anleitung</u></a></li>
<li><a href="https://win-web3.techidaily.com/comment-installer-de-virtualbox-pour-windows-10-and-11-facile-a-configurer/"><u>Comment Installer De VirtualBox Pour Windows 10 & 11 - Facile À Configurer</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/dive-deep-into-stardews-heart-with-our-guide-to-ginger-isle-for-2024/"><u>Dive Deep Into Stardew's Heart with Our Guide to Ginger Isle for 2024</u></a></li>
<li><a href="https://win-web3.techidaily.com/exportieren-von-bildern-sicherung-mit-externer-sd-karte-unter-windows-10-erklart/"><u>Exportieren Von Bildern: Sicherung Mit Externer SD-Karte Unter Windows 10 Erklärt</u></a></li>
<li><a href="https://win-answers.techidaily.com/high-performance-video-quality-deciding-between-30-fps-and-60-fps-recording/"><u>High-Performance Video Quality: Deciding Between 30 FPS and 60 FPS Recording</u></a></li>
<li><a href="https://blog-min.techidaily.com/how-to-transfer-contacts-from-realme-c67-4g-to-outlook-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>How to Transfer Contacts from Realme C67 4G to Outlook | Dr.fone</u></a></li>
<li><a href="https://win-web3.techidaily.com/resolving-teracopy-failures-in-windows-11-expert-solutions-and-tips/"><u>Resolving 'Teracopy Failures' In Windows 11 - Expert Solutions and Tips</u></a></li>
<li><a href="https://win-web3.techidaily.com/schliessen-sie-ihren-windows-11-defender-endlich-richtig-befreit-sich-jetzt/"><u>Schließen Sie Ihren Windows 11 Defender Endlich Richtig - Befreit Sich Jetzt</u></a></li>
<li><a href="https://win-web3.techidaily.com/schritt-fur-schritt-anleitung-fur-das-upgrade-auf-einen-samsung-serie-eins-nvme-ssd-np900x4c/"><u>Schritt-Für-Schritt-Anleitung Für Das Upgrade Auf Einen Samsung Serie Eins NVMe SSD (NP900x4C)</u></a></li>
<li><a href="https://extra-information.techidaily.com/the-allure-of-benq-sw320-4k-pro-display/"><u>The Allure of BenQ SW320 4K Pro Display</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://laganoo.pxf.io/c/5597632/1657396/16446" target="_top" id="1657396">
  <img src="//a.impactradius-go.com/display-ad/16446-1657396" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://laganoo.pxf.io/i/5597632/1657396/16446" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

