---
ms.date: 09/28/2020
title: Checking if you're flighting
description: How to tell if your device is on an Insider Preview build
author: bleblanc
manager: dougkim
ms.tgt_pltfrm: na
ms.devlang: na
ms.author: bleblanc
ms.localizationpriority: medium
ms.topic: article
ms.prod: w10
---

# Checking if you're flighting
Flighting is the process of running Windows 10 Insider Preview Builds on your device. We know that sometimes it can be hard to tell if you’re flighting and successfully receiving updates, but there are some quick and easy ways to know which Insider Preview build your device is on and what your Windows Insider settings are.

To see the latest build number for your channel, [check out Flight Hub](./flight-hub/index.md).

## Check for the watermark

If you’re on an Insider Preview build, you should be able to see a watermark on the bottom right of your desktop, right above the time and date in your taskbar, that tells you exactly which version of Windows you’re running.

![Windows watermark for Windows 10 Insider Preview Builds showing Build 20211.](images/Watermark.jpg "Windows Insider watermark on desktop.")

Sometimes, as builds in the Beta Channel and Release Preview Channel get close to retail however, this goes away. If you think you’re flighting but aren’t seeing the watermark, double-check which version you’re on with one of the other methods below.

## Look at About in Settings

You can also see which version of Windows your device is on in the About section of Settings. Go to [**Settings** > **System** > **About** > **Windows specifications**](https://aka.ms/AboutSettings) to see which edition, version, and OS build your device is on.

![Windows' About Settings, scrolled down to the Windows specifications section to highlight your current OS build.](images/About-w11.jpg "Windows About Settings page.")

## Run the winver command

Need a quick, easy way to pull up your Windows details? Just type **winver** into the search on your taskbar, then select it to run the command. A window will open telling you which version and Insider Preview build you’re on.

![The About Windows module that pops up from running the winver command, highlighting the Build 22000.100 the device is on.](images/winver-w11.jpg "Windows About dialog box.")

## Check your build with PowerShell

Prefer to use PowerShell to check your build? Open PowerShell on your device, and in the prompt, type in:

* **Get-WmiObject win32_operatingsystem | select Version**

Hit enter, and it will pull up which version your device is on. The last numbers in the set are the Insider Preview build you’re on.

![Windows PowerShell running this command to check your version, highlighting that you're on Build 20211.](images/Powershell.jpg "Channels overview and how rings move to them.")

## Double-check your Windows Insider settings

If checking your device information made you realize you’re not on the build that you expected, make sure your Windows Insider Program settings are right. Go to [**Settings** > **Windows Upadate** > **Windows Insider Program**](https://aka.ms/WIPSettings) to check if your registered Insider account is connected and if you’re in the right channel. [Learn more about our channels and what you can expect to see in each.](./flighting.md)

![The Windows Insider Program's section in Settings showing your channel and the Insider account tied to your device.](images/WIP-settings-w11.jpg "Windows Insider Program Settings page.")

If everything there looks correct, but you still aren’t receiving updates, [check out our troubleshooting section for more help fixing your updates](./troubleshooting.md#not-receiving-updates).

