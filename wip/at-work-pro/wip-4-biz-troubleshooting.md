---
title: Windows Insider Program troubleshooting
description: how to fix common problems and uninstall or unregister from the Windows Insider Program
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

# Troubleshooting
You can find answers to common issues here. 

## I'm not getting updates

Here are some things you can check if you are not getting updates. 
* Manually check for updates by opening <b>Settings > Update & Security</b>. You can review available updates or select Check for Updates. If you have set Active Hours, ensure your device is left turned on and signed in during the off-hours so the install process can complete.
* Check for Windows activation in <b>Settings > Update & Security > Activation </b>. Your copy of Windows must be activated in order to participate in the Windows Insider Program.
* Check to see that you have chosen a Windows readiness level by going to <b>Settings > Update & Security > Windows Insider Program. Choose your Insider level using the drop-down selection box
* If you've recently done a clean install, the appropriate targeting needs to take place for your PC. This is true even for devices that previously received Windows Insider preview builds. This background process is known as Compatibility Checker and will run during idle time on your PC and may take up to 24 hours.

## Something went wrong error message

The option for users to give consent for apps to access their profile data is controlled through Azure Active Directory. This means the AAD administrators have the ability to allow or block users from giving consent.
If the administrators blocked this option, the user will see the following error message when they sign in with an AAD account.

![alt text](images/waas-wipfb-aad-error.png "something went wrong")

## Do I have the right license?

To install Windows 10 Insider Preview, you’ll also need to be running a licensed version of Windows 10 on your PC. If your PC is currently running Windows 7/8/8.1, you can install Windows 10 [here](https://www.microsoft.com/en-us/windows/get-windows-10?step=Win10Question1). If you are having problems installing Windows 10, you can download a [Windows 10 Insider Preview ISO](https://www.microsoft.com/en-us/software-download/windowsinsiderpreviewadvanced). To check what version of Windows your device is using, go to <b>Start</b>, type <b>winver</b>, click <b>winver - run command</b>.

## Other resources

If you can find an answer to your issue, try these resources.

* [Windows Insider Blog](https://blogs.windows.com/windowsexperience/tag/windows-insider-program/)
* [Windows Insider Program forums](https://answers.microsoft.com/en-us/insider?OCID=WIP_r_Welcome3_Body_InsidersForum)
