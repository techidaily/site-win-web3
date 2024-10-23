---
title: How to Use Multiline Comments in Lua with EmEditor Text Editor
date: 2024-10-18T22:03:13.582Z
updated: 2024-10-23T05:33:11.512Z
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
<li><a href="https://youtube-web.techidaily.com/ed-2024-approved-from-device-footage-to-youtube-shorts-your-streamlined-approach/"><u>[Updated] 2024 Approved From Device Footage to YouTube Shorts - Your Streamlined Approach</u></a></li>
<li><a href="https://facebook-video-files.techidaily.com/2024-approved-unlock-potential-the-15-best-tools-for-transforming-fb-revenue/"><u>2024 Approved Unlock Potential The 15 Best Tools for Transforming FB Revenue</u></a></li>
<li><a href="https://win-web3.techidaily.com/5-easy-ways-to-backup-your-windows-1011-computer-using-cloud-storage/"><u>5 Easy Ways to Backup Your Windows 10/11 Computer Using Cloud Storage</u></a></li>
<li><a href="https://win-web3.techidaily.com/iphoneitunes4/"><u>解决iPhone与iTunes不能同步时丢失数据的4项修复步骤</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/bidding-on-shadows-the-2023-virtual-vault-showdown/"><u>Bidding on Shadows The 2023 Virtual Vault Showdown</u></a></li>
<li><a href="https://win-web3.techidaily.com/come-trasferire-il-tuo-sistema-windows-similar-meaning-in-italian-easy-steps-con-due-soluzioni-alternative/"><u>Come Trasferire Il Tuo Sistema Windows # Similar Meaning in Italian | Easy Steps Con Due Soluzioni Alternative</u></a></li>
<li><a href="https://win-web3.techidaily.com/effizientes-back-up-management/"><u>Effizientes Back-Up-Management</u></a></li>
<li><a href="https://fox-glue.techidaily.com/in-2024-6-periscope-alternative-apps-for-android-and-ios/"><u>In 2024, 6 Periscope Alternative Apps for Android and iOS</u></a></li>
<li><a href="https://youtube-tips.techidaily.com/24-giggle-genesis-conceptualizing-7-funny-youtube-sessions/"><u>In 2024, Giggle Genesis Conceptualizing 7 Funny YouTube Sessions</u></a></li>
<li><a href="https://win-web3.techidaily.com/in-depth-analysis-of-data-resumption-methods-warm-site-cold-site-and-hot-site-in-disaster-preparedness-plans/"><u>In-Depth Analysis of Data Resumption Methods: Warm Site, Cold Site, and Hot Site in Disaster Preparedness Plans</u></a></li>
<li><a href="https://hardware-reviews.techidaily.com/in-depth-assessment-of-the-corsair-tx5-problems/"><u>In-Depth Assessment of the Corsair TX5# Problems</u></a></li>
<li><a href="https://games-able.techidaily.com/is-quick-resume-a-worthwhile-feature-of-your-xbox-series-xs/"><u>Is Quick Resume a Worthwhile Feature of Your Xbox Series X|S?</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/premium-podcast-reviews-by-gpodcasts-for-2024/"><u>Premium Podcast Reviews by GPodcasts for 2024</u></a></li>
<li><a href="https://win-web3.techidaily.com/solution-pour-laffichage-des-6-derniers-fichiers-dans-excel-comment-resoudre-le-probleme/"><u>Solution Pour L’Affichage Des 6 Derniers Fichiers Dans Excel: Comment Résoudre Le Problème?</u></a></li>
<li><a href="https://win-web3.techidaily.com/synchronisierung-von-dateien-per-automatisierung-mit-google-drive-entdecken-sie-4-effiziente-methoden/"><u>Synchronisierung Von Dateien per Automatisierung Mit Google Drive - Entdecken Sie 4 Effiziente Methoden</u></a></li>
<li><a href="https://win11.techidaily.com/the-ultimate-guide-to-a-flawless-in-place-windows-11-reboot/"><u>The Ultimate Guide to a Flawless, In-Place Windows 11 Reboot</u></a></li>
<li><a href="https://win-web3.techidaily.com/ubertragung-musik-auf-ihrem-iphone-ohne-pc-oder-itunes-mit-fonebackup-eine-einfache-anleitung/"><u>Übertragung Musik Auf Ihrem iPhone Ohne PC Oder iTunes Mit FoneBackup: Eine Einfache Anleitung</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2144276/7443" target="_top" id="2144276">
  <img src="//a.impactradius-go.com/display-ad/7443-2144276" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2144276/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

