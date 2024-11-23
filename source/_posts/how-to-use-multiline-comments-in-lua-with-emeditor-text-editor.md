---
title: How to Use Multiline Comments in Lua with EmEditor Text Editor
date: 2024-11-19T00:57:25.695Z
updated: 2024-11-23T02:52:03.638Z
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
<li><a href="https://youtube-data.techidaily.com/024-approved-savvy-sponsorship-strategies-for-small-scale-sites/"><u>[New] 2024 Approved Savvy Sponsorship Strategies for Small-Scale Sites</u></a></li>
<li><a href="https://youtube-lab.techidaily.com/approved-epicurean-elites-top-food-vloggers-you-cant-miss/"><u>2024 Approved Epicurean Elites Top Food Vloggers You Can't Miss</u></a></li>
<li><a href="https://video-capture.techidaily.com/2024-approved-examining-the-breadth-of-features-in-obs-studio/"><u>2024 Approved Examining the Breadth of Features in OBS Studio</u></a></li>
<li><a href="https://win-web3.techidaily.com/comprehensive-tutorial-on-managing-vmware-vcenters-statistical-data/"><u>Comprehensive Tutorial on Managing VMware vCenter's Statistical Data</u></a></li>
<li><a href="https://win-web3.techidaily.com/enhancing-user-interactions-crafting-improved-conversations-with-emeditor-your-advanced-text-editing-solution/"><u>Enhancing User Interactions: Crafting Improved Conversations with EmEditor - Your Advanced Text Editing Solution</u></a></li>
<li><a href="https://tools.techidaily.com/epubor/tidal-downloader/"><u>Epubor Tidal Downloader</u></a></li>
<li><a href="https://win-web3.techidaily.com/guide-syncing-your-ipod-touch-with-itunes-steps-for-successful-music-transfer/"><u>Guide: Syncing Your iPod Touch with iTunes – Steps for Successful Music Transfer</u></a></li>
<li><a href="https://fox-cloud.techidaily.com/in-2024-app-analysis-vll-perspective/"><u>In 2024, App Analysis VLL Perspective</u></a></li>
<li><a href="https://ios-unlock.techidaily.com/in-2024-iphone-is-disabled-here-is-the-way-to-unlock-disabled-apple-iphone-7-by-drfone-ios/"><u>In 2024, iPhone Is Disabled? Here Is The Way To Unlock Disabled Apple iPhone 7</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/in-2024-pros-hunters-rate-action-camera-winners/"><u>In 2024, Pros Hunters Rate Action Camera Winners</u></a></li>
<li><a href="https://win-web3.techidaily.com/kostenlose-datentransfer-apps-schnell-und-einfach-von-telefon-auf-computer-ubertragen/"><u>Kostenlose Datentransfer-Apps: Schnell Und Einfach Von Telefon Auf Computer Übertragen!</u></a></li>
<li><a href="https://win-web3.techidaily.com/resepsi-gratis-untuk-mudah-mudahan-file-yang-ditulaskan-dalam-windows-11/"><u>Resepsi Gratis Untuk Mudah-Mudahan File Yang Ditulaskan Dalam Windows 11</u></a></li>
<li><a href="https://win-web3.techidaily.com/securely-install-a-solid-state-drive-into-your-lenovo-thinkpad-(span-stylecolor-000)13-tips-and-techniques-for-successful-upgrades/"><u>Securely Install a Solid-State Drive Into Your Lenovo ThinkPad <Span Style=color: #000;>13: Tips and Techniques for Successful Upgrades</u></a></li>
<li><a href="https://ai-vdieo-software.techidaily.com/the-top-online-video-flipper-tools/"><u>The Top Online Video Flipper Tools</u></a></li>
<li><a href="https://youtube-sure.techidaily.com/-ios-apps-turn-youtube-videos-into-mp3-files/"><u>Top 6 iOS Apps Turn YouTube Videos Into MP3 Files</u></a></li>
<li><a href="https://win-web3.techidaily.com/troubleshooting-tips-for-unauthenticated-microsoft-windows-installations/"><u>Troubleshooting Tips for Unauthenticated Microsoft Windows Installations</u></a></li>
<li><a href="https://win-web3.techidaily.com/ultimate-guide-restoring-access-to-your-unresponsive-micro-sd-storage-device/"><u>Ultimate Guide: Restoring Access to Your Unresponsive Micro SD Storage Device</u></a></li>
<li><a href="https://fake-location.techidaily.com/will-the-ipogo-get-you-banned-and-how-to-solve-it-on-infinix-smart-8-drfone-by-drfone-virtual-android/"><u>Will the iPogo Get You Banned and How to Solve It On Infinix Smart 8 | Dr.fone</u></a></li>
<li><a href="https://win-web3.techidaily.com/windows-10-hdd/"><u>Windows 10에서 HDD를 교체하기 전에 데이터 백업을 위한 두 가지 방법</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/9sk53d1bBhY?si=yaTeDogLb3D4dYu1&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

