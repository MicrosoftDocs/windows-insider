---
title: Providing feedback
description: How to provide constructive feedback
manager: eliotgra
ms.tgt_pltfrm: na
ms.devlang: na
ms.date: 10/1/19
ms.author: arshields7
author: cdmm12
ms.localizationpriority: medium
ms.topic: article
ms.prod: w10
---

# Providing feedback

One of the benefits of being a Windows Insider is knowing that your feedback can change and improve Windows for users around the world. The more detailed your feedback is, the more effectively our engineering teams can identify and respond to it.

To provide feedback, visit the [Feedback Hub](http://insiderhub://home/) app, which you can find in your **Start menu**. The tips below can help you make the most of the Feedback Hub. You can also use the [Language Community App](https://docs.microsoft.com/en-us/windows-insider/at-home/troubleshooting#support-resources) to help us make Windows better in your language (PC only).

There are two types of feedback, problems and suggestions. If something is broken, you're getting errors, or something is missing, you should file a problem. If there's a new feature or change you'd like to see, you should file a suggestion.

## Checking for existing feedback

Before logging a new piece of feedback, check to see if someone else has already reported that issue or requested that change by. 

When searching for a problem, you can choose to either add a comment to an existing problem or add your own piece of similar feedback. When adding your own similar piece of feedback, it will ask you to provide additional details, which can better help engineers define the problem and its scope. 

If you're searching for a suggestion and find that someone has already suggested it, you should upvote the existing feedback item instead of recreating the suggestion. You can also add comments to their suggestion to provide more information or add situations for review.

### Searching for existing feedback

To search for existing feedback, use the search bar on the main page of the Feedback Hub or in the Feedback section, and begin narrowing down your search by typing in keywords, (like Task View, Magnifier, etc.) to see a list of existing collections and feedback items. 

From there, you can narrow down your search to see if yours already exists. Select the link next to “Filters” at the top of the Feedback section to filter between problems and suggestions, to find feedback that’s already been addressed or needs more information, or to see feedback where someone from Microsoft has already posted a response. 

You can also filter different categories and subcategories of feedback by selecting the link next to Categories. 

If you don't find existing feedback, it's time to add new feedback.

![Feedback Hub's filters that let you search for existing feedback](images/FeedbackHubHome.png "Feedback Hub filters")

*The Feedback Hub lets you filter feedback based on a variety of criteria.*

### Looking for collections

You should also look for collections in your results. Collections gather together similar feedback and were created based on users identifying duplicate feedback items in the Feedback Hub. Collections are identified with an icon next to their title, so you can easily tell them apart from individual feedback. The upvote count you see on a collection includes all the upvotes represented in the duplicate feedback items that have been added to the collection. The title of a collection describes how we've understood the sentiment of the collection. Share your thoughts in a joint comment thread. [Learn more about collections.](https://insider.windows.com/en-us/community-news/feedback-hub-collections/)

## Adding new feedback

### Use a descriptive title

Descriptive and precise titles help Windows engineers understand the issue being reported. An example of a good title: “Groove crashes with error 80041007 when connected to Bluetooth.”

### Select the correct category

The Feedback Hub will automatically select a category based on the title you gave your feedback item. Use the dropdown menus to check or change the category. It's important to have the correct category to make sure your feedback is processed accurately and that certain logs and system settings are collected. For example, we may not be able to address a Bluetooth bug that gets filed under the Start menu, because we wouldn't receive the correct logs.

### Provide items one at a time

When you provide feedback one item at a time, it helps us make sure the correct logs and data are being collected for each submission.

### Provide a clear and detailed description

When sharing additional details, it's important to share as much detail about the issue as possible. For example, include the steps to reproduce the issue, attach screenshots (if applicable) and use the “reproduce issue” option, if available for the type of feedback you're submitting.

### Provide additional information

Sharing additional information can be extremely helpful in describing the issue and showing details of what you're experiencing. You can do this by attaching a screen shot or file (such as a dxdiag, .cab files, or other) and recreating the problem with Capture Mode. Capture Mode helps us capture detailed logs while the issue is happening, which can be extremely helpful.

### Use Capture Mode

Capture Mode is an important method of bug re-creation that provides detailed logs for our engineering teams to review. To use this process, follow these steps:

1. Create a new feedback item.
2. Select “Problem.”
3. Fill in the title and detail fields as appropriate.
4. Select the appropriate category and subcategory dropdowns.
5. If applicable, you'll see a section titled “Recreate the problem.”
6. Select the appropriate type of logging you’d like to attach.
7. Select “Start Capture”.
8. [Reproduce the issue you’re sharing feedback about.]
9. Select “Stop Capture”. You’ll see a note that the log files are now attached to your feedback.
10.	Submit your feedback item. All the appropriate logs and data will auto-attach to your submission.

### Sharing your submission

After you submit feedback, you'll be able to share your submission with other Insiders. They might be experiencing the same issue as you or want the same feature or change that you’re suggesting. If you're asked to communicate directly with a Microsoft engineer later, you may also be asked to share a link to your feedback. 

To create a feedback link for sharing:

1. Open the **Feedback Hub**.
2. Navigate to the **Feedback** tab.
3. Search for and open the feedback item you’d like to share. If you're looking for feedback you created, select the **My Feedback** tab at the top.
4. After selecting the right feedback item, choose the **Share** button in the upper right corner. A small window will open with the newly created link.

## Checking the status of feedback

As Microsoft engineers process your feedback, you’ll see a banner appear on the feedback item showing its status. There are five possible statuses:

- **We've Got It:** Your feedback's been successfully submitted and is currently being reviewed by an expert.
- **Looking into It:** Your feedback has been reviewed, and we're currently investigating the best way to address the problem or suggestion. 
- **Working on It:** We’re working on making improvements to the experience based on the feedback you’ve shared.
- **Changes Made:** We’ve made changes based on this feedback! The feedback item will let you know whether they’re available on your current build or app version, or whether you’ll need to update to see them. If you think there’s more we can look into, please leave a comment!
- **Needs more info:** We need your help to understand this issue better. Please review our comments and add details below by recreating the problem or attaching files or screenshots.

When the state changes, you and other Windows Insiders who have upvoted the feedback will receive a notification from the Feedback Hub about the change.

## Submitting and tracking your organization's feedback

You can track feedback submitted to the Feedback Hub by you and others in your organization. (AAD account registration is required.) Here’s how:

1. Register as a Windows Insider with your [work account in Azure Active Directory](https://insider.windows.com/en-us/for-business-getting-started/).
2. Sign into the Feedback Hub using this same work account. On the Welcome page of the Feedback Hub, select the People icon on the lower left, and then choose or add your AAD work account. (If you have already registered and signed in using your Microsoft account, you’ll need to sign out first.)
3. Go to **Feedback**, **All Feedback**.
4. Under the **Filter** dropdown, select **My Organization** to view feedback from Insiders in your business. 

> [!NOTE] 
> Feedback filtered with this view will only show Feedback from users in your organization who sign into the Feedback Hub using their registered AAD account.

![Feedback Hub's filters that let you search for feedback from within your organization](images/FeedbackHubOrg.png "Your organization's feedback in Feedback Hub")

*Filter to view feedback submitted specifically by Windows Insiders in your organization.*

## Help us make Windows better in your language

Our Language Community App makes it quick and easy to suggest changes to Windows text translated in your language. Simply select the text you want changed, enter your suggestion or vote for suggestions from other Windows Insiders and submit.

[Download the Language Community App](ms-windows-store://pdp/?productid=9NWX2N74M2X3&cid=UCID00023)

Available for PC only. Requires Insider Preview build 16299 or above. Check store description for languages supported. Use Windows displayed in your language, not in English (United States). Check your Windows display language at **Region & language** in Settings.
