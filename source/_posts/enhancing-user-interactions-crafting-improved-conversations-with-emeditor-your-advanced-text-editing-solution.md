---
title: "Enhancing User Interactions: Crafting Improved Conversations with EmEditor - Your Advanced Text Editing Solution"
date: 2024-10-22T23:55:37.462Z
updated: 2024-10-28T20:46:32.957Z
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
<li><a href="https://facebook-video-share.techidaily.com/new-in-2024-exporting-your-creativity-imovie-videos-for-youtube-audiences/"><u>[New] In 2024, Exporting Your Creativity IMovie Videos for YouTube Audiences</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/updated-in-2024-breaking-barriers-next-level-strategies-for-fb-video-success/"><u>[Updated] In 2024, Breaking Barriers Next-Level Strategies for FB Video Success</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/updated-seamless-video-communication-in-whatsapp-web-for-laptops-and-desktops-for-2024/"><u>[Updated] Seamless Video Communication in WhatsApp Web for Laptops and Desktops for 2024</u></a></li>
<li><a href="https://win-web3.techidaily.com/100-free-effortless-automatic-sync-securely-store-your-precious-memories-on-microsoft-onedrive/"><u>100% Free] Effortless Automatic Sync: Securely Store Your Precious Memories on Microsoft OneDrive</u></a></li>
<li><a href="https://article-posts.techidaily.com/2024-approved-motion-magic-quick-photography-tricks-for-samsung-users/"><u>2024 Approved Motion Magic Quick Photography Tricks for Samsung Users</u></a></li>
<li><a href="https://win-web3.techidaily.com/5-methods-zum-wiederherstellen-von-loschten-daten-unter-windows-10-eine-schrittweise-anleitung/"><u>5 Methods Zum Wiederherstellen Von Löschten Daten Unter Windows 10: Eine Schrittweise Anleitung</u></a></li>
<li><a href="https://win-web3.techidaily.com/windows-11-ssd-c/"><u>安全地将 Windows 11 系统在 SSD 上部署: 通过 C 驱动器克隆技术</u></a></li>
<li><a href="https://android-unlock.techidaily.com/bypassing-google-account-with-vnrom-bypass-for-samsung-galaxy-a34-5g-by-drfone-android/"><u>Bypassing Google Account With vnROM Bypass For Samsung Galaxy A34 5G</u></a></li>
<li><a href="https://win-web3.techidaily.com/come-risolvere-i-problemi-occasionali-di-windows-11-e-evitare-il-blocco-imprevisto-del-sistema-operativo/"><u>Come Risolvere I Problemi Occasionali Di Windows 11 E Evitare Il Blocco Imprevisto Del Sistema Operativo</u></a></li>
<li><a href="https://win-web3.techidaily.com/comment-pouvez-vous-transferer-un-systeme-de-demarrage-sur-une-cle-usb-dun-ordinateur-sous-windows-11-10-ou-plus-anciennes-versions/"><u>Comment Pouvez-Vous Transférer Un Système De Démarrage Sur Une Clé USB D'un Ordinateur Sous Windows 11, 10 Ou Plus Anciennes Versions ?</u></a></li>
<li><a href="https://blog-min.techidaily.com/free-download-complete-collection-of-disney-movie-scores-big-hero-6-into-the-woods-and-frozen/"><u>Free Download: Complete Collection of Disney Movie Scores - Big Hero 6, Into the Woods & Frozen</u></a></li>
<li><a href="https://twitter-videos.techidaily.com/in-2024-tweetvidcutter-mp4webm-extractor/"><u>In 2024, TweetVidCutter MP4/WebM Extractor</u></a></li>
<li><a href="https://win-web3.techidaily.com/macaomei/"><u>Mac电脑简单设置AOMEI云管线自动备份及同步</u></a></li>
<li><a href="https://technical-tips.techidaily.com/score-the-new-apple-ipad-10gen-at-an-unbeatable-price-of-299-exclusive-post-prime-day-bargain-zdnet-news/"><u>Score the New Apple iPad 10Gen at an Unbeatable Price of $299 - Exclusive Post-Prime Day Bargain! | ZDNET News.</u></a></li>
<li><a href="https://win-web3.techidaily.com/seamless-transition-from-windows-7-to-windows-10-effective-data-backup-strategies/"><u>Seamless Transition From Windows 7 to Windows 10: Effective Data Backup Strategies</u></a></li>
<li><a href="https://unlock-android.techidaily.com/top-10-password-cracking-tools-for-xiaomi-civi-3-by-drfone-android/"><u>Top 10 Password Cracking Tools For Xiaomi Civi 3</u></a></li>
<li><a href="https://techtrends.techidaily.com/1722881732203-unmissable-discounts-on-ipads-buy-today/"><u>Unmissable Discounts on iPads – Buy Today!</u></a></li>
<li><a href="https://win-web3.techidaily.com/windows-11-onedrive0x803def7/"><u>Windows 11 OneDrive错误0x80ˈ3def7终结</u></a></li>
<li><a href="https://win-web3.techidaily.com/1728499961670-pc/"><u>フリープログラムを使用したPC同士のネットワーク内ファイル同期テクニック</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://ephamedtechinc.pxf.io/c/5597632/2137218/26400" target="_top" id="2137218">
  <img src="//a.impactradius-go.com/display-ad/26400-2137218" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://ephamedtechinc.pxf.io/i/5597632/2137218/26400" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

