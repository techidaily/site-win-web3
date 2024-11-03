---
title: "Enhancing User Interactions: Crafting Improved Conversations with EmEditor - Your Advanced Text Editing Solution"
date: 2024-11-02T16:20:03.141Z
updated: 2024-11-03T18:13:22.878Z
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
<li><a href="https://remote-screen-capture.techidaily.com/new-2024-approved-expert-guide-screen-capture-on-windows-8-devices/"><u>[New] 2024 Approved Expert Guide Screen Capture on Windows 8 Devices</u></a></li>
<li><a href="https://youtube-clips.techidaily.com/2024-approved-effortless-guide-never-see-youtube-shorts-again/"><u>2024 Approved Effortless Guide Never See YouTube Shorts Again</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/2024-approved-exploring-nikon-d850-vs-d7500-features/"><u>2024 Approved Exploring Nikon D850 Vs D7500 Features</u></a></li>
<li><a href="https://win-web3.techidaily.com/1728487696597-aomei-backupper/"><u>如何高效使用AOMEI Backupper進行資料夾間的同步技巧</u></a></li>
<li><a href="https://win-web3.techidaily.com/1728466045693-windows-111087/"><u>効率的なデータ保護: Windows 11/10/8/7用バックアップスケジューラの作り方</u></a></li>
<li><a href="https://android-unlock.techidaily.com/bypassing-google-account-with-vnrom-bypass-for-samsung-galaxy-s23-fe-by-drfone-android/"><u>Bypassing Google Account With vnROM Bypass For Samsung Galaxy S23 FE</u></a></li>
<li><a href="https://win-web3.techidaily.com/el-software-ideal-para-transferir-tus-informaciones-de-samsung-a-windows-version-para-windows-781011/"><u>El Software Ideal Para Transferir Tus Informaciones De Samsung a Windows: Versión Para Windows 7/8/10/11</u></a></li>
<li><a href="https://sound-issues.techidaily.com/fixing-black-ops-cold-war-solutions-to-voice-chat-issues/"><u>Fixing Black Ops Cold War: Solutions to Voice Chat Issues</u></a></li>
<li><a href="https://techidaily.com/full-guide-to-hard-reset-your-vivo-t2-5g-drfone-by-drfone-reset-android-reset-android/"><u>Full Guide to Hard Reset Your Vivo T2 5G | Dr.fone</u></a></li>
<li><a href="https://win-web3.techidaily.com/how-to-access-emeditor-search-without-find-button-on-toolbar/"><u>How to Access EmEditor Search Without 'Find' Button on Toolbar</u></a></li>
<li><a href="https://vp-tips.techidaily.com/in-2024-high-gear-comparison-gopros-best-match-ghost-s-drift/"><u>In 2024, High Gear Comparison GoPro's Best Match? Ghost-S Drift</u></a></li>
<li><a href="https://review-topics.techidaily.com/in-2024-how-to-simulate-gps-movement-in-ar-games-on-vivo-t2-5g-drfone-by-drfone-virtual-android/"><u>In 2024, How to Simulate GPS Movement in AR games On Vivo T2 5G? | Dr.fone</u></a></li>
<li><a href="https://win-web3.techidaily.com/protect-your-virtual-servers-with-free-aomei-backupper-easy-hyper-v-image-management-and-disaster-recovery/"><u>Protect Your Virtual Servers with Free AOMEI Backupper – Easy Hyper-V Image Management and Disaster Recovery</u></a></li>
<li><a href="https://ai-vdieo-software.techidaily.com/s-most-popular-video-reversal-websites/"><u>S Most Popular Video Reversal Websites</u></a></li>
<li><a href="https://win-web3.techidaily.com/transfer-ibooks-between-iphones-discover-these-4-quick-and-effective-techniques/"><u>Transfer iBooks Between iPhones - Discover These 4 Quick and Effective Techniques</u></a></li>
<li><a href="https://win-web3.techidaily.com/tutorial-passo-passo-per-copiare-un-servers-fisico-a-disco-nuovo-o-con-vmware/"><u>Tutorial Passo-Passo per Copiare Un Servers Fisico a Disco NUovo O Con VMware</u></a></li>
<li><a href="https://win-web3.techidaily.com/1728484051749-usb2/"><u>USBから失われたデータ復旧のプロセス：2つのエキスパートソフトウェアの使用例</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://unicoeye.pxf.io/c/5597632/2148771/18498" target="_top" id="2148771">
  <img src="//a.impactradius-go.com/display-ad/18498-2148771" border="0" alt="https://techidaily.com" width="350" height="90"/>
</a>
<img height="0" width="0" src="https://unicoeye.pxf.io/i/5597632/2148771/18498" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

