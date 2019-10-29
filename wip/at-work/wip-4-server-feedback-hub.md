---
title: Share Feedback via the Feedback Hub
description: how to provide feedback for Windows Insider builds for Server.
author: lizap
manager: dougkim
ms.tgt_pltfrm: na
ms.devlang: na
ms.date: 10/25/2018
ms.author: elizapo
ms.localizationpriority: medium
ms.topic: article
ms.prod: w10
---

# Share Feedback on Windows Server via Feedback Hub
Sharing your feedback is quick and easy. Use your registered Windows Insider device and use the [Feedback Hub](feedback-hub:///) application. In the app, click the __Add Feedback__ button. Choose the __Windows Server__ category and then the appropriate subcategory for your feedback. In the title of the Feedback, please indicate the build number you are providing feedback on in this format:

[Server #####] Title of my feedback

Users can sign into the Feedback Hub using either their personal Microsoft Account (MSA) or Azure Active Directory (AAD) organizational account. Signing in with an AAD account allows users to submit feedback to Microsoft on behalf of their organization. Additionally, this feedback from Azure AD users can be tracked through the Feedback Hub other users in the organization.



## Submit feedback on behalf of your organization
1. Register as a Windows Insider with your work account in Azure Active Directory.
2. Sign into the Feedback Hub using this same work account. On the Welcome page of the Feedback Hub, click on the People icon, lower left and select or add your AAD work account. If you're signed in to the Feedback Hub App using your personal MSA, you can switch to your work account by clicking on your account, signing out and signing back in.

__Note:__ The Feedback Hub needs a user's consent to access their AAD account profile data (we read name, organizational tenant ID, and user ID). When users sign in for the first time with their AAD account, they will see a pop-up asking for permission. If a user cannot give consent in the pop-up, Feedback Hub may be blocked. Administrators can unblock in the [Azure portal](https://portal.azure.com/). Go to __Enterprise applications__ section and enable __Users can allow apps to access their data__. 

3. To submit feedback, go to the Feedback Hub and click on the __Feedback tab__ in the upper-left corner off the screen. For more information on submitting effective feedback, see: [How to provide effective feedback](https://insider.windows.com/en-us/how-to-feedback/).  

## Track feedback from users in your organization
4. To track feedback submitted to the Feedback Hub by other users in your organization, go to __Feedback>All Feedback__. Under the __Filter__ drop-down, select __My Organization__. 
__NOTE:__ You must sign in with your registered AAD account to track feedback from users in your organization. Feedback filtered with this view will only show feedback from users in your organization who sign into the Feedback Hub using their registered work account in AAD. 

![organizational feedback](images/wip-4-server-feedback.png "organizational feedback"). 

## Related topics
[Send feedback to Microsoft with the Feedback Hub app](https://support.microsoft.com/help/4021566/windows-10-send-feedback-to-microsoft-with-feedback-hub-app)