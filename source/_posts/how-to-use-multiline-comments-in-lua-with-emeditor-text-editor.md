---
title: How to Use Multiline Comments in Lua with EmEditor Text Editor
date: 2025-01-24T01:07:00.202Z
updated: 2025-01-26T17:27:08.716Z
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
<li><a href="https://fox-access.techidaily.com/new-2024-approved-unveiling-iphones-premium-tools-for-image-watermarking/"><u>[New] 2024 Approved Unveiling iPhone's Premium Tools for Image Watermarking</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/new-in-2024-advanced-game-monitoring-tools-for-diverse-formats/"><u>[New] In 2024, Advanced Game Monitoring Tools for Diverse Formats</u></a></li>
<li><a href="https://youtube-docs.techidaily.com/n-2024-your-pathway-to-youtube-live-success-stories/"><u>[New] In 2024, Your Pathway to YouTube Live Success Stories</u></a></li>
<li><a href="https://screen-capture.techidaily.com/new-leading-game-reviews-top-business-sims-for-24/"><u>[New] Leading Game Reviews Top Business Sims for '24</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/new-ultimate-guide-to-top-video-editors-for-webcams/"><u>[New] Ultimate Guide to Top Video Editors for Webcams</u></a></li>
<li><a href="https://fox-helps.techidaily.com/updated-top-accessories-to-elevate-your-sj4000-experience/"><u>[Updated] Top Accessories to Elevate Your SJ4000 Experience</u></a></li>
<li><a href="https://win-web3.techidaily.com/1-comprehensive-steps-to-create-bootable-clones-with-paragon-hard-disk-manager/"><u>1. Comprehensive Steps to Create Bootable Clones with Paragon Hard Disk Manager</u></a></li>
<li><a href="https://extra-resources.techidaily.com/2024-approved-advanced-tutorial-exploiting-googles-automatic-transcription-features/"><u>2024 Approved Advanced Tutorial Exploiting Google's Automatic Transcription Features</u></a></li>
<li><a href="https://win-web3.techidaily.com/iusruwplusqewplusjoajiplusobqpluswfpeociplusodioodqeodluodqzrjg4njg6njgqtjg5bjga7jg5xjgqnjg7zjg6djg6zjg53jg7zjg4gi/"><u>修復後手に入るトラブル:ドライブのフォームレポート</u></a></li>
<li><a href="https://win-web3.techidaily.com/discover-the-top-three-free-tools-for-recovering-lost-data-on-your-pc-windows-1011/"><u>Discover the Top Three Free Tools for Recovering Lost Data on Your PC (Windows 10/11)</u></a></li>
<li><a href="https://win-web3.techidaily.com/hyper-v-tipps-und-tricks-einfaches-erstellen-von-virtuellen-maschinen/"><u>Hyper-V Tipps Und Tricks: Einfaches Erstellen Von Virtuellen Maschinen</u></a></li>
<li><a href="https://location-social.techidaily.com/in-2024-set-your-preferred-job-location-on-linkedin-app-of-your-asus-rog-phone-8-pro-drfone-by-drfone-virtual-android/"><u>In 2024, Set Your Preferred Job Location on LinkedIn App of your Asus ROG Phone 8 Pro | Dr.fone</u></a></li>
<li><a href="https://facebook.techidaily.com/navigating-the-world-of-business-facebook-client-partnerships/"><u>Navigating the World of Business-Facebook Client Partnerships</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/YpnYKIrpgZQ?si=94zicAHp1CH-0oso" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

