---
title: The Changelog
description: New Windows 10 features for Insider Preview builds in the Dev Channel.
author: bleblanc
manager: dougkim
ms.tgt_pltfrm: na
ms.devlang: na
ms.author: bleblanc
ms.localizationpriority: medium
ms.topic: article
ms.prod: w10
---

# The Changelog
The Changelog represents everything new from all the builds from the Active Development Branch released to the **Dev Channel**. This page includes everything noted as part of the "What's new" and "General changes & improvements" sections of the blog posts published for each build [on the Windows Blog](https://blogs.windows.com/windows-insider/) and does not contain other noted updates for Insiders, fixes, or known issues. 

## Build 21370
Windows 10 Insider Preview Build 21354 was released to the Dev Channel on [4/14/2021](https://blogs.windows.com/windows-insider/2021/04/14/announcing-windows-10-insider-preview-build-21359/).

### Improving the Bluetooth audio experience
Over the past several months, we have been adding new features to make Bluetooth audio streaming easier, better, and more performant.

![Improved Bluetooth audio experience](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/04/unified_endpoint.png "Updates to the “Select playback device” dropdown on the taskbar for Bluetooth audio devices. ")

* Unified audio endpoint: No more clicking through multiple audio endpoints to make your Bluetooth headset’s voice and mic work properly. We now only expose one audio endpoint in the UI and will switch to the correct one automatically for you for a seamless experience. Listening to Spotify and then have to hop onto a Teams call? You can also now directly control the volume of your headset.
* Support for AAC codec: Enjoy premium audio streaming quality wirelessly on your Bluetooth headphones and speakers with AAC codec. Short for Advanced Audio Codec, AAC is a lossy codec that delivers high quality audio streaming in smaller files – great for listening to music online.

### Changes and Improvements
* We’ve made some small adjustments to the icons in File Explorer’s address bar.
* We’ve improved the touch keyboard launch animation to make it smoother in cases where UWP apps reflow when it appears.
* We made a change so that if you set focus to the Run dialog, the touch keyboard will now show a backslash (\) key.

## Build 21364
Windows 10 Insider Preview Build 21354 was released to the Dev Channel on [4/21/2021](https://blogs.windows.com/windows-insider/2021/04/21/announcing-windows-10-insider-preview-build-21364/).

### Run Linux GUI applications directly on Windows using the first preview of GUI app support on the Windows Subsystem for Linux (WSL)
The Windows Subsystem for Linux now includes a first preview of support for GUI applications! This means you can now run your favorite GUI editors, tools, and applications, to develop, test, build and run your Linux apps! For more info on this change please view [this blog post](https://devblogs.microsoft.com/commandline/the-initial-preview-of-gui-app-support-is-now-available-for-the-windows-subsystem-for-linux-2/).

### Task Manager supports Microsoft Edge process classification
We partnered with the Microsoft Edge team to support process classification in Task Manager. This will help you to identify resource consumption under Microsoft Edge. The classification is broken down to several different components like Tabs, Browser processes (Browser, GPU Process, Crashpad), Utility plugins (Utility: Audio Service Extensions), Dedicated & Service workers etc. It also features separate icons for each process to help you identify them including fav icon for website. Head over to this Microsoft Edge blog post for a list of detailed improvements.

![Edge processes in Task Manager](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/04/task-manager-edge.png "Showing Microsoft Edge process classification support in Task Manager.")

>[!NOTE]
>NOTE: This feature is available to Windows Insiders that are running the latest Microsoft Edge Canary or Dev builds. Insiders can download the latest version here. This feature is also rolling out to a subset of Insiders in the Dev Channel at first, to help us quickly identify issues that may impact performance and reliability. Rest assured they will be gradually rolled out to everyone in the Dev Channel.

### Eco mode in Task Manager
Task Manager has a new experimental feature in this build called “Eco mode” which provides users with an option to throttle process resources. It will also help identify apps that are already running in Eco mode. This feature is helpful when you notice an app consuming high resources and would like to limit its consumption so that the system gives priority to other apps which will lead to faster foreground responsiveness and better energy efficiency.

![Right-click Eco mode in Task Manager](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/04/task-manager-eco.png "Right-click on child processes in Task Manager to enable “Eco mode”.")

Here is how to enable Eco mode for any process:

1. Open Task Manager.
2. Click on Processes tab.
3. Right-click on a child process or an individual process.
4. Click on “Eco mode” in the context menu to apply throttling.
5. The status column in the Processes tab should show Eco mode for the process.

This same process also works on the Details tab too.

If “Eco mode” is greyed out, then it’s a parent/group process. You can expand the process tree to apply Eco mode on one of its child processes.

And if Microsoft Edge (or Chrome) is showing “Eco mode” as enabled but you did not apply it, this is due to both Microsoft Edge and Chrome experimenting with lowering base priority and applying power efficiency APIs to improve performance which is similar to what Task Manager is doing to identify “Eco” efficient apps. You may see other apps with “Eco mode” if they adapt to similar techniques to improve performance.

You can submit feedback on these recent Task Manager changes in Feedback Hub under Desktop Environment > Task Manager.

>[!NOTE]
>NOTE: This feature is rolling out to a subset of Insiders in the Dev Channel at first, to help us quickly identify issues that may impact performance and reliability. Rest assured they will be gradually rolled out to everyone in the Dev Channel.

### Japanese 50-on touch keyboard
We’re excited to introduce a new touch keyboard layout for Japanese, 50-on touch keyboard. 50-on touch keyboard is a popular layout widely used for Kiosk devices in Japan. It allows you to input Japanese texts intuitively without knowing how to compose Hiragana characters.

![50-on touch keyboard layout for Japanese](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/04/1_Japanese50onTouchKeyboardHiraganaView.png "The new 50-on touch keyboard layout for Japanese.")

You can switch to 50-on layout from [⚙] > [50-on]. It also provides alphabet and symbol views newly designed specifically for the layout. You may notice some known issues where inserting a full-width space using Shift key doesn’t work and typing some characters shows garbled suggestion candidates. We’re actively working on addressing them. Thank you for your patience. We’re looking forward to your feedback via [Give feedback] menu!

![Enable 50-on touch keyboard layout for Japanese](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/04/2_Japanese50onTouchKeyboardSwitchingLayout.png "Enabling the new 50-on touch keyboard.")

### Changes and Improvements
* Based on feedback, we’re updating the notification that used to say “We need to fix your account (most likely your password changed)”, to be more representative of what it’s for, and now say “Select here to sign in to your account to continue using apps between this device and your other devices.”
* When you turn on or off night light manually, for example via the Action Center, night light will now turn on immediately rather than slowly transition.
* You can now turn off Aero Shake via Settings > System > Multitasking and choosing the “off” toggle under “Title bar window shake”. This setting is now off by default so for those who want it back will need to turn this setting on.

## Build 21359
Windows 10 Insider Preview Build 21354 was released to the Dev Channel on [4/14/2021](https://blogs.windows.com/windows-insider/2021/04/14/announcing-windows-10-insider-preview-build-21359/).

### News and interests available to 100% of Dev Channel
As of Build 21359, we’re rolling out news and interests on the taskbar to 100% of the Dev Channel! News and interests makes it easy to stay up to date with information at a glance and has incorporated ongoing improvements based on Insider feedback. We acknowledge that many of you have had to wait some time to experience it and appreciate your patience. We can’t wait to hear what you think!

### Changes and Improvements
* We have added an option under the Power menu on the Start menu to restart apps after signing in when you reboot your device. When this setting is checked, it toggles the option under Settings > Accounts > Sign-in options > Restart apps we introduced in 20H1.
![Power menu restart apps](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/04/new-restart-apps.png "We have added an option under the Power menu on the Start menu to restart apps after signing in when you reboot your device.")
* If you have your activity history synced across your devices through your Microsoft account (MSA), you’ll no longer have the option to upload new activity in Timeline. AAD-connected accounts won’t be impacted. To view web history, Edge and other browsers have the option to look back at recent web activities. You can also view recently used files using OneDrive and Office. **Note: Timeline and all your local activity history still remain on Windows 10.**
* We’re updating the Ease of Access category in Settings to now be called Accessibility.
* We’re updating the Ebrima font to now support characters from Bamum (Unicode block U+A6A0 to U+A6FF).
* We’re updating the Nirmala UI font family to improve how the Chakma characters are displayed when combined based on feedback.
* Thank you to the Insiders who have taken the time to share feedback about the new version of our Korean IME. For the time being we will be reverting to the version included in previous releases.

## Build 21354
Windows 10 Insider Preview Build 21354 was released to the Dev Channel on [4/7/2021](https://blogs.windows.com/windows-insider/2021/04/07/announcing-windows-10-insider-preview-build-21354/).

### New personalization options for news and interests on the taskbar
Thanks for your continued feedback for news and interests on the Windows taskbar! We’re continuing to develop the experience based on your suggestions. Today, we’re pleased to announce a new set of features rolling out for personalizing the feed to suit your interests.

Now, when you hover on the weather on your taskbar, you’ll see a new “Manage interests” button appear at the top of the window. This button links to a new full-page personalization experience, where you can choose the topics that you’re interested in. New users may also see a personalization card in their feed to help them get started.

![News and interests manage](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/04/news-and-interests-flyout-scaled.jpg "News and interests on the Windows taskbar showing a new “Manage interests” button and personalization card to help new users get started with their feed.")

Use the search box at the top of the “My interests” page to search for the topics or publishers you want to follow. You can also discover interests by browsing over a dozen categories, including different types of news, entertainment, and sports topics. When you select a topic to follow, you’ll see more stories about it in your feed as stories become available. You can manage the topics you’re following by selecting “Followed interests” in the left navigation.

![News and interests My Interests](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/04/news-and-interests-personalization-flow.gif "The “My interests” page enables you to follow topics you’re interested in and tune your feed with publishers and articles that pique your interest.")

We’re also excited to announce, “Tune your feed”, available from the left navigation on the “My interests” page. This experience makes it easy to explore and follow publishers from our partner ecosystem and select example articles that pique your interest. Select a couple of publishers and stories to get started or scroll to see more. You can see and manage the publishers you’re following by clicking “Followed Publishers” on the left navigation. You can also tune your feed wherever you see a story. Click the “X” on the top right of the card to remove the article and provide feedback: “Not interested in this story”, “Don’t like the source”, or “Report an issue”. We’ve refined this experience based on user feedback, to give you another way to fine-tune your feed for your preferences.

These new personalization experiences are now available in several markets, including the U.S., U.K., Canada, India, and Australia, with global rollout continuing. We look forward to hearing what you think about these new options for personalizing news and interests!

>[!NOTE]
>Reminder: We continue to roll out news and interests to Windows Insiders, so it isn’t available to everyone in the Dev Channel just yet.

### Improvements to Display Settings
**Content adaptive brightness control (CABC) disabling:** CABC helps improve battery performance on PCs, but with the trade-off of decreased image quality. It can result in distracting brightness changes that interfere in experiences where image quality is of high importance such as for creative professionals looking for color accuracy. The ability to turn CABC off has been a highly requested feature and Windows Insiders can now disable CABC directly in the Display settings via Settings > System > Display.

![CABC disable](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/04/CABC-UI.png "Windows Insiders can now disable CABC directly in the Display settings via Settings > System > Display.")

*Note: Depending on your device, you may see just one (or both) of the checkboxes seen under the brightness slider below. To find out if your device has CABC support, you can look at your GPU control panel.*

**HDR certification:** To bring awareness to high quality HDR displays and educate customers, we are bringing HDR certification to Settings > System > Display under “Advanced display settings” with the latest Insider Preview builds. Under this settings page, a display’s HDR certifications will be shown.

We will be rolling out this feature over time and are starting with select Dolby Vision and VESA DisplayHDR models, so please don’t be alarmed if in the Advanced display settings, you see that your display has no HDR certification even though it is certified.

### New Camera Settings page
We are extremely excited to introduce a new Camera Settings page we’ve been working on, giving users the ability to add/remove cameras and configure the default image settings of each one.

![New Camera Settings page](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/04/Camera-L1-light.png "The Camera Settings Page lets you discover, pair and unpair ONVIF IP cameras, as well as view and manage all video cameras on the device.")

This page allows you to manage cameras through the Settings app, whether they’re connected directly to the device (like a webcam) or are ONVIF IP cameras on your local network (for more info on ONVIF support in Windows, see this blog post). This new Settings page can be found at Settings > Devices > Camera. Each camera has a “Configure” button that lets you make changes to the default brightness and contrast – letting you get rid of the pesky backlight that always shadows your face in your video calls. Depending on what features are supported by your camera, you can configure brightness and contrast, enable Video HDR or Eye Contact, or correct for camera rotation.

![Configure camera on Camera Settings page](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/04/Camera-L2-light.png "The Configure page for cameras allows you to adjust default image settings such as brightness and contrast.")

We look forward to hearing your feedback about this new feature. Please try out the Configure default image settings for your camera Quest on Feedback Hub and then send us your feedback at the end – we’d love to hear what other features you’d like to see, and if you run into any issues with your specific PC, camera and/or video app.

### Inbox app updates
**MSPaint is now updated via the Microsoft Store:**

![New MSPaint icon](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/04/Paint-Icon.png "New MSPaint app icon.")

MSPaint is now updateable via the Microsoft Store outside major OS updates. It also has a new icon and has been promoted out of the Windows Accessories folder to its own place in the Start menu.

**Snipping Tool is now updated via the Microsoft Store:**

![Snipping Tool icon](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/04/Snipping-Tool-icon.png "Snipping Tool app icon.")

Snipping Tool is now updateable via the Microsoft Store outside major OS updates. It has been packaged together with Snip & Sketch so we can deliver updates for both at the same time. It has also been promoted out of the Windows Accessories folder to its own place in the Start menu.

*NOTE: Because we’re combining both Snip & Sketch and Snipping Tool, Insiders who previously did not have Snip & Sketch installed will see Snipping Tool removed after updating to this build and will have to go and install Snip & Sketch from the Store to get it back.*

**Organizing all the admin and system tools under Windows Tools:**

![New Windows Tools icon](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/04/Windows-Tools-icon.png "The Windows Tools shortcut icon.")

In Build 21343, we announced we changed the name of the Windows Administrative Tools folder in Start to Windows Tools as part of an effort to better organize all the admin and system tools in Windows 10. In Build 21354, we are continuing that effort. The Windows Accessories, Windows Administrative Tools, Windows PowerShell, and Windows System folders have now been removed from Start and the apps within these folders can now be accessed via the Windows Tools entry point that directs to the full apps list in File Explorer. All these apps will still appear in via search, launch via any method, can be pinned to Start or taskbar, and any customized shortcuts in the folder paths will remain intact. Also, File Explorer has been moved into its own place in the Start menu as part of this work.

### Changes and Improvements
* [News and interests] As [mentioned previously](https://blogs.windows.com/windows-insider/2021/03/10/announcing-windows-10-insider-preview-build-21332/), we have enabled the ability to deselect “Open on hover” in the “News and interests” taskbar options. This is based on your feedback.
* The default path to access Linux files from Windows using the Windows Subsystem for Linux has been changed from `\\wsl\\` to `\\wsl.localhost\\` to improve performance and reliability. You will still be able to access Linux files using `\\wsl$\\`.
* Under Settings > Update & Security > Change active hours, you will find the toggle turned on for “Automatically adjust active hours for this device based on activity”, if you have never adjusted this feature. We are starting a roll out a change for Insiders that makes this setting on by default. With this setting turned on, Windows Update will be able to schedule automatic restarts when you are typically not using your device more accurately.
* As of the latest versions of Microsoft Edge, all pinned sites (regardless of what version you were using when you pinned them), should now use the taskbar behavior described [here](https://blogs.windows.com/windows-insider/2020/07/22/announcing-windows-10-insider-preview-build-20175/) without you first having to unpin and re-pin the site.
* On ARM64 devices, you can now toggle compatibility settings for x64 applications.
* Under Settings > Personalization > Device usage, you can select all the ways you plan to use your device to get customized suggestions for tips, tools, and services.

## Build 21343
Windows 10 Insider Preview Build 21343 was released to the Dev Channel on [3/24/2021](https://blogs.windows.com/windows-insider/2021/03/24/announcing-windows-10-insider-preview-build-21343/).

### New icons in File Explorer
We first [began updating the icons in Windows 10 last year](https://blogs.windows.com/windows-insider/2020/02/20/announcing-windows-10-insider-preview-build-19569/) starting with the built-in apps. Since then, we have continued updating icons throughout Windows 10 including [the icon for Windows Security](https://blogs.windows.com/windows-insider/2020/03/05/announcing-windows-10-insider-preview-build-19577/), [the Narrator icon](https://blogs.windows.com/windows-insider/2021/02/12/announcing-windows-10-insider-preview-build-21313/), and most recently [the icon for Notepad](https://blogs.windows.com/windows-insider/2021/03/17/announcing-windows-10-insider-preview-build-21337/). Now we’re taking the next step by updating many of the system icons used throughout File Explorer.

*Please note: After upgrading to this build, any custom folders pinned to Quick Access will disappear. You can either make note of them prior to updating to this build or pause updates until we get a fix in.*

![New icons in File Explorer](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/03/file-explorer-icons.png "New system icons in File Explorer.")

Several changes, such as the orientation of the folder icons and the default file type icons, have been made for greater consistency across Microsoft products that show files. Notably, the top-level user folders such as Desktop, Documents, Downloads, and Pictures have a new design that should make it a little easier to tell them apart at a glance. And yes, the Recycle Bin icon has also been updated!

![New Photos icons in File Explorer](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/03/Pictures-Folder@2x-refresh.png "Before and after Photos icons in File Explorer.")

![New hard drive and Recycle Bin icons in File Explorer](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/03/DriveAndRecycle@2x.png "Before and after of hard drive and Recycle Bin icons.")

As you can imagine, there are a lot of icons in Windows 10 and more icons will continue to get updated over time.

### Changes and Improvements
* We’re changing the name of the Windows Administrative Tools folder in Start to Windows Tools. We are working to better organize all the admin and system tools in Windows 10.
* [News and interests] Update on the rollout: following our [last update](https://blogs.windows.com/windows-insider/2021/02/12/announcing-windows-10-insider-preview-build-21313/) on languages and markets, this week we’re also introducing the experience to China! We continue to roll out news and interests to Windows Insiders, so it isn’t available to everyone in the Dev Channel just yet.
* We are now rolling out the [new IME candidate window design](https://aka.ms/wip21313) to all Windows Insiders in the Dev Channel using Simplified Chinese IMEs.
* We’re updating the “Get Help” link in the touch keyboard to now say “Learn more”.
* We’re updating File Explorer when renaming files to now support using CTRL + Left / Right arrow to move your cursor between words in the file name, as well as CTRL + Delete and CTRL + Backspace to delete words at a time, like other places in Windows.
* We’ve made some updates to the network related surfaces in Windows so that the displayed symbols use [the updated system icons we recently added in the Dev Channel](https://blogs.windows.com/windows-insider/2021/03/03/announcing-windows-10-insider-preview-build-21327/).
* Based on feedback, if the Shared Experiences page identifies an issue with your account connection, it will now send the notifications directly into the Action Center rather than repeated notification toasts that need to be dismissed.

### Improvements to Windows Sandbox and Microsoft Defender Application Guard (MDAG)
Both Windows Sandbox and Microsoft Defender Application Guard [take advantage of special container technology built into Windows 10](https://docs.microsoft.com/windows/security/threat-protection/windows-sandbox/windows-sandbox-architecture). Previously, the container runtime matched the host. Starting with Build 21343, we are introducing a new runtime that is designed and optimized for container scenarios. It is lightweight and allows faster launch times for both Windows Sandbox and Microsoft Defender Application Guard.

We do not expect this change to affect the application compatibility inside Windows Sandbox. However, this is a significant change and users may encounter some differences in behavior.

Additionally, Windows Sandbox now includes the new Chromium based Microsoft Edge browser (as of [Build 21313](https://blogs.windows.com/windows-insider/2021/02/12/announcing-windows-10-insider-preview-build-21313/)). Here are instructions on [how to get started with Windows Sandbox](https://docs.microsoft.com/windows/security/threat-protection/windows-sandbox/windows-sandbox-overview).

## Build 21337
Windows 10 Insider Preview Build 21337 was released to the Dev Channel on [3/17/2021](https://blogs.windows.com/windows-insider/2021/03/17/announcing-windows-10-insider-preview-build-21337/).

### Reorder and customize your Virtual Desktops
We’ve heard your feedback asking for more control over Virtual Desktops. Starting with Build 21337, we are bringing the ability to reorder and customize the backgrounds for each of your Virtual Desktops! You can access your Virtual Desktops via Task View (Win + Tab).

![Right-click Virtual Desktops](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/03/vd-right-click.png "You can now reorder and customize the backgrounds for each of your Virtual Desktops.")

Virtual Desktops help you cognitively separate different tasks on your PC, including helping to create work-life separation. They can be swapped into view, letting you shift your work from one desktop to another. Instead of juggling multiple windows, you can switch between Virtual Desktops to multitask.

![Drag and drop Virtual Desktops](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/03/dragdrop.gif "Dragging and droping to reorder Virtual Desktops!")

Here are the steps you can take to try these new features out.

**Change Virtual Desktop background:**

1. Under Settings > Personalization > Background, left click a background to change the background for the active Virtual Desktop.
2. Right clicking a background on this Settings page has a new option to change the background for a specific Virtual Desktop.
3. Once you’ve made the change, you’ll see your new background when you switch to that Virtual Desktop, and in the preview thumbnail in Task View.

**Reorder Virtual Desktops:**

1. Enter Task View (via Win + Tab), create multiple new Virtual Desktops.
2. Drag and drop a Virtual Desktop to another position in the list in Task View.
3. Right click a Virtual Desktop thumbnail in task view and select “Move left” or “Move right” in the context menu to move the desktop to another position.
4. Use keyboard navigation to set focus to the desired Virtual Desktop in Task View, and then press ALT + Shift + Left / Right Arrow to move it in either direction in the list.

If you have any feedback about these changes, please file it under Desktop Environment > Virtual Desktops in the Feedback Hub.

### Auto HDR Preview for PC
Today we’re excited to bring you a preview of Auto HDR for your PC gaming experience and we’re looking for your help to test it out. When enabled on your HDR capable gaming PC, you will automatically get awesome HDR visuals on an additional 1000+ DirectX 11 and DirectX 12 games! Check out our DirectX blog post for more details!

### File Explorer Layout Update
The default layout of File Explorer adds additional padding between elements. For users who prefer a more information-dense layout, there is a setting in View Options called “Use compact mode,” which will restore the classic layout of File Explorer. **The UX for toggling this setting is not final.** The level of padding is designed for better consistency with modern (XAML) experiences. This should also make it easier to work with File Explorer when using a touch screen.

![File Explorer Layout Update](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/03/file-explorer-layout-update.png "The default layout of File Explorer adds additional padding between elements.")

### Updates to Captions Settings for Windows Insiders
Thanks to feedback from customers and Windows Insiders, we are making updates to the captions settings in the latest Insider Preview builds. To get started, go to Settings > Ease of Access > Hearing > Captions.

![Captions settings update](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/03/captions.png "Displaying the updated Captions page in Settings.")

To learn more about how to make your app accessible, go to [Accessibility overview – UWP applications | Microsoft Docs](https://docs.microsoft.com/en-us/windows/uwp/design/accessibility/accessibility-overview).

Please note, the option to discard changes may not work as expected in this build – we’re working on a fix.

### Inbox app updates
We are making some changes to existing inbox apps and adding some new ones.

**Notepad is now updated via the Microsoft Store:**

![New Notepad icon](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/03/NotepadLargeTile.scale-400.png "New Notepad app icon.")

Notepad is now updateable via the Microsoft Store outside major OS updates. It also has a new icon and has been promoted out of the Windows Accessories folder to its own place in the Start menu.

**Windows Terminal now included as an inbox app:**

![Windows Terminal icon](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/03/LargeTile.scale-400.png "Windows Terminal app icon.")

Windows Terminal is now an inbox app. Windows Terminal is a modern, fast, efficient, powerful, and productive terminal application for users of command line tools and shells like Command Prompt, PowerShell, and Windows Subsystem for Linux (WSL). Its main features include multiple tabs, panes, Unicode and UTF-8 character support, a GPU accelerated text rendering engine, and custom themes, styles, and configurations. Updates for Windows Terminal will continue to come through the Microsoft Store.

**Power Automate Desktop now included as an inbox app:**

![Power Automate icon](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/03/PowerAutomateAppIcon.scale-400.png "Power Automate Desktop app icon. ")

Power Automate Desktop is now an inbox app. Power Automate Desktop allows you to automate web and desktop applications on your Windows desktop by mimicking the user interface actions like clicks, and keyboard input. You can also combine these actions with predefined support for applications like Excel to help automate repetitive tasks. You can find Power Automate within the Windows Accessories folder from the Start menu. During Microsoft Ignite earlier this month, we announced Power Automate Desktop will be available to Windows 10 users at no additional cost. [Check out this blog post from the Power Automate Team for more details](https://flow.microsoft.com/en-us/blog/automate-tasks-with-power-automate-desktop-for-windows-10-no-additional-cost/)!

*NOTE: Power Automate Desktop isn’t yet available for ARM PCs.*

**Updating WordPad integrations:** We’ve made some small changes to make Word or Notepad the text editor/viewer of choice in Windows when launching text file types, but if WordPad is your text editor of choice, it’s still available.

### Changes and Improvements
* We are now rolling out [the new IME candidate window design](http://aka.ms/wip21313) to all Windows Insiders in the Dev Channel using Japanese, Chinese Traditional, and Indic IMEs. We’ll let you know once the rollout for the remaining IMEs increases.
* We’re updating the emoji panel (WIN + Period) to support searching in more languages, including Amharic, Belarus, Cherokee, Filipino, Faroese, Icelandic, Khmer, Mongolian (Cyrillic script), Burmese, Sindhi, Serbian (Cyrillic script), Serbian (Latin script), Swahili, Thai, Turkmen, Tonga, Uzbek (Latin script), and Cantonese (Traditional). Please continue sharing feedback about the emoji search results in the Feedback Hub under Input and Language > Emoji Panel.
* Live previews for websites pinned to the taskbar from Microsoft Edge are now rolling out for all Insiders.
* We have moved the settings for showing Windows Ink Workspace, Touch Keyboard button, and Task View from right-clicking on Taskbar to Settings > Personalization > Taskbar.

## Build 21332
Windows 10 Insider Preview Build 21332 was released to the Dev Channel on [3/10/2021](https://blogs.windows.com/windows-insider/2021/03/10/announcing-windows-10-insider-preview-build-21332/).

### An update on the roll out of news and interests
Over the last two months, we’ve been trying out several variations of the news and interests experience on the Windows taskbar. We have received a lot of great feedback from Windows Insiders and as a result, have landed on what we believe to be the best experience for customers. The news and interests flyout experience will now show two columns of content, making it easy to quickly glance over your feed of weather, headlines, money, and more. By default, it will open via hover or click. Based on your feedback, we will also be introducing an option to only open via click in a coming update. As a result of these changes, we’re resetting the roll out of news and interests to Insiders in the Dev Channel. This means that Insiders who previously had news and interests enabled on their taskbars may see it go away. Don’t worry, we hope to make news and interests available to everyone in the Dev Channel soon!

It is important to reiterate that by gradually rolling out features to Insiders like this, it really helps us quickly identify issues that may impact performance and reliability.

### Changes and Improvements
* Our new option [to paste as plain text](https://blogs.windows.com/windows-insider/2021/02/19/announcing-windows-10-insider-preview-build-21318/) from clipboard history (WIN + V) is now rolling out to all Insiders in the Dev Channel.
Theme-aware splash screens have been re-enabled for everyone in the Dev Channel with this build.
* 3D Viewer and Paint 3D will no longer be preinstalled on clean installs of the latest Insider Preview builds. Both apps will still be available in the Store and will stay on your device after an OS update. So, if you upgraded your PC like normal, you shouldn’t see these apps changed in your app list.
* Due to increasingly low usage, Math Input Panel is being removed. However, the input control and math recognition engine that powered the app is remaining as an optional feature titled “Math Recognizer” which can be installed via Settings > Apps > Apps & features and clicking “Optional features”. So, while the app itself will no longer be there, the features it enabled for math equation input in OneNote, Excel, and elsewhere, will continue to work and developers can continue to utilize the input control.

## Build 21327
Windows 10 Insider Preview Build 21327 was released to the Dev Channel on [3/3/2021](https://blogs.windows.com/windows-insider/2021/03/03/announcing-windows-10-insider-preview-build-21327/).

### News and interests has an updated look!
Thanks for your ongoing feedback about news and interests on the Windows taskbar! Today, we’re excited to start rolling out a new design that makes it even more delightful to scan and interact with the headlines and stories in your feed. Imagery from articles now shines through with a vibrant and colorful design, making your feed more glanceable, engaging, and beautiful.

![News and interests updated design](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/03/News-and-interests-redesign.gif "News and interests on the Windows taskbar showing a vibrant new design for stories in the feed.")

There are more updates when you click “See more news”. The new feed experience that opens in the browser has been redesigned to help you catch up with the top headlines at a glance and enjoy a vibrant feed that brings your personalized stories to light. Larger cards can now also show article text, helping you get a sense of a topic before diving in.

![News and interests updated design on the web](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/03/Feeds-browser-redesign-scaled.jpg "By clicking “See more news”, you get a redesigned feed experience with top headlines and a vibrant feed of personalized stories.")

Across news and interests and the homepage, we are also making it easier to share your reaction to the news, with updated emoji graphics so you can respond with a like, love, surprise, anger, and more.

We look forward to hearing what you think! This updated design will start to roll out to Insiders with news and features in the U.S. first. Over time, it’ll roll out to other markets so stay tuned if you do not see these changes immediately.

>[!NOTE]
>REMINDER: We continue to roll out news and interests to Windows Insiders which means it isn’t available to everyone in the Dev Channel just yet.

### Changes and Improvements
* Sharped-eyed Windows Insiders will notice many of the system icons in this build have been updated and now align to the Microsoft Fluent Design style. This build includes a new font Segoe Fluent Icons. Areas of the OS that use the Segoe MDL2 assets such as the Start menu and Settings app will include the new icon designs which have a more rounded and simplified look and feel.

![New Segoe Fluent Icons font](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/03/fluent_monolineIcons.jpg "The new Segoe Fluent Icons font includes new icon designs which have a more rounded and simplified look and feel.")

* On ARM64 devices, the default architecture for PowerShell is now x64 rather than x86.

## Build 21322
Windows 10 Insider Preview Build 21322 was released to the Dev Channel on [2/24/2021](https://blogs.windows.com/windows-insider/2021/02/24/announcing-windows-10-insider-preview-build-21322/).

### Changes and Improvements
* The 3D Objects folder will no longer be shown as a special folder in File Explorer after updating to this build. If you need to access this folder, you can do so via typing %userprofile% in File Explorer or through the navigation pane option “Show all folders”.
* [News and interests] We removed the “Reduce taskbar updates” option from the context menu. We expect it to return in a future update.
* We have temporarily removed the touch keyboard refinements [noted in Build 21301](https://blogs.windows.com/windows-insider/2021/01/27/announcing-windows-10-insider-preview-build-21301/) to fix some issues. However, the updates to the default keyboard layout on 12” or larger screens and the candidate bar remain available to everyone in Dev Channel [as noted last week with Build 21318](https://blogs.windows.com/windows-insider/2021/02/19/announcing-windows-10-insider-preview-build-21318/).

## Build 21318
Windows 10 Insider Preview Build 21318 was released to the Dev Channel on [2/19/2021](https://blogs.windows.com/windows-insider/2021/02/19/announcing-windows-10-insider-preview-build-21318/).

### Paste as plain text in clipboard history
Simply open clipboard history (WIN + V) and click the … button next to any text-based entry in your clipboard history – you will now see a “Paste as plain text” option alongside pin and delete! When you use this action in clipboard history, it pastes the text content of the clipboard without its original formatting (font, color, size etc.), allowing it to match the formatting of the destination document.

![Paste as plain text](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/02/paste-in-plain-text.png "Displaying the new Paste as Text option in clipboard history.")

We look forward to you trying it! Please file any feedback you have for clipboard history under Input and Language > Clipboard (Copy and Paste) in the Feedback Hub.

>[!NOTE]
>This feature is rolling out to a subset of Insiders in the Dev Channel at first, to help us quickly identify issues that may impact performance and reliability. Rest assured they will be gradually rolled out to everyone in the Dev Channel.

### Changes and Improvements
* Insiders using x64 apps on ARM64 will no longer need to download and install a separate preview version of the ARM64 C++ redistributable package.
* We’re making a change so that [the notification](https://docs.microsoft.com/windows-hardware/design/component-guidelines/bluetooth-swift-pair) when pairing supported Bluetooth devices will now stay on the screen a little longer, given you the chance to interact with it before it goes away. If you’d like to dismiss it before then, you can still do so at any point by clicking the X in the notification, middle clicking the notification, or sliding the notification off the screen.
* Touch keyboard improvements as mentioned in [Build 21301](https://blogs.windows.com/windows-insider/2021/01/27/announcing-windows-10-insider-preview-build-21301/) such as updates to the default keyboard layout on 12” or larger screens and the candidate bar are now rolling out to all Insiders in the Dev Channel.
* We’ve improved the smoothness of motion while using Magnifier – for the scenario where you are transitioning between mouse and keyboard focus.

## Build 21313
Windows 10 Insider Preview Build 21313 was released to the Dev Channel on [2/12/2021](https://blogs.windows.com/windows-insider/2021/02/12/announcing-windows-10-insider-preview-build-21313/).

### Expanding news and interests to more languages and markets
We’ve heard your feedback! Today we’re excited to announce that we’re expanding the news and interests experience on the taskbar to a broader set of international languages and markets. Previously, the experience was only available in United States, Canada, Great Britain, Australia, and India. This now means that the news content, weather forecasts, sports and finance updates will be based on your location anywhere in the world!

![Expanded news and interests to more markets](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/02/News-and-interests-JP-updated2.jpg "News and interests on the Windows taskbar as seen from a Windows Insider’s PC in Japan.")

News and interests will automatically detect your language and location, and deliver a localized experience consisting of content from local publishers and data providers.

Please let us know what you think and how we can make news and interests better through Feedback Hub (go to Desktop Environment > News and interests). The team is excited to hear what you think!

The experience is not yet available in China. We hope to bring this experience to customers soon.

>[!NOTE]
>As a reminder, we continue to roll out news and interests to Windows Insiders which means it isn’t available to everyone in the Dev Channel just yet.

### The new Microsoft Edge to replace Microsoft Edge Legacy
With the release of Windows 10 Insider Preview Build 21313, Microsoft Edge Legacy will be replaced by the new Microsoft Edge. This will be the case for Windows 10 Insider Preview builds moving forward.

With Microsoft Edge, it’s time to expect more. You get world-class performance, with more privacy, more productivity, and more value as you browse.

And if you’d like to try out upcoming features in Microsoft Edge, join the Microsoft Edge Insider Program. Be one of the first to see what’s new by downloading the Microsoft Edge Canary, Dev, or Beta channels [from the Microsoft Edge Insider website](https://www.microsoftedgeinsider.com/download?form=MD19OP&OCID=MD19OP).

### Modernizing our IME candidate window design
An IME (Input Method Editor) is fundamental for typing East Asian languages, and leverages something we call a candidate window to enables users to insert characters efficiently. With recent releases of Windows 10, we started introducing new versions of our IMEs. Today, we’re excited to share the next part of those efforts – based on your feedback, the new candidate window offers:

A modern design – more aligned with our Fluent Design principles, including an acrylic background, a new selection visual, and dark theme support.
Optimized font size – we’ve adjusted the font size in the Candidate Window UI to minimize the intrusiveness while securing visibility.
Quick access to emoji – to help improve discoverability, we’re adding direct access to the Emoji Panel via a button from the candidate window UI. Please note: We are still working to improve the experience of this button. Currently the composition string is finalized when it is pressed.
Improved performance – input is at the core of how you interact with your PC, and we want to ensure you have the best possible experience as we roll out these changes.

For those unfamiliar with the previous design, it looked like this when you started typing:

![Previous IME candidate window design](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/02/Previous-Japanese-IME-candidate-window-UI.png "Previous Japanese IME candidate window design, showing conversion candidates of “kyou”.")

We’re looking forward for Insiders to try our updated design:

![New IME candidate window design 1](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/02/New-Japanese-IME-candidate-window-UI.png "New (1) Japanese IME candidate window design, in light and dark mode. Design now follows Fluent Design principles.")

![New IME candidate window design 2](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/02/New-Chinese-Simplified-IME-candidate-window-UI.png "New (2) Japanese IME candidate window design, in light and dark mode. Design now follows Fluent Design principles.")

The new UI design is available for the following languages/keyboards:

* Japanese – Microsoft IME
* Chinese (Simplified) – Microsoft Pinyin
* Chinese (Simplified) – Microsoft Wubi
* Chinese (Traditional) – Microsoft Bopomofo
* Chinese (Traditional) – Microsoft ChangJie
* Chinese (Traditional) – Microsoft Quick
* Korean – Microsoft IME
* Hindi – Hindi Phonetic
* Bangla – Bangla Phonetic
* Marathi – Marathi Phonetic
* Telugu – Telugu Phonetic
* Tamil – Tamil Phonetic
* Kannada – Kannada Phonetic
* Malayalam – Malayalam Phonetic
* Gujarati – Gujarati Phonetic
* Odia – Odia Phonetic
* Punjabi – Punjabi Phonetic

>[!NOTE]
>This feature is rolling out to a subset of Insiders in the Dev Channel at first, to help us quickly identify issues that may impact performance and reliability. Rest assured they will be gradually rolled out to everyone in the Dev Channel. If you have any feedback for these changes as they roll out to you, please file them in the Feedback Hub under Input and Language > Text Input.

### Changes and Improvements
* Based on feedback, and to align with the fact that Dev Channel builds are not matched to a specific Windows 10 release, we have updated the displayed version name to now be Dev.
* We heard feedback that it wasn’t clear how to turn off news and interests if this was your preference. To help address this, we changed the “Hidden” option in the taskbar context menu to now say “Turn off” to make this functionality clearer.
* Based on feedback, we’ve made some small adjustments to the [new app launch animation](http://aka.ms/wip21277) to improve speed and make it a little smoother.
The improvement to the candidate bar on the touch keyboard [announced in Build 21301](https://blogs.windows.com/windows-insider/2021/01/27/announcing-windows-10-insider-preview-build-21301/) where it displays 5 candidates maximum and centers them into position above the keyboard has begun rolling out.
* The new voice typing experience that was [announced in Build 20206](https://blogs.windows.com/windows-insider/2020/09/02/announcing-windows-10-insider-preview-build-20206/) has begun rolling out to all Insiders in the Dev Channel. Press the Windows key plus H if you’d like to try it out in one of the supported languages.
* The change to enable pinning items in our [updated clipboard history design](https://blogs.windows.com/windows-insider/2020/09/02/announcing-windows-10-insider-preview-build-20206/) (inside the emoji picker) is now rolling out to all Insiders in the Dev Channel.
* We’ve made a few more updates to our emoji search teams based on feedback, including that programming will now return the 3 technologist emojis and RIP will now return the tombstone emoji. We’ve also updated the search in Russian so that emoji with the letter ё in their keywords can now also be found by using the letter e. Please keep the feedback coming!
* We are removing the capability to copy and paste a screen snip directly into a folder in File Explorer for now due to an issue discovered thanks to the feedback from Windows Insiders. We hope to re-enable this capability in a future update after we address this issue. (This change was also released to Windows Insiders in the Beta Channel as part of the [recent Windows Feature Experience Pack update](https://blogs.windows.com/windows-insider/2021/01/26/releasing-windows-feature-experience-pack-120-2212-2020-0-to-the-beta-channel/).)
* As part of our continued iconography work, this build introduces a new design for our Narrator icon.
![Updated Narrator icon](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/02/narratroicon.png "The essence of the icon is the same (a computer with a speech bubble), but now the speech bubble is brightly colored rather than just white lines on a blue background.")

## Build 21301
Windows 10 Insider Preview Build 21301 was released to the Dev Channel on [1/27/2021](https://blogs.windows.com/windows-insider/2021/01/27/announcing-windows-10-insider-preview-build-21301/).

### Improving the touch keyboard design
Building on the design changes already live in the Dev Channel, Windows Insiders will start to notice some more refinements rolling out for the touch keyboard based on their feedback. Those refinements include:

* When undocking the keyboard, it now switches to the Small keyboard layout, and you can easily move the keyboard around using the gripper region at the top of the keyboard.
* Small and split layouts will now feature an updated symbol’s view based on the default layout.
* The settings menu now has a nested structure for improved clarity and less clutter.
* Finally, we have a new password feedback icon to the left of the space bar for when you are in a password field and would like to turn on visual key press feedback on the touch keyboard.

>[!NOTE]
>The above mentioned refinements have been temporarily removed as of Build 21322 to fix some issues.

![Touch keyboard layout improvements](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/01/Updated-keyboard-menu.png "The revamped touch keyboard settings menu allows you to quickly change between keyboard modes, access more settings and give feedback.")

Some Insiders may also see updates to the default keyboard layout on 12” or larger screens with the keyboard having a more traditional keyboard layout featuring an ESC, Tab, and Windows key and other small tweaks.

![Touch keyboard layout improvements 2](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/01/Updated_keyboard.jpg "The updated default layout now features the Esc, Tab, Windows, and Alt keys.")

One thing we heard from our customers is that the candidate bar can feel cluttered and hard to quickly process. To reduce the cognitive overload we will be displaying 5 candidates maximum and centering them into position above the keyboard.

![Touch keyboard layout improvements 3](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/01/Updated_candidate_bar.png "The candidate suggestion bar is now centered and features 5 candidates for you to choose from.")

>[!NOTE]
>The updates to the default keyboard layout on 12” or larger screens and the candidate bar remain available to everyone in Dev Channel as of Build 21322.

### Changes and Improvements
* We made a change so that when you right click locally saved files displayed in jump lists, in addition to Open you will now have the option to Open File Location.
* We updated our N’Ko keyboard layout to add access to currency and some other symbols by tapping the keys along the top row of your keyboard while holding the Shift key.
* We updated the Touchpad on/off toggle under Settings > Devices > Touchpad such that it no longer requires admin privileges to change.
* We updated our backend dictionaries to help improve spellchecking and text prediction relevance.

## Build 21296
Windows 10 Insider Preview Build 21296 was released to the Dev Channel on [1/21/2021](https://blogs.windows.com/windows-insider/2021/01/21/announcing-windows-10-insider-preview-build-21296/).

### Changes and Improvements
* We’re starting to roll out an update to [our converged clipboard history design](https://aka.ms/wip20206) (WIN + V) to support pinning, unpinning, deleting, and syncing individual entries. Appreciate your patience and feedback while we’ve been working on this. If you have any other feedback in this space, we welcome it in the Feedback Hub under Input and Language > Clipboard.
* The [ability to manage and create Storage Spaces from within Settings](https://blogs.windows.com/windows-insider/2021/01/06/announcing-windows-10-insider-preview-build-21286/) is now rolling out to all Insiders in the Dev Channel. If you have any feedback as you explore the changes, please file it under Files, Folders, and Online Storage > Storage spaces in the Feedback Hub.

## Build 21292
Windows 10 Insider Preview Build 21292 was released to the Dev Channel on [1/13/2021](https://blogs.windows.com/windows-insider/2021/01/13/announcing-windows-10-insider-preview-build-21292/).

### Changes and Improvements
* Based on feedback, we’re updating Settings > System > Sounds to now display a message when microphone permissions have been turned off for the whole system or for all apps, with a link to the microphone privacy settings page.

## Build 21286
Windows 10 Insider Preview Build 21286 was released to the Dev Channel on [1/6/2021](https://blogs.windows.com/windows-insider/2021/01/06/announcing-windows-10-insider-preview-build-21286/).

### Introducing news and interests on the taskbar

With news and interests on the Windows taskbar, you get quick access to an integrated feed of dynamic content such as news and weather that updates throughout the day.

![News and feeds on the taskbar](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/01/News-and-interests.png "News and interests on the Windows taskbar gives you quick access to an integrated feed of dynamic content such as news and weather that updates throughout the day.")

You can personalize your feed with relevant content tailored for you. Instead of switching between apps or your PC and phone to stay up to date with the news and interests you care about – seamlessly peek into your feed directly from the taskbar anytime you want throughout your day.

![News and feeds on the taskbar gif](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/01/News-and-interests-video.gif "Showing news and interests on the taskbar with the flyout of content just for you.")

* **Staying up to date:** Quickly glance at your news and interests directly from the taskbar. Get caught up on the latest headlines, weather, sports, and more, then go back to whatever you were doing without disrupting your workflow. You have convenient access to news and interesting content from over 4,500 global brands such as The New York Times, BBC or The Verge, and gorgeous live weather maps. Select an article to open a streamlined reading view with fewer distractions, so you can save time and stay focused.
* **Personalize your feed:** You can tell us which content you like seeing or don’t like seeing (select More options … and choose “More stories like this” or “Fewer stories like this”) and over time, more stories about the things you care about will show up in your feed, including ones you might otherwise miss. You can also use emoji to react to stories, too.
* **You’re in control:** At Microsoft, we believe privacy starts with putting you in control and giving you the tools and information, you need to make informed choices. Through news and interests, there is quick access to the Microsoft Privacy Dashboard. Through the Microsoft Edge browser, there are built-in controls to limit tracking from advertisers and third parties. And if news and interests doesn’t appeal to you, you can easily turn it off by right-clicking on the taskbar.

As more of us are spending time on our PCs to work, learn, connect, and play, news and interests on the taskbar is a nice companion for those who want to stay connected with information on the latest current events. Over time, we hope to bring your feed of news and interests to other places, such as in Microsoft Edge, so no matter where you are, you’ll be able to stay up to date.

**We are beginning to roll out news and interests to Windows Insiders today starting with Build 21286 in the Dev Channel and Insiders will need to reboot after installing Build 21286 to enable this feature.** Managing the rollout of features like this allows us to quickly identify issues that may impact performance and reliability. We plan to evolve this experience over time, so please let us know what you think and how we can make it better through Feedback Hub (go to Desktop Environment > News and interests). The team is excited to hear what you think!

_IMPORTANT NOTE: This feature is currently only available to Windows Insiders in United States, Canada, Great Britain, Australia, and India. This feature also requires the new Chromium-based Microsoft Edge browser to be installed on your PC. We are also testing different variations of this experience so some Insiders may see a different experience than others._

### Modernized Storage Spaces Settings
You can now create and manage Storage Spaces from within the Settings app. This includes creating storage pools and storage spaces, adding, and removing disks, and optimizing pools. This new experience provides an accessible, modern experience integrated with other storage features.

![Modern Storage Spaces](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/01/mods.gif "Managing Storage Spaces in the Settings up via Settings > System > Storage.")

Go to **Settings > System > Storage** and click the **Manage Storage Spaces** under “More storage settings” to get started.

>[!NOTE]
>This feature is rolling out to a subset of Insiders in the Dev Channel at first, to help us quickly identify issues that may impact performance and reliability. Rest assured they will be gradually rolled out to everyone in the Dev Channel.

### Introducing New File System Command Line Tool DiskUsage
As some Insiders have noticed, we’re working on an enhancement to the file system utilities family – called DiskUsage, enabling users to view and query disk space usage via the command line. With DiskUsage, you can now track files and directories which are consuming excessive amount of space on the drive. It scans the specified directory recursively or the entire drive with detailed information on how much each subfolder is using. It also supports extensive filtering and output customization options.

For example: >> diskusage /d:1

This will display the used space under each folder of the current directory.

Get started today by typing diskusage /? in a command line window for more options and usage information.

![New DiskUsage Tool](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/01/diskusage.png "Running the DiskUsage command in Windows Terminal.")

### Run commands on start up in the Windows Subsystem for Linux (WSL)
We have added an option that allows you to run any specified Linux command on startup of a WSL distribution. You can accomplish this by editing the /etc/wsl.conf file in your distribution and adding an option titled “command” under a section titled “boot”. This command will run whenever your specific WSL distribution starts up. The example below shows using this functionality to create a method to log the time and date for each startup of this WSL distro.

![WSL startup commands](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/01/wsl-terminal-startup-commands.png "A screenshot of Windows Terminal displaying a user interacting with WSL.")

This command will run when a WSL distribution is first started. WSL distributions will remain running for a few minutes even after the last Linux process inside of them is closed. You can view if your WSL distro is running using wsl --list --verbose and you can manually shut down all WSL distributions using wsl --shutdown.

### Improving your experience when transitioning between time zones
Based on feedback, we’re making a couple small adjustments for users of “Set time zone automatically” in Date & Time Settings:

* When your time zone is updated because of a high confidence detected location change, we’ll now send a notification letting you know about it. The notification will include information about the new time zone and clicking it will open the Date & Time Settings.
* If we detect a low confidence location change and there is a single administrator on the device, we will now send a notification asking if you would like to update your time zone – clicking the OK button in the prompt will make the change.

![Improved time zone transitions](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2021/01/timezonenotifications.png "Displaying examples of the two possible time zone notifications.")

### Changes and Improvements
* Based on feedback, (GitHub issue #1495) we’re adding an option to disable automatic controller-to-virtual-key mapping for UWP apps. If you have a need to do this, add the following registry key, with a DWORD value of Enabled set to 0: HKLM\Software\Microsoft\Input\Settings\ControllerProcessor\ControllerToVKMapping.

## Build 21277
Windows 10 Insider Preview Build 21277 was released to the Dev Channel on [12/10/2020](https://blogs.windows.com/windows-insider/2020/12/10/announcing-windows-10-insider-preview-build-21277/).

### Introducing x64 emulation in preview for Windows 10 on ARM PCs
Windows Insiders with ARM PCs who install this build can try out x64 emulation by installing x64 apps from the Microsoft Store or from any other location of their choosing. For more details on this experience, please head on over [and read this blog post from Hari Pulapaka](https://blogs.windows.com/windows-insider/?p=174852)!

### Adding Support for Unicode Emoji 12.1 and 13.0
Starting with this build, Insiders will get their first look at the emoji we’ve designed to support Emoji 12.1 and 13.0! This update brings over 200 new glyphs to Windows – including bubble tea, a smiling face with tear, a ninja, a magic wand, and more:

![New Emoji 12.1 and 13.0 emojis](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/12/Emoji13@2x.png "Showing an array of the new emoji that will be added, including ninja, bubble tea, face wearing a disguise, and smiling face with a tear.")

As part of this change, we’re introducing a gender-neutral emoji design, which you can now select alongside the corresponding male or female design in our emoji panel and touch keyboard:

![Gender-neutral emoji design](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/12/GenderInclusive@2x.png "Displaying 3 versions (male, female, and gender-neutral) of various emoji (genie, superhero, person shrugging, etc.).")

You’ll also find we’ve made some tweaks to our existing emoji to improve cross-platform consistency:

(OLD)
![Old emoji design](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/12/RedesignBefore@2x.png "Some existing emoji and how they’ve been tweaked (face with mask, giraffe, and confused face).")

(NEW)
![New emoji design](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/12/RedesignAfter@2x.png "Some existing emoji and how they’ve been tweaked (face with mask, giraffe, and confused face).")

Some existing emoji and how they’ve been tweaked (face with mask, giraffe, and confused face).
To bring up the emoji panel and check out all the changes, press Windows key + Period (.) or Windows key + Semicolon (;).

One final note: we’ve made several improvements to our emoji search terms based on your feedback – if you update to today’s build and still find the expected emoji isn’t being returned when you search for it, please let us know! You can file feedback for this in the Feedback Hub under Input and Language > Emoji panel. Please specify what words you used, and which emoji you expected to appear.

### Changes and Improvements
* We’ve updated the animation when opening or closing a window to make the transition smoother. Do you notice a difference? Let us know!
* Based on Insider feedback, you can now use the built-in screen snipping experience in Windows (WIN + SHIFT + S) to create a snip of your screen and paste it directly into a folder of your choice in File Explorer to save the screenshot there. Try it out! (This was released to Windows Insiders in the Beta Channel [as part of the recent Windows Feature Experience Pack update](https://blogs.windows.com/windows-insider/2020/11/30/releasing-windows-feature-experience-pack-120-2212-1070-0-to-the-beta-channel/).)
* Using the touch keyboard in a portrait posture on a 2-in-1 touch device now supports split keyboard mode. (This was released to Windows Insiders in the Beta Channel [as part of the recent Windows Feature Experience Pack update](https://blogs.windows.com/windows-insider/2020/11/30/releasing-windows-feature-experience-pack-120-2212-1070-0-to-the-beta-channel/).)
* It’s now possible to uninstall the Snipping Tool. If you choose to uninstall it, it can be reinstalled via the Optional Features page in Settings.
* We’ve made some adjustments to improve the scaling logic of the graphs in Task Manager’s Performance tab.
We’ve updated Registry Editor so that the Find window, renaming a key, and other places all now support CTRL + Backspace to delete words at a time.
* When using the Delete key or Dismiss button in Action Center to clear groups of notifications, Narrator will now announce that the notification group has been cleared instead of just moving focus to the next notification group.
* Based on feedback we’re adjusting a few strings in Offline Maps Settings to improve clarity.
* To help you find what you’re looking for faster, we’ve updated our folder logic in Start menu’s all apps list so that if a folder only contains a single item we will now display that item in place of the folder.

![Updated folder logic on Start](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/12/Start-menu-folder.png "Showing Visual Studio code in a folder by itself and then (after) not in a folder.")

## Build 20279
Windows 10 Insider Preview Build 20279 was released to the Dev Channel on [12/14/2020](https://blogs.windows.com/windows-insider/2020/12/14/announcing-windows-10-insider-preview-build-20279/).

## Build 20277
Windows 10 Insider Preview Build 20277 was released to the Dev Channel on [12/10/2020](https://blogs.windows.com/windows-insider/2020/12/10/announcing-windows-10-insider-preview-build-20277/).

## Build 20270
Windows 10 Insider Preview Build 20270 was released to the Dev Channel on [12/3/2020](https://blogs.windows.com/windows-insider/2020/12/03/announcing-windows-10-insider-preview-build-20270/).

### Changes and Improvements
* The new “Advanced View” checkbox in Optimize Drives is now up and running and checking it will display volumes previously not visible in this window (for example system and recovery partitions).
* Using the touch keyboard in a portrait posture on a 2-in-1 touch device now supports split keyboard mode. (This was released to Windows Insiders in the Beta Channel as part of the recent Windows Feature Experience Pack update.)

## Build 20262
Windows 10 Insider Preview Build 20262 was released to the Dev Channel on [11/18/2020](https://blogs.windows.com/windows-insider/2020/11/18/announcing-windows-10-insider-preview-build-20262/).

## Build 20257
Windows 10 Insider Preview Build 20257 was released to the Dev Channel on [11/11/2020](https://blogs.windows.com/windows-insider/2020/11/11/announcing-windows-10-insider-preview-build-20257/).

### Changes and Improvements
* Based on feedback, we’re updating our Start menu tile theming logic such that the tile background for Win32 apps will no longer adjust based on detected contrast ratio, except in the case of pinned Microsoft Edge PWAs.

## Build 20251
Windows 10 Insider Preview Build 20251 was released to the Dev Channel on [11/4/2020](https://blogs.windows.com/windows-insider/2020/11/04/announcing-windows-10-insider-preview-build-20251/).

## Build 20246
Windows 10 Insider Preview Build 20246 was released to the Dev Channel on [10/29/2020](https://blogs.windows.com/windows-insider/2020/10/29/announcing-windows-10-insider-preview-build-20246/).

### Changes and Improvements
* We added automatic Linux distro installation to the wsl.exe --install command! This means that users who wish to install the Windows Subsystem for Linux quickly can just type in wsl.exe --install into the command line and then will have a fully set up WSL instance ready to go, including their Linux distro of choice.

## Build 20241
Windows 10 Insider Preview Build 20241 was released to the Dev Channel on [10/21/2020](https://blogs.windows.com/windows-insider/2020/10/21/announcing-windows-10-insider-preview-build-20241/).

### Introducing theme-aware splash screens for apps
Building on theme-aware tiles in Start, we’re introducing theme-aware splash screens for Universal Windows Platform (UWP) apps. Now, when an eligible UWP app is launched, the splash screen color will match your default app mode. For example, if you have light theme turned on, you’ll see a light theme splash screen, and if you have dark theme turned on (for the “default app mode”) then you’ll see a dark theme splash screen.

Settings app splash screen before and after in light theme:

![Theme-aware splash light 1](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/10/Settings-Light-Before-After-GIF.gif "Settings splash screen before and after in light theme.")

Settings app splash screen before and after in dark theme:

![Theme-aware splash light 2](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/10/Settings-Dark-Before-After-GIF.gif "Settings splash screen before and after in dark theme.")

The following apps support theme-aware splash screens today:

* Settings
* Store
* Windows Security
* Alarms & Clock
* Calculator
* Maps
* Voice Recorder
* Groove
* Movies & TV
* Snip & Sketch
* Microsoft ToDo
* Office
* Feedback Hub
* Microsoft Solitaire Collection

Over time, more apps will be updated via the Store to support having a theme-aware splash screen.

_NOTE: Some apps like Store and Feedback Hub may show an extended splash screen in your accent color instead of the theme-aware light or dark theme._ 

>[!NOTE]
>This feature is rolling out to a subset of Insiders in the Dev Channel at first to help us quickly identify issues that may impact performance and reliability. Rest assured they will be gradually rolling out to everyone in the Dev Channel. 

### Enhancing your defrag experience
We’re making a few changes to the Optimize Drives page (**Settings** > **System** > **Storage** > **Optimize Drives**), including:

* Adding a new “Advanced View” checkbox to list all volumes including hidden volumes. Please note we’re still getting this one up and running, so you’ll see the checkbox in this build, but may not notice any differences when you select it.
* Listing more details in the “Current status” column when volumes are not available for defrag (for example, “Partition type not supported” and “File system type not supported”).
* Adding support for pressing F5 to refresh.

### Changes and Improvements
* To help ensure Narrator users are aware of notifications on the screen, if a high priority notification appears while the computer is locked and stays on the screen, we will now also read it out when unlocking your PC and not just at arrival time.
* We’re removing the Japanese Address and Rinna candidate suggestion services from the Japanese IME – thank you Windows Insiders who’ve shared feedback on them.

## Build 20236
Windows 10 Insider Preview Build 20236 was released to the Dev Channel on [10/14/2020](https://blogs.windows.com/windows-insider/2020/10/14/announcing-windows-10-insider-preview-build-20236/).

### Change Refresh Rate of your display
You can now go to **Settings** > **System** > **Display** > **Advanced display settings** and change the refresh rate of your selected display. A higher refresh rate allows for smoother motion. The presented refresh rates can vary with the supported hardware on your device.

![Refresh rate](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/10/refresh-rate.png "Showing the new refresh rate dropdown in Advanced Display Settings.")

### Changes and Improvements
* To improve accessibility of PDFs for Narrator and other screen reader users, in the cases where Unicode is not provided by the printing application, we’re updating our Microsoft Print to PDF option to make an attempt to convert the provided font glyphs to Unicode.

## Build 20231
Windows 10 Insider Preview Build 20231 was released to the Dev Channel on [10/7/2020](https://blogs.windows.com/windows-insider/2020/10/07/announcing-windows-10-insider-preview-build-20231/).

### Improving relevancy of initial device setup
Based on feedback, we’re exploring adding a page to Windows setup (OOBE) to help better understand how you plan to use your device and aid in customizing your device given your intended usage.

![OOBE usage screen](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/10/Intent.jpg "Displaying a page in OOBE prompting you to customize your device by saying if you plan to use it for things like gaming or business.")

This is the initial wave of work for this feature, and Insiders may notice different options presented in OOBE depending on what they select, however at this time Insiders will not notice any other configuration differences after exiting OOBE. We look forward to sharing future improvements in this space.

>[!NOTE]
>This feature is rolling out to a subset of Insiders in the Dev Channel at first, to help us quickly identify issues that may impact performance and reliability. Rest assured they will be gradually rolled out to everyone in the Dev Channel. NOTE: You will see this feature if you choose to reset your PC and when you do a clean install of Windows with the ISO for Build 20231 and higher. 

### Better Management Options for App Default File Associations 
Enterprise customers can now modify file associations on a per-user or per-device basis. This change will apply to existing users as well as users with new deployments. This means that IT admins can set which apps will automatically open various file types or links. For example, this makes it easy to set Microsoft Edge as your organization’s default browser, or always open PDFs in your organization’s preferred app. Leveraging this group policy for the default browser and common file types means that your organization’s end users will not have to decide on these defaults themselves.

Deployment/Testing Steps:

1. Generate Default Application Associations XML file by following [this page](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-8.1-and-8/hh825038(v=win.10)?redirectedfrom=MSDN).
2. Manually modify the XML by adding 2 new properties:
3. Add Version=”1“ to the DefaultAssociations tag.
4. Add Suggested=”True” to any Association tag.
5. Enable the group policy to set the default file associations by following [this doc](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/set-the-default-browser-using-group-policy?redirectedfrom=MSDN&f=255&MSPPError=-2147217396).
6. Reboot or log in as the user.

_Please note: If your device does not have this feature enabled, the policy will fall back to the default logic and will not respect the “Version” and “Suggested” fields of the policy._

>[!NOTE]
>This feature is rolling out to a subset of Insiders in the Dev Channel at first, to help us quickly identify issues that may impact performance and reliability. Rest assured they will be gradually rolled out to everyone in the Dev Channel.

### Changes and Improvements
* [Meet Now in the Windows 10 Taskbar](https://blogs.windows.com/windows-insider/2020/09/23/announcing-windows-10-insider-preview-build-20221/) is now available to all Windows Insiders in the Dev Channel.
* We’re starting to roll out a change to enable displaying graphics card information listed under **Settings** > **System** > **About**, and some Insiders may see this on their PCs.
* Our change to enable [moving the text cursor via gestures on the touch keyboard](https://blogs.windows.com/windows-insider/2020/09/02/announcing-windows-10-insider-preview-build-20206/) is now rolling out to all Insiders in the Dev Channel.

## Build 20226
Windows 10 Insider Preview Build 20226 was released to the Dev Channel on [9/30/2020](https://blogs.windows.com/windows-insider/2020/09/30/announcing-windows-10-insider-preview-build-20226/).

### Storage health monitoring to protect user data
Attempting to recover data after drive failure is both frustrating and expensive. This feature is designed to detect hardware abnormalities for NVMe SSDs and notify users with enough time to act. It is strongly recommended that users immediately back up their data after receiving a notification.

![Storage alert toast](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/09/DriveHealthToast.png "Image of toast notification sent to users when NVMe SSD abnormalities are detected.")

Selecting the notification or navigating to the drive properties page in Storage Settings (**Settings** > **System** > **Storage** > **Manage disks and volumes** > **Properties**) will provide additional details.

![SSD properties page with alert](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/09/DriveHealth-Cropped.png "Image of toast notification sent to users when NVMe SSD abnormalities are detected.")

### Changes and Improvements
* We’re starting to roll out a change that will turn off theme syncing. As part of that, you will no longer see “Theme” as an option in Sync your settings, and changes made to your background will not sync across device. If you have been using theme synchronization, when setting up a new PC or account there will be a one-time download of the last saved synchronized desktop background to %LOCALAPPDATA%\Microsoft\Windows\WallpaperBackup if you need to access it.
* Thanks for your patience – after making some reliability improvements, we’re re-enabling the ability for Notepad windows to persist update and restarts (if “Restart apps” is enabled in Sign-in Settings).
* When you have a PWA installed from Microsoft Edge, Task Manager will now correctly display it under Applications instead of Background Processes in the Processes tab, and will show the app icon associated with the PWA.
* We’re updating File Explorer so that if you right-click on a zipped OneDrive file that was set to online-only, you’ll now see an Extract All option, same as if the file was available locally on the PC.
* We’re updating the new DNS options in Settings to make a static DNS entry required when entering a static IP, and to make gateway not a required field.
* We’re updating the N’Ko keyboard layout so that pressing **Shift** + **6** will now insert ߾ (U+07FE ) and pressing **Shift** + **7** will now insert ߿ (U+07FF).

## Build 20221
Windows 10 Insider Preview Build 20221 was released to the Dev Channel on [9/23/2020](https://blogs.windows.com/windows-insider/2020/09/23/announcing-windows-10-insider-preview-build-20221/).

### Introducing Meet Now in the Windows 10 Taskbar
Earlier this year we introduced Meet Now in Skype. Meet Now makes it easy to connect with anyone in as little as two clicks for free and each call can last up to 24 hours. Today, we’re excited to share that we are extending this capability in Windows 10 by bringing Meet Now right to the Taskbar. You can now easily set up a video call and reach friends and family in an instant by selecting the Meet Now icon in the notification area (system tray) of the Taskbar in Windows 10. No sign ups or downloads needed.

Create a meeting:

![Create a meeting](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/09/menow21-startshort-800-v5.C0.5.gif "Create a meeting with Meet Now.")

Join a meeting:

![Join a meeting](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/09/menow21-join-800-v3.C0.9.gif "Join a meeting in Meet Now.")

>[!NOTE]
>This feature is rolling out to a subset of Insiders in the Dev Channel at first, to help us quickly identify issues that may impact performance and reliability. Rest assured they will be gradually rolled out to everyone in the Dev Channel.~~ This is now available to all Insiders in the Dev Channel as of Build 20231.

### Changes and Improvements
* As some Insiders may have noticed, we’re adding a notification to let you know when an app registers to run at startup (**Settings** > **Apps** > **Startup Apps**).
* With most of the launches of the People app coming directly from within the Mail and Calendar apps in Windows 10, the People app no longer appears as a standalone app in Start. It remains as an inbox app and can be launched to manage your contacts from the button in the Mail and Calendar apps.

## Build 20215
Windows 10 Insider Preview Build 20215 was released to the Dev Channel on [9/10/2020](https://blogs.windows.com/windows-insider/2020/09/16/announcing-windows-10-insider-preview-build-20215/).

## Build 20211
Windows 10 Insider Preview Build 20211 was released to the Dev Channel on [9/10/2020](https://blogs.windows.com/windows-insider/2020/09/10/announcing-windows-10-insider-preview-build-20211/).

### Adding Search to the Default Apps pages in Settings
After making some updates to help improve performance, this change to enable searching the lists of file types, protocols, and apps when setting a default is now rolling out to all Insiders in the Dev Channel – thanks everyone who’s shared feedback along the way.

![Default apps search](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/09/default-apps.png "Search the lists of file types, protocols, and apps when setting a default.")

### Access Linux file systems in the Windows Subsystem for Linux
This latest insiders preview build adds the ability for users to attach and mount a physical disk inside of a WSL 2 distro. This enables you to access file systems that aren’t natively supported by Windows (such as ext4). So if you’re dual booting with Windows and Linux, and are using different disks, you can now access your Linux files from Windows! To learn more about this feature please read [this blog post](https://devblogs.microsoft.com/commandline/access-linux-filesystems-in-windows-and-wsl-2/) on the Windows Command Line blog.

## Build 20206
Windows 10 Insider Preview Build 20206 was released to the Dev Channel on [9/2/2020](https://blogs.windows.com/windows-insider/2020/09/02/announcing-windows-10-insider-preview-build-20206/).

### Evolving the Emoji Picker
Over the last 3 years, we have been adding ways to express yourself when typing in Windows. In addition to adding an emoji picker and support for more emoji, we have also added support for many more languages, kaomoji, and symbols. We have also added ways to manage your clipboard history. We are evolving the emoji picker in Windows to bring many of these separate experiences together as well as introduce some new capabilities such as easy access to animated GIFs.

![Updated Emoji Picker](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/09/Screenshot-2020-09-01-172040.png "The revamped emoji picker is your one-stop for expressing yourself with quick access to emoji, kaomoji, symbols, animated GIFs and your clipboard.")

We know that you need more than just emojis to properly convey your message when communicating using text. To that end, we’ve revamped the emoji picker to be a one-stop for expressing yourself while you type on your device!  This new experience offers:

* An updated design: We are making the experience more aligned with our Fluent Design principles, including a new acrylic background.
* Emoji search: We are improving discoverability of emoji search in supported languages by having an inline search box.
* Animated GIF support, including search: Going forward, **Win** + **(period)** and **Win** + **(semicolon)** will now enable you to quickly input animated GIFs. The selection of animated gifs will be continuously updated based on current trends and #hashtags. Search is also available for those times where you need to find the perfect reaction gif to succinctly communicate your message.
* Converging our input experiences across emoji and clipboard history: We are bringing input and clipboard history together into a single experience. You can still press **Win** + **V** to go straight to clipboard history, but now you can also access it by switching to the **Clipboard** category after pressing **Win** + **(period)** or **Win** + **(semicolon)**.

We will be continuing to work on input in Windows and would love to hear your thoughts on further improvements. We are lighting up a new area path in the Feedback Hub for you to share your suggestions: **Input and Language** > **Emoji, Kaomoji, GIF and other input**.

_Please note: In order to insert an animated GIF when typing, the text field needs to support it. Animated GIF search requires an internet connection and is powered by Tenor. For more details about languages where animated GIF search is supported by Tenor, please see here._

>[!NOTE] 
>This feature is rolling out to a subset of Insiders in the Dev Channel at first, to help us quickly identify issues that may impact performance and reliability. Rest assured they will be gradually rolled out to everyone in the Dev Channel.

### Introducing Voice Typing
Windows voice typing is the new and improved version of Windows dictation that enables you to type effortlessly with your voice wherever there’s a text field on your PC. Sometimes, using your voice is more comfortable and efficient than typing on a keyboard – with Windows voice typing, you can relax your hands and just say what you want to write.

Improved features for voice typing include:

* A modern design – optimized for use with touch keyboards.
* Auto-punctuation that allows you to effortlessly put your thoughts down without worrying about question marks and periods (turn it on in settings).
* An updated back end for the most reliable voice typing experience ever on Windows.
Easily start voice typing any time by using the keyboard shortcut (**Win** + **H**) or tapping the microphone button on the touch keyboard.

When using the hardware keyboard:

![Voice Typing Hardware Keyboard](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/09/VoiceTypingFloaty-300x239.png "Use the Win + H keyboard shortcut for quick access to the microphone button for voice to text.")

When using the touch keyboard:

![Voice Typing Touch Keyboard](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/09/VoiceTypingKeyboard-1024x427.png "When using the touch keyboard in Windows, you can use the microphone icon to quickly use voice to text.")

Want to up your voice typing to the next level? Try out the following supported voice commands:

![Voice Typing Commands List](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/09/VTCommands.png "List of voice commands in different languages. ")

Voice typing is available in the following languages/locales*:

* English (US)
* English (Australia)
* English (India)
* English (Canada)
* English (United Kingdom)
* French (France)
* French (Canada)
* Portuguese (Brazilian)
* Simplified Chinese
* Spanish (Mexico)
* Spanish (Spanish)
* German
* Italian
* Japanese**

_*Voice typing will automatically use the language your keyboard is set to (if supported).
**Auto-punctuation is not available in Japanese at this time._

_Please note: we are still working to improve the feature and how it interacts with different applications. In some Office apps you may experience random pauses while using the voice typing feature. If this happens, select the microphone icon again to restart the listening experience._

>[!NOTE] 
>This feature is rolling out to a subset of Insiders in the Dev Channel at first, to help us quickly identify issues that may impact performance and reliability. Rest assured they will be gradually rolled out to everyone in the Dev Channel.

### Improving the touch keyboard design
Some Insiders will start to see our new touch keyboard design rolling out to their PCs. The updated design includes a fresh aesthetic and many other small tweaks, including updated key sizes / layouts to optimize for typing comfort & accuracy. We have also done some work to help improve discoverability and usability of available features.

While exploring the updated design, you will notice a number of refinements, including:

* New key press animations and sounds.
* Child keys have been optimized for quicker entry – try pressing and holding keys like “e” or “-“ and see how it looks.
* For those who prefer to keep their keyboard undocked, the option now accessible via a button directly in the candidate bar, and you can easily move the keyboard around using the gripper region at the top of the keyboard.
* All entries in the settings menu now have labels for improved clarity of available options.
We are bringing emoji search to the touch keyboard, so you no longer need to hunt through the different categories to find the one you are looking for. More so, you can also now search for animated GIFs. All accessible from our new expressive input button in the candidate bar. (For more – see our section above on evolving the emoji panel.)
* A new entry point into voice typing has been added to the left of the space bar in supported languages. (See above section on voice typing.)

![Touch Keyboard Redesign](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/09/2020-09-01-6.png "The redesigned touch keyboard introduces a variety of improvements such as new key press animations and sounds, quick access to emoji and animated GIFs, and a new entry point for voice typing.")

![Touch Keyboard Redesign 2](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/09/2020-09-01-5-1024x644.png "The redesigned touch keyboard offers quick access to emoji and animated GIFs so you and express yourself any way you like while typing in Windows.")

The touch keyboard can also be invoked on any PC from the touch keyboard button on the Taskbar, although you may need to enable the button. To do so, right-click or press and hold on the Taskbar, then select “Show touch keyboard button” in the menu. Once the touch keyboard is open, try typing or shapewriting on the keyboard and let us know how it feels.

We want to thank Insiders for sharing their feedback about the touch keyboard over the years – your comments directly inspired these changes. We look forward to you trying them out and to even more feedback!

_Please note: Some of the keyboard layouts for certain languages are still in the process of being updated to the new design. Currently shapewriting is only supported when using the wide or onehanded touch keyboard layouts._

>[!NOTE] 
>This feature is rolling out to a subset of Insiders in the Dev Channel at first, to help us quickly identify issues that may impact performance and reliability. Rest assured they will be gradually rolled out to everyone in the Dev Channel.

### Cursor movement using the space bar  
One thing we heard from our customers is the desire to change the cursor position with the touch keyboard. Based on that feedback, we are updating the keyboard so that you can now quickly do this in any text field using gestures on the space bar.

All you need to do is place a finger on the space bar and slide your finger left, right, up, or down. As your finger moves, so will the cursor – one character or line at a time.

![Cursor movement spacebar](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/44/2020/09/Single-Portrait-Docked-1-1024x423.png "Press and hold on the space bar on the touch keyboard to move the cursor on your screen.")

We’ll be continuing to work on input in Windows and would love to hear your thoughts on further improvements.

>[!NOTE] 
>This feature is rolling out to a subset of Insiders in the Dev Channel at first, to help us quickly identify issues that may impact performance and reliability. Rest assured they will be gradually rolled out to everyone in the Dev Channel.~~ This is now available to all Insiders in the Dev Channel as of Build 20231. 

## Build 20201
Windows 10 Insider Preview Build 20201 was released to the Dev Channel on [8/26/2020](https://blogs.windows.com/windows-insider/2020/08/26/announcing-windows-10-insider-preview-build-20201/).

## Build 20197
Windows 10 Insider Preview Build 20197 was released to the Dev Channel on [8/21/2020](https://blogs.windows.com/windowsexperience/2020/08/21/announcing-windows-10-insider-preview-build-20197/).

### Bringing Disk Management into Settings
We mentioned we had more Settings work on the way, and here’s the next one – as of today’s build you’ll now be able to manage your disks and volumes from within the Settings app. This includes tasks such as viewing disk information, creating and formatting volumes, and assigning drive letters.

Unlike the existing Disk Management MMC snap-in, this modern experience was built from the ground up to with accessibility in mind. It also features better integration with features such as Storage Spaces and the Storage breakdown page.

Go to **Settings** > **System** > **Storage** and select **Manage Disks and Volumes** to get started. We’d love to hear your feedback once you try it out.

![The Manage Disks and Volumes page in Settings. C drive is selected and shows Explorer and Properties options.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/08/113cc52773bb5f5e6b6b6d761e294222.png)

The existing Disk Management MMC snap-in is still available for those that need it.

### Changes and Improvements
* We’re updating the [**Alt** + **Tab** behavior with Microsoft Edge tabs](https://aka.ms/wip20161) to now have a default of displaying at most 5 tabs, rather than any recent tabs. If at any point you’d like to change this, you can under **Settings** > **System** > **Multitasking**.
* We’re exploring including a Web Browsing section [in the Settings header](https://docs.microsoft.com/windows-insider/archive/new-in-19H1#updated-settings-homepage), and Insiders may start to see this.
* Going forward only the currently active profile picture will display under Your Info in Settings.
* Based on feedback we’re turning off ESENT Warning Event ID 642.
* It’s now possible to select the new Microsoft Edge as your desired app in Assigned Access.
* We’ve updated Narrator so that now when using the Microsoft Pinyin IME, Narrator is able to distinguish candidate characters/words by providing detailed reading information.

## Build 20190
Windows 10 Insider Preview Build 20190 was released to the Dev Channel on [8/12/2020](https://blogs.windows.com/windowsexperience/2020/08/12/announcing-windows-10-insider-preview-build-20190/).

### New post-update experience
We know that it doesn’t always feel clear what changed with a major update, or even how you can learn about and try out new features and improvements. This means that updates can feel time consuming without real benefit to you, and we want to change that. We’re introducing a new first run experience via the Tips app that highlights the most exciting changes on your PC after a major Windows 10 feature update is installed. After installing this build, Insiders will see the Tips app is launched highlight some of the most recent new features from the latest Insider Preview builds in the Dev Channel. To see this experience on your device, make sure the **Show me the Windows welcome experience** checkbox in **Settings** > **System** > **Notifications & actions** is checked.

![The Tips app launches post-update to highlight new features from the latest Insider Preview builds.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/08/cb69036429ed8a259c5ed6e5da6b4153.png)

This experience will show up for Windows Insiders in EN locales such as US, UK, AU, IN, and CA.

__NOTE: The new post update experience with the Tips app mentioned with Build 20190 was a trial run for this experience to get feedback and gauge interest and specific only to Build 20190. You will not see this experience on newer builds. Insiders may see other experiences like this one on newer builds coming soon.__

### Improved Graphics Settings experience
While this isn’t a new feature all together, we have made significant changes based on customer feedback that will benefit our customers’ Graphics Settings experience. We have made the following improvements:

* __We’ve updated the Graphics Settings to allow users to specify a default high performance GPU.__
* __We’ve updated the Graphics Settings to allow users to pick a specific GPU on a per application basis.__

If you’re a power user that has multiple high performance GPUs and would like to specify which of those GPUs should be the one used for high performance uses cases, you can now do that by going to **Settings** > **System** > **Display** > **Graphics settings** or **Settings** > **Gaming** > **Graphics settings**. What this means is that an application that asks for a high-performance GPU will by default use the high-performance GPU you specify on this page.

![Default high performance GPU selection page.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/08/16635566f758c021e6b341dfba58769d.jpg)

Now if you want even more control, we have also added the ability for you to specify exactly which GPU you want an app to run on using the new “Specific GPU” option. As you can see below, an application can be set to run on your GPU of choice.

![The new per-application specific GPU selection option.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/08/bfb6378b0d407e4d79ce6527c67c35bd.jpg)

## Build 20185
Windows 10 Insider Preview Build 20185 was released to the Dev Channel on [8/5/2020](https://blogs.windows.com/windowsexperience/2020/08/05/announcing-windows-10-insider-preview-build-20185/).

### Improving DNS configuration in Settings
We’re making a few changes to the Network section in Settings. 

__Making DNS settings more easily accessible:__ Editing your DNS server assignment is now a top-level option when you go into your network’s properties page.

__Encrypted DNS controls in the Settings app:__ Encrypted DNS (DNS over HTTPS, or DoH) [can help increase privacy and security while browsing the web](https://techcommunity.microsoft.com/t5/networking-blog/windows-insiders-can-now-test-dns-over-https/ba-p/138128). You can now configure DoH directly in the Settings app to more easily take advantage of this feature:

* For ethernet connections: Go to **Settings** > **Network & Internet** > **Status**. Select **Properties**, then select **Edit IP assignment** or **Edit DNS server assignment**, and it will be available in the popup. 

* For Wi-Fi connections: Go to **Settings** > **Network & Internet** > **Wi-Fi**. Select the adapter properties link, then select **Edit IP assignment** or **Edit DNS server assignment**, and it will be available in the popup. Currently you will not see the encryption options if you go to the individual network’s property page.

You can add any IP address listed here to unlock the DoH dropdown and choose to use encryption. Once encryption is enabled, you can confirm it’s working by looking at the applied DNS servers in the network properties and see them labeled as “(Encrypted)” servers. If you want to try a custom DoH server we don’t recognize yet, you can configure an IP address to be recognized as a DoH server by using the netsh command documented here at the end of the blog post.

![The new Edit Network DNS settings popup in Settings.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/08/7783c5f1f83fba22ff585bc2c57ac6fc.png)

### New ADMX Backed Policies for MDM
Starting with Windows 10 Insider Preview Build 20175, we have enabled 647 new MDM policies across 56 ADMX files to enable commercial customers to configure policies that are also supported through Group Policies. Contains ADMX based Policies such as App Compat, Event Forwarding, Servicing and Task Scheduler. These new policies can be configured using Intune custom profile. Intune UX is planned to be available later this year.

ADMX file name:

* AddRemovePrograms.admx
* AppCompat.admx
* AuditSettings.admx
* CipherSuiteOrder.admx
* COM.admx
* Cpls.admx
* CtrlAltDel.admx
* DigitalLocker.admx
* DnsClient.admx
* DWM.admx
* EncryptFilesonMove.admx
* EventForwarding.admx
* FileServerVSSProvider.admx
* FileSys.admx
* FolderRedirection.admx
* Help.admx
* HelpAndSupport.admx
* kdc.admx
* LanmanServer.admx
* LinkLayerTopologyDiscovery.admx
* MMC.admx
* MMCSnapins.admx
* MSAPolicy.admx
* nca.admx
* NCSI.admx
* Netlogon.admx
* OfflineFiles.admx
* PeerToPeerCaching.admx
* PerformanceDiagnostics.admx
* PreviousVersions.admx
* QOS.admx
* Reliability.admx
* Scripts.admx
* sdiageng.admx
* Securitycenter.admx
* Servicing.admx
* Setup.admx
* SharedFolders.admx
* Sharing.admx
* Shell-CommandPrompt-RegEditTools.admx
* Smartcard.admx
* Snmp.admx
* TaskScheduler.admxtcpip.admx
* Thumbnails.admx
* TPM.admx
* UserExperienceVirtualization.admx
* W32Time.admx
* WinCal.admx
* WindowsAnytimeUpgrade.admx
* WindowsConnectNow.admx
* WindowsMediaDRM.admx
* WindowsMediaPlayer.admx
* WindowsMessenger.admx
* WinInit.admx

### Changes and Improvements
* We’re moving the 3D Viewer app into the Windows Accessories folder in the Start menu all apps list.

## Build 20180
Windows 10 Insider Preview Build 20180 was released to the Dev Channel on [7/29/2020](https://blogs.windows.com/windowsexperience/2020/07/29/announcing-windows-10-insider-preview-build-20180/).

### Changes and Improvements
* Based on feedback, we’re changing the tablet posture logic for 2-in-1 devices to now only apply when using a single screen.
* Based on feedback we’re updating the new folder icon in the Start menu’s All app’s list to be a little smaller so it better aligns with the size of the other icons.
* We’ve updated the search box in the Default Apps settings pages to improve performance.

## Build 20175
Windows 10 Insider Preview Build 20175 was released to the Dev Channel on [7/22/2020](https://blogs.windows.com/windowsexperience/2020/07/22/announcing-windows-10-insider-preview-build-20175/).

### Improving pinned sites in Microsoft Edge
Earlier this month, we announced **Alt** + **Tab** between apps and sites, the first of our new productivity enhancements coming to Microsoft Edge on Windows 10. Today, we’re announcing another feature we’ve been working on to make you more efficient when browsing the web: quick access to tabs for your pinned sites. selecting a pinned site on the Taskbar will now show you all of the open tabs for that site across any of your Microsoft Edge windows, just like you’d expect for any app with multiple open windows. Please let us know what you think!

![Selecting a pinned site on the Taskbar will now show you all of the open tabs for that site across any of your Microsoft Edge windows.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/07/f50733d9580bd7b17dd3b245952a8634.gif)

Selecting a pinned site on the Taskbar will now show you all of the open tabs for that site across any of your Microsoft Edge windows.

__This feature is currently rolling out to a subset of Insiders today and requires Microsoft Edge Insider Build 85.0.561.0 or higher (Canary or Dev Channel).__

NOTE: Since this is an early preview, existing sites on your Taskbar will not experience this new behavior until you remove and re-pin them.

For more details on our new multitasking improvements, [check out our post on the Microsoft Edge blog](https://blogs.windows.com/msedgedev/2020/07/22/multitasking-improvements-windows-10-microsoft-edge/).

### Introducing Reset-AppxPackage
For some time now, you’ve been able to reset your UWP apps in Settings – with today’s build we’re now exposing this ability via PowerShell as well. To do this, you’ll need the appx package name, so your use of the command may look like this:

>> Get-AppxPackage *calculator* | Reset-AppxPackage

The benefit of enabling this via PowerShell is that if needed you will now be able to run the reset commands for certain system components that are not currently listed as available to reset in Settings, for example Start.

Please note by nature of this command, if you choose to run it it will reset your experience back to the default experience and you will lose the associated app data.

### Make a more personal connection with Eye Contact on Surface Pro X
Powered by artificial intelligence capabilities of the Microsoft SQ1(TM) processor, Eye Contact helps to adjust your gaze on video calls so you appear to be looking directly in the camera on your Surface Pro X. Windows Insiders can turn this feature on via the Surface app on their Surface Pro X.

![Eye Contact helps to adjust your gaze on video calls so you appear to be looking directly in the camera on your Surface Pro X.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/07/7395420e4c7efa64b0fbff4552d9a54b-1024x796.png)

## Build 20170
Windows 10 Insider Preview Build 20170 was released to the Dev Channel on [7/15/2020](https://blogs.windows.com/windowsexperience/2020/07/15/announcing-windows-10-insider-preview-build-20170/).

### Improving your Sound Settings experience
Last week we mentioned we were planning on bringing more Control Panel capabilities forward into Settings, and here’s another one – we’re updating **Settings** > **System** > **Sound** > **Manage sound devices** to now let you know which device is default, and if not, enable you to set it as your default device or default communication device.

We’ve also updated the volume mixer to include a link to the per app audio settings, which you can use to redirect audio endpoints per app.

There is more work on the way in this area—stay tuned!

### Changes and Improvements
* As part of our ongoing efforts [to update the iconography across Windows](https://medium.com/microsoft-design/iconic-icons-designing-the-world-of-windows-5e70e25e5416), Insiders will notice we’re introducing a new Settings icon in this build. The new Settings icon looks great on the Start menu with the theme-aware tiles [introduced in Build 20161](https://blogs.windows.com/windowsexperience/2020/07/01/announcing-windows-10-insider-preview-build-20161/)!
The new Settings icon as it will appear on Start with theme-aware tiles. 
![New Settings icon with theme-aware tiles on Start.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/07/48b8ca797ac8591eb4e6f8532915f91e-1024x314.png)
* While we work on improving reliability, we’re temporarily turning off Notepad’s ability to persist open windows across restarts and updates.
* An experimental implementation of Transport Layer Security (TLS) 1.3 is enabled by default starting with Insider Preview Build 20170. IIS/HTTP.SYS have TLS 1.3 enabled by default. SSPI callers can use TLS 1.3 by passing the new crypto-agile [SCH_CREDENTIALS](https://docs.microsoft.com/windows/win32/api/schannel/ns-schannel-sch_credentials) structure when calling [AcquireCredentialsHanlde](https://docs.microsoft.com/windows/win32/secauthn/acquirecredentialshandle--schannel). SSPI callers using TLS 1.3 need to make sure their code correctly handles [SEC_I_RENEGOTIATE](https://docs.microsoft.com/windows/win32/secauthn/recognizing-a-request-to-renegotiate-a-connection).

## Build 20161
Windows 10 Insider Preview Build 20161 was released to the Dev Channel on [7/1/2020](https://blogs.windows.com/windowsexperience/2020/07/01/announcing-windows-10-insider-preview-build-20161/).

### Theme-aware tiles in Start
We are freshening up the Start menu with a more streamlined design that removes the solid color backplates behind the logos in the apps list and applies a uniform, partially transparent background to the tiles. This design creates a beautiful stage for your apps, especially the Fluent Design icons for Office and Microsoft Edge, as well as the redesigned icons for built-in apps like Calculator, Mail, and Calendar that we started rolling out earlier this year.

![Theme-aware tiles on the Start menu.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/07/dabfa329dfacdc1a2669002649ed75d6.gif)

This refined Start design looks great in both dark and light theme, but if you’re looking for a splash of color, first make sure to turn on Windows dark theme and then toggle **Show accent color on the following surfaces** for **Start, Taskbar, and action center** under **Settings** > **Personalization** > **Color** to elegantly apply your accent color to the Start frame and tiles.

### Alt + Tab between apps and sites
Are you a multitasker? We have exciting news for you! Beginning with today’s build, all tabs open in Microsoft Edge will start appearing in **Alt** + **Tab**, not just the active one in each browser window. We’re making this change so you can quickly get back to whatever you were doing—wherever you were doing it.

![Alt + Tab between apps and sites.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/07/634dd641ac5d268c671631222138c910.gif)

If you’d prefer fewer tabs or the classic **Alt** + **Tab** experience, we’ve added some settings for you under **Settings** > **System** > **Multitasking**. You can configure **Alt** + **Tab** to only show your last three or five tabs or choose to turn this feature off completely.

__This feature is currently rolling out to a subset of Insiders today in the Dev Channel and requires a Canary or Dev build of Microsoft Edge (version 83.0.475.0 or higher).__

This is just the beginning of productivity enhancements coming to Microsoft Edge—stay tuned!

### A more personalized Taskbar for new users
We want to help customers get the most out of their PCs from day one, and that starts with offering a cleaner, more personalized, out-of-box experience to give you the content you want and less clutter. This provides us with a flexible, cloud-driven infrastructure to test customer reception of default Taskbar content and tailor these layouts based on user and device signal.

We will evaluate the performance of individual default properties, monitoring diagnostic data and user feedback to assess an audience’s reception. Using this information, we will tune default layouts to minimize clutter and perceptions of bloatware.

__Please note that this experience is limited to new account creation or first logon scenarios. We will not use Programmable Taskbar to alter the Taskbar layout on existing accounts.__

![A more personalized Taskbar for new users.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/07/2a484fd68334970e192f8a1138aedc73-1536x635.jpg)

### Improving the notification experience
We are making some changes to improve the notifications experience in Windows 10.

First, know where your toast is coming from by checking out the app logo at the top. Done with the notification? Select the X on the top right corner to quickly dismiss and move on with your life.

![See where your notification toast is coming from by checking out the app logo at the top and quicklt dismiss by selecting the X on the top right corner.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/07/5db65c59e8b5b819bd9203996bf7b8c3.png)

And second, we are turning off the Focus Assist notification and summary toast by default, so we will no longer let users know that Focus Assist has been turned on through an automatic rule via a notification. This can be changed back to the previous behavior via Settings.

### Making Settings even better
We’re continuing to work on bringing capabilities from Control Panel forward into Settings. As part of this ongoing effort, we are migrating information found in Control Panel’s System page into the Settings About page under **Settings** > **System** > **About**. Links that would open the System page in Control Panel will now direct you to About in Settings. We are also bringing new improvements like making your device information copyable and streamlining the security information shown. And don’t worry—if you’re looking for more advanced controls that lived in the System page in Control Panel, you can still get to them from the modern About page if you need them!

![We are migrating information found in Control Panel’s System page into the Settings About page under **Settings** > **System** > **About**.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/07/329ddd5b6ac1257e88fbc73d79d9e7a9-1536x1112.png)

There will be more improvements coming that will further bring Settings closer to Control Panel. If you rely on settings that only exist in Control Panel today, please file feedback and let us know what those settings are.

### Improving the tablet experience for 2-in-1 devices
Previously, when detaching the keyboard on a 2-in-1 device, a notification toast would appear asking if you wanted to switch into tablet mode. If you selected yes, you would switch into tablet mode. If you chose no, it would give you the new tablet posture experience [introduced in the May 2020 Update](https://docs.microsoft.com/windows-insider/archive/new-in-20H1#introducing-a-new-tablet-experience-for-2-in-1-convertible-pcs-build-18970) (or simply the desktop on earlier versions of Windows 10). We are further updating this experience by changing the default, so that this notification toast no longer appears and instead will switch you directly into the new tablet experience, with some improvements for touch. You can change this setting by going to **Settings** > **System** > **Tablet**. Some users may have already seen this change on Surface devices.

And to address confusion with some users getting stuck in tablet mode on non-touch devices, we are removing the tablet mode quick action on non-touch devices.

In addition, new logic is incorporated to let users boot into the appropriate mode according to the mode they were last in and whether the keyboard is attached or not.

## Build 20152
Windows 10 Insider Preview Build 20152 was released to the Dev Channel (Fast ring) on [6/24/2020](https://blogs.windows.com/windowsexperience/2020/06/24/announcing-windows-10-insider-preview-build-20152/).

## Build 20150
Windows 10 Insider Preview Build 20150 was released to the Dev Channel (Fast ring) on [6/17/2020](https://blogs.windows.com/windowsexperience/2020/06/17/announcing-windows-10-insider-preview-build-20150/).

### Three new Windows Subsystem for Linux (WSL) features: GPU compute, WSL install, and WSL update
This build contains three new exciting WSL features. The first is GPU compute: a feature that allows your Linux binaries to leverage your GPU, which makes it possible to do more machine learning development and data science workflows directly in WSL. Secondly, we’ve added a new command: `wsl –install` which allows you to install WSL with just one command. Lastly, we’ve added `wsl –update` which gives you the ability to easily manage the Linux kernel version used by WSL 2 distros. To view a summary of these announcements [please read this post on the Windows Command line blog](https://devblogs.microsoft.com/commandline/gpu-compute-wsl-install-and-wsl-update-arrive-in-the-windows-insiders-fast-ring-for-the-windows-subsystem-for-linux), and for in-depth details on GPU compute in WSL please [read this post](https://blogs.windows.com/windowsdeveloper/?p=55781) on the Windows Developer blog.

![GPU Compute via WSL.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/06/3d39cf80787a7208278a716ceb76d29a.gif)

### General changes & improvements
* With this week’s build, we’ll be starting to roll out [the new search box on the default app settings pages](https://blogs.windows.com/windowsexperience/2020/04/15/announcing-windows-10-insider-preview-build-19608/). As part of this, we’ve done some work to improve the performance of the search box.
* [The new Korean IME](https://blogs.windows.com/windowsexperience/2019/12/16/announcing-windows-10-insider-preview-build-19536/) is now available again for Insiders to use.
* Based on feedback, we’re updating the text of the **Settings** > **Privacy** > **Location** page to clarify that the icon displayed when your location is being used will be displayed in the Taskbar.

## Build 19645
Windows 10 Insider Preview Build 19640 was released to the Fast ring on [6/10/2020](https://blogs.windows.com/windowsexperience/2020/06/10/announcing-windows-10-insider-preview-build-19645/).

### General changes & improvements
* We changed the servicing model for the Linux kernel inside of Windows Subsystem for Linux 2 distributions. This build includes this change to remove the Linux kernel from the Windows image, and instead have it be serviced via Microsoft Update, the same way that 3rd party drivers (like graphics, or touchpad drivers) are installed and updated on your machine today. For full details [please read this blog post on the Windows Command Line blog](https://devblogs.microsoft.com/commandline/wsl2-will-be-generally-available-in-windows-10-version-2004/) and for information about the kernel version please [view the kernel docs page here](https://docs.microsoft.com/windows/wsl/kernel-release-notes).
* Support for [Nested Virtualization](https://docs.microsoft.com/virtualization/hyper-v-on-windows/user-guide/nested-virtualization) on AMD processors is now available. Being an early release we recommend you [read this blog post](https://techcommunity.microsoft.com/t5/virtualization/amd-nested-virtualization-support/ba-p/1434841) for details on what platforms currently work as well as how to enable the feature.

## Build 19640
Windows 10 Insider Preview Build 19640 was released to the Fast ring on [6/3/2020](https://blogs.windows.com/windowsexperience/2020/06/03/announcing-windows-10-insider-preview-build-19640/).

## Build 19635
Windows 10 Insider Preview Build 19635 was released to the Fast ring on [5/28/2020](https://blogs.windows.com/windowsexperience/2020/05/28/announcing-windows-10-insider-preview-build-19635/).

## Build 19631
Windows 10 Insider Preview Build 19631 was released to the Fast ring on [5/21/2020](https://blogs.windows.com/windowsexperience/2020/05/21/announcing-windows-10-insider-preview-build-19631/).

### General changes & improvements
* We updated the configuration of Windows Hello to make sure it works well with 940nm wavelength cameras.

## Build 19628
Windows 10 Insider Preview Build 19628 was released to the Fast ring on [5/13/2020](https://blogs.windows.com/windowsexperience/2020/05/13/announcing-windows-10-insider-preview-build-19628/).

### General changes & improvements
* We’re adding initial support for DNS over HTTPS, so that you can opt into using encryption when Windows makes DNS queries. [Follow the instructions in this blog post](https://techcommunity.microsoft.com/t5/networking-blog/windows-insiders-can-now-test-dns-over-https/ba-p/1381282) to opt in as it will be off by default.
* Thanks everyone who shared feedback about the updated version of Korea Microsoft IME introduced with Build 18941. For the moment, the IME version will be returning to the previous one while we take your feedback into consideration.

## Build 19624
Windows 10 Insider Preview Build 19624 was released to the Fast ring on [5/6/2020](https://blogs.windows.com/windowsexperience/2020/05/06/announcing-windows-10-insider-preview-build-19624/).

### General changes & improvements
* We’re temporarily turning off the new search box in the default apps Settings pages while we work on improving performance and reliability.
* We’re updating the VPN connection logic based on feedback, so that if you disconnect from a VPN network, it will now uncheck the option to auto-connect (similar to how it’s handled for Wi-Fi).
* Based on feedback we’re updating the text of the Add a Device dialog so the list of examples under Bluetooth includes controllers.
* We’re updating the Optional Updates Available section that appears in Windows Update settings, so that you will now be able to copy the text in case you need it.

## Build 19619
Windows 10 Insider Preview Build 19619 was released to the Fast ring on [4/29/2020](https://blogs.windows.com/windowsexperience/2020/04/29/announcing-windows-10-insider-preview-build-19619/).

### General changes & improvements
* If the Sync button under **Settings** > **Time & Language** > **Time** fails due to network connectivity, the error now tells you that’s the issue.

## Build 19613
Windows 10 Insider Preview Build 19613 was released to the Fast ring on [4/22/2020](https://blogs.windows.com/windowsexperience/2020/04/22/announcing-windows-10-insider-preview-build-19613/).

## Build 19608
Windows 10 Insider Preview Build 19608 was released to the Fast ring on [4/15/2020](https://blogs.windows.com/windowsexperience/2020/04/15/announcing-windows-10-insider-preview-build-19608/).

### Improving your default apps experience
Over the years, we’ve made a number of improvements to Settings based on your feedback, and we’re happy to share the next one is starting to roll out. We’re adding the ability to search the lists of file types, protocols, and apps when setting a default.

![Showing the Choose default apps by file type Settings window, now with a search box.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/04/bc885b7c284ce0a6d23eb6a909890cdd.png)

This change is currently available for 50% of Insiders in the Fast ring as we evaluate the quality. We’ll let you know when that rollout increases. Please give it a try once it’s available on your device, and let us know what improvements you’d like to see next!

## Build 19603
Windows 10 Insider Preview Build 19603 was released to the Fast ring on [4/8/2020](https://blogs.windows.com/windowsexperience/2020/04/08/announcing-windows-10-insider-preview-build-19603/).

### File Explorer Integration in the Windows Subsystem for Linux (WSL)
If you have WSL installed and open up File Explorer, you’ll see a familiar face!

![Pointing out the Linux entry in the File Explorer navigation pane.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/04/a115bf3a1a66ef9a9a76190839835e4c.png)

[We’ve had the ability to access your Linux files since Windows 10 version 1903](https://devblogs.microsoft.com/commandline/whats-new-for-wsl-in-windows-10-version-1903/), but now you can easily get to them from your left-hand navigation pane in File Explorer. Selecting the Linux icon will show you a view of all your distros, and selecting those will place you in the Linux root file system for that distro.

![Showing the folders under the Linux section in File Explorer.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/04/834929eb91b182277df7061b7ce9333a.jpg)

### User cleanup recommendations in Storage Settings
Free up disk space with this Storage Settings feature that gathers unused files and apps so you can digitally cleanse your device.

![Find User cleanup recommendations in the Storage Settings page.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/04/a061c6428b4ed25b7ecba3738744a6ae.png)

Windows cannot predict whether you want to delete personal files, uninstall apps, or remove local copies of files synced to the cloud. With this tool, all the content is gathered in one page and removable by you with a few clicks.

![User cleanup recommendations is made up of 4 sections: Temporary files, Large or unused files, Files synced to the cloud and Unused apps.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/04/c74dc6e055fe56a9832899f6ca8e6995.png)

### General changes & improvements
* Going forward, services that are implemented by binaries residing in the user profiles will be persisted on upgrades.
* Narrator will no longer automatically enable scan mode when interacting with the Ideas pane in Excel. In the new Microsoft Edge, Narrator now automatically enables scan mode and starts reading webpages.

## Build 19592
Windows 10 Insider Preview Build 19592 was released to the Fast ring on [3/25/2020](https://blogs.windows.com/windowsexperience/2020/03/25/announcing-windows-10-insider-preview-build-19592/).

### Tablet posture improvements for 2-in-1 convertible PCs
We are beginning to roll out (again*) the new tablet experience for 2-in-1 convertible PCs as a preview to some Windows Insiders in the Fast ring. This experience is separate from the Tablet Mode experience that you will still be able to use. This new experience allows users entering tablet posture to stay in the familiar desktop experience without interruption with a few key touch improvements:

* Taskbar icons are spaced out
* Search box on Taskbar is collapsed into icon-only mode
* Touch keyboard auto invokes when you tap a text field
* File explorer elements will have a little more padding, to make them comfortable to interact with using touch
* You’ll also notice we’ve updated some of the related Tablet settings under **Settings** > **System**, so as to give you control over the experience.

![Tablet posture improvements for 2-in-1 convertible PCs.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/03/068d5e0abaf805d92a03526f7e208e88.jpg)

In order to help ensure quality, the feature will be rolling out slowly, starting with a portion of the Insiders that have never detached their keyboard before, or have their tablet mode settings set to __Don’t ask me and don’t switch__.

We’d love to hear your feedback about the experience:

1. Use your convertible PC with apps as you normally would.
2. When you’re ready to pick it up and go or simply lean back on the couch, you can fold back the keyboard or remove it altogether.
3. Use your device as a tablet with touch, without going into Tablet Mode.
4. Screenshot showing improvements to tablet posture, like collapsed search, increased spacing between icons, and a touch keyboard option in your Taskbar.

>[!NOTE] 
>This feature was previously rolled out as an experiment to Windows Insiders in 20H1 Build 18970 and ended in Build 19013. After some refinement, we’re reintroducing it to Windows Insiders in this build and plan to deliver this experience to customers in a future Windows 10 update.

### General changes & improvements
* The Windows Search Platform (Indexer) has been updated with improved logic to help find better times to perform indexing of your files and avoiding heavily indexing while you are using your machine. An improvement was also made to significantly limit the amount of times the service indexes your files for content that doesn’t have an impact on search experiences, and gives you a better experience on Windows.

## Build 19587
Windows 10 Insider Preview Build 19587 was released to the Fast ring on [3/18/2020](https://blogs.windows.com/windowsexperience/2020/03/18/announcing-windows-10-insider-preview-build-19587/).

### General changes & improvements
* Based on feedback, when you have muted your volume, the volume will now not unmute when using the hardware keyboard volume keys until you raise the volume (or manually unmute).
* We made a couple of improvements to Narrator and how it works with some of the controls in Windows:
    * Narrator now uses a more friendly string to describe the audio output in the Select playback device dropdown menu in the volume flyout.
    * Narrator now announces more information in the Add Bluetooth or other devices dialog in the Settings application when first opened.

## Build 19582
Windows 10 Insider Preview Build 19582 was released to the Fast ring on [3/12/2020](https://blogs.windows.com/windowsexperience/2020/03/12/announcing-windows-10-insider-preview-build-19582/).

### Eye Control Improvements
Eye Control enables users to interact with Windows using only their eyes. Based on feedback, with this build, we’re updating the Eye Control settings to now span multiple pages, in order to give the options a bit more room to breathe.

![Updated Eye Control Settings that span multiple pages.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/03/d39bb5a9d70f13c8c4ae23340e4aa927.png)

To get started with Eye Control, connect a supported eye tracking device, then [follow the steps here](https://support.microsoft.com/help/4043921/windows-10-get-started-eye-control).

### General changes & improvements
* We’re working on giving you control over whether apps can disable the screen capture border. The page isn’t finished being wired up yet, but you’ll see it listed under Privacy Settings.
* We’ve updated the “set time zone automatically” toggle in Time & Date settings to now be greyed out if location has been disabled.
* Based on feedback, we’re updating the Scottish Gaelic keyboard in these ways:
    * Pressing **AltGR** + **7** will now input ⁊ (U+204A TIRONIAN SIGN ET).
    * Pressing **(‘)** will now directly insert that character (right single quote).
    * Pressing **AltGr** + **(’)** will now act as a dead key to combine an acute accent with a subsequent letter.

## Build 19577
Windows 10 Insider Preview Build 19577 was released to the Fast ring on [3/5/2020](https://blogs.windows.com/windowsexperience/2020/03/05/announcing-windows-10-insider-preview-build-19577/).

### Diagnostic data changes in Settings
As part of the Microsoft initiative to increase transparency and control over data, we’re making some changes to the Settings app and Group Policy settings that will start showing up in Windows Insider builds this month. Basic diagnostic data is now known as Required diagnostic data and Full diagnostic data is now Optional diagnostic data. If you’re a commercial customer and choose to send Optional diagnostic data, we will also be providing more granular Group Policy settings to configure the data that’s collected within your organization. We’ll publish more specifics around the new policies when we get closer to the retail release, and in the meantime, check out the Microsoft Privacy Report for more information around our data collection practices.

__Note: Please make sure your device is set to “Full” before updating to Build 19577. You will not be able to take future flights if your diagnostic level is left at “Enhanced”. AAD/Domain-joined PCs set to “Enhanced” will be blocked from taking Build 19577. For more information, [see this Answers post](https://aka.ms/ddchanges).__

### More new icons: Windows Security
We’re continuing to roll out updated icons to many of the built-in apps in Windows 10. In today’s build, we’ve updated the Windows Security icon to match the new design principles outlined here from the Microsoft Design Team. Unlike many of the built-in apps in Windows 10, which can be updated through the Store, the new Windows Security icon is updated through the OS and will rollout in a future Windows 10 feature update.

![The new Windows Security icon as it appears on the Taskbar.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/03/254a7cea7eb9aed8586fc445faeaa227.png)

### General changes & improvements
* Following up on [our post about the new Cortana app](https://insider.windows.com/articles/cortana-windows-beta/), we wanted to let you know that in addition to timers and instant answers, which lit up last month, assistant conversations are now online. Some examples to try are “tell me a dad joke”, “tell me a bedtime story”, or “rock, paper, scissors.” We appreciate your patience while we worked on this. This is a server-side change, however we’re noting it here for awareness.
* We’ve updated the behavior of Advanced startup (**Settings** > **Update & Security** > **Recovery** > **Advanced startup** > **Restart now**) to enable some Ease of Access features to work properly. For example, previously, if the narrator feature was enabled prior to launching Advanced startup, it would stop working. Now, Advanced startup will reboot directly into the Windows Recovery Environment.
* While the Vietnamese alphabet doesn’t include the Latin letters F, J, W, or Z, based on feedback we’re updating the grouping in the Start menu’s all app’s list to account for these letters when using this display language, so that apps like Windows PowerShell are included in the expected group.

## Build 19569
Windows 10 Insider Preview Build 19569 was released to the Fast ring on [2/20/2020](https://blogs.windows.com/windowsexperience/2020/02/20/announcing-windows-10-insider-preview-build-19569/).

### Evolving the Windows 10 icons
We are currently working on a multi-year effort across Microsoft’s design teams to redesign the icons across all our products. We started with the Office icons, and now we’re moving forward with updating the icons in Windows 10, starting with the built-in apps like Alarms & Clock, Calculator, Mail, and Calendar. Research and feedback from Windows Insiders showed a desire to see consistency in design and connection to the brand, with enough differences to aid in recognition. You can read all about our approach to updating the icons in Windows 10 in this Medium post from the Microsoft Design Team!

![View of updated design for web preview in search results.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/02/7e4667f9c9e488683aca797991b5a747.png)

Many of these icons will be updated as app updates from the Microsoft Store. We are beginning to roll them out to Windows Insiders in the Fast ring first, starting today. The Mail and Calendar icons rolled out this morning to Release Preview. Over the coming months, Insiders will see more of the icons in Windows 10 get updated with new designs!

## Build 19564
Windows 10 Insider Preview Build 19564 was released to the Fast ring on [2/12/2020](https://blogs.windows.com/windowsexperience/2020/02/12/announcing-windows-10-insider-preview-build-19564/).

### Graphics Settings Improvements
We’ve updated the Graphics settings page (**Settings** > **System** > **Display** > **Graphics settings**), allowing for better control over designating which GPU your apps run on. With this update, the app list and GPU preference are pre-populated on a best effort basis to improve the default preference management experience. If your desired app isn’t pre-populated, you can still add it by using the app selection drop-down.

![The updated Graphics settings page with pre-populated app preference management.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/02/ab377b0f73f0fd7001039bc50d2681ff.jpg)

You’ll notice alongside this, we’ve also added a search box and a filter for the list of apps.

## Build 19559
Windows 10 Insider Preview Build 19559 was released to the Fast ring on [2/5/2020](https://blogs.windows.com/windowsexperience/2020/02/05/announcing-windows-10-insider-preview-build-19559/).

### General changes & improvements 
* For any of our Insiders using an arm64 device, such as the Surface Pro X, running Enterprise or Pro edition, you’ll now be able to see and install Hyper-V features.

## Build 19555
Windows 10 Insider Preview Build 19551 was released to the Fast ring on [1/30/2020](https://blogs.windows.com/windowsexperience/2020/01/30/announcing-windows-10-insider-preview-build-19555/).

## Build 19551
Windows 10 Insider Preview Build 19551 was released to the Fast ring on [1/23/2020](https://blogs.windows.com/windowsexperience/2020/01/23/announcing-windows-10-insider-preview-build-19551/).

## Build 19546
Windows 10 Insider Preview Build 19546 was released to the Fast ring on [1/16/2020](https://blogs.windows.com/windowsexperience/2020/01/16/announcing-windows-10-insider-preview-build-19546/).

## Build 19541
Windows 10 Insider Preview Build 19541 was released to the Fast ring on [1/8/2020](https://blogs.windows.com/windowsexperience/2020/01/08/announcing-windows-10-insider-preview-build-19541/).

### Location in-use icon update
As some keen eyed Insiders have noticed, we’ve updated the notification area icon for when an app is using your location. The new icon looks like this:

![Showing the new arrow icon for location in use.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/01/f3b5ee974cf44250d484db25447cce28.png)

### Showing architecture in Task Manager
When you’re using the Details tab in Task Manager, we’ve added a new option to show the architecture of each process. If you’re interested, you can add it by right-clicking on a column header, choosing Select Columns, and selecting Architecture from the list.

![When you're in the Details tab of Task Manager, you can now add this Architecture option.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2020/01/5cd3aaadea5f925716341c53a4b89b20.png)

## Build 19536
Windows 10 Insider Preview Build 19536 was released to the Fast ring on [12/16/2019](https://blogs.windows.com/windowsexperience/2019/12/16/announcing-windows-10-insider-preview-build-19536/).

### Optional Drivers
[We’re still working on making it easier for you to see all optional updates](https://aka.ms/wip18985) (including drivers, feature updates, and monthly non-security quality updates) in one place. When optional updates are detected, they will be listed under **Settings** > **Update & Security** > **Windows Update** > **View optional updates**.

For drivers, you no longer need to browse Device Manager for a specific device to update. Windows Update will automatically keep your drivers up to date, but if you’re having a problem, one of those optional drivers might help.

View optional updates option in the Windows Update section of Update & Security Settings.

### Re-releasing the updated Korean IME
During 19H1 development, we’d started work on an updated version of the Korean IME as part of our ongoing efforts to modernize and improve your typing experience in Windows. Based on feedback, we decided not to ship this with 19H1, and instead worked on further improving the experience first. With Build 19536, we’re re-releasing the updated IME, along with some improvements that help it work better with various apps.

To recap the most noticeable changes included as part of this IME work:

* For those who’re familiar with typing in Korean when writing in Hanja, we have a new candidate selection window that uses modern controls and clearer typography:

![Showing the candidate selection window of the updated Korean IME.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2019/12/17baa87bb553ab0d1bc9f5de682d3a7d.png)

* The new IME version also comes with an updated algorithm used for text prediction when writing Korean using the touch keyboard. Text suggestions should now be more accurate and relevant to what you are writing.

### Family group setup
[Microsoft has family features that span across multiple platforms](https://account.microsoft.com/family/about), like Windows, Xbox, and Android. On Windows, you can set things up for your family, like screen time limits, content filters, have kids ask before they buy things, or even stay organized with a shared family calendar, OneNote, and Office 365 Home subscription. If you share a device with family, it’s easy to get their account set up in a family group to take advantage of all these features.

![New Who will use this device screen when setting up a new Windows 10 PC.](https://46c4ts1tskv22sdav81j9c69-wpengine.netdna-ssl.com/wp-content/uploads/prod/sites/2/2019/12/df545e6188f866eee1db8f9f73382240.png)

In this build, we want to help customers set up their device to be used by multiple people in their family. While we’re not releasing an ISO for this build, some Insiders who choose to reset their PC may see a screen during setup that asks who’ll be using the device. If they select People in my family, we’ll help them get set up in a family group once they get to their desktop, so that they’re ready to get started with all the features.

If you see this new page, let us know what you think by going to Security and **Privacy** > **Child accounts and family settings** in the Feedback Hub.
