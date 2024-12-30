---
title: "Enhancing User Interactions: Crafting Improved Conversations with EmEditor - Your Advanced Text Editing Solution"
date: 2024-12-24T22:15:33.139Z
updated: 2024-12-29T21:21:30.939Z
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
<li><a href="https://facebook-video-content.techidaily.com/new-facebook-insights-how-to-use-it-for-beginners-for-2024/"><u>[New] Facebook Insights How to Use It for Beginners for 2024</u></a></li>
<li><a href="https://youtube-tips.techidaily.com/ransform-videos-affordable-high-quality-effs-in-2024/"><u>[New] Transform Videos - Affordable, High-Quality Effs, In 2024</u></a></li>
<li><a href="https://fox-boxes.techidaily.com/updated-in-2024-blending-images-with-moving-screens-on-iphone/"><u>[Updated] In 2024, Blending Images with Moving Screens on iPhone</u></a></li>
<li><a href="https://fox-boxes.techidaily.com/updated-in-2024-elevate-your-visual-content-mastery-of-image-backdrop-removal-in-canva/"><u>[Updated] In 2024, Elevate Your Visual Content Mastery of Image Backdrop Removal in Canva</u></a></li>
<li><a href="https://common-error.techidaily.com/directx-error-resolution-handling-the-unrecoverable-error-exception/"><u>DirectX Error Resolution: Handling the 'Unrecoverable Error' Exception</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/how-to-remove-iphone-13-pro-sim-lock-by-drfone-ios/"><u>How to Remove iPhone 13 Pro SIM Lock?</u></a></li>
<li><a href="https://win-web3.techidaily.com/identifying-graphic-card-problems-expert-advice-from-yl-innovations-inc/"><u>Identifying Graphic Card Problems: Expert Advice From YL Innovations Inc.</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/leading-mac-snipper-programs-analyzed-for-2024/"><u>Leading Mac Snipper Programs Analyzed for 2024</u></a></li>
<li><a href="https://technical-tips.techidaily.com/presidents-holiday-sale-limited-time-deal-at-300-off-the-latest-m2-macbook-air-zdnet/"><u>President's Holiday Sale: Limited-Time Deal at $300 Off the Latest M2 MacBook Air | ZDNET</u></a></li>
<li><a href="https://win-answers.techidaily.com/troubleshooting-steps-for-when-minecraft-wont-let-you-enter-the-game-world/"><u>Troubleshooting Steps for When Minecraft Won't Let You Enter the Game World</u></a></li>
<li><a href="https://win-web3.techidaily.com/unlock-your-pcs-secrets-a-detailed-walkthrough-of-accessing-the-device-manager-to-check-connected-devices-with-yl-software-expertise/"><u>Unlock Your PC's Secrets: A Detailed Walkthrough of Accessing the Device Manager to Check Connected Devices with YL Software Expertise</u></a></li>
<li><a href="https://win-web3.techidaily.com/yl-computing-presents-exquisite-high-resolution-wallpapers-of-south-koreas-gorgeous-girls-background-pictures-and-photos-galore/"><u>YL Computing Presents: Exquisite High-Resolution Wallpapers of South Korea's Gorgeous Girls – Background Pictures & Photos Galore!</u></a></li>
<li><a href="https://win-web3.techidaily.com/yl-software-solutions-explained-how-to-incorve-programs-into-your-control-panel-seamlessly/"><u>YL Software Solutions Explained: How To Incorve Programs Into Your Control Panel Seamlessly</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/TJCye_oCTTw?si=6bVyBphcSgSFdyuq" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

