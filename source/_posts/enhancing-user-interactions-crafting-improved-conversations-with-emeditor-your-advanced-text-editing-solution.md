---
title: "Enhancing User Interactions: Crafting Improved Conversations with EmEditor - Your Advanced Text Editing Solution"
date: 2024-10-16T08:24:52.178Z
updated: 2024-10-22T19:01:04.102Z
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
<li><a href="https://screen-mirroring-recording.techidaily.com/new-efficient-video-editing-with-timestamps-and-on-screen-text/"><u>[New] Efficient Video Editing with Timestamps & On-Screen Text</u></a></li>
<li><a href="https://youtube-tips.techidaily.com/ed-techie-gamers-income-streams-2024/"><u>[Updated] Techie Gamers' Income Streams 2024</u></a></li>
<li><a href="https://discover-forum.techidaily.com/iumbsuocueodioodroodvoocuoikhplusavsoapnpluseoruobiplusocieobruodhplusodvoocvpluswplusqewfgplusazltrln7rmnkznmotjgarjgqzjgqtjg4ki/"><u>雲ストレージ複数機種からのデータ復元法:基本的なガイド</u></a></li>
<li><a href="https://facebook.techidaily.com/beware-of-phishing-schemes-in-your-news-feed/"><u>Beware of Phishing Schemes in Your News Feed</u></a></li>
<li><a href="https://win-extraordinary.techidaily.com/cross-platform-file-management-system-efficient-and-reliable/"><u>Cross-Platform File Management System - Efficient and Reliable</u></a></li>
<li><a href="https://win-web3.techidaily.com/how-to-access-emeditor-search-without-find-button-on-toolbar/"><u>How to Access EmEditor Search Without 'Find' Button on Toolbar</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/how-to-add-videos-in-instagram-story-for-2024/"><u>How to Add Videos in Instagram Story for 2024</u></a></li>
<li><a href="https://win-web3.techidaily.com/how-to-fix-hulus-pts2n07-error-message-a-comprehensive-guide/"><u>How to Fix Hulu's PTS2n07 Error Message: A Comprehensive Guide</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/in-2024-3-steps-for-perfect-instagram-video-margins/"><u>In 2024, 3 Steps for Perfect Instagram Video Margins</u></a></li>
<li><a href="https://vp-tips.techidaily.com/les-15-meilleurs-logiciels-de-conversion-video-4k-sans-cout-pour-windows-et-mac-guide-complet/"><u>Les 15 Meilleurs Logiciels De Conversion Vidéo 4K Sans Coût Pour Windows Et Mac - Guide Complet</u></a></li>
<li><a href="https://win-web3.techidaily.com/loschprozess-fur-alte-backup-dateien-wie-gehen-sie-vor/"><u>Löschprozess Für Alte Backup-Dateien: Wie Gehen Sie Vor?</u></a></li>
<li><a href="https://win-web3.techidaily.com/qnapwindows-10/"><u>QNAP機器でWindows 10を信頼性高く安全にバックアップするためのステップごとのガイド</u></a></li>
<li><a href="https://win-web3.techidaily.com/tutorial-passo-passo-per-copiare-un-servers-fisico-a-disco-nuovo-o-con-vmware/"><u>Tutorial Passo-Passo per Copiare Un Servers Fisico a Disco NUovo O Con VMware</u></a></li>
<li><a href="https://win-web3.techidaily.com/1728484051749-usb2/"><u>USBから失われたデータ復旧のプロセス：2つのエキスパートソフトウェアの使用例</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://laganoo.pxf.io/c/5597632/1657396/16446" target="_top" id="1657396">
  <img src="//a.impactradius-go.com/display-ad/16446-1657396" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://laganoo.pxf.io/i/5597632/1657396/16446" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

