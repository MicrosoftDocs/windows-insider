---
title: What's new in the Windows Server 10 Insider Program for Business Preview Builds
description: New features to use and test in the Windows 10 Insider Program for Business Preview Builds
services: WIP-at-work-pro
author: dawn.wood
manager: elizapo
ms.service: WIP-at-work-pro
ms.date: 07/12/2018
ms.author: dawn.wood
---

# What’s New in Windows 10 Insider Program for Business Preview Builds 

## Power scheme for pro for workstations 

<b>A new power scheme – Ultimate Performance</b>: Demanding workloads on workstations always desire more performance. As part of our effort to provide the absolute maximum performance we’re introducing a new power policy called Ultimate Performance. Windows has developed key areas where performance and efficiency tradeoffs are made in the OS. Over time, we’ve amassed a collection of settings which allow the OS to quickly tune the behavior based on user preference, policy, underlying hardware or workload.
This new policy builds on the current High-Performance policy, and it goes a step further to eliminate micro-latencies associated with fine grained power management techniques. The Ultimate Performance Power plan is selectable either by an OEM on new systems or selectable by a user. To do so, you can go to Control Panel and navigate to Power Options under Hardware and Sound (you can also “run” Powercfg.cpl). Just like other power policies in Windows, the contents of the Ultimate Performance policy can be customized.

![alt text](images/ultimate-power-scheme.png "Ultimate power scheme")

As the power scheme is geared towards reducing micro-latencies it may directly impact hardware; and consume more power than the default balanced plan. The Ultimate Performance power policy is currently not available on battery powered systems.

<b>Productivity focused out of box applications</b>: The out of box experience for Windows 10 Pro for Workstations display  productivity and enterprise focused applications in place of consumer applications and games. 

![alt text](images/productivity_apps.png "productivity apps")

## Remote Desktop with Biometrics
We’re happy to share that with this build of Windows 10, Azure Active Directory and Active Directory users using Windows Hello for Business can use biometrics to authenticate to a remote desktop session!

![Enter your credentials](images/RDPwBioTime.png "Windows Hello")

To get started, bring up Remote Desktop Connection (mstsc.exe), type the name of the computer to which you want to connect and tap or click <b>Connect</b>.

Because you signed using Windows Hello for Business, Windows remembers how you signed in and automatically selects Windows Hello for Business to authenticate you to your RDP session but, you can click <b>More choices</b> to choose alternate credentials.

![Enter your credentials](images/RDPwBio2.png "Windows Hello personal")

In this example, Windows uses facial recognition to authenticate the RDP session to the Windows Server 2016 Hyper-V server. You can continue to use Windows Hello for Business in the remote session, but you must use your PIN.

![Microsoft Hyper-V Server 2016](images/hyper-v.png "Microsoft Hyper-V Server 2016")


## Registry editor improvements

Have you ever been typing into the regedit address bar, and the next part of the path is just on the tip of your tongue, but you can’t remember? Starting with build 17711, you’ll see a dropdown as you type to help complete the next part of the path. You can also press Ctrl + Backspace to delete the last "word," which makes backing up work that much faster (Ctrl + Delete will delete the next word).

![Registry editor dropdown](images/regeditor.png "Registry editor dropdown")

## Security updates

We’ve continued to work on the **Current threats** area in  [Virus & threat protection](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-security-center/wdsc-virus-threat-protection), which now displays all threats that need action. You can quickly take action on threats straight from this screen: 

![Virus & threat protection settings](images/virus-and-threat-protection.png "Virus & threat protection settings")

You can enable a new protection setting, **Block suspicious behaviors**, which brings [Windows Defender Exploit Guard attack surface reduction technology](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-exploit-guard/attack-surface-reduction-exploit-guard) to all users. To enable this setting, go to the Virus & threat protection section and click **Manage settings**, as shown in the following screenshot:

![Block suspicious behaviors](images/block-suspicious-behaviors.png "Block suspicious behaviors")

With Controlled folder access you can help prevent ransomware and other destructive malware from changing your personal files. In some cases, apps that you normally use might be blocked from making changes to common folders like Documents and Pictures. We’ve made it easier for you to add apps that were recently blocked so you can keep using your device without turning off the feature altogether.

When an app is blocked, it will appear in a recently blocked apps list, which you can get to by clicking **Manage settings** under the **Ransomware protection** heading, and then **Allow an app through Controlled folder access**. After the prompt, click the plus button and choose **Recently blocked apps**. Select any of the apps to add them to the allowed list. You can also browse for an app from this page as well.

We've added a new assessment for the Windows time service to the **Device performance & health** section. If we detect that your device’s time is not properly synced with our time servers and the time-syncing service is disabled, we’ll provide the option for you to turn it back on.

We’re continuing to work on how other security apps you’ve installed show up in the Windows Security app. There’s a new page called **Security providers** that you can find in the Settings section of the app. Click **Manage providers** to see a list of all the other security providers (including antivirus, firewall, and web protection) that are running on your device. Here you can easily open the providers’ apps, or get more information on how to resolve any issue that they have reported to you through the Windows Security app.

This also means you’ll see more links to other security apps within the Windows Security app. For example, if you open the **Firewall & network protection** section, you’ll see the firewall apps that are running on your device under each firewall type (domain, private, and public networks).

## Web sign-in to Windows 10
Until now, Windows logon only supported the use of identities federated to ADFS or other providers that support the WS-Fed protocol. We are introducing “Web Sign-in,” a new way of signing into your Windows PC. Web Sign-in enables Windows logon support for non-ADFS federated providers(e.g.SAML).

![Web sign-in](images/websignin.png "web sign-in")

### To try out web sign-in:
1. Azure AD Join your Windows 10 PC. (Web Sign-in is only supported on Azure AD Joined PCs).
2. Set the Policy CSP/Authentication/EnableWebSignIn policy to enable Web Sign-in. 
3. On the lock screen, select Web Sign-in under Sign-in options.
4. Click the “Sign in” button to continue.

## Faster sign-in to a Windows 10 shared pc
Do you have shared PCs deployed in your work place? Introducing “Fast Sign-in,” which enables users to sign in to a shared Windows 10 PC in a flash!
![Web sign-in](images/fastsignin.png "web sign-in")

To enable Fast Sign in,
1. Set up a shared or guest PC with Windows 10
2. Set Policy/Authentication/EnableFastFirstSignIn to enable fast sign-in
3. With the policy enabled, sign-in to a shared PC with your account and notice the difference!

## Windows Defender Application Guard Improvements 
Windows Defender Application Guard introduced a new user interface inside Windows Security in this release. Standalone users can now install and configure their Windows Defender Application Guard settings in Windows Security without needing to change Registry key settings. Additionally, users who are managed by enterprise policies will be able to check their settings to see what their administrators have configured for their machines to better understand the behavior of Windows Defender Application Guard. This new UI aims to improve the overall experience for users to manage and check their Windows Defender Application Guard settings. As long as devices meet the minimum requirements, these settings will appear in Windows Security.
