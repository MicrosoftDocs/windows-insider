---
title: PowerToys uodates
description: The latest updates to PowerToys
author: bleblanc
manager: dougkim
ms.tgt_pltfrm: na
ms.devlang: na
ms.author: v-allsh
ms.localizationpriority: medium
ms.topic: article
ms.prod: w10
---

# PowerToys

PowerToys is a set of utilities for power users to tune and streamline their Windows experience for greater productivity. Inspired by the [Windows 95 era PowerToys](https://en.wikipedia.org/wiki/Microsoft_PowerToys) project, this reboot brings you features to squeeze more efficiency out of Windows 10 and customize Windows for your individual workflows.

All the code for the project is on our [PowerToys GitHub](https://github.com/microsoft/PowerToys), which also has all the information and tools you need to understand how the PowerToys’ utilities work together and how to create your own utilities. 

The main PowerToys service runs when Windows starts and a user logs in. When the service is running, a PowerToys icon appears in the system tray. Selecting the icon launches the PowerToys settings UI. The settings UI lets you enable and disable individual utilities and provides settings for each. There is also a link to the help doc for each utility. You can right click the tray icon to quit the PowerToys service.
 
Note that some PowerToys functionality requires running in an elevated process. Elevation is required to interact with and manipulate windows from processes that have a higher set of rights than the current user. This is why the PowerToys.exe requests elevation when launched.

If you find bugs or have suggestions, please [open an issue in the Power Toys GitHub repo](https://github.com/microsoft/PowerToys/issues/new).

## March 5, 2020

### Announcing PowerToys 0.15.1

Yesterday, the PowerToys Team announced [the release of PowerToys 0.15.1](https://github.com/microsoft/PowerToys/releases/tag/v0.15.0). PowerToys 0.15.1 includes these improvements:

* Notifies you there’s a new version from within PowerToys.
* Removed requirement to always ‘run as admin.’
* Added almost 300 unit tests to increase stability and prevent regressions.
* Resolved almost 100 issues.
* Made .NET Framework parts of the source run faster with NGEN.
* Improved for how we store data locally.
* Increased FancyZones compatibility with applications.
* Created the [0 strategy](https://github.com/microsoft/PowerToys/wiki/Version-1.0-Strategy), [the launcher](https://github.com/microsoft/PowerToys/wiki/Launcher), [the keyboard manager specs](https://github.com/microsoft/PowerToys/wiki/Keyboard-Manager).
* Worked on cleaning up our issue backlog and labels.

[Get more details about these improvements.](https://github.com/microsoft/PowerToys/releases/tag/v0.15.0)

## October 29, 2019

### PowerToys v0.12 now available
We’ve just released our 0.12 release of PowerToys on GitHub. We’ve gotten tons of great feedback and suggestions from the community and want to directly say thank you to everyone.

New features include a great new utility called PowerRename, which makes it easy to batch rename a bunch of files, improvements to FancyZones, and support for Dark Mode.

Check out our [latest article](https://insider.windows.com/articles/powertoys-v012-now-available/) for all the details.

![New PowerRename feature](images/19003-1.gif)

## September 5, 2019

The first preview release of PowerToys has two utilities, the Windows key shortcut guide and a window manager called FancyZones. To try these out, [download the installer here](https://github.com/microsoft/PowerToys/releases). The main PowerToys service runs when Windows starts and a user logs in. When the service 

### Windows key shortcut guide

The Windows key shortcut guide is a full screen overlay utility that provides a dynamic set of Windows key shortcuts for the given desktop and currently active window. When the Windows key is held down for one second, (this time can be tuned in settings,) an overlay appears on the desktop showing all available Windows key shortcuts and what action those shortcuts will take given the current state of the desktop and active window. If the Windows key continues to be held down after a shortcut is issued, the overlay will remain up and show the new state of the active window.

Find detailed information on [the Windows key shortcut guide](https://github.com/Microsoft/PowerToys/tree/master/src/modules/shortcut_guide/README.md), the [backlog for this utility](https://github.com/microsoft/PowerToys/blob/master/doc/planning/ShortcutGuideBacklog.md), and the [source code](https://github.com/Microsoft/PowerToys/tree/master/src/modules/shortcut_guide).

![Windows key shortcut guide](images/Powertoys-1.png)

### FancyZones windows manager
FancyZones is a window manager that’s designed to make it easy to arrange and snap windows into efficient layouts for your workflow, and also to restore these layouts quickly. FancyZones allows the user to define a set of window locations for a desktop that are drag targets for windows. When the user drags a window into a zone, the window is resized and repositioned to fill that zone.
 
To get started with FancyZones, you need to enable the utility in the PowerToys settings, and then open the FancyZones setup UI. There’s a button in settings to open this UI, or you can press Win+~ to launch it. When first launched, the UI presents a list of zone layouts that can be quickly adjusted by how many windows are on the monitor. Choosing a layout shows a preview of that layout on the monitor. Pressing the save and close button sets that layout to the monitor.

![FancyZones editor](images/Powertoys-2.png)
 
The editor also supports creating and saving custom layouts. This functionality is in the Custom tab in the editor UI. There are two ways to create custom zone layouts, window layout, and table layout. These can also be thought of as additive and subtractive models. The additive window layout model starts with a blank layout and supports adding zones that can be dragged and resized, similar to windows.

The subtractive table layout model starts with a table layout and allows zones to be created by splitting and merging zones and then resizing the gutter between zones.
 
Find [more information on FancyZones](https://github.com/Microsoft/PowerToys/tree/master/src/modules/fancyzones/README.md), the [backlog for the utility](https://github.com/microsoft/PowerToys/blob/master/doc/planning/FancyZonesBacklog.md), and the [source code](https://github.com/Microsoft/PowerToys/tree/master/src/modules/fancyzones).
