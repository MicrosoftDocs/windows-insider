---
title: Manage Windows Insider Preview builds
description: how to use management solutions to install and monitor builds in your organization
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

# Manage Windows Insider Preview builds
If you have registered a domain and want to control how and when devices receive Windows Insider Preview builds, you have two choices. The first is to use group policy, the second is to use MDM. 

In either case, you will be using the <b>Manage preview builds</b> and <b>Branch Readiness Level</b> settings. The <b>Manage preview builds</b> setting allows you to enable or disable installation of the preview builds. The <b>Branch Readiness Level</b> setting allows you to set which branch a device receives their updates from.

## Group policy
To set group policy, use the 
<b>Computer Configuration/Administrative Templates/Windows Components/Windows Update/Windows Update for Business/Manage preview builds</b> setting and the <b>Computer Configuration/Administrative Templates/Windows Components/Windows Update/ Windows Update for Business</b> setting. 

## MDM
To use MDM, use the [Update/ManagePreviewBuilds](https://docs.microsoft.com/en-us/windows/client-management/mdm/policy-csp-update#update-managepreviewbuilds) setting. To set the readiness level, use the [Update/BranchReadinessLevel](https://docs.microsoft.com/en-us/windows/client-management/mdm/policy-csp-update#update-branchreadinesslevel).

## Related topics

* [Register for the Windows Insider Program for Business](wip-4-biz-register.md)
* [Share Feedback via the Feedback Hub](wip-4-biz-feedback-hub.md)
