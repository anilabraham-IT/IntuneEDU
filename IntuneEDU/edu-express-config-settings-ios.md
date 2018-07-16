---
# required metadata

title: Default iOS settings in Express Configuration
titleSuffix: Intune for Education
description: Lists the default setting names and behaviors set when using Express Configuration.
keywords:
author: lenewsad
ms.author: lanewsad
manager: angrobe
ms.date: 02/20/2018
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
Express configuration is preset with Microsoft-suggested settings to help you quickly set up a group of devices or users. Intune for Education chooses settings that are both Microsoft-recommended and best for school environments. This article describes those settings.

 Make changes to fit your school's rules and policies, or click straight through the settings page to apply our recommendations. 

For the complete list of settings and descriptions, see [All iOS settings in Intune for Education](all-edu-settings-ios.md). 

> [!IMPORTANT]
> If iOS configurations are disabled when you launch express configuration, check to make sure you've set up both your MDM Apple Push certificate and DEP token. If you have both of these, make sure that neither has expired. For more information about setting up iOS device management see [Set up iOS device management](setup-ios-device-management.md)


## General settings
Setting name|Suggested value|
|---|---|
|Block removing device management profiles|Block|
|Block sharing device usage data with Apple|Block|
|Block users from changing diagnostic data submission settings|Block|
|Block erasing content and settings|Block|
|Block changing device name|Block|
|Block users from enabling restrictions in device settings|Block|
|Block changing device wallpaper|Block|
|Block changing notification settings|Block|
|Block untrusted TLS certificates|Block|
|Block users from trusting Enterprise Developer apps|Block|
|Block users from changing Enterprise Developer app trust settings|Block|
|Enable Activation Lock|Allow|
|Block changing account details|Block|

## Wi-Fi profiles
Setting|Suggested value|
|---|---|
|Wi-Fi profile configuration|Behavior|

## Password
Setting|Suggested value|
|---|---|
|Require passcode|Not Configured|
|Number of failed passcode attempts before wiping device|Not Configured|
|Minutes to wait before requiring passcode on lock screen|Not Configured|
|Block fingerprint unlock|Block|
|Block changing passcode|Block|
|Block changing registered fingerprint settings|Block|

## Lock screen
Setting|Suggested value|
|---|---|---|
|Block notifications on lock screen|Block||
|Block access to Control Center on lock screen|Block||
|Block access to Wallet from lock screen|Block|
|Block Today view on lock screen|Block||

## Built-in apps
Setting|Suggested value|
|---|---|
|Block Camera|Block|
|Block FaceTime|Block|
|Block Message app|Block|
|Block Siri|Block|
|Block Siri from using profanity|Block|
|Block Siri from searching for user-generated content|Block|
|Block Spotlight from searching for results on the Internet|Block|
|Block Apple News|Block|
|Block iBooks Store|Block|
|Block Podcasts app|Block|
|Block Apple Music|Block|
|Block iTunes Radio|Block|
|Block changes to Find My Friends app settings|Block|

## Connected devices
Setting|Suggested value|
|---|---|
|Block changes to bluetooth settings|Block|

## Safari
Setting|Suggested value|
|---|---|
|Block Safari|Not configured|  

## App Store
Setting|Suggested value|
|---|---|
|Block App Store|Block|
|Require password to access App Store|Not configured|
|Block in-app purchases|Block||
|Block explicit content in iTunes and the App Store|Block|
|Block downloading iBook content flagged as erotica|Block|
|Block Game Center|Block|

## Cloud and storage
|Setting|Suggested value|
|---|---|
|Block iCloud backup|Block|
|Block syncing files to iCloud|Block|
|Require iCloud backups to be encrypted|Block| 
|Block Photo Stream sync to iCloud|Block|
|Block shared Photo Stream|Block|
|Block iCloud Photo Library|Block|
|Block Activity continuation|Block| 

## Device update restrictions
|Setting|Suggested value|
|---|---|
|Prevent devices from updating during specific times|All|
|Time zone|Choose your school's time zone|
|Start Time|6:00 pm|
|End Time|6:00 pm|  

## Reset default settings
To restore all settings to their default values, click **Reset to suggested defaults**. 

## Next steps  

[Find out more about the full Windows 10 settings management experience available in Intune](https://docs.microsoft.com/intune/deploy-use/windows-10-policy-settings-in-microsoft-intune)
