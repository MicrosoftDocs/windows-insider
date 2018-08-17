---
title: Manage Windows Insider Preview builds
description: how to use management solutions to install and monitor builds in your organization
services: WIP-at-work-pro
author: dawnwood
manager: elizapo
ms.assetid: 
ms.service: WIP-at-work-pro
ms.tgt_pltfrm: na
ms.devlang: na
ms.date: 06/28/2018
ms.author: dawn.wood
ms.localizationpriority: medium
---

# Manage Windows Insider Preview builds
If you are a IT Pro, you have the option to: enable, disable, defer, and pause the installation of preview builds through policies (starting with Windows 10, version 1709), and through MDM.If you have registered a domain and want to control how and when devices receive Windows Insider Preview builds, you have two choices. The first is to use group policy, the second is to use MDM. 

In either case, you will be using the <b>Manage preview builds</b> and <b>Branch Readiness Level</b> settings. The <b>Manage preview builds</b> setting allows you to enable or disable installation of the preview builds. The <b>Branch Readiness Level</b> setting allows you to set which branch a device receives their updates from.

## Group policy
To set group policy, use the 
<b>Computer Configuration/Administrative Templates/Windows Components/Windows Update/Windows Update for Business/Manage preview builds</b> setting and the <b>Computer Configuration/Administrative Templates/Windows Components/Windows Update/ Windows Update for Business</b> setting. 

## MDM
To use MDM, use the [Update/ManagePreviewBuilds](https://docs.microsoft.com/en-us/windows/client-management/mdm/policy-csp-update#update-managepreviewbuilds) setting. To set the readiness level, use the [Update/BranchReadinessLevel](https://docs.microsoft.com/en-us/windows/client-management/mdm/policy-csp-update#update-branchreadinesslevel).

> [!NOTE]
> The signed-in user needs to be a Global Administrator of the Azure Active Directory (AAD) domain in order to be able to register the domain. Currently, the Windows Insider Program for Business supports AAD--but not on-premises Active Directory--as a corporate authentication method. 
>If your company has a paid subscription to Office 365, Microsoft Dynamics CRM Online, Enterprise Mobility Suite, or other Microsoft services--you have a free subscription to Microsoft Azure Active Directory. This subscription can be used to create users for enrollment in the Windows Insider Program for Business.
If you do not have an AAD account, install Insider Preview builds on individual devices with a registered Microsoft account.

## Related topics

* [Register for the Windows Insider Program for Business](wip-4-biz-register.md)
* [Share Feedback via the Feedback Hub](wip-4-biz-feedback-hub.md)
