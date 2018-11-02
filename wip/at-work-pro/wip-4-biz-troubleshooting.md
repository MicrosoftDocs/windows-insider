---
title: Windows Insider Program troubleshooting
description: how to fix common problems and uninstall or unregister from the Windows Insider Program
services: WIP-at-work-pro
author: lizap
manager: dougkim
ms.assetid: 
ms.service: WIP-at-work-pro
ms.tgt_pltfrm: na
ms.devlang: na
ms.date: 06/28/2018
ms.author: elizapo
ms.localizationpriority: medium
---

# Troubleshooting
You can find answers to common issues here. 

## I'm not getting Insider Preview builds

Here are some things you can check if you are not getting updates on a device. 

### Windows Update issues
* Manually check for updates on the device by opening __Settings > Update & Security__. You can review available updates or select "Check for Updates". If Active Hours are set, ensure the device is left turned on and signed in during the off-hours so the install process can complete.
* If you are getting an error message in Windows Update, you can use the information that is included in the Windowsupdate log file to troubleshoot the issue. To get log, use the following Powershell cmdlet: __Get-WindowsUpdateLog__. See [How to read the Windows Update log file](https://support.microsoft.com/en-us/help/902093/how-to-read-the-windowsupdate-log-file). See also [Fix Windows Update issues](https://support.microsoft.com/en-us/help/10164/fix-windows-update-errors).

### Group Policy issues
* If you are installing Insider Preview builds remotely using Group Policy, note that these policies can only be set using the Group Policy Management Console and cannot be set using Windows Server Update Services. 
* Also note that your organization's Azure Active Directory must be registered with the Windows Insider Program. See [Manage Windows 10 Insider Preview Builds](wip-4-biz-manage-builds.md).

## I'm getting a "Something went wrong" error message in Feedback Hub
The option for users to give consent for apps to access their profile data is controlled through Azure Active Directory. This means that Azure AD administrators have the ability to allow or block users from giving consent. If an administrator has blocked this option, the user will see a "Something went wrong error" message when they sign in with an AAD account. Administrators can unblock in the [Azure portal](https://portal.azure.com/). Go to __Enterprise applications>User Settings__ and enable __Users can consent to apps accessing company data on their behalf data__. 

## Other resources

If you can find an answer to your issue, try these resources.

* [Windows Insider Blog](https://blogs.windows.com/windowsexperience/tag/windows-insider-program/)
* [Windows Insider Program forums](https://answers.microsoft.com/en-us/insider?OCID=WIP_r_Welcome3_Body_InsidersForum)
