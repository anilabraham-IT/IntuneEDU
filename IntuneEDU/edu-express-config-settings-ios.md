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
Express Configuration comes preset to help you quickly set up your iOS devices. Intune for Education chooses options that are both Microsoft-recommended and best for school environments. This article describes those settings and their default behavior. 

 Make changes to fit your school's rules and policies, or click straight through the settings page to apply the preset recommendations. 

For the complete list of settings and descriptions, see [All iOS settings in Intune for Education](edu-settings-ios.md). 


## General settings
Setting name|Default behavior|
|---|---|
|Block removing device management profiles|Block|
|Block sharing device usage data with Apple|Block|
|Block users from changing diagnostic data submission settings|Block|
|Block erasing content and settings|Block|
|Block changing device name|Block|
|Block users from enabling restrictions in device settings|Block|
|Block changing device wallpaper|Block|//Is this a dupe. Saw under "New" in excel."|
|Block changing notification settings|Block|
|Block untrusted TLS certificates|Block|
|Block users from trusting Enterprise Developer apps|Block|
|Block users from changing Enterprise Developer app trust settings|Block|
|Enable Activation Lock|Allow|//Should this be allow or enable|
|Block changing account details|Block|//need to clarify this setting because didn't have this listed in all iOS settings|

## Wi-Fi profiles
Setting|Default behavior|
|---|---|
|Wi-Fi profile configuration|Behavior|

## Password
Setting|Default behavior|
|---|---|
|Require passcode|Not Configured|
|Number of failed passcode attempts before wiping device|Not Configured|
|Minutes to wait before requiring passcode on lock screen|Not Configured|
|Block fingerprint unlock|Block|
|Block changing passcode|Block|
|Block changing registered fingerprint settings|Block|

## Lock screen
Setting|Default behavior|Description|
|---|---|---|
|Block notifications on lock screen|Block||
|Block access to Control Center on lock screen|Block||
|Block access to Wallet from lock screen|Block|
|Block Today view on lock screen|Block||

## Built-in apps
Setting|Default behavior|
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
|Block Apple Music|Block| //Check name of this--excel string says iTunes music service|
|Block iTunes Radio|Block|
|Block changes to Find My Friends app settings|Block|

## Connected devices
Setting|Default behavior|
|---|---|
|Block changes to bluetooth settings|Block|

## Safari
Setting|Default behavior|
|---|---|
|Block Safari|Not configured|

## Home screen layout
Setting|Default behavior|
|---|---|
|Set wallpaper|Not configured|

## App Store
Setting|Default behavior|
|---|---|
|Block App Store|Block|
|Require password to access App Store|Not configured|
|Block in-app purchases|Block||
|Block explicit content in iTunes and the App Store|Block|
|Block downloading iBook content flagged as erotica|Block|
|Block Game Center|Block|

## Cloud and storage
|Setting|Default behavior|
|---|---|
|Block iCloud backup|Block|
|Block syncing files to iCloud|Block|
|Require iCloud backups to be encrypted|Block|  //Len:This is a require but value is block?|
|Block Photo Stream sync to iCloud|Block|
|Block shared Photo Stream|Block|
|Block iCloud Photo Library|Block|
|Block Activity continuation|Block| 

## Update restrictions
|Setting|Default behavior|
|---|---|
|Prevent devices from updating during specific times|All|Specify restricted days, time zone, start time, and end time.|
|Time zone|
|Start Time|6:00 pm|
|End Time|6:00 pm|  

## Reset default settings
To restore all apps to their default selections, click **Reset to app selections**. <add screenshot>  
To restore all settings to their default values, click **Reset to suggested defaults**. <add screenshot>  


[Find out more about the full Windows 10 settings management experience available in Intune](https://docs.microsoft.com/intune/deploy-use/windows-10-policy-settings-in-microsoft-intune)
