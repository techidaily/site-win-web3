---
title: How to Use Multiline Comments in Lua with EmEditor Text Editor
date: 2024-11-27T19:19:28.110Z
updated: 2024-11-30T18:43:16.307Z
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
<li><a href="https://youtube-data.techidaily.com/024-approved-essential-guide-to-enhancing-youtube-content-post-upload/"><u>[New] 2024 Approved Essential Guide to Enhancing YouTube Content Post-Upload</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/updated-2024-approved-step-by-step-guide-to-implementing-borders-on-instagram-images/"><u>[Updated] 2024 Approved Step-by-Step Guide to Implementing Borders on Instagram Images</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/2024-approved-excellent-apps-for-streamlined-igtv-vertical-cuts/"><u>2024 Approved Excellent Apps for Streamlined IGTV Vertical Cuts</u></a></li>
<li><a href="https://win-web3.techidaily.com/comment-recuperer-des-fichiers-supprimes-en-preservant-la-structure-de-dossiers-dorigine/"><u>Comment Récupérer Des Fichiers Supprimés en Préservant La Structure De Dossiers D'origine ?</u></a></li>
<li><a href="https://win-web3.techidaily.com/comment-resoudre-les-problemes-de-widgets-windows-11-non-fonctionnels-un-guide-dassistance-simple/"><u>Comment Résoudre Les Problèmes De Widgets Windows 11 Non-Fonctionnels : Un Guide D'Assistance Simple</u></a></li>
<li><a href="https://win-web3.techidaily.com/how-to-set-up-automatic-backups-from-windows-7-to-an-exterior-hdd-two-effective-methods/"><u>How to Set Up Automatic Backups From Windows 7 to an Exterior HDD: Two Effective Methods</u></a></li>
<li><a href="https://location-social.techidaily.com/in-2024-how-to-change-location-on-tiktok-to-see-more-content-on-your-motorola-razr-40-ultra-drfone-by-drfone-virtual-android/"><u>In 2024, How to Change Location on TikTok to See More Content On your Motorola Razr 40 Ultra | Dr.fone</u></a></li>
<li><a href="https://some-approaches.techidaily.com/in-2024-techniques-to-amplify-gopro-battery-duration/"><u>In 2024, Techniques to Amplify GoPro Battery Duration</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/maximizing-your-audio-quality-tips-for-amplifying-m4a-file-volumes/"><u>Maximizing Your Audio Quality - Tips for Amplifying M4A File Volumes</u></a></li>
<li><a href="https://win-dash.techidaily.com/solve-the-problem-why-is-my-samsung-blu-ray-player-not-responding/"><u>Solve the Problem: Why Is My Samsung Blu-Ray Player Not Responding?</u></a></li>
<li><a href="https://some-tips.techidaily.com/trasforma-facilmente-i-tuoi-file-amr-in-mp3-con-questi-passaggi-semplici/"><u>Trasforma Facilmente I Tuoi File AMR in MP3 Con Questi Passaggi Semplici!</u></a></li>
<li><a href="https://win-web3.techidaily.com/windows-server-wbadmin/"><u>Windows Server WBAdminツールによるバックアップファイルの削除手順</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/KKFdFHaVIJg?si=x2vLw7ty3FtHX-9T" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

