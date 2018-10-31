---
title: Windows readiness levels and flight rings
description: understand your choices for time and type of updates you want to receive
services: WIP-at-work-pro
author: dougkim
manager: dougkim
ms.assetid: 
ms.service: WIP-at-work-pro
ms.tgt_pltfrm: na
ms.devlang: na
ms.date: 06/28/2018
ms.author: dougkim
ms.localizationpriority: medium
---

# Windows readiness levels and flight rings
Flight rings are used to evaluate the quality of our software as it is released to progressively larger audiences. We will flight a Feature Update, application, etc. to the Fast ring if it passes all required automated testing in the lab. The flight will continue to be evaluated against a set of criteria to ensure it is ready before progressing to the next ring, the Slow ring. Windows readiness levels are related to flight rings; they're how you tell Microsoft what ring you want to be in. For instance, you can set your Windows readiness level to Fast, which puts you in the Fast ring. Here's an example of what you will see when you enroll in the Fast ring.

Microsoft recommends that all organizations have at least 1% of their devices enrolled in the Windows Insider Program, to include the Windows Insider Program in their deployment plans, and to provide feedback on any issues they encounter to Microsoft via the [Windows Insider Feedback Hub](wip-4-biz-feedback-hub.md). 
The Windows Insider Program doesn't replace Semi-Annual Channel deployments in an organization. Rather, it provides IT Pros, enterprise users, and other interested parties with pre-release builds of Windows 10.

## Fast flight ring
Do you want to be the first to get access to builds and feature updates? The Fast Windows readiness level is for those of you who can accept some risk to your devices in order to identify issues, and provide suggestions for the next version of Windows.
Windows Insiders with devices in the Fast Ring should be prepared for more issues that might block key activities that are important to you or might require significant workarounds. 
Because Fast Ring builds are released so early in the development cycle, we recommend limiting feature exploration in your organization to IT administrators and developers running Insider Preview builds on secondary devices.

Windows Insiders should be ready to reinstall Windows using the Media Creation Tool or Windows Device Recovery Tool when you are significantly blocked.
Remember to report any issue to us through the [Windows Insider Feedback Hub](wip-4-biz-feedback-hub.md) or the [Windows Insider community forum](https://techcommunity.microsoft.com/t5/Windows-Insider-Program/bd-p/WindowsInsiderProgram).
These builds are typically released once a week.

## Slow flight ring
The Slow Windows Insider level is for you if you prefer to see new builds of Windows with minimal risk to your devices but still want to provide feedback to Microsoft.
Builds are sent to the Slow Ring after feedback has been received from the Fast Ring and analyzed by our Engineering teams. These builds will include updates to fix key issues that would prevent many Windows Insiders from being able to use the build on a daily basis. In addition to Insiders who might have participated in feature exploration, we also recommend including a small group of application users from each business department to ensure a representative sample. Slow ring builds might still have issues that will be addressed in a future flight.
These builds are typically released once a month.

## Release Preview
If you're an Insider who wants to get early access to updates for the Semi-Annual Channel, applications, and drivers, this is the safest level with minimal risk to your devices. And, you still get to provide feedback.
Insiders on this level receive builds of Windows right before Microsoft releases them through the Semi-Annual Channel. Although Release Preview builds aren’t final, they are the most complete and stable builds available to Windows Insider Program participants. This level provides the best testing platform for organizations that conduct early application compatibility testing on Windows Insider devices.
The Release Preview Ring will only be visible when your Windows build version is the same as the Semi-Annual Channel.
To move from a Preview build to the Semi-Annual Channel, use the Media Creation Tool (for device) or Windows Device Recovery Tool (for Mobile) to reinstall Windows. 

## Compatibility check
Once your device is updated to Windows 10 and you select your desired Windows readiness level, the process known as "Compatibility check" needs to run in the background. There is no manual way to force this process to run. This process allows for the discovery of your OS type (32-bit, 64-bit), build edition (Home, Pro, Enterprise), country and language settings, and other required information. Once this process is complete, your device will be auto-targeted for the next available flight for your selected Windows readiness level. For the first build on any given device, this might take up to 24 hours to complete.

## Related topics

* [Register for the Windows Insider Program for Business](wip-4-biz-register.md)
* [Manage Windows Insider Preview builds](wip-4-biz-manage-builds.md)