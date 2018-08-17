---
title: Install Windows 10 preview builds
description: how to install Windows Insider builds for enterprise client devices
services: WIP-at-work-pro
author: dawn.wood
manager: elizapo
ms.assetid: 
ms.service: WIP-at-work-pro
ms.tgt_pltfrm: na
ms.devlang: na
ms.date: 06/28/2018
ms.author: dawn.wood
ms.localizationpriority: medium
---



# Install Windows Insider for Business Preview builds
The Windows Insider for Business allows you to install preview enterprise client editions of the next version of Windows. You can install Windows 10 Insider Preview builds on individual devices, manage installation across multiple devices in an organization, or install on a virtual machine. 

## Install on an individual device
Getting set up on a single device is easy. 
1. Open Windows Insider Program settings. You can find the settings by going to <b>Start > Settings > Update & security > Windows Insider Program</b>. To see this setting, you must have administrator rights to your device.
2. Click <b>Get started</b> and follow the prompts to link your Microsoft or work account that you used to register as a Windows Insider. 

![alt text](images/wip4biz_prompts.png "Get started button for installing WIP builds")

3. Sign-in using the account you used to register for the Windows Insider Program <b>Next</b>.
4. Under “What kind of content that you would like to receive”, select <b>active development of Windows</b> to receive Windows 10 Insider Preview builds and click <b>Confirm</b>. Select “Fixes, apps and drivers” if you want to install builds from the Release Preview Ring. 
5. Under “What pace do you want to receive preview builds” select <b>Fast</b> if you would like to receive the latest Insider Preview builds. Note that this ring may contain bugs and other issues. If you prefer to wait for a more stable build, select <b>Slow</b> . Click <b>Confirm</b>. See [Windows readiness levels and flight rings](wip-4-biz-flight-levels-and-rings.md) for more information about each choice. 
6. Review the privacy statement and click <b>Continue</b>
7. Reboot the device. 
8. Go to <b>Start > Settings > Update & Security > Windows Update</b>, and click Check for updates to download the latest Insider Preview build based on the criteria you selected.
9. Once the download is complete, reboot your device again. 
10. The Windows 10 Insider Preview build is on your device. 

<b>NOTE:</b> If the user's device is not already Azure AD joined, the user needs to add an Azure AD or Microsoft account to the machine manually. Otherwise, Windows Insider Preview builds will not be installed.

## Install across multiple devices in a domain 
Administrators can install and manage Insider Preview builds centrally across devices in their domain. To register a domain, you must be registered in the Windows Insider Program with your work account in Azure Active Directory and you have to be a Global Administrator role on that AAD domain. This feature is available on Windows 10 Version 1703 or later. 

For instructions, see [Manage Windows Insider Preview builds](wip-4-biz-manage-builds.md).

## Install on a virtual machine
There isn't anything special you have to do to run Windows 10 Insider Preview builds on a virtual machine. Once you have a virtual machine set up, you install just as you would on an individual device. If you need help setting up a virtual machine, see [Introduction to Hyper-V on Windows 10](https://docs.microsoft.com/virtualization/hyper-v-on-windows/about/).

## Supported languages
Windows 10 Insider Preview is available in the following SKU languages:
Arabic (Saudi Arabia), Bulgarian (Bulgaria), Chinese (Simplified, China), Chinese (Traditional, Taiwan), Croatian (Croatia), Czech (Czech Republic), Danish (Denmark), Dutch (Netherlands), English (United Kingdom), English (United States), Estonian (Estonia), Finnish (Finland), French (Canada), French (France), German (Germany), Greek (Greece), Hebrew (Israel), Hungarian (Hungary), Italian (Italy), Japanese (Japan), Korean (Korea), Latvian (Latvia), Lithuanian (Lithuania), Norwegian, Bokmål (Norway), Polish (Poland), Portuguese (Brazil), Portuguese (Portugal), Romanian (Romania), Russian (Russia), Serbian (Latin, Serbia), Slovak (Slovakia), Slovenian (Slovenia), Spanish (Mexico), Spanish (Spain, International Sort), Swedish (Sweden), Thai (Thailand), Turkish (Turkey), Ukrainian (Ukraine).

Windows 10 Insider Preview is available in the following Language Interface Packs (LIP) languages:
Afrikaans (South Africa), Albanian (Albania), Amharic, Armenian, Assamese, Azerbaijani (Latin, Azerbaijan), Bangla (Bangladesh), Bangla (India), Basque, Belarusian (Belarus), Bosnian (Latin), Catalan (Catalan), Cherokee (Cherokee), Dari, Filipino (Philippines), Galician (Galician), Georgian, Gujarati, Hindi (India), Icelandic, Indonesian (Indonesia), Irish, Kannada, Kazakh (Kazakhstan), Khmer (Cambodia), KiSwahili, Konkani, Kyrgyz, Lao (Laos), Luxembourgish, Macedonian (Former Yugoslav Republic of Macedonia), Malay (Malaysia), Malayalam, Maltese, Maori, Marathi, Mongolian (Cyrillic), Nepali, Norwegian (Nynorsk), Odia, Persian, Punjabi, Quechua, Scottish Gaelic, Serbian (Cyrillic, Bosnia and Herzegovina), Serbian (Cyrillic, Serbia), Sindhi (Arabic), Sinhala, Tamil (India), Tatar, Telugu, Turkmen, Urdu, Uyghur, Uzbek (Latin, Uzbekistan), Valencian, Vietnamese, Welsh.

LIP languages can be installed as a language pack over [supported base languages](https://support.microsoft.com/en-us/help/14236/language-packs).

## Related topics

* [Register for the Windows Insider Program for Business](wip-4-biz-register.md)
* [Share Feedback via the Feedback Hub](wip-4-biz-feedback-hub.md)
