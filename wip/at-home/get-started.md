---
title: Getting started with Windows 10 Insider Preview Builds
description: How to install Insider Preview builds 
manager: eliotgra
ms.tgt_pltfrm: na
ms.devlang: na
ms.date: 10/24/2018
ms.author: v-colinmit
author: cdmm12
ms.localizationpriority: medium
ms.topic: article
ms.prod: w10
---

# Getting started with Windows 10 Insider Preview Builds 

To install a Windows 10 Insider Preview Build on an individual PC, follow the steps below. 

## Prerequisites
1. __Register as a Windows Insider.__ You can register on the [Windows Insider Program website](https://insider.windows.com/en-us/register/), or in Windows Insider settings on your PC. To register, use your Microsoft account or an Azure Active Directory work account. For the benefits of using a work account, see [Register for the Windows Insider Program for Business](https://docs.microsoft.com/windows-insider/at-work-pro/wip-4-biz-register). 
2. __Install Windows 10 on your PC.__ To install Windows 10 Insider Preview, you’ll need to be running a licensed version of Windows 10 on your PC. If your PC is currently running Windows 7/8/8.1, you can [install Windows 10 here](https://www.microsoft.com/en-us/windows/get-windows-10?step=Win10Question1). If you are having problems installing Windows 10, you can  [download Windows 10 Insider Preview ISO](https://www.microsoft.com/en-us/software-download/windowsinsiderpreviewadvanced).
3. __Check diagnostic settings.__ Diagnostic data settings must be set to Enhanced or Full to receive Insider Preview builds. To check and change settings, go to **Settings** > **Privacy** > **Diagnostics & feedback**. For more information see [Diagnostics, feedback and privacy in Windows 10](https://support.microsoft.com/en-us/help/4468236/diagnostics-feedback-and-privacy-in-windows-10-microsoft-privacy). 
4. __Check language support.__ Confirm that Windows 10 Insider Preview Builds support your desired language on your PC. See __Supported Languages__ below.

## Configure Windows Insider Program settings 
The following steps apply to PCs running Windows 10, Version 1809. Steps will vary slightly for earlier versions of Windows. To see these settings, you must have administrator rights to the machine. 
1. Open [Windows Insider Program Settings](ms-settings:windowsinsider) (**Start** > **Settings** > **Update & Security** > **Windows Insider Program**). 
2. Select __Get started__.
3. Under **Pick an account to get started** select **+** to link your Microsoft or work account that you used to register for the Windows Insider Program. Choose __Continue__ or, if you have not already registered for the Windows Insider Program, select __Register__. 
4. Under **What kind of content that you would like to receive**, select __Active development of Windows__ to receive Insider Preview builds and click __Confirm__. (Select **Just fixes, apps and drivers** only if you want to install builds from the [Release Preview ring](https://docs.microsoft.com/windows-insider/at-home/rings#release-preview-ring). Select **Skip ahead to the next Windows release** if you want to install build from the next release cycle. 
5. Under “What pace do you want to receive preview builds” select __Fast__ if you would like to receive the latest Insider Preview builds. If you prefer to wait for a more stable build, select __Slow__. Choose __Confirm__.

> [!NOTE] 
> The Fast ring may contain bugs and other issues. If you prefer to wait for a more stable build, select Slow. For more information, see [Working with rings and updates](rings.md)
> If you are in the Fast ring and your PC gets updated to the next release cycle (20H1), and you want to switch to the Slow or Release Preview rings, you will need to do a clean install of Windows on your PC and reset your Windows Insider Program settings.
> If the option to **Skip ahead to the next version of Windows** is not available, selecting it will default to the latest Insider Preview build in the Fast ring.

6. Review the privacy statement and program terms and select __Confirm__.
7. Select **Restart Now** or **Restart Later** to activate Windows Insider Program settings. 

## Complete and confirm installation
1.	Once your PC restarts, go to [Windows Update](ms-settings:windowsupdate) (**Start** > **Settings** > **Update & Security** > **Windows Update**) and select __Check for updates__ to download the latest Insider Preview build based on the criteria you selected in the steps above.
2.	Once the download is complete, select one of the three restart options. Select **Pick a time**, **Remind me later**, or **Restart now** to complete installation.
3.	To confirm installation of the latest Insider Preview build, type __Winver__ in the Windows search bar and run the command to get the build number of the Windows version currently running on your PC. Compare this against the latest build available as listed in [Flight Hub](https://docs.microsoft.com/windows-insider/flight-hub/). 

> [!NOTE] 
> Your devices will be automatically updated to the latest Insider Preview builds using Windows Update. See [Windows Update guidance](https://support.microsoft.com/en-us/help/4027667/windows-10-update). 
> If you're unable to install an Insider Preview build or encounter other technical related issues, see [Troubleshooting](troubleshooting.md). 

## Let us know what you think
Once you have installed an Insider Preview build, you can provide feedback on the build using the [Feedback Hub](insiderhub://home/) in Windows. Your feedback can help us fix issues and target new features and improvements. [Learn more about providing feedback.](feedback.md)

## Supported languages
Windows 10 Insider Preview Builds are available in the following SKU languages:
Arabic (Saudi Arabia), Bulgarian (Bulgaria), Chinese (Simplified, China), Chinese (Traditional, Taiwan), Croatian (Croatia), Czech (Czech Republic), Danish (Denmark), Dutch (Netherlands), English (United Kingdom), English (United States), Estonian (Estonia), Finnish (Finland), French (Canada), French (France), German (Germany), Greek (Greece), Hebrew (Israel), Hungarian (Hungary), Italian (Italy), Japanese (Japan), Korean (Korea), Latvian (Latvia), Lithuanian (Lithuania), Norwegian, Bokmål (Norway), Polish (Poland), Portuguese (Brazil), Portuguese (Portugal), Romanian (Romania), Russian (Russia), Serbian (Latin, Serbia), Slovak (Slovakia), Slovenian (Slovenia), Spanish (Mexico), Spanish (Spain, International Sort), Swedish (Sweden), Thai (Thailand), Turkish (Turkey), Ukrainian (Ukraine).

Windows 10 Insider Preview is available in the following Language Interface Packs (LIP) languages:
Afrikaans (South Africa), Albanian (Albania), Amharic, Armenian, Assamese, Azerbaijani (Latin, Azerbaijan), Bangla (Bangladesh), Bangla (India), Basque, Belarusian (Belarus), Bosnian (Latin), Catalan (Catalan), Cherokee (Cherokee), Dari, Filipino (Philippines), Galician (Galician), Georgian, Gujarati, Hindi (India), Icelandic, Indonesian (Indonesia), Irish, Kannada, Kazakh (Kazakhstan), Khmer (Cambodia), KiSwahili, Konkani, Kyrgyz, Lao (Laos), Luxembourgish, Macedonian (Former Yugoslav Republic of Macedonia), Malay (Malaysia), Malayalam, Maltese, Maori, Marathi, Mongolian (Cyrillic), Nepali, Norwegian (Nynorsk), Odia, Persian, Punjabi, Quechua, Scottish Gaelic, Serbian (Cyrillic, Bosnia and Herzegovina), Serbian (Cyrillic, Serbia), Sindhi (Arabic), Sinhala, Tamil (India), Tatar, Telugu, Turkmen, Urdu, Uyghur, Uzbek (Latin, Uzbekistan), Valencian, Vietnamese, Welsh.

LIP languages can be installed as a language pack over [supported base languages](https://support.microsoft.com/en-us/help/14236/language-packs).




