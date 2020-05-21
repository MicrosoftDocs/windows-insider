---
title: The Changelog
description: New Windows 10 features for Insider Preview builds in the Fast ring
author: lizap
manager: dougkim
ms.tgt_pltfrm: na
ms.devlang: na
ms.author: elizapo
ms.localizationpriority: medium
ms.topic: article
ms.prod: w10
---

# The Changelog

The Changelog represents everything new from all the builds from the Active Developmemnt Branch (RS_PRELEASE) released to the Fast ring. 

>[!NOTE]
> This page includes everything noted as part of the "What's new" and "General changes & improvements" sections of the blog posts published for each build [on the Windows Blog](https://blogs.windows.com/windowsexperience/tag/windows-insider-program/) and does not contain other noted updates for Insiders, fixes, or known issues. 

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

![Choose app defaults](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/04/bc885b7c284ce0a6d23eb6a909890cdd.png "Showing the Choose default apps by file type Settings window, now with a search box.")

This change is currently available for 50% of Insiders in the Fast ring as we evaluate the quality. We’ll let you know when that rollout increases. Please give it a try once it’s available on your device, and let us know what improvements you’d like to see next!

## Build 19603
Windows 10 Insider Preview Build 19603 was released to the Fast ring on [4/8/2020](https://blogs.windows.com/windowsexperience/2020/04/08/announcing-windows-10-insider-preview-build-19603/).

### File Explorer Integration in the Windows Subsystem for Linux (WSL)
If you have WSL installed and open up File Explorer, you’ll see a familiar face!

![Linux in File Explorer](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/04/a115bf3a1a66ef9a9a76190839835e4c.png "Pointing out the Linux entry in the File Explorer navigation pane.")

[We’ve had the ability to access your Linux files since Windows 10 version 1903](https://devblogs.microsoft.com/commandline/whats-new-for-wsl-in-windows-10-version-1903/), but now you can easily get to them from your left-hand navigation pane in File Explorer. Selecting the Linux icon will show you a view of all your distros, and selecting those will place you in the Linux root file system for that distro.

![Linux in File Explorer](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/04/834929eb91b182277df7061b7ce9333a.jpg "Showing the folders under the Linux section in File Explorer.")

### User cleanup recommendations in Storage Settings
Free up disk space with this Storage Settings feature that gathers unused files and apps so you can digitally cleanse your device.

![User Cleanup](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/04/a061c6428b4ed25b7ecba3738744a6ae.png "Find User cleanup recommendations in the Storage Settings page.")

Windows cannot predict whether you want to delete personal files, uninstall apps, or remove local copies of files synced to the cloud. With this tool, all the content is gathered in one page and removable by you with a few clicks.

![User Cleanup](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/04/c74dc6e055fe56a9832899f6ca8e6995.png "User cleanup recommendations is made up of 4 sections: Temporary files, Large or unused files, Files synced to the cloud and Unused apps.")

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

![Tablet Posture Improvements](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/03/068d5e0abaf805d92a03526f7e208e88.jpg "Tablet posture improvements for 2-in-1 convertible PCs.")

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

![Updated Eye Control Settings](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/03/d39bb5a9d70f13c8c4ae23340e4aa927.png "Updated Eye Control Settings that span multiple pages.")

To get started with Eye Control, connect a supported eye tracking device, then [follow the steps here](https://support.microsoft.com/en-us/help/4043921/windows-10-get-started-eye-control).

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

![New Windows Security icon](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/03/254a7cea7eb9aed8586fc445faeaa227.png "The new Windows Security icon as it appears on the taskbar.")

### General changes & improvements
* Following up on [our post about the new Cortana app](https://insider.windows.com/en-us/articles/cortana-windows-beta/), we wanted to let you know that in addition to timers and instant answers, which lit up last month, assistant conversations are now online. Some examples to try are “tell me a dad joke”, “tell me a bedtime story”, or “rock, paper, scissors.” We appreciate your patience while we worked on this. This is a server-side change, however we’re noting it here for awareness.
* We’ve updated the behavior of Advanced startup (Settings > Update & Security > Recovery > Advanced startup “Restart now”) to enable some Ease of Access features to work properly. For example, previously, if the narrator feature was enabled prior to launching Advanced startup, it would stop working. Now, Advanced startup will reboot directly into the Windows Recovery Environment.
* While the Vietnamese alphabet doesn’t include the Latin letters F, J, W, or Z, based on feedback we’re updating the grouping in the Start menu’s all app’s list to account for these letters when using this display language, so that apps like Windows PowerShell are included in the expected group.

## Build 19569
Windows 10 Insider Preview Build 19569 was released to the Fast ring on [2/20/2020](https://blogs.windows.com/windowsexperience/2020/02/20/announcing-windows-10-insider-preview-build-19569/).

### Evolving the Windows 10 icons
We are currently working on a multi-year effort across Microsoft’s design teams to redesign the icons across all our products. We started with the Office icons, and now we’re moving forward with updating the icons in Windows 10, starting with the built-in apps like Alarms & Clock, Calculator, Mail, and Calendar. Research and feedback from Windows Insiders showed a desire to see consistency in design and connection to the brand, with enough differences to aid in recognition. You can read all about our approach to updating the icons in Windows 10 in this Medium post from the Microsoft Design Team!

![New icon designs](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/02/7e4667f9c9e488683aca797991b5a747.png "view of updated design for web preview in search results")

Many of these icons will be updated as app updates from the Microsoft Store. We are beginning to roll them out to Windows Insiders in the Fast ring first, starting today. The Mail and Calendar icons rolled out this morning to Release Preview. Over the coming months, Insiders will see more of the icons in Windows 10 get updated with new designs!

## Build 19564
Windows 10 Insider Preview Build 19564 was released to the Fast ring on [2/12/2020](https://blogs.windows.com/windowsexperience/2020/02/12/announcing-windows-10-insider-preview-build-19564/).

### Graphics Settings Improvements
We’ve updated the Graphics settings page (Settings > System > Display > Graphics settings), allowing for better control over designating which GPU your apps run on. With this update, the app list and GPU preference are pre-populated on a best effort basis to improve the default preference management experience. If your desired app isn’t pre-populated, you can still add it by using the app selection drop-down.

![Updated graphics settings](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/02/ab377b0f73f0fd7001039bc50d2681ff.jpg "The updated Graphics settings page with pre-populated app preference management.")

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

![New location arrow icon](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/01/f3b5ee974cf44250d484db25447cce28.png "Showing the new arrow icon for location in use.")

### Showing architecture in Task Manager
When you’re using the Details tab in Task Manager, we’ve added a new option to show the architecture of each process. If you’re interested, you can add it by right-clicking on a column header, choosing Select Columns, and selecting Architecture from the list.

![Task Manager Architecture](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/01/5cd3aaadea5f925716341c53a4b89b20.png "When you're in the Details tab of Task Manager, you can now add this Architecture option.")

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

![Korean IME](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2019/12/17baa87bb553ab0d1bc9f5de682d3a7d.png "Showing the candidate selection window of the updated Korean IME.")

* The new IME version also comes with an updated algorithm used for text prediction when writing Korean using the touch keyboard. Text suggestions should now be more accurate and relevant to what you are writing.

### Family group setup
[Microsoft has family features that span across multiple platforms](https://account.microsoft.com/family/about), like Windows, Xbox, and Android. On Windows, you can set things up for your family, like screen time limits, content filters, have kids ask before they buy things, or even stay organized with a shared family calendar, OneNote, and Office 365 Home subscription. If you share a device with family, it’s easy to get their account set up in a family group to take advantage of all these features.

![Who OOBE page](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2019/12/df545e6188f866eee1db8f9f73382240.png "New Who will use this device screen when setting up a new Windows 10 PC.")

In this build, we want to help customers set up their device to be used by multiple people in their family. While we’re not releasing an ISO for this build, some Insiders who choose to reset their PC may see a screen during setup that asks who’ll be using the device. If they select People in my family, we’ll help them get set up in a family group once they get to their desktop, so that they’re ready to get started with all the features.

If you see this new page, let us know what you think by going to Security and Privacy > Child accounts and family settings in the Feedback Hub.
