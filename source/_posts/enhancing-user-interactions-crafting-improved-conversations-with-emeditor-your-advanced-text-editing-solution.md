---
title: "Enhancing User Interactions: Crafting Improved Conversations with EmEditor - Your Advanced Text Editing Solution"
date: 2024-11-29T02:16:06.232Z
updated: 2024-12-01T00:15:42.594Z
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
<li><a href="https://facebook-video-content.techidaily.com/new-escaping-boredom-with-a-chuckle-best-fb-incarceration-comical-stories/"><u>[New] Escaping Boredom with a Chuckle Best FB Incarceration Comical Stories</u></a></li>
<li><a href="https://vp-tips.techidaily.com/new-in-2024-cutting-edge-live-broadcast-solutions/"><u>[New] In 2024, Cutting-Edge Live Broadcast Solutions</u></a></li>
<li><a href="https://extra-hints.techidaily.com/updated-building-applications-with-azure-speech-to-text/"><u>[Updated] Building Applications with Azure Speech to Text</u></a></li>
<li><a href="https://win-web3.techidaily.com/come-effettuare-una-facile-migrazione-di-windows-11-da-un-ssd-a-un-altro/"><u>Come Effettuare Una Facile Migrazione Di Windows 11 Da Un SSD a Un Altro</u></a></li>
<li><a href="https://win-web3.techidaily.com/come-recuperare-i-dati-da-un-hard-disk-esterno-una-guida-completa/"><u>Come Recuperare I Dati Da Un Hard Disk Esterno: Una Guida Completa</u></a></li>
<li><a href="https://win-web3.techidaily.com/demystifying-windows-server-backup-compression-processes/"><u>Demystifying Windows Server Backup Compression Processes</u></a></li>
<li><a href="https://win-web3.techidaily.com/efficiently-transfer-your-mi-to-mi-data-a-guide-with-4-proven-techniques/"><u>Efficiently Transfer Your MI-to-MI Data: A Guide with 4 Proven Techniques</u></a></li>
<li><a href="https://howto.techidaily.com/fix-cant-take-screenshot-due-to-security-policy-on-tecno-spark-10-4g-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>Fix Cant Take Screenshot Due to Security Policy on Tecno Spark 10 4G | Dr.fone</u></a></li>
<li><a href="https://win-web3.techidaily.com/guide-complet-a-lechelle-detaillee-protegez-votre-configuration-windows-navigateur-vers-la-revolution-windows-10/"><u>Guide Complet À L’Echelle Détaillée : Protégez Votre Configuration Windows Navigateur Vers La Révolution Windows 10</u></a></li>
<li><a href="https://change-location.techidaily.com/how-to-fix-androidprocessmedia-has-stopped-on-motorola-moto-g14-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>How to Fix Android.Process.Media Has Stopped on Motorola Moto G14 | Dr.fone</u></a></li>
<li><a href="https://win-web3.techidaily.com/how-to-set-up-a-windows-pe-usb-stick-a-step-by-step-guide-for-transitioning-from-windows-pe-to-windows-11/"><u>How to Set Up a Windows PE USB Stick: A Step-by-Step Guide for Transitioning From Windows PE to Windows 11</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/professionals-choice-top-10-afx-templates-for-free-for-2024/"><u>Professionals' Choice Top 10 AFX Templates for FREE for 2024</u></a></li>
<li><a href="https://win-web3.techidaily.com/schnellformatierungsprozess-verstandnis-der-dateneinbusse-und-wiederherstellungstechniken-fur-verlorene-dokumente/"><u>Schnellformatierungsprozess: Verständnis Der Dateneinbuße Und Wiederherstellungstechniken Für Verlorene Dokumente.</u></a></li>
<li><a href="https://win-fantastic.techidaily.com/step-by-step-guide-turning-off-hyper-v-in-windows-os-and-servers/"><u>Step-by-Step Guide: Turning Off Hyper-V in Windows OS and Servers</u></a></li>
<li><a href="https://tech-hub.techidaily.com/tech-showdown-pixel-9-pro-xl-vs-iphone-15-pro-camera-face-off-who-won-and-whats-the-hidden-twist-analysis/"><u>Tech Showdown: Pixel 9 Pro XL Vs. IPhone 15 Pro Camera Face-Off | Who Won and What's the Hidden Twist? - Analysis</u></a></li>
<li><a href="https://hardware-updates.techidaily.com/unbeatable-prime-day-deal-the-top-non-thinkpadmacbook-laptop-boosting-productivity-at-half-price-exclusive-insights/"><u>Unbeatable Prime Day Deal: The Top Non-ThinkPad/MacBook Laptop Boosting Productivity at Half Price - Exclusive Insights</u></a></li>
<li><a href="https://win-web3.techidaily.com/understanding-the-significance-of-a-404-error-when-websites-go-missing/"><u>Understanding the Significance of a '404 Error – When Websites Go Missing</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/XS1nQCe95LU?si=A2dhdFkSAI61_nKA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

