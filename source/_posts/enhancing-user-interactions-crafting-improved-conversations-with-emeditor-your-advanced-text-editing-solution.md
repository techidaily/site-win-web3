---
title: "Enhancing User Interactions: Crafting Improved Conversations with EmEditor - Your Advanced Text Editing Solution"
date: 2024-11-11T00:12:52.881Z
updated: 2024-11-12T18:15:07.468Z
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
<li><a href="https://desktop-recording.techidaily.com/new-2024-approved-mastering-live-broadcasts-obs-on-youtube-and-twitch/"><u>[New] 2024 Approved Mastering Live Broadcasts OBS on YouTube and Twitch</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/updated-2024-approved-ace-in-the-halls-boosting-youtube-traffic/"><u>[Updated] 2024 Approved Ace in the Halls Boosting YouTube Traffic</u></a></li>
<li><a href="https://tiktok-videos.techidaily.com/updated-in-2024-bold-bio-breakthroughs-secrets-revealed-for-tripling-tiktok-viewership-via-filmora/"><u>[Updated] In 2024, Bold Bio Breakthroughs Secrets Revealed for Tripling TikTok Viewership via Filmora</u></a></li>
<li><a href="https://win-web3.techidaily.com/iuinoplusaxuuwklue9ruehroeinplusiorewumummrplusiqpdog5zub5pa56z2i55qe6lplusf6ycf5pu05q2j5rovig/"><u>解決外置硬碟設定錯誤: 四方面的迅速更正法</u></a></li>
<li><a href="https://win11.techidaily.com/conjuring-a-cohesive-file-landscape-in-win1011/"><u>Conjuring a Cohesive File Landscape in WIN10/11</u></a></li>
<li><a href="https://fox-sure.techidaily.com/das-fuhrende-clonierungsprogramm-fur-verschiedene-segmente-von-aomei-backupper/"><u>Das Führende Clonierungsprogramm Für Verschiedene Segmente Von AOMEI Backupper</u></a></li>
<li><a href="https://win-web3.techidaily.com/effective-techniques-secure-your-data-with-top-file-backup-solutions-in-windows-server-s-2016/"><u>Effective Techniques: Secure Your Data with Top File Backup Solutions in Windows Server S 2016</u></a></li>
<li><a href="https://some-approaches.techidaily.com/essential-steps-for-troubleshooting-a-laptop-that-stays-uncharged-even-with-the-power-cord-attached/"><u>Essential Steps for Troubleshooting a Laptop That Stays Uncharged, Even with the Power Cord Attached</u></a></li>
<li><a href="https://win-web3.techidaily.com/guide-syncing-your-ipod-touch-with-itunes-steps-for-successful-music-transfer/"><u>Guide: Syncing Your iPod Touch with iTunes – Steps for Successful Music Transfer</u></a></li>
<li><a href="https://win-web3.techidaily.com/how-effective-is-using-one-computers-windows-repair-usb-with-various-machines/"><u>How Effective Is Using One Computer's Windows Repair USB with Various Machines?</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/in-2024-list-of-pokemon-go-joysticks-on-lava-blaze-pro-5g-drfone-by-drfone-virtual-android/"><u>In 2024, List of Pokémon Go Joysticks On Lava Blaze Pro 5G | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ios-adoption-unleashing-chatgpt-app/"><u>IOS Adoption: Unleashing ChatGPT App</u></a></li>
<li><a href="https://win-web3.techidaily.com/kostenlose-datentransfer-apps-schnell-und-einfach-von-telefon-auf-computer-ubertragen/"><u>Kostenlose Datentransfer-Apps: Schnell Und Einfach Von Telefon Auf Computer Übertragen!</u></a></li>
<li><a href="https://win-web3.techidaily.com/la-guia-definitiva-como-copiar-el-almacenamiento-ssd-m2-nvme-opcion-de-duplicacion-perfecta/"><u>La Guía Definitiva: Cómo Copiar El Almacenamiento SSD M.2 NVMe - Opción De Duplicación Perfecta</u></a></li>
<li><a href="https://win-web3.techidaily.com/losung-fur-das-problem-recover-deleted-pdf-files-auf-ihrem-windows-pc/"><u>Lösung Für Das Problem - Recover Deleted PDF Files Auf Ihrem Windows-PC</u></a></li>
<li><a href="https://ai-video-tools.techidaily.com/new-elevate-your-videos-the-top-rated-ipad-video-editing-apps-for-2024/"><u>New Elevate Your Videos The Top-Rated iPad Video Editing Apps for 2024</u></a></li>
<li><a href="https://common-error.techidaily.com/troubleshooting-and-resolving-audioservice-issues-on-windows-7-fixed/"><u>Troubleshooting & Resolving 'AudioService' Issues on Windows 7 ([Fixed])</u></a></li>
<li><a href="https://win-web3.techidaily.com/ultimate-guide-restoring-access-to-your-unresponsive-micro-sd-storage-device/"><u>Ultimate Guide: Restoring Access to Your Unresponsive Micro SD Storage Device</u></a></li>
<li><a href="https://win-web3.techidaily.com/windows-10-hdd/"><u>Windows 10에서 HDD를 교체하기 전에 데이터 백업을 위한 두 가지 방법</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2100537/7443" target="_top" id="2100537">
  <img src="//a.impactradius-go.com/display-ad/7443-2100537" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2100537/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

