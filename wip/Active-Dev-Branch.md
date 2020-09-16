---
title: The Changelog
description: New Windows 10 features for Insider Preview builds in the Dev Channel.
author: bleblanc
manager: dougkim
ms.tgt_pltfrm: na
ms.devlang: na
ms.author: bleblanc
ms.localizationpriority: medium
ms.topic: article
ms.prod: w10
---

# The Changelog
The Changelog represents everything new from all the builds from the Active Developmemnt Branch (RS_PRELEASE) released to the **Dev Channel**. This page includes everything noted as part of the "What's new" and "General changes & improvements" sections of the blog posts published for each build [on the Windows Blog](https://blogs.windows.com/windows-insider/) and does not contain other noted updates for Insiders, fixes, or known issues. 

## Build 20215
Windows 10 Insider Preview Build 20215 was released to the Dev Channel on [9/16/2020](https://blogs.windows.com/windows-insider/2020/09/16/announcing-windows-10-insider-preview-build-20215/).

## Build 20211
Windows 10 Insider Preview Build 20211 was released to the Dev Channel on [9/10/2020](https://blogs.windows.com/windows-insider/2020/09/10/announcing-windows-10-insider-preview-build-20211/).

### Adding Search to the Default Apps pages in Settings
After making some updates to help improve performance, this change to enable searching the lists of file types, protocols, and apps when setting a default is now rolling out to all Insiders in the Dev Channel – thanks everyone who’s shared feedback along the way.

![Default apps search](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/09/default-apps.png "Search the lists of file types, protocols, and apps when setting a default.")

### Access Linux file systems in the Windows Subsystem for Linux
This latest insiders preview build adds the ability for users to attach and mount a physical disk inside of a WSL 2 distro. This enables you to access file systems that aren’t natively supported by Windows (such as ext4). So if you’re dual booting with Windows and Linux, and are using different disks, you can now access your Linux files from Windows! To learn more about this feature please read [this blog post](https://devblogs.microsoft.com/commandline/access-linux-filesystems-in-windows-and-wsl-2/) on the Windows Command Line blog.

## Build 20206
Windows 10 Insider Preview Build 20206 was released to the Dev Channel on [9/2/2020](https://blogs.windows.com/windows-insider/2020/09/02/announcing-windows-10-insider-preview-build-20206/).

### Evolving the Emoji Picker
Over the last 3 years, we have been adding ways to express yourself when typing in Windows. In addition to adding an emoji picker and support for more emoji, we have also added support for many more languages, kaomoji, and symbols. We have also added ways to manage your clipboard history. We are evolving the emoji picker in Windows to bring many of these separate experiences together as well as introduce some new capabilities such as easy access to animated GIFs.

![Updated Emoji Picker](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/09/Screenshot-2020-09-01-172040.png "The revamped emoji picker is your one-stop for expressing yourself with quick access to emoji, kaomoji, symbols, animated GIFs and your clipboard.")

We know that you need more than just emojis to properly convey your message when communicating using text. To that end, we’ve revamped the emoji picker to be a one-stop for expressing yourself while you type on your device!  This new experience offers:

* An updated design: We are making the experience more aligned with our Fluent Design principles, including a new acrylic background.
* Emoji search: We are improving discoverability of emoji search in supported languages by having an inline search box.
* Animated GIF support, including search: Going forward, WIN + [.] and WIN + [;] will now enable you to quickly input animated GIFs. The selection of animated gifs will be continuously updated based on current trends and #hashtags. Search is also available for those times where you need to find the perfect reaction gif to succinctly communicate your message.
* Converging our input experiences across emoji and clipboard history: We are bringing input and clipboard history together into a single experience. You can still press WIN + V to go straight to clipboard history, but now you can also access it by switching to the “Clipboard” category after pressing WIN + [.] or WIN + [;].

We will be continuing to work on input in Windows and would love to hear your thoughts on further improvements. We are lighting up a new area path in the Feedback Hub for you to share your suggestions: **Input and Language > Emoji, Kaomoji, GIF and other input**.

_Please note: In order to insert an animated GIF when typing, the text field needs to support it. Animated GIF search requires an internet connection and is powered by Tenor. For more details about languages where animated GIF search is supported by Tenor, please see here._

>[!NOTE] 
>TThis feature is rolling out to a subset of Insiders in the Dev Channel at first, to help us quickly identify issues that may impact performance and reliability. Rest assured they will be gradually rolled out to everyone in the Dev Channel.

### Introducing Voice Typing
Windows voice typing is the new and improved version of Windows dictation that enables you to type effortlessly with your voice wherever there’s a text field on your PC. Sometimes, using your voice is more comfortable and efficient than typing on a keyboard – with Windows voice typing, you can relax your hands and just say what you want to write.

Improved features for voice typing include:

* A modern design – optimized for use with touch keyboards.
* Auto-punctuation that allows you to effortlessly put your thoughts down without worrying about question marks and periods (turn it on in settings).
* An updated back end for the most reliable voice typing experience ever on Windows.
Easily start voice typing any time by using the keyboard shortcut (WIN + H) or tapping the microphone button on the touch keyboard.

When using the hardware keyboard:

![Voice Typing Hardware Keyboard](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/09/VoiceTypingFloaty-300x239.png "Use the WIN + H keyboard shortcut for quick access to the microphone button for voice to text.")

When using the touch keyboard:

![Voice Typing Touch Keyboard](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/09/VoiceTypingKeyboard-1024x427.png "When using the touch keyboard in Windows, you can use the microphone icon to quickly use voice to text.")

Want to up your voice typing to the next level? Try out the following supported voice commands:

![Voice Typing Commands List](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/09/VTCommands.png "List of voice commands in different languages. ")

Voice typing is available in the following languages/locales*:

* English (US)
* English (Australia)
* English (India)
* English (Canada)
* English (United Kingdom)
* French (France)
* French (Canada)
* Portuguese (Brazilian)
* Simplified Chinese
* Spanish (Mexico)
* Spanish (Spanish)
* German
* Italian
* Japanese**

_*Voice typing will automatically use the language your keyboard is set to (if supported).
**Auto-punctuation is not available in Japanese at this time._

_Please note: we are still working to improve the feature and how it interacts with different applications. In some Office apps you may experience random pauses while using the voice typing feature. If this happens, click the microphone icon again to restart the listening experience._

>[!NOTE] 
>This feature is rolling out to a subset of Insiders in the Dev Channel at first, to help us quickly identify issues that may impact performance and reliability. Rest assured they will be gradually rolled out to everyone in the Dev Channel.

### Improving the touch keyboard design
Some Insiders will start to see our new touch keyboard design rolling out to their PCs. The updated design includes a fresh aesthetic and many other small tweaks, including updated key sizes / layouts to optimize for typing comfort & accuracy. We have also done some work to help improve discoverability and usability of available features.

While exploring the updated design, you will notice a number of refinements, including:

* New key press animations and sounds.
* Child keys have been optimized for quicker entry – try pressing and holding keys like “e” or “-“ and see how it looks.
* For those who prefer to keep their keyboard undocked, the option now accessible via a button directly in the candidate bar, and you can easily move the keyboard around using the gripper region at the top of the keyboard.
* All entries in the settings menu now have labels for improved clarity of available options.
We are bringing emoji search to the touch keyboard, so you no longer need to hunt through the different categories to find the one you are looking for. More so, you can also now search for animated GIFs. All accessible from our new expressive input button in the candidate bar. (For more – see our section above on evolving the emoji panel.)
* A new entry point into voice typing has been added to the left of the space bar in supported languages. (See above section on voice typing.)

![Touch Keyboard Redesign](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/09/2020-09-01-6.png "The redesigned touch keyboard introduces a variety of improvements such as new key press animations and sounds, quick access to emoji and animated GIFs, and a new entry point for voice typing.")

![Touch Keyboard Redesign 2](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/09/2020-09-01-5-1024x644.png "The redesigned touch keyboard offers quick access to emoji and animated GIFs so you and express yourself any way you like while typing in Windows.")

The touch keyboard can also be invoked on any PC from the touch keyboard button on the taskbar, although you may need to enable the button. To do so, right-click or press and hold on the taskbar, then select “Show touch keyboard button” in the menu. Once the touch keyboard is open, try typing or shapewriting on the keyboard and let us know how it feels.

We want to thank Insiders for sharing their feedback about the touch keyboard over the years – your comments directly inspired these changes. We look forward to you trying them out and to even more feedback!

_Please note: Some of the keyboard layouts for certain languages are still in the process of being updated to the new design. Currently shapewriting is only supported when using the wide or onehanded touch keyboard layouts._

>[!NOTE] 
>This feature is rolling out to a subset of Insiders in the Dev Channel at first, to help us quickly identify issues that may impact performance and reliability. Rest assured they will be gradually rolled out to everyone in the Dev Channel.

### Cursor movement using the space bar  
One thing we heard from our customers is the desire to change the cursor position with the touch keyboard. Based on that feedback, we are updating the keyboard so that you can now quickly do this in any text field using gestures on the space bar.

All you need to do is place a finger on the space bar and slide your finger left, right, up, or down. As your finger moves, so will the cursor – one character or line at a time.

![Cursor movement spacebar](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/09/Single-Portrait-Docked-1-1024x423.png "Press and hold on the space bar on the touch keyboard to move the cursor on your screen.")

We’ll be continuing to work on input in Windows and would love to hear your thoughts on further improvements.

>[!NOTE] 
>This feature is rolling out to a subset of Insiders in the Dev Channel at first, to help us quickly identify issues that may impact performance and reliability. Rest assured they will be gradually rolled out to everyone in the Dev Channel.

## Build 20201
Windows 10 Insider Preview Build 20201 was released to the Dev Channel on [8/26/2020](https://blogs.windows.com/windows-insider/2020/08/26/announcing-windows-10-insider-preview-build-20201/).

## Build 20197
Windows 10 Insider Preview Build 20197 was released to the Dev Channel on [8/21/2020](https://blogs.windows.com/windowsexperience/2020/08/21/announcing-windows-10-insider-preview-build-20197/).

### Bringing Disk Management into Settings
We mentioned we had more Settings work on the way, and here’s the next one – as of today’s build you’ll now be able to manage your disks and volumes from within the Settings app. This includes tasks such as viewing disk information, creating and formatting volumes, and assigning drive letters.

Unlike the existing Disk Management MMC snap-in, this modern experience was built from the ground up to with accessibility in mind. It also features better integration with features such as Storage Spaces and the Storage breakdown page.

Go to __Settings > System > Storage__ and __click Manage Disks and Volumes__ to get started. We’d love to hear your feedback once you try it out.

![The Manage Disks and Volumes page in Settings. C drive is selected and shows Explorer and Properties options.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/08/113cc52773bb5f5e6b6b6d761e294222.png)

The existing Disk Management MMC snap-in is still available for those that need it.

### Changes and Improvements
* We’re updating the [ALT + Tab behavior with Microsoft Edge tabs](https://aka.ms/wip20161) to now have a default of displaying at most 5 tabs, rather than any recent tabs. If at any point you’d like to change this, you can under Settings > System > Multitasking.
* We’re exploring including a Web Browsing section [in the Settings header](https://docs.microsoft.com/windows-insider/archive/new-in-19H1#updated-settings-homepage), and Insiders may start to see this.
* Going forward only the currently active profile picture will display under Your Info in Settings.
* Based on feedback we’re turning off ESENT Warning Event ID 642.
* It’s now possible to select the new Microsoft Edge as your desired app in Assigned Access.
* We’ve updated Narrator so that now when using the Microsoft Pinyin IME, Narrator is able to distinguish candidate characters/words by providing detailed reading information.

## Build 20190
Windows 10 Insider Preview Build 20190 was released to the Dev Channel on [8/12/2020](https://blogs.windows.com/windowsexperience/2020/08/12/announcing-windows-10-insider-preview-build-20190/).

### New post-update experience
We know that it doesn’t always feel clear what changed with a major update, or even how you can learn about and try out new features and improvements. This means that updates can feel time consuming without real benefit to you, and we want to change that. We’re introducing a new first run experience via the Tips app that highlights the most exciting changes on your PC after a major Windows 10 feature update is installed. After installing this build, Insiders will see the Tips app is launched highlight some of the most recent new features from the latest Insider Preview builds in the Dev Channel. To see this experience on your device, make sure the “Show me the Windows welcome experience” checkbox in Settings > System > Notifications & actions is checked.

![The Tips app launches post-update to highlight new features from the latest Insider Preview builds.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/08/cb69036429ed8a259c5ed6e5da6b4153.png)

This experience will show up for Windows Insiders in EN locales such as US, UK, AU, IN, and CA.

__NOTE: The new post update experience with the Tips app mentioned with Build 20190 was a trial run for this experience to get feedback and gauge interest and specific only to Build 20190. You will not see this experience on newer builds. Insiders may see other experiences like this one on newer builds coming soon.__

### Improved Graphics Settings experience
While this isn’t a new feature all together, we have made significant changes based on customer feedback that will benefit our customers’ Graphics Settings experience. We have made the following improvements:

* __We’ve updated the Graphics Settings to allow users to specify a default high performance GPU.__
* __We’ve updated the Graphics Settings to allow users to pick a specific GPU on a per application basis.__

If you’re a power user that has multiple high performance GPUs and would like to specify which of those GPUs should be the one used for high performance uses cases, you can now do that by going to __Settings > System > Display > Graphics settings__ or __Settings > Gaming > Graphics settings__. What this means is that an application that asks for a high-performance GPU will by default use the high-performance GPU you specify on this page.

![Default high performance GPU selection page.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/08/16635566f758c021e6b341dfba58769d.jpg)

Now if you want even more control, we have also added the ability for you to specify exactly which GPU you want an app to run on using the new “Specific GPU” option. As you can see below, an application can be set to run on your GPU of choice.

![The new per-application specific GPU selection option.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/08/bfb6378b0d407e4d79ce6527c67c35bd.jpg)

## Build 20185
Windows 10 Insider Preview Build 20185 was released to the Dev Channel on [8/5/2020](https://blogs.windows.com/windowsexperience/2020/08/05/announcing-windows-10-insider-preview-build-20185/).

### Improving DNS configuration in Settings
We’re making a few changes to the Network section in Settings. 

__Making DNS settings more easily accessible:__ Editing your DNS server assignment is now a top-level option when you go into your network’s properties page.

__Encrypted DNS controls in the Settings app:__ Encrypted DNS (DNS over HTTPS, or DoH) [can help increase privacy and security while browsing the web](https://techcommunity.microsoft.com/t5/networking-blog/windows-insiders-can-now-test-dns-over-https/ba-p/138128). You can now configure DoH directly in the Settings app to more easily take advantage of this feature:

* For ethernet connections: Go to Settings > Network & Internet > Status. Click Properties, then select Edit IP assignment or Edit DNS server assignment and it will be available in the popup. 

* For Wi-Fi connections: Go to Settings > Network & Internet > Wi-Fi. Click the adapter properties link, then select Edit IP assignment or Edit DNS server assignment and it will be available in the popup. Currently you will not see the encryption options if you go to the individual network’s property page.

You can add any IP address listed here to unlock the DoH dropdown and choose to use encryption. Once encryption is enabled, you can confirm it’s working by looking at the applied DNS servers in the network properties and see them labeled as “(Encrypted)” servers. If you want to try a custom DoH server we don’t recognize yet, you can configure an IP address to be recognized as a DoH server by using the netsh command documented here at the end of the blog post.

![The new Edit Network DNS settings popup in Settings.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/08/7783c5f1f83fba22ff585bc2c57ac6fc.png)

### New ADMX Backed Policies for MDM
Starting with Windows 10 Insider Preview Build 20175, we have enabled 647 new MDM policies across 56 ADMX files to enable commercial customers to configure policies that are also supported through Group Policies. Contains ADMX based Policies such as App Compat, Event Forwarding, Servicing and Task Scheduler. These new policies can be configured using Intune custom profile. Intune UX is planned to be available later this year.

ADMX file name:

* AddRemovePrograms.admx
* AppCompat.admx
* AuditSettings.admx
* CipherSuiteOrder.admx
* COM.admx
* Cpls.admx
* CtrlAltDel.admx
* DigitalLocker.admx
* DnsClient.admx
* DWM.admx
* EncryptFilesonMove.admx
* EventForwarding.admx
* FileServerVSSProvider.admx
* FileSys.admx
* FolderRedirection.admx
* Help.admx
* HelpAndSupport.admx
* kdc.admx
* LanmanServer.admx
* LinkLayerTopologyDiscovery.admx
* MMC.admx
* MMCSnapins.admx
* MSAPolicy.admx
* nca.admx
* NCSI.admx
* Netlogon.admx
* OfflineFiles.admx
* PeerToPeerCaching.admx
* PerformanceDiagnostics.admx
* PreviousVersions.admx
* QOS.admx
* Reliability.admx
* Scripts.admx
* sdiageng.admx
* Securitycenter.admx
* Servicing.admx
* Setup.admx
* SharedFolders.admx
* Sharing.admx
* Shell-CommandPrompt-RegEditTools.admx
* Smartcard.admx
* Snmp.admx
* TaskScheduler.admxtcpip.admx
* Thumbnails.admx
* TPM.admx
* UserExperienceVirtualization.admx
* W32Time.admx
* WinCal.admx
* WindowsAnytimeUpgrade.admx
* WindowsConnectNow.admx
* WindowsMediaDRM.admx
* WindowsMediaPlayer.admx
* WindowsMessenger.admx
* WinInit.admx

### Changes and Improvements
* We’re moving the 3D Viewer app into the Windows Accessories folder in the Start menu all apps list.

## Build 20180
Windows 10 Insider Preview Build 20180 was released to the Dev Channel on [7/29/2020](https://blogs.windows.com/windowsexperience/2020/07/29/announcing-windows-10-insider-preview-build-20180/).

### Changes and Improvements
* Based on feedback, we’re changing the tablet posture logic for 2-in-1 devices to now only apply when using a single screen.
* Based on feedback we’re updating the new folder icon in the Start menu’s All app’s list to be a little smaller so it better aligns with the size of the other icons.
* We’ve updated the search box in the Default Apps settings pages to improve performance.

## Build 20175
Windows 10 Insider Preview Build 20175 was released to the Dev Channel on [7/22/2020](https://blogs.windows.com/windowsexperience/2020/07/22/announcing-windows-10-insider-preview-build-20175/).

### Improving pinned sites in Microsoft Edge
Earlier this month, we announced ALT + TAB between apps and sites, the first of our new productivity enhancements coming to Microsoft Edge on Windows 10. Today, we’re announcing another feature we’ve been working on to make you more efficient when browsing the web: quick access to tabs for your pinned sites. Clicking a pinned site on the Taskbar will now show you all of the open tabs for that site across any of your Microsoft Edge windows, just like you’d expect for any app with multiple open windows. Please let us know what you think!

![Selecting a pinned site on the Taskbar will now show you all of the open tabs for that site across any of your Microsoft Edge windows.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/07/f50733d9580bd7b17dd3b245952a8634.gif)

Clicking a pinned site on the Taskbar will now show you all of the open tabs for that site across any of your Microsoft Edge windows.

__This feature is currently rolling out to a subset of Insiders today and requires Microsoft Edge Insider Build 85.0.561.0 or higher (Canary or Dev Channel).__

NOTE: Since this is an early preview, existing sites on your Taskbar will not experience this new behavior until you remove and re-pin them.

For more details on our new multitasking improvements, [check out our post on the Microsoft Edge blog](https://blogs.windows.com/msedgedev/2020/07/22/multitasking-improvements-windows-10-microsoft-edge/).

### Introducing Reset-AppxPackage
For some time now, you’ve been able to reset your UWP apps in Settings – with today’s build we’re now exposing this ability via PowerShell as well. To do this, you’ll need the appx package name, so your use of the command may look like this:

>> Get-AppxPackage *calculator* | Reset-AppxPackage

The benefit of enabling this via PowerShell is that if needed you will now be able to run the reset commands for certain system components that are not currently listed as available to reset in Settings, for example Start.

Please note by nature of this command, if you choose to run it it will reset your experience back to the default experience and you will lose the associated app data.

### Make a more personal connection with Eye Contact on Surface Pro X
Powered by artificial intelligence capabilities of the Microsoft SQ1(TM) processor, Eye Contact helps to adjust your gaze on video calls so you appear to be looking directly in the camera on your Surface Pro X. Windows Insiders can turn this feature on via the Surface app on their Surface Pro X.

![Eye Contact helps to adjust your gaze on video calls so you appear to be looking directly in the camera on your Surface Pro X.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/07/7395420e4c7efa64b0fbff4552d9a54b-1024x796.png)

## Build 20170
Windows 10 Insider Preview Build 20170 was released to the Dev Channel on [7/15/2020](https://blogs.windows.com/windowsexperience/2020/07/15/announcing-windows-10-insider-preview-build-20170/).

### Improving your Sound Settings experience
Last week we mentioned we were planning on bringing more Control Panel capabilities forward into Settings, and here’s another one – we’re updating Settings > System > Sound > Manage sound devices to now let you know which device is default, and if not, enable you to set it as your default device or default communication device.

We’ve also updated the volume mixer to include a link to the per app audio settings, which you can use to redirect audio endpoints per app.

There is more work on the way in this area – stay tuned!

### Changes and Improvements
* As part of our ongoing efforts [to update the iconography across Windows](https://medium.com/microsoft-design/iconic-icons-designing-the-world-of-windows-5e70e25e5416), Insiders will notice we’re introducing a new Settings icon in this build. The new Settings icon looks great on the Start menu with the theme-aware tiles [introduced in Build 20161](https://blogs.windows.com/windowsexperience/2020/07/01/announcing-windows-10-insider-preview-build-20161/)!
The new Settings icon as it will appear on Start with theme-aware tiles. 
![New Settings icon with theme-aware tiles on Start.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/07/48b8ca797ac8591eb4e6f8532915f91e-1024x314.png)
* While we work on improving reliability, we’re temporarily turning off Notepad’s ability to persist open windows across restarts and updates.
* An experimental implementation of Transport Layer Security (TLS) 1.3 is enabled by default starting with Insider Preview Build 20170. IIS/HTTP.SYS have TLS 1.3 enabled by default. SSPI callers can use TLS 1.3 by passing the new crypto-agile [SCH_CREDENTIALS](https://docs.microsoft.com/windows/win32/api/schannel/ns-schannel-sch_credentials) structure when calling [AcquireCredentialsHanlde](https://docs.microsoft.com/windows/win32/secauthn/acquirecredentialshandle--schannel). SSPI callers using TLS 1.3 need to make sure their code correctly handles [SEC_I_RENEGOTIATE](https://docs.microsoft.com/windows/win32/secauthn/recognizing-a-request-to-renegotiate-a-connection).

## Build 20161
Windows 10 Insider Preview Build 20161 was released to the Dev Channel on [7/1/2020](https://blogs.windows.com/windowsexperience/2020/07/01/announcing-windows-10-insider-preview-build-20161/).

### Theme-aware tiles in Start
We are freshening up the Start menu with a more streamlined design that removes the solid color backplates behind the logos in the apps list and applies a uniform, partially transparent background to the tiles. This design creates a beautiful stage for your apps, especially the Fluent Design icons for Office and Microsoft Edge, as well as the redesigned icons for built-in apps like Calculator, Mail, and Calendar that we started rolling out earlier this year.

![Theme-aware tiles on the Start menu.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/07/dabfa329dfacdc1a2669002649ed75d6.gif)

This refined Start design looks great in both dark and light theme, but if you’re looking for a splash of color, first make sure to turn on Windows dark theme and then toggle “Show accent color on the following surfaces” for “Start, taskbar, and action center” under __Settings > Personalization > Color__ to elegantly apply your accent color to the Start frame and tiles.

### ALT + TAB between apps and sites
Are you a multitasker? We have exciting news for you! Beginning with today’s build, all tabs open in Microsoft Edge will start appearing in Alt + TAB, not just the active one in each browser window. We’re making this change so you can quickly get back to whatever you were doing—wherever you were doing it.

![ALT + TAB between apps and sites.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/07/634dd641ac5d268c671631222138c910.gif)

If you’d prefer fewer tabs or the classic Alt + TAB experience, we’ve added some settings for you under __Settings > System > Multitasking__. You can configure Alt + Tab to only show your last three or five tabs or choose to turn this feature off completely.

__This feature is currently rolling out to a subset of Insiders today in the Dev Channel and requires a Canary or Dev build of Microsoft Edge (version 83.0.475.0 or higher).__

This is just the beginning of productivity enhancements coming to Microsoft Edge—stay tuned!

### A more personalized Taskbar for new users
We want to help customers get the most out of their PCs from day one, and that starts with offering a cleaner, more personalized, out-of-box experience to give you the content you want and less clutter. This provides us with a flexible, cloud-driven infrastructure to test customer reception of default Taskbar content and tailor these layouts based on user and device signal.

We will evaluate the performance of individual default properties, monitoring diagnostic data and user feedback to assess an audience’s reception. Using this information, we will tune default layouts to minimize clutter and perceptions of bloatware.

__Please note that this experience is limited to new account creation or first logon scenarios. We will not use Programmable Taskbar to alter the Taskbar layout on existing accounts.__

![A more personalized Taskbar for new users.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/07/2a484fd68334970e192f8a1138aedc73-1536x635.jpg)

### Improving the notification experience
We are making some changes to improve the notifications experience in Windows 10.

First, know where your toast is coming from by checking out the app logo at the top. Done with the notification? Select the X on the top right corner to quickly dismiss and move on with your life.

![See where your notification toast is coming from by checking out the app logo at the top and quicklt dismiss by selecting the X on the top right corner.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/07/5db65c59e8b5b819bd9203996bf7b8c3.png)

And second, we are turning off the Focus Assist notification and summary toast by default, so we will no longer let users know that Focus Assist has been turned on through an automatic rule via a notification. This can be changed back to the previous behavior via Settings.

### Making Settings even better
We’re continuing to work on bringing capabilities from Control Panel forward into Settings. As part of this ongoing effort, we are migrating information found in Control Panel’s System page into the Settings About page under __Settings > System > About__. Links that would open the System page in Control Panel will now direct you to About in Settings. We are also bringing new improvements like making your device information copyable and streamlining the security information shown. And don’t worry—if you’re looking for more advanced controls that lived in the System page in Control Panel, you can still get to them from the modern About page if you need them!

![We are migrating information found in Control Panel’s System page into the Settings About page under Settings > System > About.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/07/329ddd5b6ac1257e88fbc73d79d9e7a9-1536x1112.png)

There will be more improvements coming that will further bring Settings closer to Control Panel. If you rely on settings that only exist in Control Panel today, please file feedback and let us know what those settings are.

### Improving the tablet experience for 2-in-1 devices
Previously, when detaching the keyboard on a 2-in-1 device, a notification toast would appear asking if you wanted to switch into tablet mode. If you selected yes, you would switch into tablet mode. If you chose no, it would give you the new tablet posture experience [introduced in the May 2020 Update](https://docs.microsoft.com/windows-insider/archive/new-in-20H1#introducing-a-new-tablet-experience-for-2-in-1-convertible-pcs-build-18970) (or simply the desktop on earlier versions of Windows 10). We are further updating this experience by changing the default, so that this notification toast no longer appears and instead will switch you directly into the new tablet experience, with some improvements for touch. You can change this setting by going to Settings > System > Tablet. Some users may have already seen this change on Surface devices.

And to address confusion with some users getting stuck in tablet mode on non-touch devices, we are removing the tablet mode quick action on non-touch devices.

In addition, new logic is incorporated to let users boot into the appropriate mode according to the mode they were last in and whether the keyboard is attached or not.

## Build 20152
Windows 10 Insider Preview Build 20152 was released to the Dev Channel (Fast ring) on [6/24/2020](https://blogs.windows.com/windowsexperience/2020/06/24/announcing-windows-10-insider-preview-build-20152/).

## Build 20150
Windows 10 Insider Preview Build 20150 was released to the Dev Channel (Fast ring) on [6/17/2020](https://blogs.windows.com/windowsexperience/2020/06/17/announcing-windows-10-insider-preview-build-20150/).

### Three new Windows Subsystem for Linux (WSL) features: GPU compute, WSL install, and WSL update
This build contains three new exciting WSL features. The first is GPU compute: a feature that allows your Linux binaries to leverage your GPU, which makes it possible to do more machine learning development and data science workflows directly in WSL. Secondly, we’ve added a new command: `wsl –install` which allows you to install WSL with just one command. Lastly, we’ve added `wsl –update` which gives you the ability to easily manage the Linux kernel version used by WSL 2 distros. To view a summary of these announcements [please read this post on the Windows Command line blog](https://devblogs.microsoft.com/commandline/gpu-compute-wsl-install-and-wsl-update-arrive-in-the-windows-insiders-fast-ring-for-the-windows-subsystem-for-linux), and for in-depth details on GPU compute in WSL please [read this post](https://blogs.windows.com/windowsdeveloper/?p=55781) on the Windows Developer blog.

![GPU Compute via WSL.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/06/3d39cf80787a7208278a716ceb76d29a.gif)

### General changes & improvements
* With this week’s build, we’ll be starting to roll out [the new search box on the default app settings pages](https://blogs.windows.com/windowsexperience/2020/04/15/announcing-windows-10-insider-preview-build-19608/). As part of this, we’ve done some work to improve the performance of the search box.
* [The new Korean IME](https://blogs.windows.com/windowsexperience/2019/12/16/announcing-windows-10-insider-preview-build-19536/) is now available again for Insiders to use.
* Based on feedback, we’re updating the text of the Settings > Privacy > Location page to clarify that the icon displayed when your location is being used will be displayed in the taskbar.

## Build 19645
Windows 10 Insider Preview Build 19640 was released to the Fast ring on [6/10/2020](https://blogs.windows.com/windowsexperience/2020/06/10/announcing-windows-10-insider-preview-build-19645/).

### General changes & improvements
* We changed the servicing model for the Linux kernel inside of Windows Subsystem for Linux 2 distributions. This build includes this change to remove the Linux kernel from the Windows image, and instead have it be serviced via Microsoft Update, the same way that 3rd party drivers (like graphics, or touchpad drivers) are installed and updated on your machine today. For full details [please read this blog post on the Windows Command Line blog](https://devblogs.microsoft.com/commandline/wsl2-will-be-generally-available-in-windows-10-version-2004/) and for information about the kernel version please [view the kernel docs page here](https://docs.microsoft.com/windows/wsl/kernel-release-notes).
* Support for [Nested Virtualization](https://docs.microsoft.com/virtualization/hyper-v-on-windows/user-guide/nested-virtualization) on AMD processors is now available. Being an early release we recommend you [read this blog post](https://techcommunity.microsoft.com/t5/virtualization/amd-nested-virtualization-support/ba-p/1434841) for details on what platforms currently work as well as how to enable the feature.

## Build 19640
Windows 10 Insider Preview Build 19640 was released to the Fast ring on [6/3/2020](https://blogs.windows.com/windowsexperience/2020/06/03/announcing-windows-10-insider-preview-build-19640/).

## Build 19635
Windows 10 Insider Preview Build 19635 was released to the Fast ring on [5/28/2020](https://blogs.windows.com/windowsexperience/2020/05/28/announcing-windows-10-insider-preview-build-19635/).

## Build 19631
Windows 10 Insider Preview Build 19631 was released to the Fast ring on [5/21/2020](https://blogs.windows.com/windowsexperience/2020/05/21/announcing-windows-10-insider-preview-build-19631/).

### General changes & improvements
* We updated the configuration of Windows Hello to make sure it works well with 940nm wavelength cameras.

## Build 19628
Windows 10 Insider Preview Build 19628 was released to the Fast ring on [5/13/2020](https://blogs.windows.com/windowsexperience/2020/05/13/announcing-windows-10-insider-preview-build-19628/).

### General changes & improvements
* We’re adding initial support for DNS over HTTPS, so that you can opt into using encryption when Windows makes DNS queries. [Follow the instructions in this blog post](https://techcommunity.microsoft.com/t5/networking-blog/windows-insiders-can-now-test-dns-over-https/ba-p/1381282) to opt in as it will be off by default.
* Thanks everyone who shared feedback about the updated version of Korea Microsoft IME introduced with Build 18941. For the moment, the IME version will be returning to the previous one while we take your feedback into consideration.

## Build 19624
Windows 10 Insider Preview Build 19624 was released to the Fast ring on [5/6/2020](https://blogs.windows.com/windowsexperience/2020/05/06/announcing-windows-10-insider-preview-build-19624/).

### General changes & improvements
* We’re temporarily turning off the new search box in the default apps Settings pages while we work on improving performance and reliability.
* We’re updating the VPN connection logic based on feedback, so that if you disconnect from a VPN network, it will now uncheck the option to auto-connect (similar to how it’s handled for Wi-Fi).
* Based on feedback we’re updating the text of the Add a Device dialog so the list of examples under Bluetooth includes controllers.
* We’re updating the Optional Updates Available section that appears in Windows Update settings, so that you will now be able to copy the text in case you need it.

## Build 19619
Windows 10 Insider Preview Build 19619 was released to the Fast ring on [4/29/2020](https://blogs.windows.com/windowsexperience/2020/04/29/announcing-windows-10-insider-preview-build-19619/).

### General changes & improvements
* If the Sync button under Settings > Time & Language > Time fails due to network connectivity, the error now tells you that’s the issue.

## Build 19613
Windows 10 Insider Preview Build 19613 was released to the Fast ring on [4/22/2020](https://blogs.windows.com/windowsexperience/2020/04/22/announcing-windows-10-insider-preview-build-19613/).

## Build 19608
Windows 10 Insider Preview Build 19608 was released to the Fast ring on [4/15/2020](https://blogs.windows.com/windowsexperience/2020/04/15/announcing-windows-10-insider-preview-build-19608/).

### Improving your default apps experience
Over the years, we’ve made a number of improvements to Settings based on your feedback, and we’re happy to share the next one is starting to roll out. We’re adding the ability to search the lists of file types, protocols, and apps when setting a default.

![Showing the Choose default apps by file type Settings window, now with a search box.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/04/bc885b7c284ce0a6d23eb6a909890cdd.png)

This change is currently available for 50% of Insiders in the Fast ring as we evaluate the quality. We’ll let you know when that rollout increases. Please give it a try once it’s available on your device, and let us know what improvements you’d like to see next!

## Build 19603
Windows 10 Insider Preview Build 19603 was released to the Fast ring on [4/8/2020](https://blogs.windows.com/windowsexperience/2020/04/08/announcing-windows-10-insider-preview-build-19603/).

### File Explorer Integration in the Windows Subsystem for Linux (WSL)
If you have WSL installed and open up File Explorer, you’ll see a familiar face!

![Pointing out the Linux entry in the File Explorer navigation pane.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/04/a115bf3a1a66ef9a9a76190839835e4c.png)

[We’ve had the ability to access your Linux files since Windows 10 version 1903](https://devblogs.microsoft.com/commandline/whats-new-for-wsl-in-windows-10-version-1903/), but now you can easily get to them from your left-hand navigation pane in File Explorer. Selecting the Linux icon will show you a view of all your distros, and selecting those will place you in the Linux root file system for that distro.

![Showing the folders under the Linux section in File Explorer.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/04/834929eb91b182277df7061b7ce9333a.jpg)

### User cleanup recommendations in Storage Settings
Free up disk space with this Storage Settings feature that gathers unused files and apps so you can digitally cleanse your device.

![Find User cleanup recommendations in the Storage Settings page.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/04/a061c6428b4ed25b7ecba3738744a6ae.png)

Windows cannot predict whether you want to delete personal files, uninstall apps, or remove local copies of files synced to the cloud. With this tool, all the content is gathered in one page and removable by you with a few clicks.

![User cleanup recommendations is made up of 4 sections: Temporary files, Large or unused files, Files synced to the cloud and Unused apps.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/04/c74dc6e055fe56a9832899f6ca8e6995.png)

### General changes & improvements
* Going forward, services that are implemented by binaries residing in the user profiles will be persisted on upgrades.
* Narrator will no longer automatically enable scan mode when interacting with the Ideas pane in Excel. In the new Microsoft Edge, Narrator now automatically enables scan mode and starts reading webpages.

## Build 19592
Windows 10 Insider Preview Build 19592 was released to the Fast ring on [3/25/2020](https://blogs.windows.com/windowsexperience/2020/03/25/announcing-windows-10-insider-preview-build-19592/).

### Tablet posture improvements for 2-in-1 convertible PCs
We are beginning to roll out (again*) the new tablet experience for 2-in-1 convertible PCs as a preview to some Windows Insiders in the Fast ring. This experience is separate from the Tablet Mode experience that you will still be able to use. This new experience allows users entering tablet posture to stay in the familiar desktop experience without interruption with a few key touch improvements:

* Taskbar icons are spaced out
* Search box on taskbar is collapsed into icon-only mode
* Touch keyboard auto invokes when you tap a text field
* File explorer elements will have a little more padding, to make them comfortable to interact with using touch
* You’ll also notice we’ve updated some of the related Tablet settings under Settings > System, so as to give you control over the experience.

![Tablet posture improvements for 2-in-1 convertible PCs.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/03/068d5e0abaf805d92a03526f7e208e88.jpg)

In order to help ensure quality, the feature will be rolling out slowly, starting with a portion of the Insiders that have never detached their keyboard before, or have their tablet mode settings set to __Don’t ask me and don’t switch__.

We’d love to hear your feedback about the experience:

1. Use your convertible PC with apps as you normally would.
2. When you’re ready to pick it up and go or simply lean back on the couch, you can fold back the keyboard or remove it altogether.
3. Use your device as a tablet with touch, without going into Tablet Mode.
4. Screenshot showing improvements to tablet posture, like collapsed search, increased spacing between icons, and a touch keyboard option in your Taskbar.

>[!NOTE] 
>This feature was previously rolled out as an experiment to Windows Insiders in 20H1 Build 18970 and ended in Build 19013. After some refinement, we’re reintroducing it to Windows Insiders in this build and plan to deliver this experience to customers in a future Windows 10 update.

### General changes & improvements
* The Windows Search Platform (Indexer) has been updated with improved logic to help find better times to perform indexing of your files and avoiding heavily indexing while you are using your machine. An improvement was also made to significantly limit the amount of times the service indexes your files for content that doesn’t have an impact on search experiences, and gives you a better experience on Windows.

## Build 19587
Windows 10 Insider Preview Build 19587 was released to the Fast ring on [3/18/2020](https://blogs.windows.com/windowsexperience/2020/03/18/announcing-windows-10-insider-preview-build-19587/).

### General changes & improvements
* Based on feedback, when you have muted your volume, the volume will now not unmute when using the hardware keyboard volume keys until you raise the volume (or manually unmute).
* We made a couple of improvements to Narrator and how it works with some of the controls in Windows:
    * Narrator now uses a more friendly string to describe the audio output in the Select playback device dropdown menu in the volume flyout.
    * Narrator now announces more information in the Add Bluetooth or other devices dialog in the Settings application when first opened.

## Build 19582
Windows 10 Insider Preview Build 19582 was released to the Fast ring on [3/12/2020](https://blogs.windows.com/windowsexperience/2020/03/12/announcing-windows-10-insider-preview-build-19582/).

### Eye Control Improvements
Eye Control enables users to interact with Windows using only their eyes. Based on feedback, with this build, we’re updating the Eye Control settings to now span multiple pages, in order to give the options a bit more room to breathe.

![Updated Eye Control Settings that span multiple pages.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/03/d39bb5a9d70f13c8c4ae23340e4aa927.png)

To get started with Eye Control, connect a supported eye tracking device, then [follow the steps here](https://support.microsoft.com/help/4043921/windows-10-get-started-eye-control).

### General changes & improvements
* We’re working on giving you control over whether apps can disable the screen capture border. The page isn’t finished being wired up yet, but you’ll see it listed under Privacy Settings.
* We’ve updated the “set time zone automatically” toggle in Time & Date settings to now be greyed out if location has been disabled.
* Based on feedback, we’re updating the Scottish Gaelic keyboard in these ways:
    * Pressing AltGR + 7 will now input ⁊ (U+204A TIRONIAN SIGN ET).
    * Pressing ‘ will now directly insert that character (right single quote).
    * Pressing AltGr +’ will now act as a dead key to combine an acute accent with a subsequent letter.

## Build 19577
Windows 10 Insider Preview Build 19577 was released to the Fast ring on [3/5/2020](https://blogs.windows.com/windowsexperience/2020/03/05/announcing-windows-10-insider-preview-build-19577/).

### Diagnostic data changes in Settings
As part of the Microsoft initiative to increase transparency and control over data, we’re making some changes to the Settings app and Group Policy settings that will start showing up in Windows Insider builds this month. Basic diagnostic data is now known as Required diagnostic data and Full diagnostic data is now Optional diagnostic data. If you’re a commercial customer and choose to send Optional diagnostic data, we will also be providing more granular Group Policy settings to configure the data that’s collected within your organization. We’ll publish more specifics around the new policies when we get closer to the retail release, and in the meantime, check out the Microsoft Privacy Report for more information around our data collection practices.

__Note: Please make sure your device is set to “Full” before updating to Build 19577. You will not be able to take future flights if your diagnostic level is left at “Enhanced”. AAD/Domain-joined PCs set to “Enhanced” will be blocked from taking Build 19577. For more information, [see this Answers post](https://aka.ms/ddchanges).__

### More new icons: Windows Security
We’re continuing to roll out updated icons to many of the built-in apps in Windows 10. In today’s build, we’ve updated the Windows Security icon to match the new design principles outlined here from the Microsoft Design Team. Unlike many of the built-in apps in Windows 10, which can be updated through the Store, the new Windows Security icon is updated through the OS and will rollout in a future Windows 10 feature update.

![The new Windows Security icon as it appears on the taskbar.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/03/254a7cea7eb9aed8586fc445faeaa227.png)

### General changes & improvements
* Following up on [our post about the new Cortana app](https://insider.windows.com/articles/cortana-windows-beta/), we wanted to let you know that in addition to timers and instant answers, which lit up last month, assistant conversations are now online. Some examples to try are “tell me a dad joke”, “tell me a bedtime story”, or “rock, paper, scissors.” We appreciate your patience while we worked on this. This is a server-side change, however we’re noting it here for awareness.
* We’ve updated the behavior of Advanced startup (Settings > Update & Security > Recovery > Advanced startup “Restart now”) to enable some Ease of Access features to work properly. For example, previously, if the narrator feature was enabled prior to launching Advanced startup, it would stop working. Now, Advanced startup will reboot directly into the Windows Recovery Environment.
* While the Vietnamese alphabet doesn’t include the Latin letters F, J, W, or Z, based on feedback we’re updating the grouping in the Start menu’s all app’s list to account for these letters when using this display language, so that apps like Windows PowerShell are included in the expected group.

## Build 19569
Windows 10 Insider Preview Build 19569 was released to the Fast ring on [2/20/2020](https://blogs.windows.com/windowsexperience/2020/02/20/announcing-windows-10-insider-preview-build-19569/).

### Evolving the Windows 10 icons
We are currently working on a multi-year effort across Microsoft’s design teams to redesign the icons across all our products. We started with the Office icons, and now we’re moving forward with updating the icons in Windows 10, starting with the built-in apps like Alarms & Clock, Calculator, Mail, and Calendar. Research and feedback from Windows Insiders showed a desire to see consistency in design and connection to the brand, with enough differences to aid in recognition. You can read all about our approach to updating the icons in Windows 10 in this Medium post from the Microsoft Design Team!

![View of updated design for web preview in search results.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/02/7e4667f9c9e488683aca797991b5a747.png)

Many of these icons will be updated as app updates from the Microsoft Store. We are beginning to roll them out to Windows Insiders in the Fast ring first, starting today. The Mail and Calendar icons rolled out this morning to Release Preview. Over the coming months, Insiders will see more of the icons in Windows 10 get updated with new designs!

## Build 19564
Windows 10 Insider Preview Build 19564 was released to the Fast ring on [2/12/2020](https://blogs.windows.com/windowsexperience/2020/02/12/announcing-windows-10-insider-preview-build-19564/).

### Graphics Settings Improvements
We’ve updated the Graphics settings page (Settings > System > Display > Graphics settings), allowing for better control over designating which GPU your apps run on. With this update, the app list and GPU preference are pre-populated on a best effort basis to improve the default preference management experience. If your desired app isn’t pre-populated, you can still add it by using the app selection drop-down.

![The updated Graphics settings page with pre-populated app preference management.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/02/ab377b0f73f0fd7001039bc50d2681ff.jpg)

You’ll notice alongside this, we’ve also added a search box and a filter for the list of apps.

## Build 19559
Windows 10 Insider Preview Build 19559 was released to the Fast ring on [2/5/2020](https://blogs.windows.com/windowsexperience/2020/02/05/announcing-windows-10-insider-preview-build-19559/).

### General changes & improvements 
* For any of our Insiders using an arm64 device, such as the Surface Pro X, running Enterprise or Pro edition, you’ll now be able to see and install Hyper-V features.

## Build 19555
Windows 10 Insider Preview Build 19551 was released to the Fast ring on [1/30/2020](https://blogs.windows.com/windowsexperience/2020/01/30/announcing-windows-10-insider-preview-build-19555/).

## Build 19551
Windows 10 Insider Preview Build 19551 was released to the Fast ring on [1/23/2020](https://blogs.windows.com/windowsexperience/2020/01/23/announcing-windows-10-insider-preview-build-19551/).

## Build 19546
Windows 10 Insider Preview Build 19546 was released to the Fast ring on [1/16/2020](https://blogs.windows.com/windowsexperience/2020/01/16/announcing-windows-10-insider-preview-build-19546/).

## Build 19541
Windows 10 Insider Preview Build 19541 was released to the Fast ring on [1/8/2020](https://blogs.windows.com/windowsexperience/2020/01/08/announcing-windows-10-insider-preview-build-19541/).

### Location in-use icon update
As some keen eyed Insiders have noticed, we’ve updated the notification area icon for when an app is using your location. The new icon looks like this:

![Showing the new arrow icon for location in use.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/01/f3b5ee974cf44250d484db25447cce28.png)

### Showing architecture in Task Manager
When you’re using the Details tab in Task Manager, we’ve added a new option to show the architecture of each process. If you’re interested, you can add it by right-clicking on a column header, choosing Select Columns, and selecting Architecture from the list.

![When you're in the Details tab of Task Manager, you can now add this Architecture option.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/01/5cd3aaadea5f925716341c53a4b89b20.png)

## Build 19536
Windows 10 Insider Preview Build 19536 was released to the Fast ring on [12/16/2019](https://blogs.windows.com/windowsexperience/2019/12/16/announcing-windows-10-insider-preview-build-19536/).

### Optional Drivers
[We’re still working on making it easier for you to see all optional updates](https://aka.ms/wip18985) (including drivers, feature updates, and monthly non-security quality updates) in one place. When optional updates are detected, they will be listed under Settings > Update & Security > Windows Update > View optional updates.

For drivers, you no longer need to browse Device Manager for a specific device to update. Windows Update will automatically keep your drivers up to date, but if you’re having a problem, one of those optional drivers might help.

View optional updates option in the Windows Update section of Update & Security Settings.

### Re-releasing the updated Korean IME
During 19H1 development, we’d started work on an updated version of the Korean IME as part of our ongoing efforts to modernize and improve your typing experience in Windows. Based on feedback, we decided not to ship this with 19H1, and instead worked on further improving the experience first. With Build 19536, we’re re-releasing the updated IME, along with some improvements that help it work better with various apps.

To recap the most noticeable changes included as part of this IME work:

* For those who’re familiar with typing in Korean when writing in Hanja, we have a new candidate selection window that uses modern controls and clearer typography:

![Showing the candidate selection window of the updated Korean IME.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2019/12/17baa87bb553ab0d1bc9f5de682d3a7d.png)

* The new IME version also comes with an updated algorithm used for text prediction when writing Korean using the touch keyboard. Text suggestions should now be more accurate and relevant to what you are writing.

### Family group setup
[Microsoft has family features that span across multiple platforms](https://account.microsoft.com/family/about), like Windows, Xbox, and Android. On Windows, you can set things up for your family, like screen time limits, content filters, have kids ask before they buy things, or even stay organized with a shared family calendar, OneNote, and Office 365 Home subscription. If you share a device with family, it’s easy to get their account set up in a family group to take advantage of all these features.

![New Who will use this device screen when setting up a new Windows 10 PC.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2019/12/df545e6188f866eee1db8f9f73382240.png)

In this build, we want to help customers set up their device to be used by multiple people in their family. While we’re not releasing an ISO for this build, some Insiders who choose to reset their PC may see a screen during setup that asks who’ll be using the device. If they select People in my family, we’ll help them get set up in a family group once they get to their desktop, so that they’re ready to get started with all the features.

If you see this new page, let us know what you think by going to Security and Privacy > Child accounts and family settings in the Feedback Hub.
