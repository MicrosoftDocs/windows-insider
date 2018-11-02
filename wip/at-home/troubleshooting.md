---
title: Troubleshooting 
description: Troubleshooting tips 
services: WIP-at-home
manager: eliotgra
ms.service: WIP-at-home
ms.tgt_pltfrm: na
ms.devlang: na
ms.date: 11/1/2018
ms.author: v-colinmit
author: cdmm12
ms.localizationpriority: medium
---

# Troubleshooting tips 

## Not able to install Windows 10 Insider Preview Builds 
* To install Windows 10 Insider Preview Builds, you need to be running a licensed version of Windows 10 on your PC. If your PC is currently running Windows 7/8/8.1, you can install Windows 10 [here](https://www.microsoft.com/en-us/windows/get-windows-10?step=Win10Question1). If you are having problems installing Windows 10, you can download a [Windows 10 Insider Preview ISO](https://www.microsoft.com/en-us/software-download/windowsinsiderpreviewadvanced). To check what version of Windows your device is using, go to __Start__, type __winver__, click __winver - run command__.
* Windows must be activated in order to participate in the Windows Insider Program. Check for Windows activation in __Settings > Update & Security > Activation__.

## Not receiving updates
After registering in the Windows Insider Program, you may find that your PC is not updating to the latest Insider Preview build as expected. This is rare, however, there are a few key items to review should you end up in this state.

__Perform a manual check for updates:__ Open Settings > Update & Security and review available updates or select Check for Updates. If you have set Active Hours, ensure your device is left turned on and signed in during the off-hours so the install process can complete.

__Is the MSA or Azure AD account connected to your PC registered for receiving builds?__ [Click here to sign in with your MSA or Azure AD account](https://insider.windows.com/en-us/insidersigninboth/). You will land on the page “Welcome back!” if your MSA or Azure AD account is registered with the Windows Insider Program.

__Have you selected a ring?__ Open Settings >Update & Security > Windows Insider Program and view the drop-down under "What pace do you want to get new builds?"

__Have you recently done a roll-back?__ Check your Windows Insider Preview settings, including ring-selection, Microsoft Account, and branch-selection.

__Are there any known issues for your current build?__ There may be an issue with an Insider Preview build that could lead to issues with updates being received.  Please check the most recent [Windows Insider Blog post](https://blogs.windows.com/blog/tag/windows-insider-program/) or reach out to us [@WindowsInsider](http://twitter.com/windowsinsider/).

## Recovering a PC
If you are in a situation where you are unable to use your PC as expected, follow these steps to recover your PC to a good state.

### Assess the impact
* What is the impact of the issue? Single app?  Minor functionality? 
* Can you continue using your device or is key functionality not working? 
* Are you able to work around the issue? Would an alternate app suffice? 
* Is a newer build available that may have a fix for any known bugs being faced?

### Troubleshoot & Discover
__Troubleshoot the issue.__ There may be a workaround available. Reach out to us via the [Windows Insider Forums](https://answers.microsoft.com/en-us/insider/forum/insider_wintp-insiderplat_pc?sort=lastreplydate&dir=desc&tab=threads&status=all&mod=&modAge=&advFil=&postedAfter=&postedBefore=&threadType=all&tm=1475533679179) or [@WindowsInsider](http://twitter.com/windowsinsider) on Twitter. If important functionality is unusable, you may want to reinstall your current OS version. Prior to doing any reinstall or rollback, ensure you have backed up important files.  While it is rare to lose data during this process, it is best to back up key data.

__OS Reinstall__ You will have several options to choose from, including an operating system-only reinstall or a clean wipe of your device: Go to Settings > Update & Security > Recovery and click Get Started under Reset this PC. Follow the on-screen directions to refresh or clean install the OS.

__Roll-back to Prior Build.__ If your PC was working as expected on the prior build and you’d like to roll back without losing any data, you may try this option: Go to Settings > Update & Security > Recovery, and select Get Started under Go Back to an Earlier Build. Note: After installing an update to your PC, you will have seven (7) days to roll back if necessary.  If required afterward, you will need to take a future update or you may clean install an older build via bootable media.

__Clean Install Insider Build via Bootable Media.__ Creating a bootable USB with a Windows Installation (from an ISO file) can be helpful in various scenarios, from recovering a machine from a bad build, to bypassing various types of bugs, or even joining a new PC into the Windows Insider program. Should you want (or need) to create a bootable USB drive from a Windows Insider ISO file, please see [these directions](https://answers.microsoft.com/en-us/insider/forum/insider_wintp-insider_install-insiderplat_pc/creating-a-bootable-usb-for-windows-insider-isos/9ebe3cbc-3c8b-4052-9484-0b7cc9b63bec?tm=1519414191218).
