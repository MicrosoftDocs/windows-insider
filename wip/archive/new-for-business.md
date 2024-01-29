---
ms.date: 06/18/2018
title: What was new in the Windows 10 Insider Program for Business Preview Builds
description: What was new in preview builds for Windows Insider for Business
author: bleblanc
manager: bleblanc
ms.tgt_pltfrm: na
ms.devlang: na
ms.author: allieshields
ms.localizationpriority: medium
ms.topic: article
ms.prod: w10
---

# What was new for business in Windows 10 Insider Preview Builds

## Windows Hello PIN in Safe mode (Build 18995)
Safe mode starts Windows in a basic state, using a limited set of files and drivers to help you troubleshoot problems on your PC. If a problem doesn’t happen in Safe mode, this means that default settings and basic device drivers aren’t causing the issue. [Read more about Safe mode](https://support.microsoft.com/help/12376/windows-10-start-your-pc-in-safe-mode).

With the latest flight, we’re taking another step forward in our Passwordless journey by adding Windows Hello PIN sign-in support to Safe mode, so that you no longer have rely on your password when troubleshooting your device. Try it out with the instructions below and let us know what you think!

* Set up Windows Hello in Settings > Accounts > Sign-in options
* Boot your device into Safe mode: 
1. Go to Settings > Update and Security > Recovery. 
2. Under Advanced startup select Restart now. 
3. After your PC restarts to the Choose an option screen, select Troubleshoot > Advanced options > Startup Settings > Restart. You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). 
4. After your PC restarts, you’ll see a list of options. Select 4 or press F4 to start your PC in Safe Mode. You can also select 5 or press F5 to use Safe Mode with Networking.
* Sign in to your device with your Windows Hello PIN

![Lock screen showing use of PIN in safe mode.](images/18995-1.png)

