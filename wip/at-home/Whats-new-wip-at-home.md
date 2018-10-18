---
title: What's new in the Windows 10 Insider Preview Builds (19H1)
description: New Windows features for Windows Insider Program Preview Builds
services: WIP-at-home
author: dawnwood
manager: eliotgra
ms.assetid: 
ms.service: WIP-at-home
ms.tgt_pltfrm: na
ms.devlang: na
ms.date: 10/08/2018
ms.author: dawn.wood
ms.localizationpriority: medium
---

# What's new in the Windows 10 Insider preview builds (19H1)
The [Windows Insider Program](https://insider.windows.com/en-us/) lets you preview builds of the upcoming release of Windows 10. This topic lists all new Windows 10 features for you to try. 

## DPI Awareness in Task Manager (Build 18262)
We added a new optional column to the **Details** tab of **Task Manager** so you can look at DPI awareness per process as in the following example:

![Showing the DPI Awareness category in Task Manager, with examples of Per-Monitor and System ](images/dpi-aware-task-manager.png "Showing the DPI Awareness category in Task Manager, with examples of Per-Monitor and System ")

To show the column, right-click on any of the column headers in the **Details** tab, click **Select Columns**, then add **DPI Awareness** to the list. To learn more about DPI Awareness, see [High DPI Desktop Application Development on Windows](https://docs.microsoft.com/en-us/windows/desktop/hidpi/high-dpi-desktop-application-development-on-windows).

## Uninstall additional inbox apps (Build 18262)
In 19H1, we are adding the ability to uninstall the following (preinstalled) Windows 10 inbox apps via the context menu on the **Start** menu **All Apps** list:
* 3D Viewer (previously called Mixed Reality Viewer)
* Calculator
* Calendar
* Groove Music
* Mail
* Movies & TV
* Paint 3D
* Snip & Sketch
* Sticky Notes
* Voice Recorder

In the Windows 10 October 2018 Update and prior, only the following inbox apps could be uninstalled via the context menu on the **Start** menu **All Apps** list: 
* Microsoft Solitaire Collection
* My Office
* OneNote
* Print 3D
* Skype
* Tips
* Weather

## Narrator Improvements (18262)
**Narrator Read by Sentence**: You can now read next, current and previous sentences in Narrator. Read by sentence is available with the keyboard and with touch. Move by sentence doesn’t yet work for Braille. 
* Caps + Ctrl + Period (.) to Read next sentence
* Caps + Ctrl + Comma (,) to Read current sentence
* Caps + Ctrl + M to Read previous sentence 
Sentence is now a new Narrator view and can be reached via Caps + Page Up or Caps + Page Down and then you can navigate with Caps + Left arrow for move by previous sentence and Caps + Right arrow for move by next sentence. 

## Enhanced settings for Ethernet (Build 18252)
You can now use the **Settings** app to configure advanced Ethernet IP settings. We have added support for configuring a static IP address as well as setting a preferred DNS server. These settings were previously accessed within **Control Panel**, but you will now find them on the connection properties page under **IP settings**.

![Showing the enhanced ethernet settings](images/enhanced-ethernet-settings.png "Showing the enhanced ethernet settings")

## New icon for disconnected Internet (Build 18252)
First seen on Always Connected PCs, we brought the disconnected internet icon to all devices running Windows 10. This single icon appears when there is no internet connection detected, and replaces the individual disconnected icons for Cellular, Wi-Fi, and Ethernet. This new icon should help you quickly identify network problems so that you can take action to resolve them.

![Showing the new icon for disconnected internet](images/disconnected-internet-icon.png "Showing the new icon for disconnected internet")

## Ebrima font addition with ADLaM support (Build 18252)
You can now read your ADLaM documents and webpages with the Windows Ebrima font!

ADLaMis a writing system for Pular/Fulfulde, the language of the Fulani people, predominantly residing in west Africa. In the early 1990s, two young teenager brothers, Abdoulaye and Ibrahima Barry, created this writing system. Their work became “Bindi Pulaar” and eventually “ADLaM,” ADLaM is enabling literacy and growing in use for commerce, education, and publishing across western Africa. It was added to Unicode in Unicode 9.0.

The Ebrima font also supports other African writings systems N’ko, Tifinagh, Vai and Osmanya – here’s a sample of what the font looks like:

![Showing sample of the Ebrima font](images/ebrima-font.png "Showing sample of the Ebrima font")

## Bringing acrylic to the Windows sign-in screen (Build 18237)
The Windows sign-in screen now supports [acrylic](https://docs.microsoft.com/en-us/windows/uwp/design/style/acrylic), a type of brush from the [Fluent Design System](https://docs.microsoft.com/en-us/windows/uwp/design/fluent-design-system/index), to the sign-in screen background.  The translucent texture of this transient surface helps you focus on the sign-in task by moving the actionable controls up in the visual hierarchy while maintaining their accessibility.

![Showing acrylic in Windows sign-in screen](images/acrylic-sign-in.png "Showing sample of the Ebrima font")