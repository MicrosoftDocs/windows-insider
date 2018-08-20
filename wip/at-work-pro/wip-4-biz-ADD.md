---
title: Windows Insider Program for Business using Azure Active Directory
description: how to use AAD using Windows Insider builds for business
services: WIP-at-work-pro
author: dawnwood
manager: elizapo
ms.assetid: 
ms.service: WIP-at-work-pro
ms.tgt_pltfrm: na
ms.devlang: na
ms.date: 7/25/2018
ms.author: dawnwood
ms.localizationpriority: medium
---

# Windows Insider Program for Business using Azure Active Directory

You can download Windows 10 Insider Preview builds using your corporate credentials in Azure Active Directory (AAD). By enrolling devices in AAD, you increase the visibility of feedback submitted by users in your organization – especially on features that support your specific business needs. 

__Note__: The Windows Insider Program for Business only supports Azure Active Directory (and not Active Directory on premises) as a corporate authentication method.

If your company is currently not using AAD – but has a paid subscription to Office 365, Microsoft Dynamics CRM Online, Enterprise Mobility Suite, or other Microsoft services – you have a free subscription to Microsoft Azure Active Directory. This subscription can be used to create users for enrollment in the Windows Insider Program for Business.

In order to get the most benefit out of the Windows Insider Program for Business, organizations should not use a test tenant of AAD. There will be no modifications to the AAD tenant to support the Windows Insider Program as it will only be used as an authentication method.

## Register your organization's Azure AD domain to the Windows Insider Program for Business

Rather than have each user in your organization register for Windows 10 Insider Preview builds, you can now simply register your domain – and cover all users with just one registration.

__Important__ You need to be signed in as a Global Administrator of the Azure AD domain in order to be able to register the domain.

1. On the [Windows Insider website](https://insider.windows.com/), go to__For Business__ >__Getting Started__ to [register your organizational Azure AD account](https://insider.windows.com/en-us/insidersigninaad/).
2. [Register your domain](https://insider.windows.com/en-us/for-business-organization-admin/) and control settings centrally.

## Is your device connected to your company’s AAD subscription?

Go to__Settings > Accounts > Access work or school__. If a corporate account is on Azure Active Directory and it is connected to the device, you will see the account listed as highlighted in the image below.

![ADD subscription](images/wip-4-biz-settings.png "ADD")

## Enroll a device with an AAD account

1. Make sure that you have administrator rights to the machine and that it has latest Windows updates.
2. Navigate to the [Getting Started](https://insider.windows.com/en-us/getting-started/) page on [insider.windows.com](https://insider.windows.com/).
3. Go to__Register your organization account__ and follow the instructions.
4. On your Windows 10 device, go to__Settings > Updates & Security > Windows Insider Program__. 
5. Enter the AAD account that you used to register and follow the on-screen directions. 

## Switch device enrollment from your Microsoft account to your AAD account

1. Visit [insider.windows.com](http://insider.windows.com) to register your AAD account. If you are signed in with your Microsoft account, sign out, then sign back in with your corporate AAD account. 
2. Click__Get started__, read and accept the privacy statement and program terms and click__Submit__. 
3. On your Windows 10 PC, go to__Settings > Updates & Security > Windows Insider Program__. 
4. Under__Windows Insider account__, click your Microsoft account, then__Change__ to open a Sign In box. 
5. Select your corporate account and click__Continue__ to change your account. 

![ADD change user](images/wip-4-biz-change-user.png "change user")

## User consent for Feedback Hub

With the current version of the Feedback Hub app, we need the user's consent to access their AAD account profile data (We read their name, organizational tenant ID and user ID). When they sign in for the first time with the AAD account, they will see a popup asking for their permission, like this:

![ADD user consent](images/wip-4-biz-aad-consent.png "user consent")

Once agreed, everything will work fine, and that user won't be prompted for permission again.

### Something went wrong error

The option for users to give consent for apps to access their profile data is controlled through Azure Active Directory. This means the AAD administrators have the ability to allow or block users from giving consent.

In case the administrators blocked this option, when the user signs in with the AAD account, they will see the following error message:

![something went wrong](images/wip-4-biz-aad-consent.png "something went wrong")

This blocks the user from signing in, which means they won't be able to use the Feedback Hub app with their AAD credentials.

To fix this issue, an administrator of the AAD directory will need to enable user consent for apps to access their data.

To do this through the classic Azure portal:
1. Go to https://manage.windowsazure.com/ .
2. Switch to the Active Directory dashboard.

![AAD dashboard](images/wip-4-biz-classic-aad.png "AAD dashboard")

3. Select the appropriate directory and go to the__Configure__ tab.
4. Under the__integrated applications__ section, enable__Users may give applications permissions to access their data__.

![enable applications](images/wip-4-biz-aad-classic-enable.png "enable applications")

To do this through the new Azure portal:
1. Go to [https://portal.azure.com/](https://portal.azure.com/)
2. Switch to the Active Directory dashboard.

![new ADD dashboard](images/wip-4-biz-new-aad.png "new ADD dashboard")

3. Switch to the appropriate directory.

![new directory](images/wip-4-biz-aad-new-directory-button.png "new directory")

4. Under the Manage section, select User settings.

![user settings](images/wip-4-biz-aad-new-user-settings.png "user settings")

5. In the Enterprise applications section, enable Users can allow apps to access their data.
![enable users](images/wip-4-biz-aad-new-enable.png "enable users")

## Stop receiving updates
You can “unlink” your account by going to__Settings > Updates & Security > Windows Insider Program__, select__Windows Insider Account__ and click__Unlink__.

## New to Azure Active Directory? 

 Try these topics to learn more about Azure Active Directory (AAD).
 1. [Introduction to AAD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)
 2. [Add users](https://docs.microsoft.com/azure/active-directory/active-directory-users-create-azure-portal)
 3. [Device registration](https://docs.microsoft.com/azure/active-directory/active-directory-device-registration-overview) 
 4. [Integrate your on-premises directories with Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)


