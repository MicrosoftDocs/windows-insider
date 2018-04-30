---
title: Windows readiness levels and flight rings
description: understand your choices for time and type of updates you want to receive
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

# Windows readiness levels and flight rings
Flight rings are used to evaluate the quality of our software as it is released to progressively larger audiences. We will flight a Feature Update, application, etc. to the first ring if it passes all required automated testing in the lab. The flight will continue to be evaluated against a set of criteria to ensure it is ready to progress to the next ring.

## Release Preview
Best for Insiders who prefer to get early access to updates for the Semi-Annual Channel, Microsoft applications, and drivers, with minimal risk to their devices, and still want to provide feedback to make Windows devices great.
Insiders on this level receive builds of Windows just before Microsoft releases them to the Semi-Annual Channel. Although these builds aren’t final, they are the most complete and stable builds available to Windows Insider Program participants. This level provides the best testing platform for organizations that conduct early application compatibility testing on Windows Insider devices.
The Release Preview Ring will only be visible when your Windows build version is the same as the Semi-Annual Channel.
To move from a Preview build to the Semi-Annual Channel, use the Media Creation Tool (for device) or Windows Device Recovery Tool (for Mobile) to reinstall Windows. 

## Slow flight level
The Slow Windows Insider level is for users who prefer to see new builds of Windows with minimal risk to their devices but still want to provide feedback to Microsoft about their experience with the new build.
Builds are sent to the Slow Ring after feedback has been received from Windows Insiders within the Fast Ring and analyzed by our Engineering teams. 
These builds will include updates to fix key issues that would prevent many Windows Insiders from being able to use the build on a daily basis. 
These builds still might have issues that would be addressed in a future flight.
These builds are typically released once a month.

## Fast flight level

Best for Windows Insiders who prefer being the first to get access to builds and feature updates--with some risk to their devices--in order to identify issues, and provide suggestions and ideas to make Windows software and devices great.
Windows Insiders with devices in the Fast Ring should be prepared for more issues that might block key activities that are important to you or might require significant workarounds. 
Because we are also validating a build on a smaller set of devices before going to Fast, there is also a chance that some features might work on some devices but might fail in other device configurations. 
Windows Insiders should be ready to reinstall Windows using the Media Creation Tool or Windows Device Recovery Tool when you are significantly blocked.
Remember to report any issue to us through the Windows Insider Feedback Hub or the Windows Insider community forum.
These builds are typically released once a week.

## Compatibility check
Once your device is updated to Windows 10 and you select your desired flight ring, the process known as "Compatibility check" will need to run in the background. There is no manual way to force this process to run. This process allows for the discovery of your OS type (32-bit, 64-bit), build edition (Home, Pro, Enterprise), country and language settings, and other required information. Once this process is complete, your device will be auto-targeted for the next available flight for your selected ring. For the first build on any given device, this might take up to 24 hours to complete.