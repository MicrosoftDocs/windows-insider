---
title: What's new in the Windows 10 Insider Preview Builds
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

#  What's new in the Windows 10 Insider Preview Builds for 1804
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

-<b>Keyboard shortcuts</b>
--<b>Ctrl + Win + Tab</b> – switch to next tab.
--<b>Ctrl + Win + Shift + Tab</b> – switch to previous tab.
--<b>Ctrl + Win + T </b>– open a new tab.
--<b>Ctrl + Win + W </b>– close current tab.

Finally, we’ve added some new UI for easily opening new tabs and windows in the File Menu.

![alt text](images/tabsinfilewindow.png "tabs in file explorer")


And also, in the context menu when right-clicking on a folder.

TODO: IMAGE HERE

<b>New context menu options for tabs in Sets</b>: If you right-click on a Sets tab, you’ll discover we’ve added several options for you to leverage, including “close other tabs”, “move to new window”, and “close tabs to the right”.

TODO: IMAGE HERE

Improvements to Previous Tabs: We’ve done a few things to improve the experience in this space, including:

TODO: IMAGE HERE

-You can now pick and choose which Previous Tabs you want to restore, instead of only being able to restore all tabs. Note: if you use the Sets activity card in Timeline, it will automatically restore all tabs.

-You can now restore Previous Tabs from any type of activity – whereas with the previous wave of features we only supported restoring tabs when the primary window was a document.

-When you open a document that previously had tabs, a prompt will appear offering to restore those tabs, and the Previous Tabs button will be in the filled state. For things that aren’t documents, a prompt will not automatically appear, but you’ll know that there are tabs available to restore because the Previous Tabs button will be in the filled state.

-We added an animation to the experience when there are no Previous Tabs available to be restored.

## Bluetooth battery percentage in Settings

In Bluetooth & other devices Settings, you can now check the battery level of your Bluetooth devices. For Bluetooth devices that support this feature, the battery percentage will update whenever your PC and the device are connected.

TODO: IMAGE HERE

## Windows Calculator 

Windows Calculator has been updated (version 10.1803.711.0) to now correctly calculate square roots for perfect squares (integers that are squares of other integers). Because of the [arbitrary precision arithmetic library](https://blogs.msdn.microsoft.com/oldnewthing/20160628-00/?p=93765) used by the Calculator app, the square root calculation is an approximation calculated using the [Exponential Identity](https://en.wikipedia.org/wiki/Methods_of_computing_square_roots%23Exponential_identity) function.
Previously, when you would calculate the square root of 4, the result would be 1.99999999999999999989317180305609 which would be rounded to 2 when displayed, because we calculated enough digits to do the rounding correctly. However, as soon as you subtract 2, you would see the remaining digits.
After this update, the square root calculation now recognizes perfect squares and correctly returns exactly 2 for the square root of 4.