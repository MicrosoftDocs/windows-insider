---
ms.date: 10/07/2019
title: What was new in 19H2 Windows 10 Insider Preview Builds
description: What was new in 19H2 preview builds
author: bleblanc
manager: dougkim
ms.tgt_pltfrm: na
ms.devlang: na
ms.author: allieshields
ms.localizationpriority: medium
ms.topic: article
ms.prod: w10
---

# What was new in 19H2 Windows 10 Insider Preview Builds
The Windows Insider Program lets you preview builds of the upcoming release of Windows 10. This lists all of the Windows 10 features for you to try in 19H2. 

The next feature update for Windows 10 will be a scoped set of features for select performance improvements, enterprise features, and quality enhancements. To deliver these updates in a less disruptive fashion, we will deliver this feature update in a new way, using servicing technology (like the monthly update process) for customers running the May 2019 Update who choose to update to the new release. For more details on how we will be releasing this feature update–[please read this blog post from John Cable](https://blogs.windows.com/windowsexperience/2019/07/01/evolving-windows-10-servicing-and-quality-the-next-steps/).

The following new features are being introduced as part of this update.

- This update will be published to WSUS so that customers can deploy and manage Insider Preview builds alongside their standard ConfigMan/WSUS approach. [See this blog post for details](https://techcommunity.microsoft.com/t5/Windows-IT-Pro-Blog/Publishing-pre-release-Windows-10-feature-updates-to-WSUS/ba-p/845054).  

- We are offering pre-release support for 19H2 offered to Windows Insider Program for Business (WIP4Biz) customers who face blocking issues that prevent them from feature evaluation or device use. [See this article for details](https://insider.windows.com/articles/19h2-support-available-for-business-users/). 

- A fix to allow OEMs to reduce the inking latency based on the hardware capabilities of their devices rather than being stuck with latency selected on typical hardware configuration by the OS.

- Key-rolling or Key-rotation feature enables secure rolling of Recovery passwords on MDM managed AAD devices upon on demand request from Microsoft Intune/MDM tools or upon every time recovery password is used to unlock the BitLocker protected drive. This feature will help prevent accidental recovery password disclosure as part of manual BitLocker drive unlock by users.

- A change to enable third-party digital assistants to voice activate above the Lock screen.

- You can now quickly create an event straight from the Calendar flyout on the Taskbar. Just select the date and time at the lower right corner of the Taskbar to open the Calendar flyout and pick your desired date and start typing in the text box–you’ll now see inline options to set a time and location.
 
![Create an event from the Calendar flyout on Taskbar.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2019/08/cc9a9d57f8c15907344cb5f718ca63ce.png)

- The navigation pane on the Start menu now expands when you hover over it with your mouse to better inform where clicking goes.

- We have added friendly images to show what is meant by “banner” and “Action Center” when adjusting the notifications on apps in order to make these settings more approachable and understandable.

![Images to demonstrate banner and Action center when adjusting notifications on apps](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2019/08/6c36cef63ea624500333417377850ba7.png)
 
- Notifications settings under Settings > System > Notifications will now default to sorting notification senders by most recently shown notification, rather than sender name. This makes it easier to find and configure frequent and recent senders. We have also added a setting to turn off playing sound when notifications appear.

- We now show the options to configure and turn off notifications from an app/website right on the notification, both as a banner and in Action Center.

- We have added a “Manage notifications” button to the top of Action Center that launches the main “Notifications & actions” Settings page.

- We have added additional debugging capabilities for newer Intel processors. This is only relevant for hardware manufacturers.

- We have made general battery life and power efficiency improvements for PCs with certain processors.

- A CPU may have multiple “favored” cores (logical processors of the highest available scheduling class). To provide better performance and reliability, we have implemented a rotation policy that distributes work more fairly among these favored cores.

- We have enabled Windows Defender Credential Guard for ARM64 devices for additional protection against credential theft for enterprises deploying ARM64 devices in their organizations.

- We have enabled the ability for enterprises to supplement the Windows 10 in S Mode policy to allow traditional Win32 (desktop) apps from Microsoft Intune.

- We’re updating the search box in File Explorer to now be powered by Windows Search. This change will help integrate your OneDrive content online with the traditional indexed results. [More details here.](https://blogs.windows.com/windowsexperience/2019/05/08/announcing-windows-10-insider-preview-build-18894/)

- We have added the ability for Narrator and other assistive technologies to read and learn where the FN key is located on keyboards and what state it is in (locked versus unlocked).

