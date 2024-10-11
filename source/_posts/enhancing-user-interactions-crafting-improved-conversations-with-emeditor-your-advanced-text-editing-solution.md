---
title: "Enhancing User Interactions: Crafting Improved Conversations with EmEditor - Your Advanced Text Editing Solution"
date: 2024-10-05T09:37:16.862Z
updated: 2024-10-11T07:37:58.235Z
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
<li><a href="https://snapchat-videos.techidaily.com/updated-simplified-methods-for-migrating-snapshots-to-storage-for-2024/"><u>[Updated] Simplified Methods for Migrating Snapshots to Storage for 2024</u></a></li>
<li><a href="https://fox-direct.techidaily.com/2024-approved-echoes-of-yesteryear-a-digital-compilation-of-ringtones/"><u>2024 Approved Echoes of Yesteryear A Digital Compilation of Ringtones</u></a></li>
<li><a href="https://some-approaches.techidaily.com/2024-approved-the-artisans-path-to-creating-3d-luts/"><u>2024 Approved The Artisan’s Path to Creating 3D LUTs</u></a></li>
<li><a href="https://win-web3.techidaily.com/comprehensive-jabra-evolve2-75-headset-assessment-perfect-for-telecommuting-and-hybrid-teams-featuring-noise-cancellation-and-extended-chat-capacity-insight128/"><u>Comprehensive Jabra Evolve2 75 Headset Assessment: Perfect for Telecommuting & Hybrid Teams Featuring Noise Cancellation & Extended Chat Capacity - Insights From ZDNet</u></a></li>
<li><a href="https://blog-min.techidaily.com/convert-wav-audio-tracks-free-into-mp4-format-with-movavis-web-tool/"><u>Convert WAV Audio Tracks Free Into MP4 Format with Movavi's Web Tool</u></a></li>
<li><a href="https://win-web3.techidaily.com/effective-techniques-for-cleaning-up-and-deleting-preinstalled-apps-in-windows/"><u>Effective Techniques for Cleaning Up and Deleting Preinstalled Apps in Windows</u></a></li>
<li><a href="https://windows11.techidaily.com/expedite-data-access-seamless-entry-into-windows-11-disk-editor/"><u>Expedite Data Access: Seamless Entry Into Windows 11 Disk Editor</u></a></li>
<li><a href="https://win-web3.techidaily.com/get-ahead-of-the-crowd-with-the-latest-tech-deal-surface-laptop-go-2-drops-at-just-599-pre-order-now-on-zdnet/"><u>Get Ahead of the Crowd with the Latest Tech Deal: Surface Laptop Go 2 Drops at Just $599, Pre-Order Now on ZDNet!</u></a></li>
<li><a href="https://review-topics.techidaily.com/in-2024-dose-life360-notify-me-when-someone-checks-my-location-on-lava-yuva-2-drfone-by-drfone-virtual-android/"><u>In 2024, Dose Life360 Notify Me When Someone Checks My Location On Lava Yuva 2? | Dr.fone</u></a></li>
<li><a href="https://android-transfer.techidaily.com/in-2024-how-can-you-transfer-files-from-infinix-hot-30i-to-iphone-151413-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>In 2024, How Can You Transfer Files From Infinix Hot 30i To iPhone 15/14/13? | Dr.fone</u></a></li>
<li><a href="https://win-web3.techidaily.com/insiders-picks-top-recommendations-from-best-buy-experts-on-optimal-windows-machines-confirmed-by-zdnet/"><u>Insider's Picks: Top Recommendations From Best Buy Experts on Optimal Windows Machines - Confirmed by ZDNet</u></a></li>
<li><a href="https://games-able.techidaily.com/next-gen-platform-battle-series-x-vs-pc-builds/"><u>Next Gen Platform Battle: Series X Vs. PC Builds</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://unicoeye.pxf.io/c/5597632/2148771/18498" target="_top" id="2148771">
  <img src="//a.impactradius-go.com/display-ad/18498-2148771" border="0" alt="https://techidaily.com" width="350" height="90"/>
</a>
<img height="0" width="0" src="https://unicoeye.pxf.io/i/5597632/2148771/18498" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

