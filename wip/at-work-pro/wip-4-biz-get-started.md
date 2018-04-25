---
title: Getting Started with the Windows 10 Insider Program for Business
description: how to enroll and setup Windows Insider builds for enterprise client devices.
services: WIP-at-work-pro
author: dawn.wood
manager: elizapo
ms.assetid: 
ms.service: WIP-at-work-pro
ms.tgt_pltfrm: na
ms.devlang: na
ms.date: 05/01/2018
ms.author: dawn.wood
---

# Getting started with the Windows 10 Insider Program for Business
The are two steps for you to take to make you a Windows Insider: register for the program, and install an insider build. After that, you're ready to use the features and provide feedback directly to Microsoft. We take you feedback into account when deciding what to work on next. 

## Register for the Windows Insider Program for Business
If you are an IT administrator in an enterprise environment, you work with your end-users to participate in the Windows Insider Program for Business. Microsoft recommends that all enterprise devices register with a work account in Azure Active Directory (AAD), either individually or as part of a domain registration. It is required to submit feedback on behalf of your organization, and for you as administrator to manage Insider Preview builds on other devices in your domain.

Registering with your AAD account requires Windows 10 Version 1703 or later. Confirm by going to <b>Settings>System>About</b>. If you do not have an AAD account, find out how to get an [Azure Active Directory tenant](https://docs.microsoft.com/azure/active-directory/develop/active-directory-howto-tenant).

If you want to register using a Microsoft account, see [Quick Start](https://insider.windows.com/en-us/getting-started).

Once you have an MSA or corporate AAD account, you can register [here](https://insider.windows.com/en-us/register/). 

### Switch between your MSA and your Corporate AAD account
You can switch between your Microsoft Account (MSA) and your organizational account (AAD) by going to <b>Settings > Updates & Security > Windows Insider Program</b>. Under <b>Windows Insider account</b> select <b>Change</b>.

![alt text](images/waas-wipfb-change-user.png "switch between accounts")


## Install Windows Insider Preview builds
You can install Windows 10 Insider Preview builds on individual devices, manage installation across multiple devices in an organization, or install on a virtual machine. 

### Install on an individual device
Getting set up on a single device is easy. 
1. Open Windows Insider Program settings. You can find the settings by going to <b>Start > Settings > Update & security > Windows Insider Program</b>. To see this setting, you must have administrator rights to your device.
2. Click <b>Get started</b> and follow the prompts to link your Microsoft or work account that you used to register as a Windows Insider. 
![alt text](images/wip4biz_prompts.png "Get started button for installing WIP builds")
3. Sign-in using the account you used to register for the Windows Insider Program.
4. Read the privacy statement and then click <b>Next</b>.
5. Restart the device. After restarting, you are now ready to install your first preview build.
6. To install the first preview, open <b>Start > Settings > Update & security > Windows Insider Program</b> and select your Windows Insider level. The device receives the most recent Windows Insider build for the Windows Insider level you select. 

See [Windows readiness levels and flight rings](wip-4-biz-flight-levels-and-rings.md) for more information about each choice. 

### Install across multiple devices in a domain
Administrators can install and manage Insider Preview builds centrally across devices in their domain. To register a domain, you must be registered in the Windows Insider Program with your work account in Azure Active Directory and you must be assigned a Global Administrator role on that AAD domain. Also requires Windows 10 Version 1703 or later. 

### Install on a virtual machine
There isn't anything special you have to do to run Windows 10 Insider Preview builds on a virtual machine. Once you have a virtual machine set up, you install just as you would on an individual device. If you need help setting up a virtual machine, see [Introduction to Hyper-V on Windows 10](https://docs.microsoft.com/virtualization/hyper-v-on-windows/about/).
