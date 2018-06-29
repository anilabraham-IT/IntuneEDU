---
# required metadata

title: Available settings
titleSuffix: Intune for Education
description: Learn more about the settings available for Intune for Education.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 06/25/2018
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.technology:
ms.assetid: 2221009e-68cf-4171-8118-0d750b0f35f1
searchScope:
- IntuneEDU

# optional metadata

#ROBOTS:
#audience:
#ms.devlang:
#ms.reviewer: rashok
#ms.suite: ems
#ms.tgt_pltfrm:
#ms.custom: intune-education

---

# iOS device settings in Intune for Education 

This article lists and describes all iOS device settings in Intune for Education. To view and edit these settings in the portal, click **Group** >**Settings** > **iOS Device Settings**.   

## Cannot see or use iOS options in Intune for Education  

If you find that the iOS dropdown is not visible or if it is disabled, [set up iOS device management](setup-ios-device-management.md). After setup is complete, all iOS controls will become enabled.

## Apply settings to groups  
Apply [group settings](what-are-groups.md) to establish access and security boundaries on devices throughout your school. You can assign the same settings across all groups in your school; or you can customize the classroom experience and apply settings to individual groups.

## Configuration options
Many settings in Intune for Educations are configured to **Block** or **Allow**. For some settings, **Not configured** is an option. When toggled to **Not Configured**, the device will either:  
* Use the default setting 
* Allow the device user (student or teacher) to customize the setting from their device  

> [!NOTE]
> User, app, and device settings differ from [tenant settings](edu-tenant-general-settings.md). Tenant settings target the subscription and management settings at the organization's administrative level.


  ![The settings page for a group](./media/settings-001-list-of-settings.png)

  
## Basic device restrictions  
Setting|What it does|
|---|---|
|Block users from changing diagnostic data submission settings|Blocks students from changing if or how the device sends diagnostic data. |  
|Block screen capture|Block students from capturing the contents of the screen as an image.|  
|Block remote screen observation by Classroom app​ |Blocks the Apple Classroom app from viewing the screen of iOS devices.|  
|Block unprompted screen observation by Classroom app​|Blocks teachers from being able to observe student screens, without the students knowledge, through the Classroom app.|  
|Block untrusted TLS certificates|Blocks untrusted Transport Layer Security (TSL) certificates on the device.|  
|Block installing trusted enterprise developer apps​ |Block |  
|Block users from changing trust enterprise developer app installation settings​|Block students from changing the app installation settings you've defined.|  
|Block users from changing device restrictions in device settings​|Block students from changing restrictions (parental controls) on the device.|  
|Block erasing content and settings|Block students from erasing all content and settings on the device.|  
|Block changing device name|Block students from changing the name of the device.|  
|Block changing notification settings|Block students from changing the device notification settings.|  
|Block wallpaper modification |What it does|    
|Block configuration profile changes |Block students from being able to install configuration profiles.||  
|Block Activation Lock|Block Activation Lock on supervices iOS devices.|  

## Lock screen and passcode  

Setting|What it does|
|---|---|
|Block notifications on lock screen|Block students from viewing notifications when device is locked.|
|Block access to Control Center on lock screen|Block student from accessing the control center app when device is locked.|
|Block Siri on lock screen|Block the use of Siri when device is locked.|
|Block access to Wallet from lock screen|Block access to the Wallet app when device is locked.|
|Block Today view on lock screen|Block students from seeing the Today view when device is locked.|
|Require passcode|Require students to enter a passcode to unlock device.|
|Block changing passcode|Block students from changing, adding, or removing device passcode. |
|Minutes of inactivity before the screen locks|Specifies the number of minutes the device can remain idle before the device screen locks.|
|Minutes to wait before requiring passcode on lock screen|Specifies how long the device can remain idle before the student must re-enter device password.|
|Number of failed passcode attempts before wiping device|Specifies the number of unique, bad password attempts allowed before the student must re-enter device password.
|Block fingerprint unlock|Block students from using a fingerprint to unlock devices.|
|Block changing registered fingerprint settings|Block students from changing, addiing, or removing TouchID settings.|  

## App Store settings  

Setting|What it does|
|---|---|
|Block App Store|Block students from accessing the App Store on school devices.|
|Require password to access App Store|Require the student to enter a password before they can access the App Store.|
|Block automatically downloading apps purchased on other devices|Block apps that were purchased on another school device from being downloaded to another device.|
|Block in-app purchases|Block attempts to make store purchases from within a running app.|
|Block apps by age rating|What it does|//
|Block explicit content in iTunes and the App Store|Block students from accessing content rated as adult in the App Store.|
|Block downloading iBook content flagged as erotica|Block students from downloading books classified as erotica.|
|Block Game Center|Block the use of the Game Center app on devices.|
|Block adding friends in Game Center|Block students from adding friends in the Game Center app.|

## Keyboard and dictionary  

|Setting|What it does|  
|---|---|  
|Block looking up word definitions|Block the use of the iOS feature that lets you highlight a word and look up its definition.|  
|Block predictive keyboard suggestions|Block the use of predictive keyboards that suggest words when typing.|

|Block auto-correction|Block the device from automatically correcting misspelled words.|
|Block keyboard spell-check|Block the device spell checker.|
|Block keyboard shortcuts|Block the use of keyboard shortcuts.|
|Block keyboard dictation|Block students from being able to use voice input to enter text.|

## Cloud and storage  

|Setting|What it does|  
|---|---|  
|Block iCloud backup|What it does|  
|Block syncing documents to iCloud|What it does|  
|Block Photo Stream|What it does|  
|Require iCloud backups to be encrypted|What it does|  
|Block iCloud Photo Library|What it does|  
|Block shared Photo Stream|What it does|  
|Block Handoff|What it does|  

## Device update restrictions

|Setting|What it does|
|---|---|
|Prevent devices from updating specific times|What it does|
IX Note: Describe that the user can then specificy restricted days, time zone, start time, and end time.

## Inventory tracking  

|Setting|What it does|
|---|---|
|Asset tag information|What does it do|
|Lock screen footnote|What does it do|

## Built-in apps  

Setting|What it does|
|---|---|
|Block Camera|What it does|
|Block FaceTime|What it does|
|Block Siri|What it does|
|Block Siri profanity filter|What it does|
|Block Siri from searching for user-generated content|What it does|
|Block Spotlight from searching for user-generated content|What it does|
|Block Apple News|What it does|
|Block iBooks Store|What it does|
|Block Messages app|What it does|
|Block Podcasts app|What it does|
|Block Apple Music|What it does|
|Block iTunes Radio|What it does|
|Block changes to Find My Friends app settings|What it does|

## Safari  

Setting|What it does|  
|---|---|  
|Block Safari|What it does|  
|Block autofill|What it does|  
|Block cookies|What it does|  
|Show warning when visiting a fraudulent website|What it does|  
|Block pop-ups|What it does|

## Wi-Fi profiles  
Select from the list of Wi-Fi profiles to assign them to the group.  

## Wireless and connectivity  

Setting|What it does|
|---|---|
|Block AirDrop|What it does|
|Block personal hotspot|What it does|
|Block changing Bluetooth settings|What it does|
|Description|What it does|

## Next steps
[Find out more about the full Windows 10 settings management experience available in Intune](https://docs.microsoft.com/intune/deploy-use/windows-10-policy-settings-in-microsoft-intune)
