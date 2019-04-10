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
Express configuration is preset with iOS setting suggestions to help you quickly set up a group of devices or users. Intune for Education chooses settings that are both Microsoft-recommended and best for school environments. Make changes to fit your school's rules and policies, or click straight through the settings page to apply our recommendations. 

For the complete list of settings and descriptions, see [All iOS settings in Intune for Education](all-edu-settings-ios.md). 

> [!IMPORTANT]
> If iOS configurations are disabled when you launch express configuration, check to make sure you've set up both your MDM Apple Push certificate and DEP token. If you have both of these, make sure that neither has expired. For more information about setting up iOS device management see [Set up iOS device management](setup-ios-device-management.md)


## App Store, iTunes Store, and Book Store  
Setting|Suggested value|  
|---|---|
|Block App Store|Block|
|Block in-app purchases|Block|
|Block explicit content in App Store and iTunes Store|Block|
|Block downloading Apple Books content flagged as erotica|Block|  

## Built-in apps  
Setting|Suggested value|  
|---|---|
|Block Camera|Block|
|Block FaceTime|Block|
|Block Game Center|Block|  
|Block Apple Music|Block|
|Block Messages app|Block|
|Block Apple Books|Block|  

## Device restrictions  
Setting name|Suggested value|
|---|---|
|Block changing device name|Block|
|Block changing wallpaper|Block|
|Block changing notification settings|Block|
|Block changes to content and privacy restrictions|Block|
|Block button that erases all content and settings|Block|  

## iCloud
|Setting|Suggested value|
|---|---|
|Block iCloud backup|Block|
|Block syncing documents to iCloud|Block|
|Block iCloud Photo Library|Block|  

## Lock screen and wallpaper
Setting|Suggested value|
|---|---|
|Block notifications on lock screen|Block|
|Block access to Wallet from lock screen|Block|
|Set device lock screen image|A .jpg or .png file, 960 KB max|
|Set device home screen image|A .jpg or .png file, 960 KB max|  

## Passcode, Touch ID, and Face ID  
Setting|Suggested value|
|---|---|  
|Require passcode|Not Configured|
|Block changing passcode|Block|
|Number of failed passcode attempts before wiping device|Not Configured|
|Block Touch ID and Face ID|Block|

## Siri and search 
Setting|Suggested value|
|---|---|   
|Block Siri|Block|  

## Reset default settings
To restore all settings to their default values, click **Reset to suggested defaults**. 

## Next steps  
Learn all about groups, settings, and monitoring conflicts in Intune for Education. 
* Find out the difference between [assigned and dynamic](create-groups.md) groups
* Assign [group admins](group-admin-delegate.md) to help you manage classroom settings within your school or across the district
* Learn how [settings inheritance](settings-inheritance.md) affects group assignments
* Review [reports](what-are-reports.md) to pinpoint and troubleshoot setting conflicts
