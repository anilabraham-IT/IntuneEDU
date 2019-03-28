---
# required metadata

title: In development - Microsoft Intune for Education
titlesuffix: 
description: Microsoft Intune for Education features in development
keywords:
author: lenewsad  
ms.author: lanewsad   
manager: dougeby
ms.date: 03/28/2019
ms.topic: conceptual
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: 

# optional metadata


#audience:
#ms.devlang:
ms.reviewer: cacampbell
ms.suite: ems
search.appverid: MET150
#ms.tgt_pltfrm:
ms.custom: seodec18
ms.collection: M365-identity-device-management
---

# In development for Microsoft Intune - April 2019

To assist in your readiness and planning, this page lists Intune for Education updates and features that are in development but not yet released. 

- When a feature is launched in production, the feature description will move off this page and onto the [What's new page](whats-new-in-edu.md).
- This page and the [What's New page](whats-new-in-edu.md) are updated periodically. Check back for additional updates.  

> [!Note]
> These items reflect Microsoft’s current expectations about Intune for Education capabilities coming in a future release. Dates and individual features may change. Not all items in development have a feature description on this page.  

<!-- 1904 start-->

### Improved iOS settings names and tooltips  
We’re revising many of the iOS setting names, tooltips, and categories in Intune for Education to make settings easier to find and understand. For a detailed list of these settings, see [iOS device settings in Intune for Education](all-edu-settings-ios.md).  

### Refined list of iOS settings in Express Configuration   
We're adjusting the [list of iOS setttings in Express Configuration](edu-express-config-settings-ios.md) so that you can get your devices and groups set up even faster. You'll see some settings moved out of Express Configuration, and new settings moved in. Settings that are removed from Express Configuration will still be available to configure in **Groups** > **Settings** > **iOS Device Settings**. For the full list of device settings in Intune for Education, see [iOS device settings](all-edu-settings-ios.md) and [Windows 10 device settings](all-edu-settings-windows.md).  

###  New settings for Windows 10 devices  
There will be several new Windows 10 device settings. Here's just a few of the settings you'll see:  
* Windows Update notifications: This setting lets you choose whether or not users see notifications about Windows Updates.  
* Manual Windows Update: This setting lets you choose whether or not users have access to the Windows Update scan, download, and install features.  

### Apply iOS device naming template  
We're adding new naming settings to help you group and identify your iOS devices. During iOS enrollment and MDM server token setup, Intune for Education will automatically name each of your devices with their unique device serial number. You'll then have the option to add a custom name, such as *Contoso* or *Math1*, to the prefix. If you do customize the name, the device serial number will be attached to the end of it. For example: *Contoso012a345b67c8*  

### See also  
See [What’s new in Intune for Education](whats-new-in-edu.md) for details about recent developments.  
