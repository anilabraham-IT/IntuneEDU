---
# required metadata

title: Add free apps from the iOS store
titleSuffix: Intune for Education
description: Learn how to add free apps from the iOS store to Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 07/23/2018
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: 24ab6547-aa65-428a-b184-06b806e95bd1
searchScope:
 - IntuneEDU

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
#ms.reviewer: travisj
#ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom: intune-education

---

# Add free iOS apps to Intune for Education  
Search for and add free apps from the iOS App Store to your app inventory. This article describes how to purchase free iOS apps so that you can view and assign them in the Intune for Education portal.
 
Instructions apply only to apps that are listed as **Free** in the App Store. To add a paid-for app, see the article, [Add VPP-purchased iOS apps to Intune](add-vpp-apps-ios.md).

## Recommendation: Set up VPP token

You do not need a VPP token to install free apps, but we recommended it. A VPP token permits you to purchase all apps--free and paid--through the VPP store. Intune silently installs VPP-purchased apps on devices, and does not require an Apple ID to authenticate.  

If you choose not to use a VPP token to purchase your app, you will only be able to manage free apps in the Intune for Education. The device user will also need to sign in with an Apple ID to install assigned apps.

## Add new iOS app
Complete the following steps to add an iOS app to Intune for Education.
1. Sign in to the Intune for Education portal.
2. Click **Apps**.
3. In the left pane, under **IOS APPS**, click **New app**.
5. In the search box, type the full or partial name of an app.
6. Select the app and click **Save** to add the app to your Intune inventory.

## View app details in Intune for Education
Added apps appear in the app list, under **iOS store**. Click the app to view its:

* **Overview**: Lists app name, publisher, and date you added it to Intune. Click the app name to see the app in iTunes.
* **Groups**: Lists all groups that are assigned the app. Change group assignments here or go to the details page for a specific group.
* **Install status**: Shows details about the app's installation, such as the device it was assigned to. The status also lists last check-in time and if the installation was a success, failure, or still-in-progress.  

## Next steps
- [Find out more about the full experience managing apps using Intune](https://docs.microsoft.com/intune/deploy-use/add-apps)
