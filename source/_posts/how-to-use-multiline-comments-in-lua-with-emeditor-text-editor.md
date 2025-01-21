---
title: How to Use Multiline Comments in Lua with EmEditor Text Editor
date: 2025-01-16T04:31:34.947Z
updated: 2025-01-21T06:40:05.933Z
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
<li><a href="https://youtube-data.techidaily.com/n-2024-earnings-enlightenment-joshi-and-youtube-success-stories/"><u>[New] In 2024, Earnings Enlightenment Joshi and YouTube Success Stories</u></a></li>
<li><a href="https://snapchat-videos.techidaily.com/updated-2024-approved-snap-tales-with-flair-unearth-over-120-ingenious-titles-for-your-unique-snapchat-chronicles/"><u>[Updated] 2024 Approved Snap Tales with Flair Unearth over 120 Ingenious Titles for Your Unique Snapchat Chronicles</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/updated-a-gamers-guide-to-seamless-ps4-recording-and-streaming-via-obs-for-2024/"><u>[Updated] A Gamer's Guide to Seamless PS4 Recording and Streaming via OBS for 2024</u></a></li>
<li><a href="https://techno-recovery.techidaily.com/8-things-to-consider-before-buying-a-desktop-pc/"><u>8 Things to Consider Before Buying a Desktop PC</u></a></li>
<li><a href="https://win-dash.techidaily.com/acer-predator-helios-300-newest-graphics-drivers-for-optimal-gaming-performance/"><u>Acer Predator Helios 300 - Newest Graphics Drivers for Optimal Gaming Performance</u></a></li>
<li><a href="https://win-web3.techidaily.com/can-you-safely-disable-windows-defender-without-compromising-security-tips-and-insights-from-yl-computing/"><u>Can You Safely Disable Windows Defender Without Compromising Security? - Tips & Insights From YL Computing</u></a></li>
<li><a href="https://win-web3.techidaily.com/high-definition-easter-egg-wallpaper-designs-stunning-hd-backgrounds-perfect-for-your-device-curated-by-yl-computing/"><u>High-Definition Easter Egg Wallpaper Designs: Stunning HD Backgrounds Perfect for Your Device - Curated by YL Computing</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/how-do-i-add-my-signature-to-wbk-file-by-ldigisigner-sign-a-word-sign-a-word/"><u>How do i add my signature to .wbk file</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/how-to-delete-all-photos-from-iphone-14-pro-beyond-scope-of-recovery-stellar-by-stellar-data-recovery-ios-iphone-data-recovery/"><u>How to Delete All Photos from iPhone 14 Pro Beyond Scope of Recovery? | Stellar</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/in-2024-how-to-mirror-pc-screen-to-motorola-moto-g14-phones-drfone-by-drfone-android/"><u>In 2024, How to Mirror PC Screen to Motorola Moto G14 Phones? | Dr.fone</u></a></li>
<li><a href="https://win-web3.techidaily.com/power-supplys-role-in-enhancing-computer-efficiency-yl-software-exploration/"><u>Power Supply's Role in Enhancing Computer Efficiency: YL Software Exploration</u></a></li>
<li><a href="https://win-web3.techidaily.com/the-establishment-of-the-peoples-republic-of-china-1949-founder-and-historical-context-yl-computing-solutions/"><u>The Establishment of the People's Republic of China, 1949: Founder and Historical Context - YL Computing Solutions</u></a></li>
<li><a href="https://win-web3.techidaily.com/verify-correct-hardware-drivers-in-place-with-tips-from-yl-software-experts/"><u>Verify Correct Hardware Drivers in Place with Tips From YL Software Experts</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/hZsnjxeSh1U?si=hZIfzQPDNX5KtOCg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

