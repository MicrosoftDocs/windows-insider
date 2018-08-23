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

# Manage Windows 10 Insider Preview Builds
Administrators can manage installation of Insider Preview builds across multiple devices in their organization using the following steps: 

## Register your domain with the Windows Insider Program
By registering your organizational domain with the Windows Insider Program, you do not have to register each device or user individually into the Windows Insider Program. 
To register a domain, you must be registered in the Windows Insider Program with your work account in Azure Active Directory (See [Register](wip-4-biz-register.md)) and you must be assigned a Global Administrator role on that Azure AD domain. Also requires Windows 10 Version 1703 or later on the machine used for registration. 

> [!div class="nextstepaction"]
> [Register your domain](https://insider.windows.com/en-us/for-business-organization-admin/)

__NOTE:__ 
* You can only register Azure AD domains as the Windows Insider Program only supports Azure Active Directory (and not Active Directory on premises) as a corporate authentication method.
* In order to get the most benefit out of the Windows Insider Program for Business, organizations should not use a test tenant of AAD. There will be no modifications to the Azure AD tenant to support the Windows Insider Program as it will only be used as an authentication method.

## Create and manage policies 
Installation of Insider Preview builds can be managed across multiple devices on an organizational Azure AD domain using Group Policies or MDM Polices in Intune or another MDM product. 

__NOTE:__
Devices on Azure AD must also be joined to the same Azure AD domain that was registered into the Windows Insider Program. For guidance, see [Integrate your on-premises directories with Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect). 

### Set using Group Policy
Use Group Policy Management Console in Windows Server 2012 R2 or later to set the following policies on domain-joined devices: 
__NOTE:__ Group Policies cannot currently be set using Windows Server Update Services or System Center Configuration Manager. 

__Allow Telemetry__. To enable installation of Insider Preview builds on a device, telemetry must be set to 2 or higher. 
Group Policy: __Computer Configuration/Administrative Templates/Windows Components/Windows UpdateData Collection and Preview builds/Allow Telemetry__

__Manage preview builds__. This setting enables or prevents installation of Insider Preview builds on a device. You can also decide to stop preview builds once the release is public. 
Group Policy: __Computer Configuration/Administrative Templates/Windows Components/Windows Update/Windows Update for Business/Select when Preview Builds and Feature Updates are received.__

__Branch Readiness Level__. This setting allows enables distribution of Insider Preview builds on a PC. It also lets you to choose between preview flight rings, and defer or pause the delivery of updates. 
Group Policy: __Computer Configuration/Administrative Templates/Windows Components/Windows Update/Windows Update for Business/Select when Preview Builds and Feature Updates are received__

### Set using MDM policies (non-Intune)
To set the policies above using non-Microsoft MDM service providers, using the CSP settings below. For guidance on configuring CSPs, see [CSPs in MDM](https://docs.microsoft.com/en-us/windows/configuration/provisioning-packages/how-it-pros-can-use-configuration-service-providers#csps-in-mdm). 

[System/AllowTelemetry](https://docs.microsoft.com/en-us/windows/client-management/mdm/policy-csp-system#system-allowtelemetry)

[Update/ManagePreviewBuilds](https://docs.microsoft.com/en-us/windows/client-management/mdm/policy-csp-update#update-managepreviewbuilds) 

[Update/BranchReadinessLevel](https://docs.microsoft.com/en-us/windows/client-management/mdm/policy-csp-update#update-branchreadinesslevel).


### Set using MDM polices with Intune 
1.	Log into the Intune management portal and go to __Software Update>Windows 10 Update Rings__. Click “+” to create an Update Ring policy.
2.	Under __Servicing Channel__, select Fast or Slow to assign Insider Preview builds from an Insider Preview Ring. See [Windows readiness levels and flight rings](wip-4-biz-flight-levels-and-rings.md) for more information about each choice. 
3.	Adjust __Feature update deferral period__ if you want to defer deployment of Insider Preview builds for a certain number of days after release. 
4.	Click __OK__ and __Create__ to set policy.
5.	Go to __Assignments__ to assign policy to users and devices. Note: you can create groups with one or more users or devices in Intune under __Groups__. 

![ADD subscription](images/wip-4-biz-settings.png "ADD")

* [Register for the Windows Insider Program for Business](wip-4-biz-register.md)
* [Share Feedback via the Feedback Hub](wip-4-biz-feedback-hub.md)
