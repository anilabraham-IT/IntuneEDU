---
# required metadata

title: Add apps
titleSuffix: Intune for Education
description: Learn how to add apps to Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: angrobe
ms.date: 05/10/2017
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

# VPP-purchased iOS apps

Add and revoke volume purchase program (VPP) iOS apps from the Intune for Education portal. This article describes how to manage VPP-purchased apps that have been transfered to Microsoft Intune. 

Both free and paid-for apps are available to buy in volume through the App Store. To install free iOS apps *without a VPP token*, see <add iOS apps in Intune>. (//lenewsad SHould we be saying iOS app store, Apps and Books, App Store?)

## What is a VPP?
A VPP lets organizations buy app licenses in bulk and manage them through their mobile device manager (MDM). <//lenewsad is there a limit of licenses per app?>). From an MDM, such as Intune for Eduation, licenses can be managed and then silently deployed over-the-air to student devices. A VPP/MDM partenership is ideal in classrooms and organizations where the same app is needed on many devices. 

## Before you begin
To view and manage licenses from the Intune for Education portal, you must first:
* Configure a VPP token. <link to article>
* Purchase apps through an Apple VPP vendor or through the Apple School Manager, Apps and Books store.
* Transfer existing purchased licenses to your Intune tenant (referred to as *location* in Apple School Manager). <//lenewsad the transfer to dropdown does say choose a location. are the selections here all names of tenants?>. See the Apple School Manager documentation to learn how to transfer licenses. <link to Apple docs>.

## Search and add apps
Complete the following steps to search and get iOS paid apps from the Intune for Education portal. 

 **Free** apps are made available for purchase directly from the portal. However, these are made available so that users without a VPP account can easily get them. If you plan to deploy free apps silently and in volume to your school's devices, you should purchase them through the Apple VPP or Apple School Manager websites.  

1. Sign in to the Intune for Education portal.
2. From the left-side of the dashboard, click **Apps**.
3. From the app list, under **iOS Apps**, click **New app**.
4. Select the VPP country store. Intune synchronizes VPP apps for all locales from the specified VPP country store. <//lenewsad what does this mean?>
5. Type in the app's full or partial name. Intune returns a list of relevant results from the App Store. 
6. Select the app. 
7. A message appears that prompts you to complete your purchase through Apple School Manager or the legacy VPP site. Click the site where your Volume Purchased apps belong. 
8. Follow the steps on the external website to complete your purchase. You will be prompted to assign your licenses to your Intune tenant.
9. Return to Intune for Education > Apps. Your app will appear in the iOS Apps list. If you don't see it right away, wait a few minutes and refresh your page.

### View app details
Intune will take some time to sync the app to your Intune tenant. When completed, the app will appear in the app list, under **iOS Apps**. Click the app to view its:

* Overview: Lists app name, publisher, and date you added it to Intune. Also lists the number of licenses available to assign.
* Groups: Lists all groups that are assigned the app. Change group assignments here or go to the details page for a specific group.
* Install status: Provide details about the app's installation, such as the device it was assigned to and the user of the device <//lenewsad is this accurate--is it the user of the device--will this update each time a new user check in? user name should not be there. ). Also lists last check-in time and if the installation was a success, failure, or still-in-progress.

## Revoke VPP-purchased licenses
VPP-purchased apps cannot be deleted from Intune for Education. However, you can revoke licenses by...<//lenewsad what is this procedure? What does revoking do? What does it strip away? >

1. From the Intune for Education portal, click **Apps**.
2. Go to the app list, and under **iOS Apps** click the app that you want to delete.
3. Click ****.
4. Click **** to confirm your action.

## Find out more

- [Find out more about the full experience managing apps using Intune](https://docs.microsoft.com/intune/deploy-use/add-apps)