## Enabling automatic restart for UWP apps (Build 18990)
We already introduced a new [separate setting](./new-in-20h1.md#control-over-restarting-apps-at-sign-in-build-18965) to control if [registered desktop apps](/windows/win32/recovery/registering-for-application-restart) from your previous sign-in session are restarted when signing back in to Windows. In the latest Insider Preview builds, in addition to registered desktop apps, when you opt into this setting, the majority of open UWP apps are now also automatically restarted as well! To reduce sign-in time, UWP apps are restarted minimized, in a suspended state, giving Windows and other apps more resources to get started. To try it out:
1. Go to Settings > Accounts > Sign-in options and turn on “Automatically save my restartable apps when I sign out and restart them after I sign in.” under “Restart apps”.
2. Start one or more UWP apps, such as Feedback Hub.
3. Sign out and then sign back into Windows.

UWP apps that were started, such as Feedback Hub, should restart minimized with a taskbar button.

## Windows Subsystem for Linux (WSL) improvements (Build 18980)
In this build, we’ve added WSL2 support for ARM64 devices! We’ve also added the ability to set your distribution’s default user using the /etc/wsl.conf file. This release also contains multiple bug fixes, including a long-standing issue for legacy Windows symlinks (for example those in the user profile directory.)

For the full details of changes in this latest Insider Preview build, please see the WSL release notes.

![Fix for a long-standing issue for legacy Windows symlinks.](images/18980-1.png)

## Renaming your virtual desktops (Build 18975)
The ability to rename your virtual desktops is now available for all Insiders in the Fast ring! Thanks again everyone who shared feedback requesting this.
To get started:
1. Open Task View by selecting the Task View icon in the taskbar or pressing WIN+Tab.
2. Select New Desktop.
3. Select the desktop name (“Desktop 1”) and it should become editable, or right click the desktop thumbnail and a context menu will appear with a Rename entry.
4. Input whatever name you’d like, and press enter.
5. Done!

![Renaming your virtual desktops.](images/18963-2.gif)

## Cortana window can now move (Build 18975)
With the [new conversational Cortana experience](#new-cortana-experience-for-windows-10-build-18945), we understand that you want to keep the chat going sometimes, and the default position of the window isn’t always where you’d prefer to have it docked if you’re going to have a longer back and forth. That’s why we’ve rolled out the option to be able to move the window (by dragging the title bar area) to anywhere you’d like on the screen–just like you can with other windows. You can also resize the window if you’d like.
![Cortana window moves around the desktop.](images/18975-1.gif)

## New Reset this PC option: Cloud download (Build 18970)
Reset this PC provides users a new choice to download Windows or use local reinstall. Previously, Reset this PC was only able to do a local reinstall and would build a new Windows installation from existing Windows files. When this feature was introduced in Windows 10, version 1507, it provided the advantage of enabling Windows to be recoverable without requiring extra disk space to store a compressed backup copy of Windows in a hidden partition. We’ve heard feedback that some of you would prefer to use your high-speed internet connection to speed up this process by just downloading Windows.

>[!NOTE]
>This is a recovery operation and will remove apps you have installed. Additionally, if the “Remove everything” option is selected, user data will also be deleted. For more information on Reset this PC and other recovery options, see [Recovery options in Windows 10](https://support.microsoft.com/help/12415/windows-10-recovery-options).

The cloud download option will reinstall the same build, version, and edition, that is currently installed on your device. This new cloud download option is available to all Windows 10 devices and is different from the “Recover from the cloud” feature available on some earlier Windows 10 devices.

![Introducing a new Reset this PC option–Cloud Download.](images/18970-2.gif)

## New tablet experience for 2-in-1 convertible PCs (Build 18970)

Windows Insiders can take part in the new Beta tablet experience for 2-in-1 convertible PCs.

![The new tablet experience for 2-in-1 convertible PCs.](images/18970-1.png)

This new experience allows users entering tablet posture to stay in the familiar desktop experience without interruption, plus a few key touch improvements:
* Increased spacing between Taskbar icons.
* Search box on taskbar collapsed into an icon.
* File Explorer switches to touch-optimized layout.
* Touch keyboard auto invokes when you tap text fields.

As part of this, we’ve also made a few small changes to the tablet section in Settings.
Here are the steps once it becomes available on your PC:
1. Use your convertible PC as a laptop as you usually would–opening apps and interacting with them.
2. When you’re ready to pick it up and go or lean back on the couch, you can fold back the keyboard or remove it altogether, and it should switch to this new model shown above.
3. Now use your device as a tablet with touch.

## Control over restarting apps at sign-in (Build 18965)
Applications can register for restart, which helps in a few situations, including enabling you to get back to what you were doing if you need to restart your PC. Previously this option was tied to the “Use my sign-in info to automatically finish setting up my device” option under Sign-in options in accounts settings. We’ve heard feedback that some of you would prefer more explicit control over when Windows automatically restarts apps that were open when you restart your PC, and with 20H1 we’re bringing that option to you.

Windows puts you in control with a new app restart setting. When turned on, Windows automatically saves your restartable apps when signing out, restarting, or shutting down Windows, and restarts them next time you sign in. This setting is off by default and you can change it any time in Settings > Accounts > Sign-in options, and can find it by searching for “restart apps” in Start or the search box.

![Control over restarting apps at sign-in.](images/18965-1.png)

## Improving the Optional Features page in Settings (Build 18963)
Based on your feedback, we’ve made a number of usability improvements to the Optional Features page in Settings (Settings > Apps & Features > Optional Features).

* __Multi-select:__ You can select and install multiple optional features at the same time.
Better list management: You can search through lists of optional features and sort them by Name, Size, and Install date.
* __More useful information:__ You can see the install date for each optional feature in your ‘Installed features’ list. We’ve also added feature dependencies to the description of each optional feature in the list of features available for install.
* __Easier page navigation:__ View the status of your latest installs/uninstalls/cancel right on the main page in the ‘Latest actions’ section. You can add optional features and view your history via pop-up dialogues, so you never have to navigate away from the main page


![Improving the Optional Features page in Settings.](images/18963-3.jpg)

![Add an optional feature.](images/18963-4.png)

## Making Notepad store-updatable (Build 18963)
Notepad has been a well-loved text editor in Windows for over 30 years. Over the last few releases, we’ve been making a number of small improvements to Notepad based on your feedback including:

1. __Wrap-around find/replace:__ We’ve made significant improvement to the find/replace experience in Notepad. We added the option to do wrap-around find/replace to the find dialog and Notepad will now remember previously entered values and the state of checkboxes and automatically populate them the next time you open the find dialog. Additionally, when you have text selected and open the find dialog we will automatically populate the search field with the selected text.

![Notepad dialogue that supports wrap around find/replace.](images/18963-7.png)

2. __Text zooming:__ We’ve added options to make it quick and easy to zoom text in Notepad. There is a new menu option under View > Zoom to change the zoom level and we display the current zoom level in the status bar. You can also use Ctrl + Plus, Ctrl + Minus and Ctrl + MouseWheel to zoom in and out and use Ctrl + 0 to restore the zoom level to the default.

![Notepad gif showing new text zooming options.](images/18963-8.gif)

3. __Line numbers with word-wrap:__ A long outstanding request has been to add the ability to display line and column numbers when word-wrap is enabled. This is now possible in Notepad and we’ve made the status bar visible by default. You can still turn the status bar off in the View menu.

![Notepad showing that line and column numbers now work with word-wrap.](images/18963-9.gif)

4. __Modified indicator:__ Notepad will now show an asterisk in the title bar before the title of a document to indicate that a document has unsaved changes.

![Notepad title with an asterisk showing it has unsaved changes.](images/18963-6.png)

5. __Send Feedback:__ You can now send feedback directly from Notepad! Click Help > Send Feedback to open the Feedback Hub with the Notepad category selected and get your feedback directly to the product team.

![Option in Help to Send Feedback from Notepad.](images/18963-10.png)

__UTF-8 Encoding:__ We’ve made significant improvements to the way Notepad handles encoding. Starting with this build, we are adding the option to save files in UTF-8 without a [Byte Order Mark](https://en.wikipedia.org/wiki/Byte_order_mark) and making this the default for new files. UTF-8 without a Byte Order Mark is backwards-compatible with ASCII and will provide better interoperability with the web, where UTF-8 has become the default encoding. Additionally, we added a column to the status bar that displays the encoding of the document.

__Other Updates__

* __[Expanding line support](https://devblogs.microsoft.com/commandline/extended-eol-in-notepad/)__
* We’ve added support for some additional shortcuts:
  * Ctrl+Shift+N will open a new Notepad window.
  * Ctrl+Shift+S will open the Save as… dialog.
  * Ctrl+W will close the current Notepad window.
* Notepad can now open and save files with a path that is longer than 260 characters, also known as MAX_PATH.
* We’ve fixed a bug where Notepad would count lines incorrectly for documents with very long lines.
* We’ve fixed a bug where, when you select a placeholder file from OneDrive in the File Open dialog, we would download the file to determine its encoding.
* We’ve fixed a recent regression where Notepad would no longer create a new file when launched with a file path that didn’t exist.
* We’ve improved the performance when opening large files in Notepad.
* Notepad now supports Ctrl + Backspace to delete the previous word.
* Arrow keys now correctly unselect text first and then move the cursor.
* When saving a file in Notepad, the line and column number no longer reset to 1.
* Notepad now correctly displays lines that don’t fit entirely on the screen.


Starting with this build, we’re making a change so that future Notepad updates will be automatically available via the store. This will allow us the flexibility to respond to issues and feedback outside the bounds of Windows releases. As always, if you have any feedback for Notepad, we welcome it in the Feedback Hub under [Apps > Notepad](https://aka.ms/notepadfeedback).

## Adding Mouse Cursor speed to Settings (Build 18963)
You can set your mouse cursor speed from within Settings! This is the latest piece of our larger ongoing effort to converge Settings and Control Panel experiences. You can find the setting under Settings > Devices > Mouse.

!["Adding Mouse Cursor speed to Settings](images/18963-5.png)

## GPU temperature comes to Task Manager (Build 18963)
One of the longstanding requests we’ve been tracking for Task Manager is to add temperature monitoring support, and with today’s build we’re making progress on that ask. If you have a dedicated GPU card, we will bubble up the current temperature next to its listing in the Performance Tab.

![GPU temperature comes to Task Manager.](images/18963-1.png)

## A redesigned Network Status page in Settings (Build 18956)
Based on your feedback, we’re revamping the Network & Internet landing page in Settings to provide more information at a glance about your device’s connectivity, combining several pages to give you one clear view of how you are connected to the internet.
* __New view of active connections:__ We show all available connection interfaces on the Status page, so you can quickly see what is connected and view and change properties as needed. If you have multiple connections, only one will be used for internet connectivity at a time, and that one is still shown in the Status diagram at the top of the page.

![New view of active connections.](images/18956-1.png)

* __Integrated Data Usage:__ You can see how much data is being used by a network right from the Status page! If it looks like you’re using a lot of data, you can drill into the Data Usage page to create a limit for that network, which will warn you if you get close or go over your limit. You can also see how much data each app is using on that network.

![Integrated Data Usage](images/18956-2.png)

We hope you like the changes! If you have any feedback about these, you can share it via the Feedback Hub under **Network and Internet** > **Networking Experience – Look and Feel**.

## Notification settings improvements (Build 18956) 
Thanks everyone who’s tried out our [improvements so far](#refining-your-notification-settings-build-18932). To recap what you’ll see when you have the change:
* If you hover your mouse over an incoming notification, you’ll see a settings icon to make it easy to adjust that app’s notification settings.
* We’ve updated the design of the per-app notification settings for visual clarity.
* There’s a direct link to notification settings at the top of the Action Center.
* Notifications & Action Settings has a checkbox for muting the sound of all notifications.
* By default, the senders in Notifications & Action Settings are sorted by “most recently sent a notification.”

![Notification settings improvements rolling out to all of Fast.](images/18956-4.png)

## Windows Subsystem for Linux (WSL) Improvements (Build 18945) 
### Added connecting via localhost to WSL 2 Linux apps from Windows and global WSL configuration options

You’ll be able to connect to your WSL 2 Linux networking applications using localhost. For example, the image below shows starting a NodeJS server in a WSL 2 distro, and then connecting to it in the Edge Browser with localhost.

![Added connecting via localhost to WSL 2 Linux apps from Windows and global WSL configuration options.](images/18945-2.png)

Additionally, we’ve added global configuration options for WSL. These are options that will apply to each of your WSL distros. This also allows you to specify options that relate to the WSL 2 virtual machine (VM), as all your WSL 2 distros run inside of the same VM. The most exciting option that you’ll get access to in this build is able to specify a custom Linux kernel!
For the full details on what’s new in this release, check out [What’s new for WSL in Insiders Preview Build 18945](https://devblogs.microsoft.com/commandline/whats-new-for-wsl-in-insiders-preview-build-18945) on the Windows command line blog.


## New File Explorer search experience (Build 18945)

We heard your feedback asking for increased consistency, and to make it easier to find your files. We are happy to announce that you can now take advantage of the new File Explorer search experience – powered by Windows Search. This change will help integrate your OneDrive content online with the traditional indexed results.

What does that mean for you? Once you have the new experience, as you type in File Explorer’s search box, you’ll now see a dropdown populated with suggested files at your fingertips that you can pick from.

These improved results can be launched directly by clicking the entry in the new suggestions box, or if you want to open the file location, just right-click the entry and there’ll be an option to do so. If you need to use commands or dig deeper into non-indexed locations, you can still press enter and populate the view with the traditional search results.

Showing the new dropdown that appears when you type in File Explorer’s search box.

![Updated File Explorer search.](images/18945-4.png)

We’ve also updated the design, so as soon as you click the search box in File Explorer (or press CTRL+E to set focus to it), you’ll see the dropdown list with your search history.

If you encounter any issues, or have any feedback, file them under “Files, Folders, and Online Storage” > “File Explorer” in the Feedback Hub.

>[!NOTE]
>You may notice in the screenshot, we’ve made the File Explorer search box wider so the suggestions dropdown has a bit more room to show results – that’s not a new option, but we figured you might want to know how to do it: just move your mouse to the starting border of the search box, and your mouse should turn into a resizing double arrow cursor. Just click down and drag the search box to be a bit wider.


## New Cortana experience for Windows 10 (Build 18945)
Now available, a new Cortana experience for Windows 10 as a Beta to Windows Insiders in the U.S. This new experience features a brand-new chat-based UI that gives you the ability to type or speak natural language queries.

![Introducing a new Cortana experience for Windows 10.](images/18945-1.png)

It supports most of the Cortana features people enjoy using on Windows, such as Bing answers, Assistant conversations, opening apps, managing lists, and setting reminders, alarms, and timers. And we’ve added some new features we think people will enjoy:

* Cortana supports both light and dark themes in Windows.
* We have created a new, less intrusive screen for “Hey Cortana” queries so you can stay in the flow while you work.
* We have updated Cortana with new speech and language models, and significantly improved performance – making it faster and more reliable than ever before.

Not all the features from the previous Cortana experience are available just yet. As a Beta, we plan to add more features over time with updates to Cortana from the Microsoft Store.

To get started, choose the Cortana icon on the taskbar next to the search box. You can also leverage the speed and convenience of voice with improved speech recognition by simply saying “Hey Cortana”. You may need to sign-in with your account to get started.

>[!NOTE]
> This requires enabling this functionality in Settings > Voice activation privacy settings  – Talk to Cortana. 

Additional markets and languages will become available at a later date. You must be signed in to use Cortana. Historically, there were quite a few skills that could be used unauthenticated (Bing answers, open apps, Assistant conversations) but this is no longer the case.

## Refining your notification settings (Build 18932)
Over the last few releases, based on your feedback, we’ve been working on giving you more control over potential interruptions. [Introducing Focus Assist](https://blogs.windows.com/windowsexperience/2018/05/09/windows-10-tip-how-to-enable-focus-assist-in-the-windows-10-april-2018-update/) to automatically suppress notifications when you’re trying to stay in the moment and not get distracted, and adding the option to use middle click to dismiss notifications if you want to quickly make a notification toast go away.
One thing we’ve heard from you, though, is that our notification settings aren’t easily discoverable. In addition, once you find the settings, they can be difficult to understand.
In order to address this, we’ve made a few changes, including:
1. When you receive a notification toast, there will be an inline option to turn off notifications for that app, or head to the app’s notification settings.

![Notification toast you can now right-click to open notification settings.](images/18932-5.gif)

2. When you dive into an app’s notification settings, you’ll find that we’ve added pictures to help articulate the impact of a certain settings.

![The new notifications settings.](images/18932-6.png)

3. Prefer to have all your notifications muted? You no longer have to go to the old sound control panel to do that – we’ve added it as a top-level option in Notification & Actions Settings.

4. But wait, there’s more! We’ve also added a new direct link at the top of the Action Center to manage notifications, so it takes one less step to get to Notification & Actions settings. To make room for this we’ve moved the “no notifications” text down to the middle of the Action Center, which also means your eyes don’t have to traverse as far to see it when you launch the Action Center from the bottom of the screen.

![Manage your notifications settings is now just one click away in the Action Center.](images/18932-7.png)

5. Finally, ever dismissed a notification you wanted to disable, and went to Notification & Actions Settings only to find the list of notification senders to be really long? You can sort the list by which apps most recently sent notifications.

![Most recent filter in notification settings to make it easier to adjust what you've seen recently.](images/18932-8.png)

## Windows Subsystem for Linux 2 (Build 18917)
WSL 2 is a new version of the architecture that powers the Windows Subsystem for Linux to run ELF64 Linux binaries on Windows. This new architecture, which uses a real Linux kernel, changes how these Linux binaries interact with Windows and your computer’s hardware, but still provides the same user experience as in WSL 1 (the current widely available version). WSL 2 delivers a much faster file system performance and full system call compatibility, which lets you run more applications like Docker!
[Read more about the release of WSL 2](https://devblogs.microsoft.com/commandline/wsl-2-is-now-available-in-windows-insiders/).

![Introducing Windows Subsystem for Linux 2.](images/18917-2.gif)

## New download throttling options for Delivery Optimization (Build 18917)
We’ve heard from our users with very low connection speeds that setting download throttling as a percentage of available bandwidth isn’t providing enough relief in reducing the impact on their network. That’s why we’ve added a new option to throttle the bandwidth used by Delivery Optimization as an absolute value. You can set this separately for Foreground downloads (downloads that you initiate from Windows Store for example) or background downloads. This option already exists for IT Pros who use Group Policies or MDM policies to configure Delivery Optimization. In this build, we’ve made it easier to set via the settings page. You can access this option via Settings > Update & Security > Delivery Optimization > Advanced Options

![New download throttling options.](images/18917-1.jpg)


## Disk type visible in Task Manager Performance tab (Build 18898)
A small, but perhaps convenient change — you’ll be able to see the disk type (e.g. SSD) for each disk listed in Task Manager’s performance tab. This is particularly helpful in cases where you have multiple disks listed, so you can differentiate between them.

![Expanded language support.](images/18898-1.png)

## Improved Windows Sandbox accessibility (Build 18855)
We have made several updates to improve Windows Sandbox accessibility scenarios. This includes: 
* Microphone support
* Added functionality to configure the audio input device via the Windows Sandbox config file
* A Shift + Alt + PrintScreen key sequence in Windows Sandbox which activates the ease of access dialog for enabling high contrast mode.
* A ctrl + alt + break key sequence in Windows Sandbox which allows entering/exiting fullscreen mode

## Windows Sandbox configuration file support (Build 18841)
Windows Sandbox supports configuration files! These files allow users to configure some aspects of the sandbox, such as vGPU, networking and shared folders. [Check out the blog post explaining this new feature](https://aka.ms/WindowsSandbox_ConfigFile).
