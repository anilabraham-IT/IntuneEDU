---
# required metadata

title: Add free apps from the iOS store
titleSuffix: Intune for Education
description: Learn how to add free apps from the iOS store to Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 06/19/2018
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

# Add iOS apps to Intune for Education  
Before you assign apps to your school's groups, you must add eligible apps to your Intune tenant. 

From the Intune for Education portal you can search, add, and then assign apps purchased through the iOS Store. This article describes how to add and delete these apps. Instructions apply only to apps that are listed as **Free** in the App Store. To install a paid app, see the article, [Add VPP managed apps](add-vpp-apps-ios.md).

You do not need a VPP token to install free apps, but it is recommended. A VPP token permits you to purchase all apps through the VPP store. Intune silently installs VPP-purchased apps on devices, and does not require an Apple login to authenticate. 

If you choose not to use a VPP token to purchase your app, the device user will need to log in with an Apple ID to install the app.

## Get free iOS apps  
Complete the following steps to add an iOS app to Intune.
1. Sign in to the Intune for Education portal.
2. From the left-side of the dashboard, click **Apps**.
3. In the left pane of the blade, under **IOS APPS**, click **New app**.
4. In the New iOS app pane, select the VPP country store. Intune synchronizes VPP apps for all locales from the specified VPP country store.
5. In the search box, type the full or partial name of an app.
6. Select the app and click **Save** to add the app to your Intune inventory.

### View app details  
Intune will take some time to sync the app to your Intune tenant. When completed, the app will appear in the app list, under **iOS store**. Click the app to view its:

* Overview: Lists app name, publisher, and date you added it to Intune. Click the app name to see the app in iTunes.
* Groups: Lists all groups that are assigned the app. Change group assignments here or go to the details page for a specific group.
* Install status: Lists the installation status of the app for each device it was deployed to. 

## Delete iOS apps  
Delete an iOS app from your Intune tenant. When you delete an app, it is removed from group assignments. To assign the app again, you will need to add it back to your Intune tenant through the App Store. (//lenewsad--does this uninstall the app from the devce? what do they need to do to remove it from the device?  follow-up)

1. From the Intune for Education portal, click **Apps**.
2. Go to the app list, and under **iOS Apps** click the app that you want to delete.
3. Click **Delete App**.
4. Click **Delete** to confirm your action.  

## Next steps
- [Find out more about the full experience managing apps using Intune](https://docs.microsoft.com/intune/deploy-use/add-apps)
