---
title: How to Use Multiline Comments in Lua with EmEditor Text Editor
date: 2024-11-06T19:30:32.854Z
updated: 2024-11-12T21:49:18.435Z
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
<li><a href="https://screen-sharing-recording.techidaily.com/new-open-world-opus-top-10-similar-video-games-for-2024/"><u>[New] Open World Opus Top 10 Similar Video Games for 2024</u></a></li>
<li><a href="https://fox-links.techidaily.com/updated-in-2024-the-ultimate-guide-to-iphone-photo-watermarks-apps/"><u>[Updated] In 2024, The Ultimate Guide to iPhone Photo Watermarks Apps</u></a></li>
<li><a href="https://win-web3.techidaily.com/comment-recuperer-des-fichiers-supprimes-en-preservant-la-structure-de-dossiers-dorigine/"><u>Comment Récupérer Des Fichiers Supprimés en Préservant La Structure De Dossiers D'origine ?</u></a></li>
<li><a href="https://win-web3.techidaily.com/comment-resoudre-les-problemes-de-widgets-windows-11-non-fonctionnels-un-guide-dassistance-simple/"><u>Comment Résoudre Les Problèmes De Widgets Windows 11 Non-Fonctionnels : Un Guide D'Assistance Simple</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/delete-your-chathistory-with-gpt/"><u>Delete Your ChatHistory with GPT</u></a></li>
<li><a href="https://hardware-help.techidaily.com/get-the-newest-nvidia-quadro-rtx-8000-driver-for-win-11-8-and-7-systems/"><u>Get the Newest Nvidia Quadro RTX 8000 Driver for Win 11, 8 and 7 Systems</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/gigglegenius-customize-memes-faster-than-you-think-for-2024/"><u>GiggleGenius Customize Memes Faster Than You Think for 2024</u></a></li>
<li><a href="https://win-web3.techidaily.com/gratis-methoden-zur-wiederherstellung-geloschter-microsoft-office-dokumente/"><u>Gratis Methoden Zur Wiederherstellung Gelöschter Microsoft Office Dokumente</u></a></li>
<li><a href="https://blog-min.techidaily.com/how-to-transfer-contacts-from-tecno-pova-5-to-outlook-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>How to Transfer Contacts from Tecno Pova 5 to Outlook | Dr.fone</u></a></li>
<li><a href="https://iphone-unlock.techidaily.com/in-2024-how-to-unlock-stolen-iphone-11-in-different-conditionsin-drfone-by-drfone-ios/"><u>In 2024, How To Unlock Stolen iPhone 11 In Different Conditionsin | Dr.fone</u></a></li>
<li><a href="https://location-social.techidaily.com/simple-and-effective-ways-to-change-your-country-on-youtube-app-of-your-motorola-edge-40-neo-drfone-by-drfone-virtual-android/"><u>Simple and Effective Ways to Change Your Country on YouTube App Of your Motorola Edge 40 Neo | Dr.fone</u></a></li>
<li><a href="https://audio-editing.techidaily.com/the-ultimate-how-to-syncing-audio-with-newly-updated-avi-content-for-2024/"><u>The Ultimate How-To Syncing Audio with Newly Updated AVI Content for 2024</u></a></li>
<li><a href="https://win-web3.techidaily.com/wd-my-cloud-and-iphone-a-guide-to-restoring-your-disrupted-auto-backup-functionality/"><u>WD My Cloud and iPhone: A Guide to Restoring Your Disrupted Auto-Backup Functionality</u></a></li>
<li><a href="https://win-web3.techidaily.com/alaadyd-mn-alhzm-alshfafa-lnskh-bramgk-il-krs-ssd-taalymat-tfsylya-lthoyl-hdd-il-tknya-akthr-kfaaaa/"><u>العديد من الحزم الشفافة لنسخ برامجك إلى قرص SSD: تعليمات تفصيلية لتحويل HDD إلى تقنية أكثر كفاءة</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<span id="1993654">
					<video width="128" height="480" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1993654.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1993654">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1993654.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:80px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1993654%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1993654/22993" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

