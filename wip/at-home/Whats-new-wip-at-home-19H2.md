---
title: What's new in the Windows 10 Insider Preview Build 19H2
description: New Windows features for Windows Insider Program Preview Builds
author: jessyrod
manager: Blair Glennon
ms.tgt_pltfrm: na
ms.devlang: na
ms.date: 08/20/2019
ms.author: jessyrod
ms.localizationpriority: medium
ms.topic: article
ms.prod: w10
---

# What's new for Windows 10 Insider Preview Build 19H2
The [Windows Insider Program](https://insider.windows.com/) lets you preview builds of the upcoming release of Windows 10. This topic lists all of the updates that were part of the 19H2 development.

## Windows 10 Insider Preview Build 18362.10000 (19H2)
Here are the [next steps we are taking at continuing to evolve Windows 10 servicing and quality](https://blogs.windows.com/windowsexperience/2019/07/01/evolving-windows-10-servicing-and-quality-the-next-steps/#oPHCjv4ShO8LVgP7.97) with the next feature update for Windows 10. This release has been referred to as 19H2 with Insiders. 19H2 will include a scoped set of features for select performance improvements, enterprise features, and quality enhancements and will be delivered to customers running the May 2019 Update using servicing technology (like the monthly Cumulative Update process).

For Insiders, this means a few differences to how they will get 19H2:

* Insiders will need to be in the Slow ring and on the May 2019 Update to receive 19H2 bits.
* 19H2 will be delivered to Insiders in the Slow ring via servicing as a Cumulative Update and not full build updates.
* Some Insiders may not see the new features right away as we perform controlled feature rollouts (CFRs) to gain better feedback on overall build quality.
* Specific to CFRs, we may ship features in these updates turned off by default and turn them on independently of bits getting downloaded to Insiders’ PCs.

Even though we will be delivering 19H2 to Insiders in the Slow ring through servicing, we plan to continue to publish blog posts for each of these flights and include information on anything new and notable and any known issues that might be included. For more information on what 19H2 means for Windows 10 servicing and quality, we recommend you [read John Cable’s blog post here](https://blogs.windows.com/windowsexperience/2019/07/01/evolving-windows-10-servicing-and-quality-the-next-steps/#Ms17JKuYz2Di52l2.97).

__We are also releasing 19H2 Build 18362.10000 to Insiders in the Slow ring today.__ This update contains two behind-the-scenes changes designed for OEMs and does not contain anything visible to Insiders. We’re using this update to test our process and servicing pipeline for delivering these updates to customers. 19H2 updates to Insiders will also be cumulative with the latest May 2019 Updates. For example, today’s release also includes the same improvements and fixes contained in [this Cumulative Update released for the May 2019 Update here](https://support.microsoft.com/en-us/help/4501375/windows-10-update-kb4501375). Going forward, these updates will continue to contain the same improvements and fixes released for the May 2019 Update in addition to new 19H2 changes.

## Windows 10 Insider Preview Build 18362.10005 (19H2)

In addition to the fixes included in [KB4507453](https://support.microsoft.com/en-us/help/4507453/windows-10-update-kb4507453) for the May 2019 Update, 19H2 Build 18362.10005 includes the following changes and improvements:

* Windows containers require matched host and container version. This restricts customers and limits Windows containers from supporting mixed-version container pod scenarios This update includes 5 fixes to address this and allow the host to run down-level containers on up-level for process (Argon) isolation.
* A fix to allow OEMs to reduce the inking latency based on the hardware capabilities of their devices rather than being stuck with latency selected on typical hardware configuration by the OS.
* Key-rolling or Key-rotation feature enables secure rolling of Recovery passwords on MDM managed AAD devices upon on demand request from Microsoft Intune/MDM tools or upon every time recovery password is used to unlock the BitLocker protected drive. This feature will help prevent accidental recovery password disclosure as part of manual BitLocker drive unlock by users.
* A change to enable third-party digital assistants to voice activate above the Lock screen.

Please note that these changes and improvements are currently __OFF__ by default in this build. As [mentioned previously](https://blogs.windows.com/windowsexperience/2019/07/01/announcing-windows-10-insider-preview-build-18362-10000-19h2/#x7xIYUv4sjtEGLXE.97), we may ship features in these updates turned off by default and turn them on via controlled feature rollouts. Doing this helps us gain better feedback on overall build quality. With today’s 19H2 build, we are testing this experience. Our plan is to quickly follow-up with another 19H2 build that turns these features on for a subset of Insiders and proceed from there based on feedback and quality.

## Windows 10 Insider Preview Build 18362.10012 & 18362.10013 (19H2)

__19H2 Build 18362.10012__ and __Build 18362.10013__ are now available to Windows Insiders in the Slow ring. As a reminder, we are testing the ability to ship these updates with features turned off by default so that we can then turn them on via controlled feature rollouts. This helps us gain better feedback on overall build quality. A subset of Insiders in the Slow ring will have features turned off by default, and another subset will have them turned on by default. __This means not everyone in the Slow ring will see new features right away:__

* IF you are on 19H2 Build 18362.__10005__ – you will receive Build 18362.10012 today with features turned OFF by default. This includes the below mentioned features as well as the features from the previous release.
* IF you are on 19H2 Build 18362.__10006__ – you will receive Build 18362.10013 with features turned ON by default.


If you’re on the Windows 10 May 2019 Update and just joining your PC into the Slow ring to take 19H2 updates, it’ll be a virtual “coin toss” as to whether your PC gets features turned on or turned off.

Other than one update has features turned off, and the other has features turned on – the two updates released today and highlighted above are identical and contain the following features in addition to the improvements from [KB4505903](https://support.microsoft.com/en-us/help/4505903/windows-10-update-kb4505903) and the previous [19H2 update](https://blogs.windows.com/windowsexperience/2019/07/15/announcing-windows-10-insider-preview-build-18362-10005-19h2/#HVsQAakbRWhzSJev.97):

* You can now quickly create an event straight from the Calendar flyout on the Taskbar. Just click on the date and time at the lower right corner of the Taskbar to open the Calendar flyout and pick your desired date and start typing in the text box – you’ll now see inline options to set a time and location.

![taskbar calendar](/wip/at-home/images/19H2ACB.png)

* The navigation pane on the Start menu now expands when you hover over it with your mouse to better inform where clicking goes.
* We have added friendly images to show what is meant by “banner” and “Action Center” when adjusting the notifications on apps in order to make these settings more approachable and understandable.

![action center & banner](/wip/at-home/images/19H2TBC.png)

* Notifications settings under Settings > System > Notifications will now default to sorting notification senders by most recently shown notification, rather than sender name. This makes it easier to find and configure frequent and recent senders. We have also added a setting to turn off playing sound when notifications appear.
* We now show the options to configure and turn off notifications from an app/website right on the notification, both as a banner and in Action Center.
* We have added a “Manage notifications” button to the top of Action Center that launches the main “Notifications & actions” Settings page.
* We have added additional debugging capabilities for newer Intel processors. This is only relevant for hardware manufacturers.
* We have made general battery life and power efficiency improvements for PCs with certain processors.
* A CPU may have multiple “favored” cores (logical processors of the highest available scheduling class). To provide better performance and reliability, we have implemented a rotation policy that distributes work more fairly among these favored cores.
