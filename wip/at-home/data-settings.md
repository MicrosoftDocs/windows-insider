---
title: Choosing your data settings
description: Choosing your diagnostic data settings for flighting 
author: bleblanc
manager: dougkim
ms.tgt_pltfrm: na
ms.devlang: na
ms.author: v-allsh
ms.localizationpriority: medium
ms.topic: article
ms.prod: w10
---

# Choosing your data settings
Your privacy is important to us, so you're in control of how much of your data you share with us. But to run Windows 10 Insider Preview Builds, you must allow us to see a certain amount of diagnostic data, so we can investigate issues you might see, like crashes and bugs. Use these instructions to update your diagnostic data settings if you want to run Insider Preview builds.

## Setting up a device for the first time

1. Go to [**Settings > Privacy > Diagnostics & feedback**](https://aka.ms/WIPDataSettings) on your device.

2. Set your device's data settings to Full.

3. Reboot your device.

4. Your device is ready to get Insider Preview builds. Go to [**Settings > Update & Security > Windows Update**](https://aka.ms/WIPWindowsUpdate) to check for the latest update.


## Changing data settings on a device already running Insider Preview builds

If you're running preview builds on a personal device, use these instructions to update your data settings:
 
1. Go to [**Settings > Privacy > Diagnostics & feedback**](https://aka.ms/WIPDataSettings) on your device.

2. Flip the **Optional Diagnostic Data** switch from **Off** to **On**.

3. Reboot your device.

4. Your device is ready to keep getting Insider Preview builds. Go to [**Settings > Update & Security > Windows Update**](https://aka.ms/WIPDataSettings) to check for the latest update.

> [!NOTE] 
>If you're on a work device that's part of an Azure Active Directory (AAD) or domain joined account where you control your data settings, and those were set to Enhanced before Build 19577 was released, you'll have to use the steps in the first section to set your device to Full, and then the steps in the second section to continue receiving Insider Preview builds.
>If you're on a a work device that's part of an Azure Active Directory (AAD) or domain joined account, your administrator will need to first set your diagnostic data policy to Full, then use the second section's steps to update to Optional. This will apply for environments controlled with all administrative methods, including Group Policy (GPO), ConfigMgr, and Intune. Once these new policies have been pushed to your device, you'll be able to receive Insider Preview builds again.
