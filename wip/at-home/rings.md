---
title: Working with rings and updates
description: definition of Insider rings and updates
manager: eliotgra
ms.tgt_pltfrm: na
ms.devlang: na
ms.date: 11/02/2018
ms.author: v-colinmit
author: cdmm12
ms.localizationpriority: medium
ms.topic: article
ms.prod: w10
---

# Working with rings and updates

## What are rings?
Windows 10 Insider Preview Builds are released in “rings." Each ring is defined by a different release frequency and level of stability. Rings are used to evaluate the quality of our software as it's released to progressively larger audiences. If the build passes automated testing in the lab, we will flight (release a build) to the next ring. 

![Ring Theory](images/Rings4.png "Windows Insider Preview Rings")

### Fast ring
The benefit of being in the Fast ring is that you will be among the first to use and provide feedback on new and improved features. Devices in the Fast ring are typically updated on a weekly basis with a new Insider Preview build through [Windows Update](https://docs.microsoft.com/windows/deployment/update/windows-update-overview). Be prepared for issues that might block key activities or might require workarounds. Because we are also validating a build on a smaller set of devices before releasing, there is a chance that some features might fail in some device configurations. If significantly blocked, report the issue to us in the [Feedback Hub](feedback-hub:///) app or the [Windows Insider forums](https://social.technet.microsoft.com/Forums/en-US/home?forum=WindowsInsiderPreview) and be ready to reinstall Windows using the Media Creation Tool. 

### Slow ring
The benefit of being in the Slow ring is that you’ll still receive Insider Preview builds with new preview features and updates, but the builds will be more stable. Devices in the Slow ring are typically updated on a monthly basis with a new Insider Preview build through Windows Update. Builds are sent to the Slow ring after feedback has been received from Insiders on the Fast ring and analyzed by our Engineering teams. Slow ring builds include Quality Update service packages to fix key issues and also receive the latest [Microsoft Security Response Center security fixes](https://blogs.technet.microsoft.com/msrc/) shortly after public availability. Note that, because these builds are from the Development Branch, they could have issues that might be addressed in a future flight. For more information, see [Servicing comes to the Slow ring](https://insider.windows.com/en-us/articles/servicing-comes-to-the-slow-ring/).

### Release Preview ring
If you want to be on the current public release of Windows 10 but still get early access to updates, applications, and drivers without taking the risk of moving to the Development Branch, the Release Preview ring is your best option. The Release Preview ring is only visible when your Windows build version is the same as the current Production Branch. The easiest way to go between the Development Branch to the current Production Branch is to reinstall Windows using the Media Creation Tool. 

### Skip Ahead
This is a unique version of the Fast ring that allows Insiders to “skip ahead” to Windows 10 Insider Preview builds in the next release of Windows while we are finishing up a current release. Enrollment in Skip Ahead is offered for a limited time to a small subset of Insiders.

### Switching between rings
Changing rings is a simple process. Go to **Settings** > **Updates & Security** and select __Windows Insider Program__. Under __What kind of content would you like to receive?__ select **Just fixes, apps and drivers** to select Release Preview. Or choose **Active development of Windows** and select **Fast** or **Slow** under **What pace do you want to get new builds?**

## Working with updates

After you've registered in the Windows Insider Program and installed your first Windows 10 Insider Preview build, you'll begin to receive updates to the device(s) you have enrolled. During the development process, the build number will change with each update. There are two different types of builds being delivered to your device(s):

### Major builds

When a major build is released, it will include any combination of new features, updates to existing features, bug fixes, application changes, or other changes. For a major build, you will see the build number increment by 1 or more. Build numbers may or may not be consecutive, which depends on internal ring promotions. For example, 14361 > 14365.

### Minor/servicing Builds

Also known as “Servicing” or “Cumulative” updates, these builds represent a smaller set of changes to a currently released Major Build. Servicing Builds often include bug fixes, minor operating system updates, or other smaller changes as needed. For example, 14361 > 14361.1002 > 14361.1003.

### What to expect in each ring

While there is no set requirement for how build numbers are delivered to each ring, in general you'll find these to be true:

**Fast ring:** Major Build releases, very few servicing builds.

**Slow ring:** Major Build with minor build fixes attached.

**Release Preview ring:** Major Build change at a release milestone, and then a continued series of Servicing Builds until the next release milestone is reached.
