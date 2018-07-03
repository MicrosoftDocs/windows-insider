---
title: Share Feedback via the Feedback Hub
description: how to provide feedback for Windows Insider builds for enterprise client devices.
services: WIP-at-work-pro
author: dawn.wood
manager: elizapo
ms.assetid: 
ms.service: WIP-at-work-pro
ms.tgt_pltfrm: na
ms.devlang: na
ms.date: 06/28/2018
ms.author: dawn.wood
---

# Share Feedback via the Feedback Hub

Sharing your feedback is quick and easy. You can go directly to the [Feedback Hub](feedback-hub:///), then click the <b>Add Feedback</b> button. You can track your feedback, and your IT administrator can track feedback provided by all users in the organization through the Feedback Hub by filtering by <b>My Organization</b>. 

If you're signed in to the Feedback Hub App using your personal Microsoft Account (MSA), you can switch to your work account by clicking on your account, signing out, and signing back in.

## User consent requirement
Feedback Hub needs your consent to access your AAD account profile data (we read name, organizational tenant ID, and user ID). When you sign in for the first time with the AAD account, you will see a popup asking for their permission. You must allow Feedback Hub to access your data in order to use it. 

In an enterprise environment, AAD administrators have the ability to allow or block users from giving consent. If you cannot give consent, Feedback Hub is blocked, your admin (or you if you're the admin) can unblock it by using the following steps.

1. Go to https://portal.azure.com/.
2. Switch to the Azure Active Directory dashboard using the <b>Azure Active Directory</b> button. 
3. Switch to the appropriate directory using the <b>Switch Directory</b> button.
4. Under the <b>Manage</b> section, select User settings. 
5. In the <b>Enterprise applications</b> section, enable <b>Users can allow apps to access their data</b>. ![alt text](images/waas-wipfb-aad-newenable.png "allow data access")

## Related topics
[Send feedback to Microsoft with the Feedback Hub app](https://support.microsoft.com/en-us/help/4021566/windows-10-send-feedback-to-microsoft-with-feedback-hub-app)

