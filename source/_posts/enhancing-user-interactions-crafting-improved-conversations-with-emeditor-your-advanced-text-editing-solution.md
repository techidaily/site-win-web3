---
title: "Enhancing User Interactions: Crafting Improved Conversations with EmEditor - Your Advanced Text Editing Solution"
date: 2024-10-10T19:17:38.763Z
updated: 2024-10-16T20:54:48.322Z
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
<li><a href="https://video-screen-grab.techidaily.com/new-savor-playtime-the-essential-guide-to-high-quality-offline-ios-games/"><u>[New] Savor Playtime – The Essential Guide to High-Quality Offline iOS Games</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/updated-2024-approved-engaging-scriptwriting-techniques-for-higher-video-rankings/"><u>[Updated] 2024 Approved Engaging Scriptwriting Techniques for Higher Video Rankings</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/updated-2024-approved-step-by-step-guide-to-mastering-streamlabs-obs-usage/"><u>[Updated] 2024 Approved Step-by-Step Guide to Mastering Streamlabs OBS Usage</u></a></li>
<li><a href="https://fox-info.techidaily.com/2024-approved-appreciate-with-us-open-source-and-subscription-outro-samples/"><u>2024 Approved Appreciate with Us Open-Source & Subscription Outro Samples</u></a></li>
<li><a href="https://win-web3.techidaily.com/windowsaomei/"><u>逐步指南：如何在Windows上设置或移除AOMEI备份程序</u></a></li>
<li><a href="https://win-web3.techidaily.com/1728489794909-approach/"><u>Approach:</u></a></li>
<li><a href="https://win-web3.techidaily.com/essential-hardware-prerequisites-for-vsphere-8-a-comprehensive-guide/"><u>Essential Hardware Prerequisites for vSphere 8: A Comprehensive Guide</u></a></li>
<li><a href="https://win-web3.techidaily.com/guide-simple-pour-changer-le-hdd-c-par-un-ssd-sur-windows-111087-techniques-et-etapes-faciles-a-suivre/"><u>Guide Simple Pour Changer Le HDD C Par Un SSD Sur Windows 11/10/8/7 - Techniques Et Étapes Faciles À Suivre</u></a></li>
<li><a href="https://win-web3.techidaily.com/how-to-restore-unallocated-space-in-your-storage-drive-using-windows-1011/"><u>How to Restore Unallocated Space in Your Storage Drive Using Windows 10/11</u></a></li>
<li><a href="https://hardware-tips.techidaily.com/navigating-the-world-of-gadgets-with-toms-hardware-expertise/"><u>Navigating the World of Gadgets with Tom's Hardware Expertise</u></a></li>
<li><a href="https://youtube-data.techidaily.com/izing-income-through-youtube-short-tutorials/"><u>Optimizing Income Through YouTube Short Tutorials</u></a></li>
<li><a href="https://techidaily.com/recover-apple-iphone-xs-max-data-from-itunes-drfone-by-drfone-ios-data-recovery-ios-data-recovery/"><u>Recover Apple iPhone XS Max Data From iTunes | Dr.fone</u></a></li>
<li><a href="https://win-blog.techidaily.com/resolving-microsoft-outlook-connection-issues-a-comprehensive-guide/"><u>Resolving Microsoft Outlook Connection Issues: A Comprehensive Guide</u></a></li>
<li><a href="https://win-web3.techidaily.com/successful-steps-to-refresh-your-system-transitioning-from-windows-11-back-to-windows-10/"><u>Successful Steps to Refresh Your System: Transitioning From Windows 11 Back to Windows 10</u></a></li>
<li><a href="https://extra-lessons.techidaily.com/superior-mkv-player-pcandroid-experience/"><u>Superior MKV Player PC/Android Experience</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://bluettide.pxf.io/c/5597632/2141683/17092" target="_top" id="2141683">
  <img src="//a.impactradius-go.com/display-ad/17092-2141683" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://bluettide.pxf.io/i/5597632/2141683/17092" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

