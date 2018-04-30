---
title: Install Windows 10 preview builds
description: how to install Windows Insider builds for enterprise client devices
services: WIP-at-work-pro
author: dawn.wood
manager: elizapo
ms.assetid: 
ms.service: WIP-at-work-pro
ms.tgt_pltfrm: na
ms.devlang: na
ms.date: 05/07/2018
ms.author: dawn.wood
---



# Install Windows Insider Preview builds
You can install Windows 10 Insider Preview builds on individual devices, manage installation across multiple devices in an organization, or install on a virtual machine. To receive Windows Insider Preview builds, set the Allow Telemetry setting in Group Policy to 2 or higher. This setting is in <b>Computer Configuration/Administrative Templates/Windows Components/Data Collection and Preview Builds</b> - Allow Telemetry. In MDM, the setting is in [System/AllowTelemetry](https://docs.microsoft.com/en-us/windows/client-management/mdm/policy-csp-system#system-allowtelemetry). 

## Install on an individual device
Getting set up on a single device is easy. 
1. Open Windows Insider Program settings. You can find the settings by going to <b>Start > Settings > Update & security > Windows Insider Program</b>. To see this setting, you must have administrator rights to your device.
2. Click <b>Get started</b> and follow the prompts to link your Microsoft or work account that you used to register as a Windows Insider. 
![alt text](images/wip4biz_prompts.png "Get started button for installing WIP builds")
3. Sign-in using the account you used to register for the Windows Insider Program.
4. Read the privacy statement and then click <b>Next</b>.
5. Restart the device. After restarting, you are now ready to install your first preview build.
6. To install the first preview, open <b>Start > Settings > Update & security > Windows Insider Program</b> and select your Windows Insider level. The device receives the most recent Windows Insider build for the Windows Insider level you select. 

See [Windows readiness levels and flight rings](wip-4-biz-flight-levels-and-rings.md) for more information about each choice. 

## Install across multiple devices in a domain 
Administrators can install and manage Insider Preview builds centrally across devices in their domain. To register a domain, you must be registered in the Windows Insider Program with your work account in Azure Active Directory and you have to be a Global Administrator role on that AAD domain. This feature is available on Windows 10 Version 1703 or later. 

## Install on a virtual machine
There isn't anything special you have to do to run Windows 10 Insider Preview builds on a virtual machine. Once you have a virtual machine set up, you install just as you would on an individual device. If you need help setting up a virtual machine, see [Introduction to Hyper-V on Windows 10](https://docs.microsoft.com/virtualization/hyper-v-on-windows/about/).

## Next step
If you have registered a domain and want to control how and when devices receive Windows Insider Preview builds, you should read [!div class="nextstepaction"][Manage Windows Insider Preview builds](wip-4-biz-manage-builds.md).

If you are installing on an individual device, you should learn how to [!div class="nextstepaction"] [Share Feedback via the Feedback Hub](wip-4-biz-feedback-hub.md).