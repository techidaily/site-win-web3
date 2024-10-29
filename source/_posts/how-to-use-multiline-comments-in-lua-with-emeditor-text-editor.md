---
title: How to Use Multiline Comments in Lua with EmEditor Text Editor
date: 2024-10-22T04:33:07.037Z
updated: 2024-10-28T19:57:48.720Z
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
<li><a href="https://article-helps.techidaily.com/new-in-2024-diving-deep-into-burst-mode-for-professional-photography/"><u>[New] In 2024, Diving Deep Into Burst Mode for Professional Photography</u></a></li>
<li><a href="https://instagram-video-files.techidaily.com/new-in-2024-stream-instagram-and-youtube-a-step-by-step-guide/"><u>[New] In 2024, Stream Instagram & YouTube A Step-by-Step Guide</u></a></li>
<li><a href="https://win-web3.techidaily.com/44cm44op44o844oj44oh44kj44k544kv44gu5lin5yw35zci44gm6kal44gk44gl44kk44gplus44gx44gf44cn44go44ge44gg44oh44od44k744o844k444ks5ywl5pyn44gz44kl5pa55rov/"><u>「ハードディスクの不具合が見つかりました」というメッセージを克服する方法</u></a></li>
<li><a href="https://android-location.techidaily.com/10-free-location-spoofers-to-fake-gps-location-on-your-nubia-z50s-pro-drfone-by-drfone-virtual/"><u>10 Free Location Spoofers to Fake GPS Location on your Nubia Z50S Pro | Dr.fone</u></a></li>
<li><a href="https://fox-tips.techidaily.com/windows-0x8078002a/"><u>解決 Windows 系統代碼 0X8078002A 時常出現的錯誤方法</u></a></li>
<li><a href="https://win-dash.techidaily.com/1722978856424-amd-gpio-device-driver-free-download-get-started-now/"><u>AMD GPIO Device Driver Free Download – Get Started Now</u></a></li>
<li><a href="https://techtrends.techidaily.com/demystifying-instagram-a-comprehensive-overview-for-beginners/"><u>Demystifying Instagram: A Comprehensive Overview for Beginners</u></a></li>
<li><a href="https://win-web3.techidaily.com/enregistrer-sur-un-disque-ssd-a-laide-dun-hdd-sous-windows-111087-guide-detaille/"><u>Enregistrer Sur Un Disque SSD À L'aide D'un HDD Sous Windows 11/10/8/7 : Guide Détaillé</u></a></li>
<li><a href="https://win-web3.techidaily.com/guide-pratique-recuperation-de-donnees-du-disque-dur-a-laide-de-la-ligne-de-commande-windows/"><u>Guide Pratique : Récupération De Données Du Disque Dur À L'aide De La Ligne De Commande Windows</u></a></li>
<li><a href="https://fox-access.techidaily.com/market-leading-6-platforms-enhancing-biz-interaction-for-2024/"><u>Market-Leading 6 Platforms Enhancing Biz Interaction for 2024</u></a></li>
<li><a href="https://win-web3.techidaily.com/reviving-disappeared-files-and-directories-in-windows-10-easy-recovery-tips/"><u>Reviving Disappeared Files and Directories in Windows 10 - Easy Recovery Tips</u></a></li>
<li><a href="https://win-web3.techidaily.com/tutoriel-complet-pour-la-restauration-de-donnees-sur-un-ssd-kingston/"><u>Tutoriel Complet Pour La Restauration De Données Sur Un SSD Kingston</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2151888/7443" target="_top" id="2151888">
  <img src="//a.impactradius-go.com/display-ad/7443-2151888" border="0" alt="https://techidaily.com" width="600" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2151888/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

