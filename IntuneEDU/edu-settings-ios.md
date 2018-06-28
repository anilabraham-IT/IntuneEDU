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

# All iOS settings in Intune for Education

Apply group settings to establish access and security boundaries on your iOS devices. Apply device and user settings the same across all groups; or customize the classroom experience and apply settings to individual groups.

Many settings in Intune for Educations are configured to **Block** or **Allow**. For some settings, **Not configured** is an option. When toggled to **Not Configured**, the device will either:  
* Use the default setting 
* Allow the device user (student or teacher) to customize the setting from their device  

> [!NOTE]
> User, app, and device settings differ from [tenant settings](edu-tenant-general-settings.md). Tenant settings target the subscription and management settings at the organization's administrative level.


  ![The settings page for a group](./media/settings-001-list-of-settings.png)

## iOS device settings  
This section describes the categories and functions of all iOS device settings. To view the settings in the portal, go to the dashboard and click **Group** >**Settings** > **iOS Device Settings**. To search for a specific setting, enter a setting name in the search field. 

If the iOS dropdown is not visible or if it is diasabled, you may need to [configure iOS management](setup-ios-device-management.md).
  
### Basic device restrictions  
Setting|What it does|
|---|---|
|Block users from changing diagnostic data submission settings|What it does|  
|Block screen capture|What it does|  
|Block remote screen observation by Classroom app​ |What it does|  
|Block unprompted screen observation by Classroom app​|What it does|  
|Block untrusted TLS certificates|What it does|  
|Block installing trusted enterprise developer apps​ |What it does|  
|Block users from changing trust enterprise developer app installation settings​|What it does|  
|Block users from changing device restrictions in device settings​|What it does|  
|Block erasing content and settings|What it does|  
|Block changing device name|What it does|  
|Block changing notification settings|What it does|  
|Block wallpaper modification |What it does|    
|Block configuration profile changes |What it does|  
|Block Activation Lock|What it does|  

### Password settings

### Lock screen and passcode  

Setting|What it does|
|---|---|
|Block notifications on lock screen|What it does|
|Block access to Control Center on lock screen|What it does|
|Block Siri on lock screen|What it does|
|Block access to Wallet from lock screen|What it does|
|Block Today view on lock screen|What it does|
|Require passcode|What it does|
|Block changing passcode|What it does|
|Minutes of inactivity before the screen locks|What it does|
|Minutes to wait before requiring passcode on lock screen|What it does|
|Number of failed passcode attempts before wiping device|What it does|
|Block fingerprint unlock|What it does|
|Block changing registered fingerprint settings|What it does|  

### App Store settings  

Setting|What it does|
|---|---|
|Block App Store|What it does|
|Require password to access App Store|What it does|
|Block automatically downloading apps purchased on other devices|What it does|
|Block in-app purchases|What it does|
|Block apps by age rating|What it does|
|Block explicit content in iTunes and the App Store|What it does|
|Block downloading iBook content flagged as erotica|What it does|
|Block Game Center|What it does|
|Block adding friends in Game Center|What it does|

### Keyboard and dictionary  

|Setting|What it does|  
|---|---|  
|Block looking up word definitions|What it does|  
|Block predictive keyboard suggestions|What it does|  
|Block auto-correction|What it does|
|Block keyboard spell-check|What it does|
|Block keyboard shortcuts|What it does|
|Block keyboard dictation|What it does|

### Cloud and storage  

|Setting|What it does|  
|---|---|  
|Block iCloud backup|What it does|  
|Block syncing documents to iCloud|What it does|  
|Block Photo Stream|What it does|  
|Require iCloud backups to be encrypted|What it does|  
|Block iCloud Photo Library|What it does|  
|Block shared Photo Stream|What it does|  
|Block Handoff|What it does|  

### Device update restrictions

|Setting|What it does|
|---|---|
|Prevent devices from updating specific times|What it does|
IX Note: Describe that the user can then specificy restricted days, time zone, start time, and end time.

### Inventory tracking
This information appears on the device lock screen.

|Setting|What it does|
|---|---|
|Asset tag information|What does it do|
|Lock screen footnote|What does it do|

### Built-in apps  

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

### Safari  

Setting|What it does|  
|---|---|  
|Block Safari|What it does|  
|Block autofill|What it does|  
|Block cookies|What it does|  
|Show warning when visiting a fraudulent website|What it does|  
|Block pop-ups|What it does|

### Wi-Fi profiles  

Setting|What it does|
|---|---|
|Profile name|What it does|
|Network name (SSID)|What it does|
|Security type|What it does|
|Description|What it does|


## Find out more
[Find out more about the full Windows 10 settings management experience available in Intune](https://docs.microsoft.com/intune/deploy-use/windows-10-policy-settings-in-microsoft-intune)
