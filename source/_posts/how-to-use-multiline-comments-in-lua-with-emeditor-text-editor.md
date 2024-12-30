---
title: How to Use Multiline Comments in Lua with EmEditor Text Editor
date: 2024-12-25T19:48:47.099Z
updated: 2024-12-29T17:56:07.245Z
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
<li><a href="https://fox-cloud.techidaily.com/new-boost-your-auditory-signature-master-sound-modification-for-zero-cost-for-2024/"><u>[New] Boost Your Auditory Signature Master Sound Modification for Zero Cost for 2024</u></a></li>
<li><a href="https://win-web3.techidaily.com/1-effective-techniques-to-remove-excess-files-and-free-up-space-on-your-computer-insights-by-yl-computing/"><u>1. Effective Techniques to Remove Excess Files and Free Up Space on Your Computer - Insights by YL Computing</u></a></li>
<li><a href="https://extra-resources.techidaily.com/2024-approved-amuse-others-via-adobe-meme-making/"><u>2024 Approved Amuse Others via Adobe Meme-Making</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-framing-frontiers-cutting-edge-app-innovations-24/"><u>2024 Approved Framing Frontiers Cutting-Edge App Innovations '24</u></a></li>
<li><a href="https://vp-tips.techidaily.com/best-free-tools-to-create-a-burned-dvd-on-windows-11-visual-guide/"><u>Best Free Tools to Create a Burned DVD on Windows 11 - Visual Guide</u></a></li>
<li><a href="https://extra-information.techidaily.com/elevating-voice-quality-top-10-microphone-guide/"><u>Elevating Voice Quality Top 10 Microphone Guide</u></a></li>
<li><a href="https://win-web3.techidaily.com/how-can-i-boost-my-pcs-performance-and-achieve-maximum-efficiency-with-yl-software-solutions/"><u>How Can I Boost My PC's Performance and Achieve Maximum Efficiency with YL Software Solutions?</u></a></li>
<li><a href="https://win-web3.techidaily.com/resolving-your-printers-error-code-a-step-by-step-guide-from-yl-computing/"><u>Resolving Your Printer's Error Code: A Step-by-Step Guide From YL Computing</u></a></li>
<li><a href="https://win-web3.techidaily.com/securely-storing-your-digital-assets-expert-tips-from-yl-computings-crypto-experts/"><u>Securely Storing Your Digital Assets: Expert Tips From YL Computing's Crypto Experts</u></a></li>
<li><a href="https://win-web3.techidaily.com/solving-video-card-issues-a-step-by-step-guide-tips-from-yl-computings-expertise/"><u>Solving Video Card Issues: A Step-by-Step Guide - Tips From YL Computing's Expertise</u></a></li>
<li><a href="https://win-web3.techidaily.com/step-by-step-guide-to-resolving-windows-graphics-card-problems-with-tips-from-yl-software-experts/"><u>Step-by-Step Guide to Resolving Windows Graphics Card Problems with Tips From YL Software Experts</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/the-6-best-sim-unlock-services-that-actually-work-on-your-oneplus-12-device-by-drfone-android/"><u>The 6 Best SIM Unlock Services That Actually Work On Your OnePlus 12 Device</u></a></li>
<li><a href="https://techidaily.com/things-you-dont-know-about-realme-gt-3-reset-code-drfone-by-drfone-reset-android-reset-android/"><u>Things You Dont Know About Realme GT 3 Reset Code | Dr.fone</u></a></li>
<li><a href="https://driver-error.techidaily.com/understanding-the-usb-composite-device-features-and-history/"><u>Understanding the USB Composite Device: Features and History</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/HSFNIAYChbA?si=4TIlsUrYmY5vP2il" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

