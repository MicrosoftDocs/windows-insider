---
title: Troubleshooting 
description: Troubleshooting tips 
manager: eliotgra
ms.tgt_pltfrm: na
ms.devlang: na
ms.date: 11/01/2018
ms.author: v-colinmit
author: cdmm12
ms.localizationpriority: medium
ms.topic: article
ms.prod: w10
---

# Troubleshooting 

This section provides tips to address issues that you many encounter when running Windows 10 Insider Preview Builds. 

> [!NOTE] 
> In many cases, issues may be isolated to your specific Insider Preview build. Please check the most recent [Windows Insider Blog post](https://blogs.windows.com/blog/tag/windows-insider-program/) or our [support resources](https://docs.microsoft.com/en-us/windows-insider/at-home/troubleshooting#support-resources), like the [Windows Insider Forums](https://answers.microsoft.com/en-us/insider/forum/insider_wintp-insiderplat_pc?sort=lastreplydate&dir=desc&tab=threads&status=all&mod=&modAge=&advFil=&postedAfter=&postedBefore=&threadType=all&tm=1475533679179). 

## Find information about your PC

These questions can help you find key information that may be useful as you participate in the program or submit feedback.

### How can I find the build number?

Go to **Start**, type **winver**, select “**winver - run command**.”

### How can I see which flight ring I'm on?

Open **Settings**, select **Update & Security**, select **Windows Insider Program**. The flight ring you've selected will be under **Pick your Insider settings**.

### How do I check which Microsoft Account (MSA) or Azure Active Directory (AAD) account I'm using for getting builds?

Open **Settings**, select **Update & Security**, select **Windows Insider Program**, and view your **Windows Insider account information**.

### How can I confirm my copy of Windows 10 is activated?
Open **Settings**, select **Update & Security**, and select **Activation**.

## Not receiving updates

While participating in the Windows Insider Program, you may find that your PC isn't updating as expected. Review these key times if you're in this state.

### Run Windows 10
To install Windows 10 Insider Preview Builds, you need to be running a licensed version of Windows 10 on your PC. If your PC is currently running Windows 7/8/8.1, you can install Windows 10 [here](https://www.microsoft.com/en-us/windows/get-windows-10?step=Win10Question1). 

If you are having problems installing Windows 10, you can download a [Windows 10 Insider Preview ISO](https://www.microsoft.com/en-us/software-download/windowsinsiderpreviewadvanced). 

### Activate Windows

Your copy of Windows must be activated to run Windows Insider Preview builds. Make sure you're activated by opening **Settings**, selecting **Update & Security**, and selecting **Activation**.

### Perform a manual check for updates

Open **Settings** > **Update & Security** and review available updates or select __Check for Updates__. If you have set Active Hours, make sure your device is left turned on and signed in during your off-hours, so the update can install.

### Sign in with an MSA or AAD account registered for receiving builds on your device

[Sign in with your MSA or AAD account.](https://insider.windows.com/en-us/insidersigninboth/) You will land on the page “Welcome back!” if your MSA or AAD account is registered with the Windows Insider Program.

### Make sure you've chosen a ring

Open **Settings** > **Update & Security** > **Windows Insider Program** and view the dropdown under **What pace do you want to get new builds?**

### Check if you've done a rollback

Check your Windows Insider Preview settings, including ring selection, Microsoft Account, and branch-selection.

### Consider a clean install

After a clean install and initial setup of a Microsoft Account, even one that has been used previously for receiving Insider builds, the appropriate targeting needs to take place. This background process is known as Compatibility Checker and will run during idle time on your PC. This may take up to 24 hours. Leave your PC turned on to make sure this occurs in timely manner.

### Check known issues for your current build

There may be an issue with a build that could lead to issues with updates being received. Check the most recent [Windows Insider Blog post](https://blogs.windows.com/blog/tag/windows-insider-program/) or reach out to us [@WindowsInsider](http://twitter.com/windowsinsider/).

## Recovering a PC
If you are in a situation where you are unable to use your PC as expected, these steps can help you return it to a good state.

### Assess the impact
- What is the impact of the issue? Single app? Minor functionality? 
- Can you continue using your device or is key functionality not working? 
- Are you able to work around the issue? Would an alternate app suffice? 
- Is a newer build available that may have a fix for any known bugs being faced?

### Troubleshoot & Discover
**OS reinstall** - If important functionality is unusable, you may want to reinstall your current OS version. You have several options to choose from, including an operating system-only reinstall or a clean wipe of your device: Go to **Settings** > **Update & Security** > **Recovery** and select **Get Started** under **Reset this PC**. Follow the on-screen directions to refresh or clean install the OS. 

> [!NOTE] 
> Before doing any reinstall or rollback, make sure you've backed up important files. While it's rare to lose data during this process, it's best to back up key data.

**Roll-back to previous build** - If your PC was working as expected on the previous build and you’d like to roll back without losing any data, go to **Settings** > **Update & Security** > **Recovery**, and select **Get Started** under **Go Back to an Earlier Build**. 

> [!NOTE] 
> After installing an update to your PC, you will have seven days to roll back if necessary. If it's needed after that, you'll need to take a future update, or you may clean install an older build via bootable media.

**Clean Install Insider Build via Bootable Media** - Creating a bootable USB with a Windows Installation (from an ISO file) can be helpful in multiple scenarios, from recovering a machine from a bad build, to bypassing some types of bugs, to even joining a new PC into the Windows Insider Program. [How to make a bootable USB drive from a Windows Insider ISO file.](https://answers.microsoft.com/en-us/insider/forum/insider_wintp-insider_install-insiderplat_pc/creating-a-bootable-usb-for-windows-insider-isos/9ebe3cbc-3c8b-4052-9484-0b7cc9b63bec?tm=1519414191218)

## Feedback Hub error

### Why am I getting a "Something went wrong" error message in Feedback Hub?

The option for users to give consent for apps to access their profile data is controlled through Azure Active Directory. This means that AAD administrators have the ability to allow or block users from giving consent. 

If an administrator has blocked this option, the user will see a "Something went wrong error" message when they sign in with an AAD account. Administrators can unblock in the [Azure portal](https://portal.azure.com/). Go to **Enterprise applications** > **User Settings** and enable **Users can consent to apps accessing company data on their behalf data**. 

## Stop receiving Insider builds

To opt a device out of the Insider program, go to **Settings** > **Update & Security** > **Windows Insider Program** and turn on the **Stop getting preview builds setting**.

If the device is currently running a public release of Windows, opting out will happen immediately. Your device will require a reboot to complete the process.

If the device is currently running a prerelease version of Windows, it will continue getting updates until the next public release is installed. At that time, we will opt out for you, without any action on your part. (Please note that depending on development timelines, this could take some time). We do this to ensure your device does not get stranded on an unsupported version of Windows that may contain security vulnerabilities.

If you do not want to wait for the next public release to opt out of Insider builds, you can [clean install Windows](https://support.microsoft.com/en-us/help/12415/windows-10-recovery-options) immediately. Please see instructions at [Download Windows 10](https://www.microsoft.com/en-us/software-download/windows10), or choose from the following, depending on which previous version you are recovering to: [Windows 7 Recovery Image](http://go.microsoft.com/fwlink/p/?LinkId=616947), [Windows 8 Recovery Image](http://go.microsoft.com/fwlink/p/?LinkId=616948), or [Windows 10 Recovery Image](http://go.microsoft.com/fwlink/p/?LinkId=616949).

## Leave the program

If you would like to stop receiving emails from the Windows Insider Program, you will need to leave the program. If you do want to leave the program, you’ll need to unregister. If you have updated your device's Settings to receive Windows 10 Insider Preview Builds, you will need to unenroll, and if you have installed Windows 10 Insider Preview Builds, you'll need to recover your device to a supported public Production Build.

If you would no longer like to receive Windows Insider builds on one or more of your devices you may do so and continue to receive emails from the program. If you do want to stop receiving Windows 10 Insider Preview Builds, you’ll need to unenroll and recover your device to a supported public Production Build.

### Unregister

On the Windows Insider Program website, sign in with your Microsoft Account (MSA) or your Azure Active Directory (AAD) account associated with the Windows Insider Program. [Sign in with your MSA or AAD.](https://insider.windows.com/en-us/insidersigninboth/)

Go to the page [leave the program](https://insider.windows.com/en-us/leave-program/) (visible in the footer of the site after you sign in,) and select **Leave the Program**. You'll then see a confirmation page.

### Unenroll
On your PC, go to **Settings** > **Update & Security** > **Windows Insider Program**, select **Stop Insider Preview Builds**, and follow the additional on-screen prompts.

### Recover your device

Follow the instructions in the [Stop receiving Insider builds section](https://review.docs.microsoft.com/en-us/windows-insider/at-home/troubleshooting?branch=pr-en-us-100#stop-receiving-insider-builds) above to return your PC to a previous version or reinstall.

## Support resources

Even though we know Insiders are self-sufficient, we're ready to help you use Windows 10 Insider Preview builds. Along with the information provided here and on our website, these options can also help you get support:

### Windows Insider Blog

With each new build, we publish a Windows Blog post that outlines key feature changes, as well as known issues that Insiders may encounter while using the build. Review the blog to stay up-to-date with news and information. [Read the Windows Insider Blog today.](https://blogs.windows.com/windowsexperience/tag/windows-insider-program)

### Feedback

Share feedback via the [Feedback Hub](insiderhub://home/). Other Insiders can add on to your feedback (and vice versa), and it will let you create links to feedback that you can share with others. [Learn more about providing feedback.](feedback.md)

### Forum

Insiders can filter between PC, Mobile, Office, Edge, and many other sections. There are also sub-topics that will help you narrow down your search to find tailored content. [Go to the Windows Insider forum.](https://answers.microsoft.com/en-us/insider?OCID=WIP_r_Welcome3_Body_InsidersForum)

### Twitter

We’re social! You’ll find new build announcements, tips and tricks, quests, contests, and direct real-time support. Follow us [@WindowsInsider](https://twitter.com/windowsinsider).
