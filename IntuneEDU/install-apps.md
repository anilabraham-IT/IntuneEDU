---
# required metadata

title: How do I install apps?
titleSuffix: Intune for Education
description: Learn how to manage apps with Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: angrobe
ms.date: 05/10/2017
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: 635a5cc7-7dd4-45f9-9b18-3eddb76d0c74
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

# Installing apps on school devices

To install an app on a school device, you have to first assign it to a group. This article describes three ways to assign apps to student teachers.  

After you assign an app, the app is sent to the appropriate device. App installation is initiated when the device checks into Intune for Education. 

## Add apps to Intune for Education inventory
By default, popular apps are available in Intune for Education for immediate assignment. If the app you want to assign isn't in your inventory, learn how to add it to Intune for Education with one of the following articles:
* [Microsoft Store for Education apps](acquire-store-apps.md)
* [Free iOS App Store apps](add-apps-ios.md)
* [iOS VPP apps](add-vpp-apps-ios.md)
* [Windows 10 desktop apps](add-desktop-apps-edu.md)
* [Web apps](add-web-apps-edu.md)  

## Assign apps with Express Configuration
Launch [Express Configuration](Express-configuration-intune-edu.md) to assign multiple apps to a single group. 

1. From the [Intune for Education dashboard](https://intuneeducation.portal.azure.com), click **Express Configuration**.  
2. Choose the group you want to add apps to. Then click **Next**.
3. Choose one or more apps to deploy to your group. Then click **Next**. 
4. The apps will automatically be assigned to your group. Continue through Express Configuration. //lenewsad Want to check if there is an early exit option.

##  Assign apps to a single group
Select a group and install one or more apps to the devices in that group.

1. From the [Intune for Education dashboard](https://intuneeducation.portal.azure.com), click **Groups**.
2. Choose the groups you want to deploy the apps to.
3. Go to the task bar at the top and click **Apps** to see a list of available apps.  
4. Choose one or more apps to deploy to your group. 
5. Choose **Save** to deploy the selected apps to that group. Installation will automatically begin the next time the device checks-in to Intune for Education.  

## Asign apps to multiple groups
Select an app and assign it to one or more groups for installation.

1. From the [Intune for Education dashboard](https://intuneeducation.portal.azure.com), click **Apps**.
2. From the list of apps on the left, choose the app you want to assign.
3. Go to the task bar at the top and click **Groups** > **Change group assignments**. 
4. Choose the groups you want to assign the app to.

## Next steps

- [Find out more about installing apps using the full app management experience in Intune](https://docs.microsoft.com/intune/deploy-use/deploy-apps)
