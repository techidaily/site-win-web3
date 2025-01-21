---
title: "Enhancing User Interactions: Crafting Improved Conversations with EmEditor - Your Advanced Text Editing Solution"
date: 2025-01-16T01:04:09.751Z
updated: 2025-01-20T16:50:25.259Z
tags:
  - product
categories:
  - emeditor
thumbnail: https://thmb.techidaily.com/be5d3a5dc447d5d228dfc067627f532a2972f66afd30f19695d88ec8cd20ea85.jpg
---

## Enhancing User Interactions: Crafting Improved Conversations with EmEditor - Your Advanced Text Editing Solution

Viewing 5 posts - 1 through 5 (of 5 total)

* Author  
Posts
* April 17, 2013 at 2:40 pm [#10952](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/f29c043a3cc5c5dac8db4e62939893e9?s=80&d=identicon&r=g)Stefan](https://www.emeditor.com/forums/users/Stefan/ "View Stefan's profile")  
Participant  
    
 For my scripts I always have the wish to be able  
 to create better dialogs then alert and input ;-)  
 One way could be to utilize http protocol to show  
 a web page and get back the inserted results and clicked options.  
 I have seen that this works well with another application.  
 (XYplorer file manager, credits to Donald)  
 Here is how it goes, maybe that would be a nifty idea for EmEditor too?  
 The key trick here is the EmEditor own ‘EEM:’ protocol:  
May 15, 2013 at 5:26 am [#11044](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/f29c043a3cc5c5dac8db4e62939893e9?s=80&d=identicon&r=g)Stefan](https://www.emeditor.com/forums/users/Stefan/ "View Stefan's profile")  
Participant  
 Hi Yutaka,  
 have you think about a way to implement  
 such GUI-features to the macro language?  
 Mostly I need the possibility to show  
 a dialog with a few check boxes, radio buttons  
 and input/edit fields. Maybe drop-down list too.  
 Then I want to get back what the user has entered/selected  
 and work on that information to further execute my code.  
 I have seen that possibility in some ways already  
 and if you need some ideas/inspirations please let my know.  
 But please be more communicative and talk with your usership  
 to let them know what you think and if the suggestion have  
 a change to get implemented or not.  
 It’s not that nice to have monologues mostly ;-)  
 Join the chat.  
 Thank You  
 Stefan  
