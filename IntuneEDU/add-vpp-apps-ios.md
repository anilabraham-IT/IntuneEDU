---
# required metadata

title: Add VPP-purchased apps
titleSuffix: Intune for Education
description: Learn how to add VPP purchased apps to Intune for Education.
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

# Add VPP-purchased iOS apps to Intune

Add volume purchase program (VPP) iOS apps from the Intune for Education portal. This article describes how to manage VPP-purchased apps that have been synced to Microsoft Intune.

Both free and paid-for apps are available to buy in volume through the App Store. To install free iOS apps *without a VPP token*, see how to [add free iOS apps in Intune](add-apps-ios.md).  

## What is a VPP?
A VPP lets organizations buy app licenses in bulk and manage them through their mobile device manager (MDM). From an MDM, such as Intune for Education, licenses can be managed and then silently deployed over-the-air to student devices. A VPP/MDM partenership is ideal in classrooms and organizations where the same app is needed on many devices. 

## Before you begin
To view and manage licenses from the Intune for Education portal, you must first:  
* Configure a [VPP token](setup-ios-device-management.md).
* Purchase apps through an Apple VPP vendor or through the Apple School Manager, Apps and Books store.
* Transfer existing purchased licenses to the appropriate Intune VPP token. See the [Apple education support site](https://support.apple.com/education) to learn how to transfer licenses. 

## Search and add apps
Complete the following steps to search and add paid-for iOS apps from the Intune for Education portal. 

Free apps are made available for purchase directly from the portal. However, these are made available so that users without a VPP account can easily get them. If you plan to deploy free apps silently and in volume to your school's devices, you should purchase them through the Apple VPP or Apple School Manager websites.

1. Sign in to the Intune for Education portal.
2. Click **Apps**.
3. From the app list, under **iOS Apps**, click **New app**.
4. Select the country from where you are purchasing the app.
5. Type in the app's full or partial name. Intune returns a list of relevant results from the App Store. 
6. Select the app. 
7. A message appears that prompts you to complete your purchase through Apple School Manager or the legacy VPP site. Click the site where your volume-purchased apps belong. 
8. Follow the steps on the external website to complete your purchase. You will be prompted to assign your licenses to the appropriate location.
9. Return to Intune for Education > Apps. Your app will appear in the **iOS Apps** list. If you don't see it right away, wait a few minutes and refresh your page.

### View app details
Apps appear in the app list, under **iOS Apps**. Click the app to view its:

* **Overview**: Lists app name, publisher, and date you added it to Intune. Also lists the number of licenses available to assign.
* **Groups**: Lists all groups that are assigned the app. Change group assignments here or go to the details page for a specific group.
* **Install status**: Shows details about the app's installation, such as the device it was assigned to. The status also lists last check-in time and if the installation was a success, failure, or still-in-progress.

## Reassign VPP-purchased licenses
VPP-purchased apps cannot be deleted from Intune for Education. However, you can remove a user from an assigned group, or remove the entire group from assignment. Learn how to [change group assignments](link).

## Next steps

- [Find out more about the full experience managing apps using Intune](https://docs.microsoft.com/intune/deploy-use/add-apps)
