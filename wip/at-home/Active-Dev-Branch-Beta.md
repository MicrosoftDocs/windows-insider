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

## Build 19569
Windows 10 Insider Preview Build 19569 was released to the Fast ring on [2/20/2020](https://blogs.windows.com/windowsexperience/2020/02/20/announcing-windows-10-insider-preview-build-19569/).

### Evolving the Windows 10 icons
We are currently working on a multi-year effort across Microsoft’s design teams to redesign the icons across all our products. We started with the Office icons, and now we’re moving forward with updating the icons in Windows 10, starting with the built-in apps like Alarms & Clock, Calculator, Mail, and Calendar. Research and feedback from Windows Insiders showed a desire to see consistency in design and connection to the brand, with enough differences to aid in recognition. You can read all about our approach to updating the icons in Windows 10 in this Medium post from the Microsoft Design Team!

![Search](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/02/7e4667f9c9e488683aca797991b5a747.png "view of updated design for web preview in search results")

Many of these icons will be updated as app updates from the Microsoft Store. We are beginning to roll them out to Windows Insiders in the Fast ring first, starting today. The Mail and Calendar icons rolled out this morning to Release Preview. Over the coming months, Insiders will see more of the icons in Windows 10 get updated with new designs!

### General changes, improvements, and fixes
* We fixed an issue resulting in OneDrive not working and using an unexpectedly high amount of CPU for some Insiders on the previous build.
* We resolved an issue where SCSI drivers weren’t being recognized with certain third-party virtual machines, which was causing c1900191 errors on these devices. We’re continuing to investigate additional c1900191 errors on other devices.
* We fixed an issue impacting Start menu reliability after upgrade for some Insiders.
* We fixed an issue resulting in some Insiders experiencing a green screen with a SYSTEMTHREAD EXCEPTION NOT HANDLED error on recent builds.

## Build 19564

## Build 19559

## Build 19541

Windows 10 Insider Preview Build 19541 was released to the Fast ring on [1/8/2020](https://blogs.windows.com/windowsexperience/2020/01/08/announcing-windows-10-insider-preview-build-19541/).

### Location in-use icon update
As some keen eyed Insiders have noticed, we’ve updated the notification area icon for when an app is using your location. The new icon looks like this:

![Search](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/01/f3b5ee974cf44250d484db25447cce28.png "Showing the new arrow icon for location in use.")

### Showing architecture in Task Manager
When you’re using the Details tab in Task Manager, we’ve added a new option to show the architecture of each process. If you’re interested, you can add it by right-clicking on a column header, choosing Select Columns, and selecting Architecture from the list.

![Search](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/01/5cd3aaadea5f925716341c53a4b89b20.png "When you're in the Details tab of Task Manager, you can now add this Architecture option.")

## Build 19536

Windows 10 Insider Preview Build 19536 was released to the Fast ring on [12/16/2019](https://blogs.windows.com/windowsexperience/2019/12/16/announcing-windows-10-insider-preview-build-19536/).

### Optional Drivers
[We’re still working on making it easier for you to see all optional updates](http://aka.ms/wip18985) (including drivers, feature updates, and monthly non-security quality updates) in one place. When optional updates are detected, they will be listed under Settings > Update & Security > Windows Update > View optional updates.

For drivers, you no longer need to browse Device Manager for a specific device to update. Windows Update will automatically keep your drivers up to date, but if you’re having a problem, one of those optional drivers might help.

View optional updates option in the Windows Update section of Update & Security Settings.

### Re-releasing the updated Korean IME
During 19H1 development, we’d started work on an updated version of the Korean IME as part of our ongoing efforts to modernize and improve your typing experience in Windows. Based on feedback, we decided not to ship this with 19H1, and instead worked on further improving the experience first. With Build 19536, we’re re-releasing the updated IME, along with some improvements that help it work better with various apps.

To recap the most noticeable changes included as part of this IME work:

* For those who’re familiar with typing in Korean when writing in Hanja, we have a new candidate selection window that uses modern controls and clearer typography:

![Search](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2019/12/17baa87bb553ab0d1bc9f5de682d3a7d.png "Showing the candidate selection window of the updated Korean IME.")

* The new IME version also comes with an updated algorithm used for text prediction when writing Korean using the touch keyboard. Text suggestions should now be more accurate and relevant to what you are writing.

### Family group setup
[Microsoft has family features that span across multiple platforms](https://account.microsoft.com/family/about), like Windows, Xbox, and Android. On Windows, you can set things up for your family, like screen time limits, content filters, have kids ask before they buy things, or even stay organized with a shared family calendar, OneNote, and Office 365 Home subscription. If you share a device with family, it’s easy to get their account set up in a family group to take advantage of all these features.

![Search](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2019/12/df545e6188f866eee1db8f9f73382240.png "New Who will use this device screen when setting up a new Windows 10 PC.")

In this build, we want to help customers set up their device to be used by multiple people in their family. While we’re not releasing an ISO for this build, some Insiders who choose to reset their PC may see a screen during setup that asks who’ll be using the device. If they select People in my family, we’ll help them get set up in a family group once they get to their desktop, so that they’re ready to get started with all the features.

If you see this new page, let us know what you think by going to Security and Privacy > Child accounts and family settings in the Feedback Hub.