May 15, 2013 at 10:34 pm [#11045](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/a0a6377144ed3636f985d87303f65ed2?s=80&d=identicon&r=g)Yutaka Emura](https://www.emeditor.com/forums/users/yemura/ "View Yutaka Emura's profile")  
Keymaster  
Hello,  
 I am very sorry for late responses.  
 I don’t want to add too many features because they might make EmEditor bloated, and it will become harder to maintain in the future.  
 I heard you can add dialog boxes using COM object such as SeraphyScriptDialog <http://sourceforge.jp/projects/seraphyscrtools/> There might be other similar COM objects.  
 However, I will think about adding more GUI interfaces.  
 Thanks!  
May 16, 2013 at 5:40 pm [#11048](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/f29c043a3cc5c5dac8db4e62939893e9?s=80&d=identicon&r=g)Stefan](https://www.emeditor.com/forums/users/Stefan/ "View Stefan's profile")  
Participant  
> Yutaka wrote:  
> Hello,  
>  
> I am very sorry for late responses.  
 Thanks for feedback.  
> Yutaka wrote:  
>  
> I heard you can add dialog boxes using COM object  
> such as SeraphyScriptDialog  
 That functions are exactly what I have searched for for years.  
 Many thanks for that link.  
 I have never found something like that.  
![](http://img16.imageshack.us/img16/7738/seraphyscriptdialog01.png)  
 Unfortunately it seams some parts are hard coded in japanisch language (see browse folder button and the path delimiter Y)  
 Also since I have to register the com object it is not fully portable. But I guess that de-/registering can be done by a script too.  
 Only it is not that nifty to share script with others if they have to register a dll first. Also they need admin rights.  
 And I have not found any help in english language till now.  
 I have to experiment a bit with that.  
 Thank you much!  
 .  
May 21, 2013 at 3:01 pm [#11057](https://tools.techidaily.com/emeditor/products/)  
[![](https://secure.gravatar.com/avatar/f29c043a3cc5c5dac8db4e62939893e9?s=80&d=identicon&r=g)Stefan](https://www.emeditor.com/forums/users/Stefan/ "View Stefan's profile")  
Participant  
Basically it works!  
![](http://img690.imageshack.us/img690/8626/seraphyscriptdialog.gif)  
#language = "VBScript"  
	set obj = CreateObject("SeraphyScriptDialog")  
	set frm = obj.CreateForm()  
	frm.FormTitle = "Modify Lines"  
	i1 = frm.DefineLabel("For every line")  
	i2 = frm.DefineEdit("Prefix Lines: ")  
	i4 = frm.DefineEdit("Append Lines: ")  
	i12 = frm.DefineButton("OK;CANCEL")  
	'OK= return code 3  
	'Cancel = return code 4  
		ret = 0  
	do  
		ret = frm.ExecuteForm()  
	loop while(ret = 0)  
	if(ret=3) Then  
		'//Insert in front of selected lines  
		Leader  = frm.Value(i2)  
		document.selection.Replace "^",Leader,  eeReplaceSelOnly or eeReplaceAll or eeFindReplaceRegExp  
		'//Insert to the end of selected lines  
		Trailer = frm.Value(i4)  
		document.selection.Replace "$",Trailer, eeReplaceSelOnly or eeReplaceAll or eeFindReplaceRegExp  
	end if  
 Note:  
 SeraphyScriptDialog.dll  
 or  
 SeraphyScriptDialogx64.dll  
 have to be reistered as COM before.  
 Works on Win7 64-bit for me.
* Author  
Posts

Viewing 5 posts - 1 through 5 (of 5 total)

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
<li><a href="https://fox-access.techidaily.com/new-boost-bandw-vibrancy-ps-grading-hacks/"><u>[New] Boost B&W Vibrancy PS Grading Hacks</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/new-diverse-video-realms-sites-outshining-youtube-for-2024/"><u>[New] Diverse Video Realms Sites Outshining Youtube for 2024</u></a></li>
<li><a href="https://youtube-zero.techidaily.com/arnessing-viral-power-your-pathway-to-youtube-fame/"><u>[New] Harnessing Viral Power Your Pathway to YouTube Fame</u></a></li>
<li><a href="https://extra-tips.techidaily.com/beat-to-visuals-an-iphone-guide-for-music-videos/"><u>Beat to Visuals An iPhone Guide for Music Videos</u></a></li>
<li><a href="https://tech-hub.techidaily.com/how-to-ensure-youre-downloading-genuine-chatgpt-programs-on-itunes/"><u>How to Ensure You're Downloading Genuine ChatGPT Programs on iTunes</u></a></li>
<li><a href="https://win-web3.techidaily.com/how-to-fix-a-broken-gpu-expert-tips-and-tricks-by-yl-computing/"><u>How to Fix a Broken GPU: Expert Tips & Tricks by YL Computing</u></a></li>
<li><a href="https://win-web3.techidaily.com/how-to-fix-a-corrupted-hardware-device-driver-expert-advice-from-yl-computing/"><u>How to Fix a Corrupted Hardware Device Driver: Expert Advice From YL Computing</u></a></li>
<li><a href="https://blog-min.techidaily.com/how-to-remove-mdm-from-iphone-6-without-password-by-drfone-ios-unlock-ios-unlock/"><u>How to Remove MDM from iPhone 6 without password?</u></a></li>
<li><a href="https://win-web3.techidaily.com/kiosk-version-of-songbookdb-easy-to-use-song-request-system-powered-by-pcdj/"><u>Kiosk Version of SongbookDB: Easy-to-Use Song Request System Powered by PCDJ</u></a></li>
<li><a href="https://hardware-reviews.techidaily.com/navigating-the-world-of-pc-components-at-toms-tech-hub/"><u>Navigating the World of PC Components at Tom's Tech Hub</u></a></li>
<li><a href="https://sound-issues.techidaily.com/silent-mic-here-are-the-steps-to-restore-your-microphones-voice-functionality/"><u>Silent Mic? Here Are The Steps to Restore Your Microphone's Voice Functionality</u></a></li>
<li><a href="https://win-web3.techidaily.com/step-by-step-guide-adjusting-your-windows-defender-firewall-preferences/"><u>Step-by-Step Guide: Adjusting Your Windows Defender Firewall Preferences</u></a></li>
<li><a href="https://win-web3.techidaily.com/troubleshooting-guide-resolving-print-issues-post-driver-update-expertise-from-yl-computing/"><u>Troubleshooting Guide: Resolving Print Issues Post-Driver Update - Expertise From YL Computing</u></a></li>
<li><a href="https://win-web3.techidaily.com/understanding-the-formal-denomination-unveiling-the-official-name-for-china-insights-by-yl-computing/"><u>Understanding the Formal Denomination: Unveiling the Official Name for China - Insights by YL Computing</u></a></li>
<li><a href="https://win-web3.techidaily.com/yl-softwares-guide-to-assembling-a-successful-crypto-portfolio-tips-and-techniques/"><u>YL Software's Guide to Assembling a Successful Crypto Portfolio: Tips and Techniques</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/XA_wP7rS9ww?si=LarMG3sEHAhSoL6q" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

