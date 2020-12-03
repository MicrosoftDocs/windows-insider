---
title: Troubleshooting 
description: Troubleshooting tips 
author: bleblanc
manager: dougkim
ms.tgt_pltfrm: na
ms.devlang: na
ms.author: v-allsh
ms.localizationpriority: medium
ms.topic: article
ms.prod: w10
---

# Troubleshooting 

Running into an issue on Windows 10 Insider Preview Builds? This section can help you with some common problems. 

> [!NOTE] 
> We document known issues for Insider Preview builds in our [flight blog posts](https://blogs.windows.com/blog/tag/windows-insider-program/). Most issues are tied to specific builds, so this is the first place you should check if you're having problems.  

## Find information about your PC

When giving feedback or getting support it can be important that you know how to find key information about your device.


- **Find the build number your device is on currently.**

Go to [**Settings** > **System** > **About**](https://aka.ms/AboutSettings), and your OS build number will show under Windows specifications. 

Or you can also type **winver** into your search and open it to see your latest Windows details, including OS build number.

[See all the ways you can check if your device is flighting.](https://docs.microsoft.com/windows-insider/check-flighting-status)


- **Find which channel your device is in.**

Go to [**Settings** > **Update & Security** > **Windows Insider Program**](https://aka.ms/WIPSettings). Under **Pick your Insider settings**, you'll see your current channel.


- **Check which Microsoft Account (MSA) or Azure Active Directory (AAD) account you're using on your device.**

Go to [**Settings** > **Update & Security** > **Windows Insider Program**](https://aka.ms/WIPSettings). Under Windows Insider account, you'll see the account it's tied to.

## Changing channels

If you install an Insider Preview build in one channel, and you want to switch to a different channel, you might need to do a clean install of Windows and reset your Windows Insider settings on that device. [Learn more about switching channels.](https://docs.microsoft.com/windows-insider/flighting#switching-between-channels)

## Not receiving updates

If your device isn't receiving updates, check for these issues.

1. **Check if you're already on the latest Insider Preview build.**

You might already be on the latest preview build for your channel. [Check Flight Hub to see what the latest build is for your channel.](https://docs.microsoft.com/windows-insider/flight-hub/) 

2. **Check the known issues.**

There may be an issue with the Insider Preview build you're on or the next build that prevents you getting new updates. Check recent [flight blog posts](https://blogs.windows.com/blog/tag/windows-insider-program/) to see if you're impacted by a known issue.

3. **Make sure you're running Windows 10.**

To install Windows 10 Insider Preview Builds, you must be running a licensed version of Windows 10 on your device. You can [install Windows 10 here](https://www.microsoft.com/windows/get-windows-10?step=Win10Question1) if your device is currently running an older version or if you need to buy Windows. If you're having issues installing Windows 10, you can also [download a Windows 10 Insider Preview ISO](https://www.microsoft.com/software-download/windowsinsiderpreviewadvanced) to get started.

4. **Make sure Windows is activated.**

Windows must be activated to run Windows Insider Preview builds. Go to [**Settings** > **Update & Security** > **Activation**](https://aka.ms/ActivationSettings) to make sure your copy is activated.

5. **Manually check for updates.**

Go to [**Settings** > **Update & Security** > **Windows Update**](https://aka.ms/WIPWindowsUpdate) and select **Check for Updates**. If you have set active hours, make sure your device is left turned on and signed in during your off-hours, so the update can install.

6. **Check you're signed in with a registered account.**

You must be registered as a Windows Insider to get preview builds. [You can register on our website.](https://insider.windows.com/getting-started) If you're already registered, when you log in to the site, you'll no longer be able to see register options on the site.

Make sure your device is connected to your registered account under [**Settings** > **Accounts** > **Access work or school**](https://aka.ms/WorkAccountSettings). 

7. **Check your program settings.**

Go to [**Settings** > **Update & Security** > **Windows Insider Program**](https://aka.ms/WIPSettings) and make sure you've activated the Windows Insider Program on your device and that you've chosen a channel to receive builds from. [Learn more about channels.](https://docs.microsoft.com/windows-insider/flighting)

8. **Check your data settings.**

Your privacy is important to us, so you're in control of how much of your data you share with us. But to run Windows 10 Insider Preview Builds, you must allow us to see a certain amount of diagnostic data, so we can investigate issues you might see, like crashes and bugs. [Make sure your data settings are at the right level to receive preview builds.](https://docs.microsoft.com/windows-insider/data-settings) 

9. **Make sure you didn't change from the Dev Channel.**

If you've already installed a build in the Dev Channel and want to switch channels or stop receiving Insider Preview builds, because it's not tied to a specific release, you'll have to do a clean install of Windows and reset your Windows Insider settings. If you only switch your channel settings and don't do a clean install, you could be stuck not receiving updates. [Learn more about how to switch channels.](https://docs.microsoft.com/windows-insider/flighting#switching-between-channels)

10. **Consider a clean install.**

If none of these options work for you, you may need to do a clean installation of Windows to reset your device. [Learn more about clean installations with ISOs.](https://docs.microsoft.com/windows-insider/ISOs)


## Dealing with issues

If you're seeing an issue on a Windows 10 Insider Preview Build, here's what you should do.

1. **Check the known issues.**

We document known issues in our [flight blog posts](https://blogs.windows.com/blog/tag/windows-insider-program/). This is the first place you should check if you're seeing an issue. We may already be working on it.

2. **Check for updates.**

Make sure there's not a newer build available that could fix the issue by going to [**Settings** > **Update & Security** > **Windows Update**](https://aka.ms/WIPWindowsUpdate) and selecting **Check for Updates**.

3. **Decide how serious the issue is.**

Can you still use your device or is key functionality broken? Is it a single app or minor functionality? Can you work around the issue? 

4. **File feedback.**

Tell us about the issue you're seeing in the [Feedback Hub](https://aka.ms/WIPFeedbackHub) and include as many details, screenshots, and logs as possible along with your feedback.

5. **Recover or reset your device.**

If an issue is preventing you from using your device, you might need to recover or reset it.


## Recovering your device

If an issue is preventing you from getting updates or using your device, you have a few options for recovering it.

> [!NOTE] 
> Before reinstalling or rolling back on your device, make sure you've backed up all of your important files.


1. **Reset your device.**

Use Reset this PC to reset your device, which will reinstall Windows on the same build you're currently on. 

Go to [**Settings** > **Update & Security** > **Recovery**](https://aka.ms/WIPRecoverySettings), and under **Reset this PC**, select **Get Started**. Follow its directions to reset your device.

2. **Roll back to a previous build.**

If your device was working on the previous build, you can roll back for 10 days (or until you take the next build) after installing the update without having to completely reset your device. After that, you'll have to take a new update or do a clean install.

To roll back, go to [**Settings** > **Update & Security** > **Recovery**](https://aka.ms/WIPRecoverySettings), and under **Go back to the previous version of Windows 10**, select **Get Started**. Follow its directions to finish rolling back.

3. **Clean install Windows or an Insider Preview build.**

For a fresh start, you can also do a clean installation of a different Insider Preview build or the latest version of Windows 10 using an ISO file. [Learn more about clean installations with ISOs.](https://docs.microsoft.com/windows-insider/ISOs)

## Build expiration

Insider Preview builds do expire eventually. Staying up to date is key to avoiding security risks, which is why expiration dates are important. 

If your device is on an expiring build, you'll start getting notifications letting you know that you need to update. Go to [**Settings** > **Update & Security** > **Windows Update**](https://aka.ms/WIPWindowsUpdate) and select **Check for Updates** to get the latest update available in your channel.   

If you aren't seeing any updates available, you might need to adjust your settings or do a clean install. [Learn more about what to do if you're not seeing updates and your build is expiring.](https://docs.microsoft.com/windows-insider/build-expiration) 

## Stop receiving Insider Preview builds

If you no longer want to receive Insider Preview builds, you'll have to unenroll your device. If you don't leave the program though, you will continue to receive emails. To unenroll your device:

1. Go to [**Settings** > **Update & Security** > **Windows Insider Program**](https://aka.ms/WIPSettings) > **Stop Insider Preview Builds** to see your options.

2. If you're in the Beta Channel or the Release Preview Channel, you can flip the switch to stop stop getting preview builds on your device when the next major release of Windows 10 launches to the public. (If your device is currently running a public release of Windows, this will immediately opt you out of getting preview builds. Just restart your device to complete the process.)

3. If you're in the Dev Channel or you'd like to stop getting preview builds immediately, you should [use these instructions to complete a clean installation of Windows 10](https://support.microsoft.com/help/4000735/windows-10-reinstall#Clean%20install%20of%20Windows%2010%20using%20installation%20media).

> [!NOTE] 
> If you're receiving Insider Preview builds through work but aren't the administrator, you will still get preview builds until your organization leaves the program or adjusts your settings. 

## Leave the program

Windows Insiders help shape the future of Windows, and your participation is important to us. But if you're sure you'd like to stop getting emails and Windows 10 Insider Preview Builds from us, you can unregister and leave the program. 

If you'd just like to stop getting Insider Preview builds, you can also unenroll your device with the steps in the **Stop receiving Insider Preview builds** section above, but stay registered to keep getting email updates from us.

> [!div class="nextstepaction"]
> [Leave the program now](https://insider.windows.com/leave-program)

Once you leave the program, use the **Stop receiving Insider Preview builds** section above to stop getting preview builds on your devices.

## Get more help

If you're still having problems, make sure you report feedback in the [Feedback Hub](https://aka.ms/WIPFeedbackHub). Then, you can also share your feedback link with us on the [Windows Insider Twitter](https://twitter.com/windowsinsider) or [Answers forum](https://answers.microsoft.com/) to get more help from our team.
