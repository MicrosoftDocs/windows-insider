---
title: Install Windows 10 preview builds
description: how to install Windows Insider builds for enterprise client devices
services: WIP-at-work-pro
author: lizap
manager: dougkim
ms.assetid: 
ms.service: WIP-at-work-pro
ms.tgt_pltfrm: na
ms.devlang: na
ms.date: 06/28/2018
ms.author: elizapo
ms.localizationpriority: medium
---

# Install Windows 10 Insider Preview Builds
You can install Insider Preview builds on individual devices, manage installation across multiple devices in an organization, or install on a virtual machine. 

NOTE: A device must be running a licensed version of Windows 10 to update to an Insider Preview build. 

## Install on an individual device 
1. Register as a Windows Insider if you haven't done so already. See [Register](wip-4-biz-register.md). 
2. Open Windows Insider Program settings. You can find the settings by going to __Start > Settings > Update & security > Windows Insider Program__. To see this setting, you must have administrator rights to your device.
3. Click __Get started__ and follow the prompts to link your Microsoft or work account that you used to register as a Windows Insider. 

![alt text](images/wip4biz_prompts.png "Get started button for installing WIP builds")

4. Sign-in using the account you used to register for the Windows Insider Program.  
5. Under “What kind of content that you would like to receive”, select __active development of Windows__ to receive Insider Preview builds and click __Confirm__. Select “Fixes, apps and drivers” if you want to install builds from the Release Preview Ring. 
6. Under “What pace do you want to receive preview builds” select __Fast__ if you would like to receive the latest Insider Preview builds. If you prefer to wait for a more stable build, select __Slow__. Click __Confirm__. 
7. Review the privacy statement and click __Continue__.
8. Reboot the device. 
9. To immediately download the latest Insider Preview build based on the criteria you selected, go to __Start > Settings > Update & Security > Windows Update__, and click __Check for updates__ 
10. Once the download is complete, reboot your device again to complete installation. 

## Install across multiple devices 
Administrators can install and manage Insider Preview builds centrally across multiple devices in their organizational domain using Group Policies or MDM Policies. This option requires an Azure AD domain which must be registered in the Windows Insider Program. For instructions, see [Manage Windows Insider Preview builds](wip-4-biz-manage.md).

## Install on a virtual machine
You can run Insider Preview builds as a virtual machine in Hyper-V. This option enables you to run Insider Preview builds without changing the Windows 10 production build already running on a PC.
* For guidance on setting up virtual machines on your PC see: [Introduction to Hyper-V on Windows 10](https://docs.microsoft.com/virtualization/hyper-v-on-windows/about/).
* To download the latest Insider Preview build ISO file to run on your virtual machine see: [Windows Insider Preview downloads](https://www.microsoft.com/en-us/software-download/windowsinsiderpreviewadvanced).

## Once you have completed installation
These tips will help you and your organization get the most out of Insider Preview builds and the Windows Insider Program for Business. 
* __Check to ensure you have the latest build version.__ Once you have installed an Insider Preview build, the version number will appear in a watermark on the lower right corner of your desktop. You can also confirm the Insider Preview build version installed by going to Settings>About your PC and scrolling to "Windows Specifications". To confirm that you have the latest Insider Preview build version, check our [Flight Hub](https://docs.microsoft.com/en-us/windows-insider/flight-hub/).  
* __Follow our Windows Insider Program blog.__ As soon as an Insider Preview build is released, we publish a blog with details on feature highlights and fixes. [See the latest blog](https://blogs.windows.com/windowsexperience/tag/windows-insider-program/#ft9PuorWX0ODx38J.97)
* __Provide us with feedback.__ To help us shape Windows to address your organization's specific needs, submit feedback on Insider Preview builds directly to the Feedback Hub in Windows. [Check guidance for submitting effective feedback](wip-4-biz-feedback-hub.md). 
* __Use Insider Preview builds to accelerate your next Windows deployment.__ Validating your apps and infrastructure on Insider Preview builds can play an important role in your Windows 10 deployment strategy. You can also use Windows Anlytics to monitor device health and issues. See [Validation guidance](https://insider.windows.com/en-us/for-business-getting-started/#validate). 
* __Join our community__. Join our [Windows Insider Tech Community](https://techcommunity.microsoft.com/t5/Windows-Insider-Program/bd-p/WindowsInsiderProgram) to share and learn from other IT experts.

## Supported languages
Windows 10 Insider Preview Builds are available in the following SKU languages:
Arabic (Saudi Arabia), Bulgarian (Bulgaria), Chinese (Simplified, China), Chinese (Traditional, Taiwan), Croatian (Croatia), Czech (Czech Republic), Danish (Denmark), Dutch (Netherlands), English (United Kingdom), English (United States), Estonian (Estonia), Finnish (Finland), French (Canada), French (France), German (Germany), Greek (Greece), Hebrew (Israel), Hungarian (Hungary), Italian (Italy), Japanese (Japan), Korean (Korea), Latvian (Latvia), Lithuanian (Lithuania), Norwegian, Bokmål (Norway), Polish (Poland), Portuguese (Brazil), Portuguese (Portugal), Romanian (Romania), Russian (Russia), Serbian (Latin, Serbia), Slovak (Slovakia), Slovenian (Slovenia), Spanish (Mexico), Spanish (Spain, International Sort), Swedish (Sweden), Thai (Thailand), Turkish (Turkey), Ukrainian (Ukraine).

Windows 10 Insider Preview is available in the following Language Interface Packs (LIP) languages:
Afrikaans (South Africa), Albanian (Albania), Amharic, Armenian, Assamese, Azerbaijani (Latin, Azerbaijan), Bangla (Bangladesh), Bangla (India), Basque, Belarusian (Belarus), Bosnian (Latin), Catalan (Catalan), Cherokee (Cherokee), Dari, Filipino (Philippines), Galician (Galician), Georgian, Gujarati, Hindi (India), Icelandic, Indonesian (Indonesia), Irish, Kannada, Kazakh (Kazakhstan), Khmer (Cambodia), KiSwahili, Konkani, Kyrgyz, Lao (Laos), Luxembourgish, Macedonian (Former Yugoslav Republic of Macedonia), Malay (Malaysia), Malayalam, Maltese, Maori, Marathi, Mongolian (Cyrillic), Nepali, Norwegian (Nynorsk), Odia, Persian, Punjabi, Quechua, Scottish Gaelic, Serbian (Cyrillic, Bosnia and Herzegovina), Serbian (Cyrillic, Serbia), Sindhi (Arabic), Sinhala, Tamil (India), Tatar, Telugu, Turkmen, Urdu, Uyghur, Uzbek (Latin, Uzbekistan), Valencian, Vietnamese, Welsh.

LIP languages can be installed as a language pack over [supported base languages](https://support.microsoft.com/en-us/help/14236/language-packs).

## Related topics

* [Register for the Windows Insider Program for Business](wip-4-biz-register.md)
* [Share Feedback via the Feedback Hub](wip-4-biz-feedback-hub.md)
