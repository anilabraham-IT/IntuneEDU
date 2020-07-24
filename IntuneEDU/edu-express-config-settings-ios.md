---
# required metadata

title: Default iOS settings in Express Configuration
titleSuffix: Intune for Education
description: Lists the default setting names and behaviors set when using Express Configuration.
keywords:
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 04/19/2019
ms.topic: article
ms.prod:
ms.service: microsoft-intune
ms.subservice: education
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
# Default iOS settings in Express Configuration
Express Configuration is preset with iOS setting suggestions to help you quickly set up a group of devices or users. Intune for Education chooses settings that are both Microsoft-recommended and best for school environments. Make changes to fit your school's rules and policies, or click straight through the settings page to apply our recommendations. 

For the complete list of settings and descriptions, see [All iOS settings in Intune for Education](all-edu-settings-ios.md). 

> [!IMPORTANT]
> If iOS configurations are disabled when you launch Express Configuration, check to make sure you've set up both your MDM Apple Push certificate and DEP token. If you have both of these, make sure that neither has expired. For more information about setting up iOS device management, see [Set up iOS device management](setup-ios-device-management.md)


## App Store, iTunes Store, and Book Store  
Setting|What it does|  
|---|---|
|Block App Store|Block students from accessing the App Store on school devices.|
|Block in-app purchases|Block attempts to make store purchases from within a running app.|
|Block explicit content in App Store and iTunes Store|Block students from accessing content rated as adult in the App Store.|
|Block downloading Apple Books content flagged as erotica|Block students from downloading books classified as erotica.|  

## Built-in apps  
Setting|What it does|  
|---|---|
|Block Camera|Block use of the camera on the device.|
|Block FaceTime|Blocks use of the FaceTime app on the device.|
|Block Game Center|Block use of the Game Center app on devices.|  
|Block Apple Music|Block use of the music streaming component of the Apple Music app on the device.|
|Block Messages app|Block use of the Messages app on the device.|
|Block Apple Books|Block students from browsing and purchasing books in the Book Store.|  

## Device restrictions  
Setting name|What it does|
|---|---|
|Block changing device name|Block students from changing the name of the device.|
|Block changing wallpaper|Blocks students from changing the device lock screen and home screen image.|
|Block changing notification settings|Block students from changing the device notification settings.|
|Block changes to content and privacy restrictions|Block students from changing restrictions (parental controls) and Screen Time settings on the device.|
|Block button that erases all content and settings|Block students from erasing all content and settings on the device. The erase button becomes unavailable and can't be selected.|  

## iCloud
|Setting|What it does|
|---|---|
|Block iCloud backup|Block students from backing up devices to iCloud.|
|Block syncing documents to iCloud|Block documents from syncing to an iCloud storage space.|
|Block iCloud Photo Library|Block students from storing photos and videos in the cloud. Photos that aren't fully downloaded from iCloud Photo Library are removed from local storage.|  

## Lock screen and wallpaper
Setting|What it does|
|---|---|
|Block notifications on lock screen|Block students from viewing notifications when the device is locked.|
|Block access to Wallet from lock screen|Block students from accessing the Wallet app when the device is locked.|
|Set device lock screen image|Choose a custom image to appear as the wallpaper for the device's lock screen.|
|Set device home screen image|Choose a custom image to appear as the wallpaper for the device's home screen.|  

## Passcode, Touch ID, and Face ID  
Setting|What it does|
|---|---|  
|Require passcode|Require students to enter a passcode to unlock the device.|
|Block changing passcode|Block students from changing, adding, or removing the device passcode.|
|Number of failed passcode attempts before wiping device|When someone exceeds the allowed number of sign-in attempts, the device erases all content and settings from the device, such as personal data, iOS software, email accounts, system and app settings, downloaded apps, and media. The device is restored to the way it was when it was first turned on. To configure this setting, enter the maximum number of sign-in attempts allowed.|
|Block Touch ID and Face ID|Block students from using a fingerprint or facial recognition to unlock devices.|

## Siri and search 
Setting|What it does|
|---|---|   
|Block Siri|Block students from using Siri, the iOS voice assistant.|  

## Reset default settings
To restore all settings to their default values, click **Reset to suggested defaults**. 

## Next steps  
Learn all about groups, settings, and monitoring conflicts in Intune for Education. 
* Find out the difference between [assigned and dynamic](create-groups.md) groups
* Assign [group admins](group-admin-delegate.md) to help you manage classroom settings within your school or across the district
* Learn how [settings inheritance](settings-inheritance.md) affects group assignments
* Review [reports](what-are-reports.md) to pinpoint and troubleshoot setting conflicts
