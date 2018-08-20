---
title: Share Feedback via the Feedback Hub
description: how to provide feedback for Windows Insider builds for enterprise client devices.
services: WIP-at-work-pro
author: dawnwood
manager: elizapo
ms.assetid: 
ms.service: WIP-at-work-pro
ms.tgt_pltfrm: na
ms.devlang: na
ms.date: 08/20/2018
ms.author: dawn.wood
ms.localizationpriority: medium
---

# Share Feedback via the Feedback Hub

Sharing your feedback is quick and easy. You can go directly to the [Feedback Hub](feedback-hub:///), then click the __Add Feedback__ button. You can track your feedback, and your IT administrator can track feedback provided by all users in the organization through the Feedback Hub by filtering by __My Organization__. 

If you're signed in to the Feedback Hub App using your personal Microsoft Account (MSA), you can switch to your work account by clicking on your account, signing out, and signing back in.

## User consent requirement
Feedback Hub needs your consent to access your AAD account profile data (we read name, organizational tenant ID, and user ID). When you sign in for the first time with the AAD account, you will see a popup asking for their permission. You must allow Feedback Hub to access your data in order to use it. 

In an enterprise environment, AAD administrators have the ability to allow or block users from giving consent. If you cannot give consent, Feedback Hub is blocked, your admin (or you if you're the admin) can unblock it by using the following steps.

1. Go to https://portal.azure.com/.
2. Switch to the Azure Active Directory dashboard using the __Azure Active Directory__ button. 
3. Switch to the appropriate directory using the __Switch Directory__ button.
4. Under the __Manage__ section, select User settings. 
5. In the __Enterprise applications__ section, enable __Users can allow apps to access their data__. 

![allow data access](images/waas-wipfb-aad-newenable.png "allow data access")

## Submit and track feedback on behalf of your organization
You can track feedback submitted to the Feedback Hub by you and others in your organization (AAD account registration required). Here’s how:

1. Register as a Windows Insider with your work account in Azure Active Directory.
2. Sign into the Feedback Hub using this same work account. On the Welcome page of the Feedback Hub, click on the People icon, lower left and select or add your AAD work account. (If you have already registered using your Microsoft account, you’ll need to sign out first.)
3. Go to __Feedback, All Feedback__.
4. Under the __Filterx__ drop-down, select __My Organization__ to view feedback from Insiders in your organization. Note: Feedback filtered with this view will only show Feedback from users in your organization who sign into the Feedback Hub using their registered work account in Azure Active Directory. 

![organizational feedback](images/WIP_feedback_WIP-B.png "organizational feedback")

## Related topics
[Send feedback to Microsoft with the Feedback Hub app](https://support.microsoft.com/en-us/help/4021566/windows-10-send-feedback-to-microsoft-with-feedback-hub-app)

