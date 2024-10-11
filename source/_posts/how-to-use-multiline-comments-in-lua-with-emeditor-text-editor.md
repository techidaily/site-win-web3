---
title: How to Use Multiline Comments in Lua with EmEditor Text Editor
date: 2024-10-04T20:08:33.988Z
updated: 2024-10-11T03:58:28.293Z
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
<li><a href="https://tiktok-video-recordings.techidaily.com/new-devising-a-personalized-tiktok-alphanumeric-marker-for-2024/"><u>[New] Devising a Personalized TikTok Alphanumeric Marker for 2024</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/new-in-2024-ultimate-techniques-streaming-hulu-on-win-mac-and-mobile/"><u>[New] In 2024, Ultimate Techniques Streaming Hulu on Win, Mac, and Mobile</u></a></li>
<li><a href="https://tiktok-videos.techidaily.com/updated-elevate-to-a-custom-hashtag-mastery-on-tiktok/"><u>[Updated] Elevate to a Custom Hashtag Mastery on TikTok</u></a></li>
<li><a href="https://some-tips.techidaily.com/updated-streamline-screen-capabilities-building-in-frame-video-experiences-on-sierra/"><u>[Updated] Streamline Screen Capabilities Building In-Frame Video Experiences on Sierra</u></a></li>
<li><a href="https://win-web3.techidaily.com/boost-your-ergonomics-essential-add-on-for-every-standing-desk-enthusiast-techwise/"><u>Boost Your Ergonomics: Essential Add-On for Every Standing Desk Enthusiast | TechWise</u></a></li>
<li><a href="https://win-web3.techidaily.com/customizing-your-windows-11-setup-and-overcoming-microsofts-limits-expert-tips/"><u>Customizing Your Windows 11 Setup & Overcoming Microsoft's Limits - Expert Tips</u></a></li>
<li><a href="https://win-web3.techidaily.com/defying-microsofts-limits-successful-reader-stories-of-upgrading-aging-pcs-to-windows-n-on-zdnet/"><u>Defying Microsoft's Limits: Successful Reader Stories of Upgrading Aging PCs to Windows N On-Zdnet</u></a></li>
<li><a href="https://location-social.techidaily.com/does-find-my-friends-work-on-oppo-k11x-drfone-by-drfone-virtual-android/"><u>Does find my friends work on Oppo K11x | Dr.fone</u></a></li>
<li><a href="https://win-web3.techidaily.com/elevate-your-productivity-essential-gadgets-to-complement-your-standing-desk-tips-by-zdnet/"><u>Elevate Your Productivity: Essential Gadgets to Complement Your Standing Desk - Tips by ZDNET</u></a></li>
<li><a href="https://youtube-webster.techidaily.com/24-navigating-top-purchasers-for-monetized-yt-channels/"><u>In 2024, Navigating Top Purchasers for Monetized YT Channels</u></a></li>
<li><a href="https://extra-skills.techidaily.com/in-2024-step-by-step-how-to-erase-photographic-backgrounds/"><u>In 2024, Step-by-Step How to Erase Photographic Backgrounds</u></a></li>
<li><a href="https://hardware-help.techidaily.com/1722978947646-latest-geforce-rtx-3080-driver-for-windows-11-secure-your-free-download-now/"><u>Latest GeForce RTX 3080 Driver for Windows 11 - Secure Your Free Download Now!</u></a></li>
<li><a href="https://win-web3.techidaily.com/top-5-premium-desks-dominating-2022-zdnets-ultimate-guide/"><u>Top 5 Premium Desks Dominating 2022: ZDNet's Ultimate Guide</u></a></li>
<li><a href="https://win-web3.techidaily.com/unraveling-the-impact-of-googles-antitrust-defeat-on-user-experience-and-search-evolution/"><u>Unraveling the Impact of Google’s Antitrust Defeat on User Experience & Search Evolution</u></a></li>
<li><a href="https://win-web3.techidaily.com/worth-the-upgrade-a-comparative-review-of-standard-and-plus-versions-of-chatgpt/"><u>Worth the Upgrade? A Comparative Review of Standard and Plus Versions of ChatGPT</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<span id="1444782">
					<video width="1024" height="576" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1444782.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/14559-1444782">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1444782.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:640px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fpropmoneyinc.pxf.io%2Fc%2F5597632%2F1444782%2F14559'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1444782/14559" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

