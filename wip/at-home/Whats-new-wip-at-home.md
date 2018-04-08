---
title: What's new in the Windows 10 Insider Preview Builds (RS5)
description: How to get setup and perform first tasks for Windows Insider Program for Server Preview Builds
services: WIP-at-work
author: dawn.wood
manager: elizapo
layout: LandingPage
ms.assetid: 
ms.service: WIP-at-work
ms.tgt_pltfrm: na
ms.devlang: na
ms.topic: landing-page
ms.date: 04/10/2018
ms.author: dawn.wood
---

#  What's new in the Windows 10 Insider Preview Builds (RS5)
The [Windows Insider Program](https://insider.windows.com/en-us/) lets you preview builds of the upcoming release of Windows 10. This topic lists all new Windows 10 features for you to try. Unlike the [Windows Insider Program Blog](https://blogs.windows.com/windowsexperience/tag/windows-insider-program) and the Windows Insider Program for Server community posts, this topic is organized by feature, then by date. 

## Sets improvements
Sets is designed to make sure that everything related to your task: relevant webpages, research documents, necessary files, and applications, is connected and available to you in one click. With Sets, 1st party experiences like Mail, Calendar, OneNote, MSN News, Windows and Microsoft Edge become more integrated to create a seamless experience, so you can get back to what’s important and be productive, recapturing that moment, saving time – we believe that’s the true value of Sets. 

Here are the new features:

-<b>Drag and drop app tabs within and between Sets windows is now supported</b>: It works just like it sounds! You can now drag an app tab around within the Set or combine tabbed app windows into Sets.
<i>Note: If you open a Microsoft Edge tab outside of a Set, you can’t drag and drop it into a Sets window. Drag and drop for Microsoft Edge web tabs within Sets isn’t supported yet and you may experience a crash if this is attempted.</i>
-<b>Tabs are now bubbled up in Alt + Tab</b>: Have Photos, Microsoft Edge, and OneNote tabbed together? You can now use Alt + Tab to switch between them. Prefer to only show the primary window in Alt + Tab? There’s a new setting – more on that in just a moment…
<i>Note: If you have multiple Microsoft Edge windows in a Set, only the one most recently accessed will be visible in Alt + Tab.</i>
-<b>Support for desktop (Win32) apps.</b> Sets now supports File Explorer, Notepad, Command Prompt, and PowerShell. One of the top feature requests by Insiders has been tabs for File Explorer and with Sets you can get a tabbed File Explorer experience.
-<b>Launch apps from the new tab page</b> by typing the app name into the search box.
-<b>UWP apps are launched in the same window</b> replacing the new tab page.
The tab UI in Sets now shows icons including website favicons and app icons.
Resume your project with more control – When restoring your projects you’ll be prompted to restore related apps and webpages. In Timeline you’ll see when a project has multiple activities associated with it.
-<b>Improved Settings for Sets</b>: We’ve updated the Settings for Sets via Settings > System > Multitasking. To start with, Sets now has its own section on this page, and is searchable (try typing “Sets” or “tabs” and it will appear in the dropdown). We’ve also added a setting to control the Alt + Tab behavior mentioned above.
![alt text](images/Win10Sets.png "Sets")
-<b>File Explorer & Sets Improvements</b>: We’ve heard your feedback – you’d like it to be easier to get two File Explorer windows grouped together, and we’re working on it. To start with, you no longer need to hold CTRL on the new tab page to launch a File Explorer window in a tab (this was a temporary necessity with the last wave). We’ve also added a new keyboard shortcut to open a new tab when a File Explorer window is in focus: Ctrl + T. Remember, you can use Ctrl + N to open a new window, and Ctrl + W to close the window/tab.

<b>New UI for opening new tabs and windows</b> in the File Menu.
![alt text](imagestabsinfilewindow/.png "tabs in file window")

-<b>Keyboard shortcuts</b>
--<b>Ctrl + Win + Tab</b> – switch to next tab.
--<b>Ctrl + Win + Shift + Tab</b> – switch to previous tab.
--<b>Ctrl + Win + T </b>– open a new tab.
--<b>Ctrl + Win + N </b> - open a new window.
--<b>Ctrl + Win + W </b>– close current tab or window.
-<b>new UI</b> for easily opening new tabs and windows in the File Menu.
![alt text](images/tabsinfilewindow.png "tabs in file explorer")
<b>New context menu options for tabs in Sets</b>: If you right-click on a Sets tab, you’ll discover several options to leverage, including “close other tabs”, “move to new window”, and “close tabs to the right”.
![alt text](images/newcontextmenu.png "new context menu")

### Improvements to Tabs

-<b>Improvements to Previous Tabs</b>: We’ve done a few things to improve the experience in this space, including:
![alt text](images/previoustabs.png "previous tabs")
-<b>You can choose which Previous Tabs you want to restore</b>, in addition to being able to restore all tabs. 
-<b>You can now restore Previous Tabs from any type of activity</b> – in addition to restoring tabs when the primary window is a document.
-When you open a document that previously had tabs, a prompt will appear offering to restore those tabs, and the Previous Tabs button will be in the filled state. For things that aren’t documents, a prompt will not automatically appear, but you’ll know that there are tabs available to restore because the Previous Tabs button will be in the filled state.
-We added an animation to the experience when there are no Previous Tabs available to be restored.

## Bluetooth battery percentage in Settings

In Bluetooth & other devices Settings, you can now check the battery level of your Bluetooth devices. For Bluetooth devices that support this feature, the battery percentage will update whenever your PC and the device are connected.

TODO: IMAGE HERE

## Windows Calculator 

Windows Calculator has been updated (version 10.1803.711.0) to now correctly calculate square roots for perfect squares (integers that are squares of other integers). Because of the [arbitrary precision arithmetic library](https://blogs.msdn.microsoft.com/oldnewthing/20160628-00/?p=93765) used by the Calculator app, the square root calculation is an approximation calculated using the [Exponential Identity](https://en.wikipedia.org/wiki/Methods_of_computing_square_roots%23Exponential_identity) function.
Previously, when you would calculate the square root of 4, the result would be 1.99999999999999999989317180305609 which would be rounded to 2 when displayed, because we calculated enough digits to do the rounding correctly. However, as soon as you subtract 2, you would see the remaining digits.
After this update, the square root calculation now recognizes perfect squares and correctly returns exactly 2 for the square root of 4.

## Input Improvements 

<b>Emoji design updates</b> Based on your feedback and to improve consistency, we’ve made adjustments to the design of some of our emoji. Examples of updated emoji include:
<b>Before</b>
![alt text](images/before_emoji.png "emojis before")
<b>After</b>
![alt text](images/after_emoji.png "emojis after")

<b>Emoji search comes to more languages</b>: You can find an emoji by keyword in over 150 locales, including English (Great Britain), French (France), German (Germany), Spanish (Spain), and more. This will help you get the emoji you want easily and quickly. As a reminder, to bring up the Emoji Panel set focus to a text field and press WIN + (period) or WIN + (semicolon).

## Windows App Permissions 

You have more control so you can now decide which UWP apps can access your full file system. Particular UWP apps will be granted permission to have broad file system access. This capability will be granted on a per app basis by Microsoft. If a UWP app has the broad file system access restricted capability, you will receive a consent dialog prompting you to accept or deny the request. If at any time you change your mind about the decision, you can go to Settings > Privacy where you’ll find a new Settings page for File System Access. On this page, you can turn access on or off globally, and if it’s on you can also turn it on or off for each app that has requested the capability. UWPs with broad file system access will not appear in the Photos, Videos, or Documents privacy settings pages. If you grant broad file system access, this includes Photos, Videos and Documents.

## New features for Windows 10 Pro for Workstations

<b>A new power scheme – Ultimate Performance</b>: Demanding workloads on workstations always desire more performance. As part of our effort to provide the absolute maximum performance we’re introducing a new power policy called Ultimate Performance. Windows has developed key areas where performance and efficiency tradeoffs are made in the OS. Over time, we’ve amassed a collection of settings which allow the OS to quickly tune the behavior based on user preference, policy, underlying hardware or workload.
This new policy builds on the current High-Performance policy, and it goes a step further to eliminate micro-latencies associated with fine grained power management techniques. The Ultimate Performance Power plan is selectable either by an OEM on new systems or selectable by a user. To do so, you can go to Control Panel and navigate to Power Options under Hardware and Sound (you can also “run” Powercfg.cpl). Just like other power policies in Windows, the contents of the Ultimate Performance policy can be customized.

![alt text](images/ultimate_power_scheme.png "Ultimate power scheme")

As the power scheme is geared towards reducing micro-latencies it may directly impact hardware; and consume more power than the default balanced plan. The Ultimate Performance power policy is currently not available on battery powered systems.

<b>Productivity focused out of box applications</b>: In the Windows 10 Fall Creators Update, the out of box experience for Windows 10 Pro for Workstations draws from the Pro edition of Windows 10. One area where this is noticeable is the suite of applications installed out of the box visible as tiles in the start menu. In the next release for Windows, you will see for Windows 10 Pro for Workstations productivity and enterprise focused applications in place of consumer applications and games. This was one of the top feedback shared with us by our partners and users and we’re delivering this in our next update.

![alt text](images/productivity_apps.png "productivity apps")

